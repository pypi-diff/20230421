# Comparing `tmp/formfyxer-0.1.1.tar.gz` & `tmp/formfyxer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formfyxer-0.1.1.tar", last modified: Fri Feb 24 17:06:44 2023, max compression
+gzip compressed data, was "formfyxer-0.2.0.tar", last modified: Fri Apr 21 19:16:33 2023, max compression
```

## Comparing `formfyxer-0.1.1.tar` & `formfyxer-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-24 17:06:44.133194 formfyxer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-02-24 17:06:27.000000 formfyxer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-24 17:06:27.000000 formfyxer-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    26914 2023-02-24 17:06:44.133194 formfyxer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    26533 2023-02-24 17:06:27.000000 formfyxer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-24 17:06:44.133194 formfyxer-0.1.1/formfyxer/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-24 17:06:44.133194 formfyxer-0.1.1/formfyxer/data/
--rw-r--r--   0 runner    (1001) docker     (122)  1246483 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/data/clf_field_names.joblib
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/data/groups.joblib
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/data/included_fields.joblib
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/data/jurisdictions.joblib
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-24 17:06:44.133194 formfyxer-0.1.1/formfyxer/keys/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/keys/openai_key.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/keys/openai_org.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/keys/spot_token.txt
--rw-r--r--   0 runner    (1001) docker     (122)    40302 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/lit_explorer.py
--rw-r--r--   0 runner    (1001) docker     (122)    48312 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/pdf_wrangling.py
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-02-24 17:06:27.000000 formfyxer-0.1.1/formfyxer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-24 17:06:44.133194 formfyxer-0.1.1/formfyxer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    26914 2023-02-24 17:06:44.000000 formfyxer-0.1.1/formfyxer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-02-24 17:06:44.000000 formfyxer-0.1.1/formfyxer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-24 17:06:44.000000 formfyxer-0.1.1/formfyxer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-02-24 17:06:44.000000 formfyxer-0.1.1/formfyxer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-24 17:06:44.000000 formfyxer-0.1.1/formfyxer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-02-24 17:06:27.000000 formfyxer-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-24 17:06:44.133194 formfyxer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-02-24 17:06:27.000000 formfyxer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.541589 formfyxer-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.537589 formfyxer-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.537589 formfyxer-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-04-21 19:16:12.000000 formfyxer-0.2.0/.github/workflows/mypy_unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-21 19:16:12.000000 formfyxer-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-04-21 19:16:12.000000 formfyxer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-21 19:16:12.000000 formfyxer-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    27232 2023-04-21 19:16:33.541589 formfyxer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    26851 2023-04-21 19:16:12.000000 formfyxer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.537589 formfyxer-0.2.0/formfyxer/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.541589 formfyxer-0.2.0/formfyxer/data/
+-rw-r--r--   0 runner    (1001) docker     (122)   483481 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/clf_field_names.joblib
+-rw-r--r--   0 runner    (1001) docker     (122)     8431 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/gendered_terms.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/groups.joblib
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/included_fields.joblib
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/jurisdictions.joblib
+-rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/data/simplified_words.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.541589 formfyxer-0.2.0/formfyxer/keys/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/keys/openai_key.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/keys/openai_org.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/keys/spot_token.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    48378 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/lit_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48382 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/pdf_wrangling.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-04-21 19:16:12.000000 formfyxer-0.2.0/formfyxer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 19:16:33.541589 formfyxer-0.2.0/formfyxer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    27232 2023-04-21 19:16:33.000000 formfyxer-0.2.0/formfyxer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-04-21 19:16:33.000000 formfyxer-0.2.0/formfyxer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 19:16:33.000000 formfyxer-0.2.0/formfyxer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-21 19:16:33.000000 formfyxer-0.2.0/formfyxer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-21 19:16:33.000000 formfyxer-0.2.0/formfyxer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-04-21 19:16:12.000000 formfyxer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 19:16:33.541589 formfyxer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-21 19:16:12.000000 formfyxer-0.2.0/setup.py
```

### Comparing `formfyxer-0.1.1/LICENSE` & `formfyxer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formfyxer-0.1.1/PKG-INFO` & `formfyxer-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: formfyxer
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool for learning about and pre-processing pdf forms.
 Home-page: https://github.com/SuffolkLITLab/FormFyxer
 Author: Suffolk LIT Lab
 Author-email: litlab@suffolk.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SuffolkLITLab/FormFyxer/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FormFyxer
+
+[![PyPI version](https://badge.fury.io/py/formfyxer.svg)](https://badge.fury.io/py/formfyxer)
+
 A Python package with a collection of functions for learning about and pre-processing pdf forms and associated form fields. This processing is done with an eye towards interoperability with the Suffolk LIT Lab's [Document Assembly Line Project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install FormFyxer.
 Rerun this command to check for and install updates directly from GitHub.
 
 ```bash
@@ -22,20 +25,29 @@
 ```
 
 If you are on Mac or Windows, you'll need to install [poppler](https://poppler.freedesktop.org/) for your respective platform.
 If you are on Anaconda, simply run `conda install poppler`. Otherwise, follow the instructions here:
 - [macOS instructions](https://macappstore.org/poppler/)
 - [Windows download](https://github.com/oschwartz10612/poppler-windows/releases/tag/v22.04.0-0)
 
+## Testing
+
+```bash
+TOOLS_TOKEN=<your_token_here> ISUNITTEST=True python -m unittest formfyxer.tests.cluster_test
+```
+
+You should test with and without `TOOLS_TOKEN`, and make sure that both pass.
+
 ## Functions
 
 Functions from `pdf_wrangling` are found on [our documentation site](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/reference/formfyxer/pdf_wrangling).
 
 - [FormFyxer](#formfyxer)
   - [Installation and updating](#installation-and-updating)
+  - [Testing](#testing)
   - [Functions](#functions)
     - [formfyxer.re\_case(text)](#formfyxerre_casetext)
       - [Parameters:](#parameters)
       - [Returns:](#returns)
       - [Example:](#example)
     - [formfyxer.regex\_norm\_field(text)](#formfyxerregex_norm_fieldtext)
       - [Parameters:](#parameters-1)
```

### Comparing `formfyxer-0.1.1/README.md` & `formfyxer-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # FormFyxer
+
+[![PyPI version](https://badge.fury.io/py/formfyxer.svg)](https://badge.fury.io/py/formfyxer)
+
 A Python package with a collection of functions for learning about and pre-processing pdf forms and associated form fields. This processing is done with an eye towards interoperability with the Suffolk LIT Lab's [Document Assembly Line Project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install FormFyxer.
 Rerun this command to check for and install updates directly from GitHub.
 
 ```bash
@@ -10,20 +13,29 @@
 ```
 
 If you are on Mac or Windows, you'll need to install [poppler](https://poppler.freedesktop.org/) for your respective platform.
 If you are on Anaconda, simply run `conda install poppler`. Otherwise, follow the instructions here:
 - [macOS instructions](https://macappstore.org/poppler/)
 - [Windows download](https://github.com/oschwartz10612/poppler-windows/releases/tag/v22.04.0-0)
 
+## Testing
+
+```bash
+TOOLS_TOKEN=<your_token_here> ISUNITTEST=True python -m unittest formfyxer.tests.cluster_test
+```
+
+You should test with and without `TOOLS_TOKEN`, and make sure that both pass.
+
 ## Functions
 
 Functions from `pdf_wrangling` are found on [our documentation site](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/reference/formfyxer/pdf_wrangling).
 
 - [FormFyxer](#formfyxer)
   - [Installation and updating](#installation-and-updating)
+  - [Testing](#testing)
   - [Functions](#functions)
     - [formfyxer.re\_case(text)](#formfyxerre_casetext)
       - [Parameters:](#parameters)
       - [Returns:](#returns)
       - [Example:](#example)
     - [formfyxer.regex\_norm\_field(text)](#formfyxerregex_norm_fieldtext)
       - [Parameters:](#parameters-1)
```

### Comparing `formfyxer-0.1.1/formfyxer/lit_explorer.py` & `formfyxer-0.2.0/formfyxer/lit_explorer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Updated on 2022-12-12
 
 import os
 import re
 import subprocess
-from sklearn.metrics import classification_report
 import spacy
 from spacy.tokens import Doc
 from pdfminer.high_level import extract_text
 from pdfminer.layout import LAParams
 
 import pikepdf
 import textstat
@@ -24,14 +23,15 @@
 from joblib import load
 import nltk
 from nltk.tokenize import sent_tokenize
 from PassivePySrc import PassivePy
 import eyecite
 from enum import Enum
 import sigfig
+import yaml
 from .pdf_wrangling import (
     get_existing_pdf_fields,
     FormField,
     FieldType,
     unlock_pdf_in_place,
 )
 
@@ -68,28 +68,34 @@
 
 tokenizer = GPT2TokenizerFast.from_pretrained("gpt2")
 
 stop_words = set(stopwords.words("english"))
 
 try:
     # this takes a while to load
-    import en_core_web_md
+    import en_core_web_lg
 
-    nlp = en_core_web_md.load()
+    nlp = en_core_web_lg.load()
 except:
-    print("Downloading word2vec model en_core_web_md")
-    import subprocess
+    try:
+        import en_core_web_sm
+
+        nlp = en_core_web_sm.load()
+    except:
+        print("Downloading word2vec model en_core_web_sm")
+        import subprocess
+
+        bashCommand = "python -m spacy download en_core_web_sm"
+        process = subprocess.Popen(bashCommand.split(), stdout=subprocess.PIPE)
+        output, error = process.communicate()
+        print(f"output of word2vec model download: {str(output)}")
+        import en_core_web_sm
 
-    bashCommand = "python -m spacy download en_core_web_md"
-    process = subprocess.Popen(bashCommand.split(), stdout=subprocess.PIPE)
-    output, error = process.communicate()
-    print(f"output of word2vec model download: {str(output)}")
-    import en_core_web_md
+        nlp = en_core_web_sm.load()
 
-    nlp = en_core_web_md.load()
 
 passivepy = PassivePy.PassivePyAnalyzer(nlp=nlp)
 
 
 # Load local variables, models, and API key(s).
 
 included_fields = load(
@@ -111,17 +117,26 @@
 ) as in_file:
     openai.organization = in_file.read().rstrip()
 with open(
     os.path.join(os.path.dirname(__file__), "keys", "openai_key.txt"), "r"
 ) as in_file:
     openai.api_key = in_file.read().rstrip()
 
-# This creates a timeout exception that can be triggered when something hangs too long.
+# TODO(brycew): remove by retraining the model to work with random_state=4.
+NEEDS_STABILITY = True if os.getenv("ISUNITTEST") else False
+
+# Define some hardcoded data file paths
 
+CURRENT_DIRECTORY = os.path.dirname(__file__)
+GENDERED_TERMS_PATH = os.path.join(CURRENT_DIRECTORY, "data", "gendered_terms.yml")
+PLAIN_LANGUAGE_TERMS_PATH = os.path.join(
+    CURRENT_DIRECTORY, "data", "simplified_words.yml"
+)
 
+# This creates a timeout exception that can be triggered when something hangs too long.
 class TimeoutException(Exception):
     pass
 
 
 @contextmanager
 def time_limit(seconds: float):
     timer = threading.Timer(seconds, lambda: _thread.interrupt_main())
@@ -254,15 +269,15 @@
         ["^Date\s?\d*$", "signature_date"],
     ]
     for regex in regex_list:
         text = re.sub(regex[0], regex[1], text, flags=re.IGNORECASE)
     return text
 
 
-def reformat_field(text: str, max_length: int = 30):
+def reformat_field(text: str, max_length: int = 30, tools_token=None):
     """
     Transforms a string of text into a snake_case variable close in length to `max_length` name by
     summarizing the string and stitching the summary together in snake_case.
     h/t https://towardsdatascience.com/nlp-building-a-summariser-68e0c19e3a93
     """
     orig_title = text.lower()
     orig_title = re.sub("[^a-zA-Z]+", " ", orig_title)
@@ -278,20 +293,22 @@
         words = len(filtered_title_words)
         av_word_len = math.ceil(
             len(" ".join(filtered_title_words)) / len(filtered_title_words)
         )
         x_words = math.floor((max_length) / av_word_len)
         sim_mat = np.zeros([len(filtered_title_words), len(filtered_title_words)])
         # for each word compared to other
+        filt_vecs = vectorize(filtered_title_words, tools_token=tools_token)
+        filt_vecs = [vec.reshape(1, 300) for vec in filt_vecs]
         for i in range(len(filtered_title_words)):
             for j in range(len(filtered_title_words)):
                 if i != j:
                     sim_mat[i][j] = cosine_similarity(
-                        nlp(filtered_title_words[i]).vector.reshape(1, 300),
-                        nlp(filtered_title_words[j]).vector.reshape(1, 300),
+                        filt_vecs[i],
+                        filt_vecs[j],
                     )[0, 0]
         try:
             nx_graph = nx.from_numpy_array(sim_mat)
             scores = nx.pagerank(nx_graph)
             sorted_scores = sorted(
                 scores.items(), key=lambda item: item[1], reverse=True
             )
@@ -315,40 +332,73 @@
             return re.sub("\s+", "_", text.lower())
 
 
 def norm(row):
     """Normalize a word vector."""
     try:
         matrix = row.reshape(1, -1).astype(np.float64)
-        return normalize(matrix, axis=1, norm="l1")[0]
+        return normalize(matrix, axis=1, norm="l2")[0]
     except Exception as e:
         print("===================")
         print("Error: ", e)
         print("===================")
         return np.NaN
 
 
-def vectorize(text: str, normalize: bool = True):
-    """Vectorize a string of text."""
-    output = nlp(str(text)).vector
-    if normalize:
-        return norm(output)
+def vectorize(text: Union[List[str], str], tools_token: Optional[str] = None):
+    """Vectorize a string of text.
+
+    Args:
+      text: a string of multiple words to vectorize
+      tools_token: the token to tools.suffolklitlab.org, used for micro-service
+          to reduce the amount of memory you need on your machine. If
+          not passed, you need to have `en_core_web_lg` installed
+    """
+    if tools_token:
+        headers = {
+            "Authorization": "Bearer " + tools_token,
+            "Content-Type": "application/json",
+        }
+        body = {"text": text}
+        r = requests.post(
+            "https://tools.suffolklitlab.org/vectorize/",
+            headers=headers,
+            data=json.dumps(body),
+        )
+        if not r.ok:
+            raise Exception("Couldn't access tools.suffolklitlab.org")
+        if isinstance(text, str):
+            output = np.array(r.json().get("embeddings", []))
+            if len(output) <= 0:
+                raise Exception("Vector from tools.suffolklitlab.org is empty")
+            return output
+        else:
+            return [np.array(embed) for embed in r.json().get("embeddings", [])]
     else:
-        return output
+        if isinstance(text, str):
+            return norm(nlp(text).vector)
+        else:
+            return [norm(nlp(indiv_text).vector) for indiv_text in text]
 
 
 # Given an auto-generated field name and context from the form where it appeared, this function attempts to normalize the field name. Here's what's going on:
 # 1. It will `re_case` the variable text
 # 2. Then it will run the output through `regex_norm_field`
 # 3. If it doesn't find anything, it will use the ML model `clf_field_names`
 # 4. If the prediction isn't very confident, it will run it through `reformat_field`
 
 
 def normalize_name(
-    jur: str, group: str, n: int, per, last_field: str, this_field: str
+    jur: str,
+    group: str,
+    n: int,
+    per,
+    last_field: str,
+    this_field: str,
+    tools_token: Optional[str] = None,
 ) -> Tuple[str, float]:
     """Add hard coded conversions maybe by calling a function
     if returns 0 then fail over to ML or other way around poor prob -> check hard-coded.
     Retuns the new name and a confidence value between 0 and 1"""
     if this_field not in included_fields:
         this_field = re_case(this_field)
         out_put = regex_norm_field(this_field)
@@ -363,15 +413,15 @@
             for item in groups:
                 if group == item:
                     params.append(1)
                 else:
                     params.append(0)
             params.append(n)
             params.append(per)
-            for vec in vectorize(this_field):
+            for vec in vectorize(this_field, tools_token=tools_token):
                 params.append(vec)
             for item in included_fields:
                 if last_field == item:
                     params.append(1)
                 else:
                     params.append(0)
             pred = clf_field_names.predict([params])
@@ -384,37 +434,51 @@
     if out_put in included_fields:
         if conf >= 0:
             return (
                 "*" + out_put,
                 conf,
             )  # this * is a hack to show when something is in the list of known fields later. I need to fix this
         else:
-            return reformat_field(this_field), conf
+            return reformat_field(this_field, tools_token=tools_token), conf
     else:
-        return reformat_field(this_field), conf
+        return reformat_field(this_field, tools_token=tools_token), conf
 
 
 # Take a list of AL variables and spits out suggested groupings. Here's what's going on:
 #
 # 1. It reads in a list of fields (e.g., `["user_name","user_address"]`)
 # 2. Splits each field into words (e.g., turning `user_name` into `user name`)
 # 3. It then turns these ngrams/"sentences" into vectors using word2vec.
 # 4. For the collection of fields, it finds clusters of these "sentences" within the semantic space defined by word2vec. Currently it uses Affinity Propagation. See https://machinelearningmastery.com/clustering-algorithms-with-python/
 
 
-def cluster_screens(fields: List[str] = [], damping: float = 0.7):
-    """Takes in a list (fields) and returns a suggested screen grouping
-    Set damping to value >= 0.5 or < 1 to tune how related screens should be"""
+def cluster_screens(
+    fields: List[str] = [], damping: float = 0.7, tools_token: Optional[str] = None
+) -> Dict[str, List[str]]:
+    """
+    Groups the given fields into screens based on how much they are related.
+
+    Args:
+      fields: a list of field names
+      damping: a value >= 0.5 and < 1. Tunes how related screens should be
+      tools_token: the token to tools.suffolklitlab.org, needed of doing
+          micro-service vectorization
+
+    returs: a suggested screen grouping, each screen name mapped to the list of fields on it
+    """
     vec_mat = np.zeros([len(fields), 300])
+    vecs = vectorize([re_case(field) for field in fields], tools_token=tools_token)
     for i in range(len(fields)):
-        vec_mat[i] = [nlp(re_case(fields[i])).vector][0]
+        vec_mat[i] = vecs[i]
     # create model
-    model = AffinityPropagation(damping=damping, random_state=None)
-    # model = AffinityPropagation(damping=damping,random_state=4) consider using this to get consistent results. note will have to require newer version
-    # fit the model
+    # note will have to require newer version to fit the model when running with random_state=4
+    # just on the unit test for now, to make sure `tools.suffolklitlab.org` and local don't differ
+    model = AffinityPropagation(
+        damping=damping, random_state=4 if NEEDS_STABILITY else None
+    )
     model.fit(vec_mat)
     # assign a cluster to each example
     yhat = model.predict(vec_mat)
     # retrieve unique clusters
     clusters = unique(yhat)
     screens = {}
     # sim = np.zeros([5,300])
@@ -586,14 +650,68 @@
         if field["max_length"] <= 100:
             return AnswerType.SLOT_IN
         else:
             return AnswerType.CREATED
     return AnswerType.GATHERED
 
 
+def get_adjusted_character_count(
+        field: FieldInfo
+)-> float:
+    """
+    Determines the bracketed length of an input field based on its max_length attribute, 
+    returning a float representing the approximate length of the field content. 
+
+    The function chunks the answers into 5 different lengths (checkboxes, 2 words, short, medium, and long)
+    instead of directly using the character count, as forms can allocate different spaces
+    for the same data without considering the space the user actually needs.
+
+    Args:
+        field (FieldInfo): An object containing information about the input field, 
+                           including the "max_length" attribute.
+
+    Returns:
+        float: The approximate length of the field content, categorized into checkboxes, 2 words, short, 
+               medium, or long based on the max_length attribute.
+
+    Examples:
+        >>> get_adjusted_character_count({"type"}: InputType.CHECKBOX)
+        4.7
+        >>> get_adjusted_character_count({"max_length": 100})
+        9.4
+        >>> get_adjusted_character_count({"max_length": 300})
+        230
+        >>> get_adjusted_character_count({"max_length": 600})
+        115
+        >>> get_adjusted_character_count({"max_length": 1200})
+        1150
+    """
+    ONE_WORD = 4.7  # average word length: https://www.researchgate.net/figure/Average-word-length-in-the-English-language-Different-colours-indicate-the-results-for_fig1_230764201
+    ONE_LINE = 115  # Standard line is ~ 115 characters wide at 12 point font
+    SHORT_ANSWER = (
+        ONE_LINE * 2
+    )  # Anything over 1 line but less than 3 probably needs about the same time to answer
+    MEDIUM_ANSWER = ONE_LINE * 5
+    LONG_ANSWER = (
+        ONE_LINE * 10
+    )  # Anything over 10 lines probably needs a full page but form author skimped on space
+    if field["type"] != InputType.TEXT:
+        return ONE_WORD
+    
+    if field["max_length"] <= ONE_LINE or (
+        field["max_length"] <= ONE_LINE * 2
+    ):
+        return ONE_WORD * 2
+    elif field["max_length"] <= SHORT_ANSWER:
+        return SHORT_ANSWER
+    elif field["max_length"] <= MEDIUM_ANSWER:
+        return MEDIUM_ANSWER
+    return LONG_ANSWER
+
+
 def time_to_answer_field(
     field: FieldInfo,
     new_name: str,
     cpm: int = 40,
     cpm_std_dev: int = 17,
 ) -> Callable[[int], np.ndarray]:
     """
@@ -621,40 +739,18 @@
     if field["type"] == InputType.CHECKBOX:
         return lambda number_samples: np.random.normal(
             loc=TIME_TO_MAKE_ANSWER[kind][0],
             scale=TIME_TO_MAKE_ANSWER[kind][1],
             size=number_samples,
         )
     else:
-        # We chunk answers into three different lengths rather than directly using the character count,
-        # as forms can give very different spaces for the same data without regard to the room the
-        # user actually needs. But small, medium, and full page is still helpful information.
-        ONE_WORD = 4.7  # average word length: https://www.researchgate.net/figure/Average-word-length-in-the-English-language-Different-colours-indicate-the-results-for_fig1_230764201
-        ONE_LINE = 115  # Standard line is ~ 115 characters wide at 12 point font
-        SHORT_ANSWER = (
-            ONE_LINE * 2
-        )  # Anything over 1 line but less than 3 probably needs about the same time to answer
-        MEDIUM_ANSWER = ONE_LINE * 5
-        LONG_ANSWER = (
-            ONE_LINE * 10
-        )  # Anything over 10 lines probably needs a full page but form author skimped on space
-        if field["max_length"] <= ONE_LINE or (
-            field["max_length"] <= ONE_LINE * 2 and kind == AnswerType.SLOT_IN
-        ):
-            time_to_write_answer = ONE_WORD * 2 / cpm
-            time_to_write_std_dev = ONE_WORD * 2 / cpm_std_dev
-        elif field["max_length"] <= SHORT_ANSWER:
-            time_to_write_answer = SHORT_ANSWER / cpm
-            time_to_write_std_dev = SHORT_ANSWER / cpm_std_dev
-        elif field["max_length"] <= MEDIUM_ANSWER:
-            time_to_write_answer = MEDIUM_ANSWER / cpm
-            time_to_write_std_dev = MEDIUM_ANSWER / cpm_std_dev
-        else:
-            time_to_write_answer = LONG_ANSWER / cpm
-            time_to_write_std_dev = LONG_ANSWER / cpm_std_dev
+        adjusted_character_count = get_adjusted_character_count(field)
+        time_to_write_answer = adjusted_character_count / cpm
+        time_to_write_std_dev = adjusted_character_count / cpm_std_dev
+
         return lambda number_samples: np.random.normal(
             loc=time_to_write_answer, scale=time_to_write_std_dev, size=number_samples
         ) + np.random.normal(
             loc=TIME_TO_MAKE_ANSWER[kind][0],
             scale=TIME_TO_MAKE_ANSWER[kind][1],
             size=number_samples,
         )
@@ -720,16 +816,16 @@
 class OpenAiCreds(TypedDict):
     org: str
     key: str
 
 
 def text_complete(prompt, max_tokens=500, creds: Optional[OpenAiCreds] = None) -> str:
     if creds:
-        openai.organization = creds["org"].strip()
-        openai.api_key = creds["key"].strip()
+        openai.organization = creds["org"].strip() or ""
+        openai.api_key = creds["key"].strip() or ""
 
     try:
         response = openai.Completion.create(
             model="text-davinci-003",
             prompt=prompt,
             temperature=0,
             max_tokens=max_tokens,
@@ -786,43 +882,60 @@
     for token in doc:
         if token.text.lower() in CALCULATION_WORDS:
             return True
     # TODO(brycew): anything better than a binary yes-no value on this?
     return False
 
 
-def get_passive_sentences(text: Union[List, str]) -> List[Tuple[str, List[str]]]:
+def get_passive_sentences(
+    text: Union[List, str]
+) -> List[Tuple[str, List[Tuple[int, int]]]]:
     """Return a list of tuples, where each tuple represents a
-    sentence in which passive voice was detected along with a list of each
-    fragment that is phrased in the passive voice. The combination of the two
-    can be used in the PDFStats frontend to highlight the passive text in an
-    individual sentence.
+    sentence in which passive voice was detected along with a list of the
+    starting and ending position of each fragment that is phrased in the passive voice.
+    The combination of the two can be used in the PDFStats frontend to highlight the
+    passive text in an individual sentence.
 
     Text can either be a string or a list of strings.
     If provided a single string, it will be tokenized with NTLK and
     sentences containing fewer than 2 words will be ignored.
     """
     # Sepehri, A., Markowitz, D. M., & Mir, M. (2022, February 3).
     # PassivePy: A Tool to Automatically Identify Passive Voice in Big Text Data. Retrieved from psyarxiv.com/bwp3t
-
+    #
     if isinstance(text, str):
         sentences = [s for s in sent_tokenize(text) if len(s.split(" ")) > 2]
         if not sentences:
             raise ValueError(
                 "There are no sentences over 2 words in the provided text."
             )
     elif isinstance(text, list):
         sentences = text
     else:
         raise ValueError(f"Can't tokenize {type(text)} object into sentences")
 
+    if not sentences:
+        return []
+
     passive_text_df = passivepy.match_corpus_level(pd.DataFrame(sentences), 0)
     matching_rows = passive_text_df[passive_text_df["binary"] > 0]
+    sentences_with_highlights = []
 
-    return list(zip(matching_rows["document"], matching_rows["all_passives"]))
+    for item in list(zip(matching_rows["document"], matching_rows["all_passives"])):
+        for fragment in item[1]:
+            sentences_with_highlights.append(
+                (
+                    item[0],
+                    [
+                        (match.start(), match.end())
+                        for match in re.finditer(re.escape(fragment), item[0])
+                    ],
+                )
+            )
+    return sentences_with_highlights
 
 
 def get_citations(text: str, tokenized_sentences: List[str]) -> List[str]:
     """
     Get citations and some extra surrounding context (the full sentence), if the citation is
     fewer than 5 characters (often eyecite only captures a section symbol
     for state-level short citation formats)
@@ -841,21 +954,112 @@
         citations_with_context.extend(
             [sentence for sentence in tokenized_sentences if token in sentence]
         )
 
     return citations_with_context
 
 
+def substitute_phrases(
+    input_string: str, substitution_phrases: Dict[str, str]
+) -> Tuple[str, List[Tuple[int, int]]]:
+    """Substitute phrases in the input string and return the new string and positions of substituted phrases.
+
+    Args:
+        input_string (str): The input string containing phrases to be replaced.
+        substitution_phrases (Dict[str, str]): A dictionary mapping original phrases to their replacement phrases.
+
+    Returns:
+        Tuple[str, List[Tuple[int, int]]]: A tuple containing the new string with substituted phrases and a list of
+                                          tuples, each containing the start and end positions of the substituted
+                                          phrases in the new string.
+
+    Example:
+        >>> input_string = "The quick brown fox jumped over the lazy dog."
+        >>> substitution_phrases = {"quick brown": "swift reddish", "lazy dog": "sleepy canine"}
+        >>> new_string, positions = substitute_phrases(input_string, substitution_phrases)
+        >>> print(new_string)
+        "The swift reddish fox jumped over the sleepy canine."
+        >>> print(positions)
+        [(4, 17), (35, 48)]
+    """
+    # Sort the substitution phrases by length in descending order
+    sorted_phrases = sorted(
+        substitution_phrases.items(), key=lambda x: len(x[0]), reverse=True
+    )
+
+    matches = []
+
+    # Find all matches for the substitution phrases
+    for original, replacement in sorted_phrases:
+        for match in re.finditer(r"\b" + re.escape(original) + r"\b", input_string, re.IGNORECASE):
+            matches.append((match.start(), match.end(), replacement))
+
+    # Sort the matches based on their starting position
+    matches.sort(key=lambda x: x[0])
+
+    new_string = ""
+    substitutions: List[Tuple[int, int]] = []
+    prev_end_pos = 0
+
+    # Build the new string and substitutions list
+    for start_pos, end_pos, replacement in matches:
+        if start_pos >= prev_end_pos:
+            new_string += input_string[prev_end_pos:start_pos] + replacement
+            substitutions.append((len(new_string) - len(replacement), len(new_string)))
+            prev_end_pos = end_pos
+
+    new_string += input_string[prev_end_pos:]
+
+    return new_string, substitutions
+
+
+def substitute_neutral_gender(input_string: str) -> Tuple[str, List[Tuple[int, int]]]:
+    """
+    Substitute gendered phrases with neutral phrases in the input string.
+    Primary source is https://github.com/joelparkerhenderson/inclusive-language
+    """
+    with open(GENDERED_TERMS_PATH) as f:
+        terms = yaml.safe_load(f)
+    return substitute_phrases(input_string, terms)
+
+
+def substitute_plain_language(input_string: str) -> Tuple[str, List[Tuple[int, int]]]:
+    """
+    Substitute complex phrases with simpler alternatives.
+    Source of terms is drawn from https://www.plainlanguage.gov/guidelines/words/
+    """
+    with open(PLAIN_LANGUAGE_TERMS_PATH) as f:
+        terms = yaml.safe_load(f)
+    return substitute_phrases(input_string, terms)
+
+
+def transformed_sentences(
+    sentence_list: List[str], fun: Callable
+) -> List[Tuple[str, str, List[Tuple[int, int]]]]:
+    """
+    Apply a function to a list of sentences and return only the sentences with changed terms.
+    The result is a tuple of the original sentence, new sentence, and the starting and ending position
+    of each changed fragment in the sentence.
+    """
+    transformed: List[Tuple[str, str, List[Tuple[int, int]]]] = []
+    for sentence in sentence_list:
+        run = fun(sentence)
+        if run[0] != sentence:
+            transformed.append((sentence, run[0], run[1]))
+    return transformed
+
+
 def parse_form(
     in_file: str,
     title: Optional[str] = None,
     jur: Optional[str] = None,
     cat: Optional[str] = None,
     normalize: bool = True,
     spot_token: Optional[str] = None,
+    tools_token: Optional[str] = None,
     openai_creds: Optional[OpenAiCreds] = None,
     rewrite: bool = False,
     debug: bool = False,
 ):
     """
     Read in a pdf, pull out basic stats, attempt to normalize its form fields, and re-write the
     in_file with the new fields (if `rewrite=1`). If you pass a spot token, we will guess the
@@ -932,15 +1136,21 @@
     if normalize:
         length = len(field_names)
         last = "null"
         new_names = []
         new_names_conf = []
         for i, field_name in enumerate(field_names):
             new_name, new_confidence = normalize_name(
-                jur or "", cat or "", i, i / length, last, field_name
+                jur or "",
+                cat or "",
+                i,
+                i / length,
+                last,
+                field_name,
+                tools_token=tools_token,
             )
             new_names.append(new_name)
             new_names_conf.append(new_confidence)
             last = field_name
         new_names = [
             v + "__" + str(new_names[:i].count(v) + 1) if new_names.count(v) > 1 else v
             for i, v in enumerate(new_names)
@@ -957,14 +1167,20 @@
         passive_sentences = get_passive_sentences(sentences)
         passive_sentences_count = len(passive_sentences)
     except ValueError:
         passive_sentences_count = 0
         passive_sentences = []
 
     citations = get_citations(original_text, tokenized_sentences)
+    plain_language_suggestions = transformed_sentences(
+        sentences, substitute_plain_language
+    )
+    neutral_gender_suggestions = transformed_sentences(
+        sentences, substitute_neutral_gender
+    )
     word_count = len(text.split(" "))
     all_caps_count = all_caps_words(text)
     field_types = field_types_and_sizes(ff)
     classified = [
         classify_field(field, new_names[index])
         for index, field in enumerate(field_types)
     ]
@@ -1009,18 +1225,21 @@
         else 0,
         "passive voice percent": (
             passive_sentences_count / sentence_count if sentence_count > 0 else 0
         ),
         "citations per field": citation_count / field_count if field_count > 0 else 0,
         "citation count": citation_count,
         "all caps percent": all_caps_count / word_count,
+        "normalized characters per field": sum(get_adjusted_character_count(field) for field in field_types ) / field_count if ff else 0,
         "difficult words": difficult_words,
         "difficult word count": difficult_word_count,
         "difficult word percent": difficult_word_count / word_count,
         "calculation required": needs_calculations(text),
+        "plain language suggestions": plain_language_suggestions,
+        "neutral gender suggestions": neutral_gender_suggestions,
     }
     if debug and ff:
         debug_fields = []
         for index, field in enumerate(field_types_and_sizes(ff)):
             debug_fields.append(
                 {
                     "name": field["var_name"],
@@ -1042,14 +1261,15 @@
                 my_pdf.Root.AcroForm.Fields
             )  # [0]["/Kids"][0]["/Kids"][0]["/Kids"][0]["/Kids"]
             # print(repr(fields_too))
             for k, field_name in enumerate(new_names):
                 # print(k,field)
                 fields_too[k].T = re.sub("^\*", "", field_name)
             my_pdf.save(in_file)
+            my_pdf.close()
         except Exception as ex:
             stats["error"] = f"could not change form fields: {ex}"
     return stats
 
 
 def _form_complexity_per_metric(stats):
     # check for fields that require user to look up info, when found add to complexity
@@ -1063,35 +1283,37 @@
     metrics = [
         {"name": "reading grade level", "weight": 10 / 7, "intercept": 5},
         {"name": "calculation required", "weight": 2},
         # {"name": "time to answer", "weight": 2},
         {"name": "pages", "weight": 2},
         {"name": "citations per field", "weight": 1.2},
         {"name": "avg fields per page", "weight": 1 / 8},
+        {"name": "normalized characters per field", "weight": 1/8},
         {"name": "sentences per page", "weight": 0.05},
         # percents will have a higher weight, because they are between 0 and 1
         {"name": "slotin percent", "weight": 2},
         {"name": "gathered percent", "weight": 5},
+        {"name": "third party percent", "weight": 10},
         {"name": "created percent", "weight": 20},
         {"name": "passive voice percent", "weight": 4},
         {"name": "all caps percent", "weight": 10},
         {"name": "difficult word percent", "weight": 15},
     ]
 
     def weight(stats, metric):
         """Handles if we need to scale / "normalize" the metrics at all."""
         name = metric["name"]
         weight = metric.get("weight") or 1
         val = 0
         if "clip" in metric:
-            val = min(max(stats[name], metric["clip"][0]), metric["clip"][1])
-        elif isinstance(stats[name], bool):
-            val = 1 if stats[name] else 0
+            val = min(max(stats.get(name,0), metric["clip"][0]), metric["clip"][1])
+        elif isinstance(stats.get(name), bool):
+            val = 1 if stats.get(name) else 0
         else:
-            val = stats[name]
+            val = stats.get(name,0)
         if "intercept" in metric:
             val -= metric["intercept"]
         return val * weight
 
     return [(m["name"], stats[m["name"]], weight(stats, m)) for m in metrics]
```

### Comparing `formfyxer-0.1.1/formfyxer/pdf_wrangling.py` & `formfyxer-0.2.0/formfyxer/pdf_wrangling.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,14 +354,16 @@
     # Make an in-memory PDF with the fields
     io_obj = io.BytesIO()
     _create_only_fields(io_obj, fields_per_page)
     temp_pdf = Pdf.open(io_obj)
 
     in_pdf = copy_pdf_fields(source_pdf=temp_pdf, destination_pdf=in_pdf)
     in_pdf.save(out_file)
+    in_pdf.close()
+    temp_pdf.close()
 
 
 def rename_pdf_fields(
     in_file: Union[str, Path, BinaryIO],
     out_file: Union[str, Path, BinaryIO],
     mapping: Mapping[str, str],
 ) -> None:
@@ -391,23 +393,25 @@
                 # we aren't changing the parent names at all, so just change the last part of the name
                 if "." in mapping[name]:
                     field["all"].T = mapping[name].split(".")[-1]
                 else:
                     field["all"].T = mapping[name]
 
     in_pdf.save(out_file)
+    in_pdf.close()
 
 
 def unlock_pdf_in_place(in_file: Union[str, Path, BinaryIO]) -> None:
     """
     Try using pikePDF to unlock the PDF it it is locked. This won't work if it has a non-zero length password.
     """
     pdf_file = Pdf.open(in_file, allow_overwriting_input=True)
     if pdf_file.is_encrypted:
         pdf_file.save(in_file)
+    pdf_file.close()
 
 
 def _unnest_pdf_fields(
     field, parent_name: Optional[List[str]] = None
 ) -> List[PikeField]:
     if parent_name is None:
         parent_name = []
@@ -882,15 +886,15 @@
         return vert_dist + hori_dist, a_vert, b_vert
 
 
 ###### Field functionality #######
 
 
 def get_possible_fields(
-    in_pdf_file: Union[str, Path, BinaryIO],
+    in_pdf_file: Union[str, Path],
     textboxes: Optional[List[List[Textbox]]] = None,
 ) -> List[List[FormField]]:
     """Given an input PDF, runs a series of heuristics to predict where there
     might be places for user enterable information (i.e. PDF fields), and returns
     those predictions.
 
     Example:
```

### Comparing `formfyxer-0.1.1/formfyxer.egg-info/PKG-INFO` & `formfyxer-0.2.0/formfyxer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: formfyxer
-Version: 0.1.1
+Version: 0.2.0
 Summary: A tool for learning about and pre-processing pdf forms.
 Home-page: https://github.com/SuffolkLITLab/FormFyxer
 Author: Suffolk LIT Lab
 Author-email: litlab@suffolk.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SuffolkLITLab/FormFyxer/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FormFyxer
+
+[![PyPI version](https://badge.fury.io/py/formfyxer.svg)](https://badge.fury.io/py/formfyxer)
+
 A Python package with a collection of functions for learning about and pre-processing pdf forms and associated form fields. This processing is done with an eye towards interoperability with the Suffolk LIT Lab's [Document Assembly Line Project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 
 ## Installation and updating
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install FormFyxer.
 Rerun this command to check for and install updates directly from GitHub.
 
 ```bash
@@ -22,20 +25,29 @@
 ```
 
 If you are on Mac or Windows, you'll need to install [poppler](https://poppler.freedesktop.org/) for your respective platform.
 If you are on Anaconda, simply run `conda install poppler`. Otherwise, follow the instructions here:
 - [macOS instructions](https://macappstore.org/poppler/)
 - [Windows download](https://github.com/oschwartz10612/poppler-windows/releases/tag/v22.04.0-0)
 
+## Testing
+
+```bash
+TOOLS_TOKEN=<your_token_here> ISUNITTEST=True python -m unittest formfyxer.tests.cluster_test
+```
+
+You should test with and without `TOOLS_TOKEN`, and make sure that both pass.
+
 ## Functions
 
 Functions from `pdf_wrangling` are found on [our documentation site](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/reference/formfyxer/pdf_wrangling).
 
 - [FormFyxer](#formfyxer)
   - [Installation and updating](#installation-and-updating)
+  - [Testing](#testing)
   - [Functions](#functions)
     - [formfyxer.re\_case(text)](#formfyxerre_casetext)
       - [Parameters:](#parameters)
       - [Returns:](#returns)
       - [Example:](#example)
     - [formfyxer.regex\_norm\_field(text)](#formfyxerregex_norm_fieldtext)
       - [Parameters:](#parameters-1)
```

### Comparing `formfyxer-0.1.1/setup.py` & `formfyxer-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import setuptools
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+# We can't simply include this as an install_requires, because pypi won't allow
+# projects with github dependencies to be hosted there.
 class InstallSpacyModelCommand(install):
     def run(self):
         install.run(self)
         import spacy
-        print("Downloading word2vec model en_core_web_lg")
-        spacy.cli.download('en_core_web_lg')
+        print("Downloading word2vec model en_core_web_sm")
+        spacy.cli.download('en_core_web_sm')
 
 
 setuptools.setup(
     name='formfyxer',
-    version='0.1.1',
+    version='0.2.0',
     author='Suffolk LIT Lab',
     author_email='litlab@suffolk.edu',
     description='A tool for learning about and pre-processing pdf forms.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/SuffolkLITLab/FormFyxer',
     project_urls = {
         "Bug Tracker": "https://github.com/SuffolkLITLab/FormFyxer/issues"
     },
     license='MIT',
     packages=['formfyxer'],
-    install_requires=['spacy', 'pdfminer.six', 'pandas', 'pikepdf',  'textstat',  'requests',  'numpy',  'scikit-learn', 'networkx',
-        'joblib',  'nltk', 'boxdetect', 'pdf2image', 'reportlab', 'pdfminer.six', 'opencv-python', 'ocrmypdf', 'eyecite', 'passivepy>=0.2.16',
-        'sigfig', 'typer>=0.4.1,<0.5.0', 'openai', 'transformers' # typer pre 0.4.1 was broken by click 8.1.0: https://github.com/explosion/spaCy/issues/10564
+    install_requires=['spacy', 'pdfminer.six', 'pandas', 'pikepdf',
+        'textstat', 'requests', 'numpy', 'scikit-learn', 'networkx', 'joblib',
+        'nltk', 'boxdetect', 'pdf2image', 'reportlab', 'pdfminer.six',
+        'opencv-python', 'ocrmypdf', 'eyecite', 'passivepy>=0.2.16', 'sigfig',
+        'typer>=0.4.1,<0.5.0', # typer pre 0.4.1 was broken by click 8.1.0: https://github.com/explosion/spaCy/issues/10564
+        'openai', 'transformers' 
     ],
     cmdclass={
       'install': InstallSpacyModelCommand,
     },
     include_package_data = True
 )
```

