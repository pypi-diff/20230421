# Comparing `tmp/pdftotree-mercurial-1.1.tar.gz` & `tmp/pdftotree-mercurial-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftotree-mercurial-1.1.tar", last modified: Fri Apr 21 18:42:27 2023, max compression
+gzip compressed data, was "pdftotree-mercurial-1.2.tar", last modified: Fri Apr 21 18:58:45 2023, max compression
```

## Comparing `pdftotree-mercurial-1.1.tar` & `pdftotree-mercurial-1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.241948 pdftotree-mercurial-1.1/
--rw-rw-rw-   0        0        0     1090 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/LICENSE
--rw-rw-rw-   0        0        0      930 2023-04-21 18:42:27.241948 pdftotree-mercurial-1.1/PKG-INFO
--rw-rw-rw-   0        0        0    10095 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.171402 pdftotree-mercurial-1.1/bin/
--rw-rw-rw-   0        0        0    15070 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/bin/extract_tables
--rw-rw-rw-   0        0        0     2845 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/bin/pdftotree
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.182421 pdftotree-mercurial-1.1/pdftotree/
--rw-rw-rw-   0        0        0    22569 2023-04-21 18:40:24.000000 pdftotree-mercurial-1.1/pdftotree/TreeExtract.py
--rw-rw-rw-   0        0        0     3732 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/TreeVisualizer.py
--rw-rw-rw-   0        0        0      298 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/__init__.py
--rw-rw-rw-   0        0        0       27 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/_version.py
--rw-rw-rw-   0        0        0     2361 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/core.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.185422 pdftotree-mercurial-1.1/pdftotree/ml/
--rw-rw-rw-   0        0        0     5333 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/ml/TableExtractML.py
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/ml/__init__.py
--rw-rw-rw-   0        0        0     5759 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/ml/features.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.191720 pdftotree-mercurial-1.1/pdftotree/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/__init__.py
--rw-rw-rw-   0        0        0     5325 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/bbox_utils.py
--rw-rw-rw-   0        0        0     2603 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/display_utils.py
--rw-rw-rw-   0        0        0     5113 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/img_utils.py
--rw-rw-rw-   0        0        0     4484 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/lines_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.206147 pdftotree-mercurial-1.1/pdftotree/utils/pdf/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/__init__.py
--rw-rw-rw-   0        0        0     6720 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/grid.py
--rw-rw-rw-   0        0        0     7810 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/layout_utils.py
--rw-rw-rw-   0        0        0     7752 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/node.py
--rw-rw-rw-   0        0        0    52985 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/pdf_parsers.py
--rw-rw-rw-   0        0        0     9496 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/pdf_utils.py
--rw-rw-rw-   0        0        0     2101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/render.py
--rw-rw-rw-   0        0        0     6101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/utils/pdf/vector_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.208147 pdftotree-mercurial-1.1/pdftotree/visual/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/visual/__init__.py
--rw-rw-rw-   0        0        0     5318 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/pdftotree/visual/visual_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.229203 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/
--rw-rw-rw-   0        0        0      930 2023-04-21 18:42:27.000000 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2023-04-21 18:42:27.000000 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:42:27.000000 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-21 18:42:27.000000 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 18:42:27.000000 pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      159 2023-04-21 18:42:27.246947 pdftotree-mercurial-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1581 2023-04-21 18:04:34.000000 pdftotree-mercurial-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:42:27.240982 pdftotree-mercurial-1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     5811 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/tests/test_basic.py
--rw-rw-rw-   0        0        0      629 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/tests/test_figures.py
--rw-rw-rw-   0        0        0     1028 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/tests/test_table_detection.py
--rw-rw-rw-   0        0        0      681 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.1/tests/test_text.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.072572 pdftotree-mercurial-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/LICENSE
+-rw-rw-rw-   0        0        0      930 2023-04-21 18:58:45.072572 pdftotree-mercurial-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10095 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.034206 pdftotree-mercurial-1.2/bin/
+-rw-rw-rw-   0        0        0    15070 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/bin/extract_tables
+-rw-rw-rw-   0        0        0     2845 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/bin/pdftotree
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.039614 pdftotree-mercurial-1.2/pdftotree/
+-rw-rw-rw-   0        0        0    22575 2023-04-21 18:58:14.000000 pdftotree-mercurial-1.2/pdftotree/TreeExtract.py
+-rw-rw-rw-   0        0        0     3732 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/TreeVisualizer.py
+-rw-rw-rw-   0        0        0      298 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/_version.py
+-rw-rw-rw-   0        0        0     2361 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/core.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.041612 pdftotree-mercurial-1.2/pdftotree/ml/
+-rw-rw-rw-   0        0        0     5333 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/TableExtractML.py
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/__init__.py
+-rw-rw-rw-   0        0        0     5759 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/ml/features.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.045613 pdftotree-mercurial-1.2/pdftotree/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/__init__.py
+-rw-rw-rw-   0        0        0     5325 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/bbox_utils.py
+-rw-rw-rw-   0        0        0     2603 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/display_utils.py
+-rw-rw-rw-   0        0        0     5113 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/img_utils.py
+-rw-rw-rw-   0        0        0     4484 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/lines_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.052647 pdftotree-mercurial-1.2/pdftotree/utils/pdf/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/__init__.py
+-rw-rw-rw-   0        0        0     6720 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/grid.py
+-rw-rw-rw-   0        0        0     7810 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/layout_utils.py
+-rw-rw-rw-   0        0        0     7752 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/node.py
+-rw-rw-rw-   0        0        0    52985 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_parsers.py
+-rw-rw-rw-   0        0        0     9496 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_utils.py
+-rw-rw-rw-   0        0        0     2101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/render.py
+-rw-rw-rw-   0        0        0     6101 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/utils/pdf/vector_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.054645 pdftotree-mercurial-1.2/pdftotree/visual/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/visual/__init__.py
+-rw-rw-rw-   0        0        0     5318 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/pdftotree/visual/visual_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.067832 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 18:58:44.000000 pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      159 2023-04-21 18:58:45.074570 pdftotree-mercurial-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1581 2023-04-21 18:58:40.000000 pdftotree-mercurial-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:58:45.071573 pdftotree-mercurial-1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     5811 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_basic.py
+-rw-rw-rw-   0        0        0      629 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_figures.py
+-rw-rw-rw-   0        0        0     1028 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_table_detection.py
+-rw-rw-rw-   0        0        0      681 2023-04-20 17:45:18.000000 pdftotree-mercurial-1.2/tests/test_text.py
```

### Comparing `pdftotree-mercurial-1.1/LICENSE` & `pdftotree-mercurial-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/PKG-INFO` & `pdftotree-mercurial-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftotree-mercurial
-Version: 1.1
+Version: 1.2
 Summary: Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without sklearn in dependencies)
 Home-page: https://github.com/HazyResearch/pdftotree
 Author: Hazy Research
 Author-email: senwu@cs.stanford.edu
 License: MIT
 Project-URL: Tracker, https://github.com/HazyResearch/pdftotree/issues
 Project-URL: Source, https://github.com/HazyResearch/pdftotree
```

### Comparing `pdftotree-mercurial-1.1/README.rst` & `pdftotree-mercurial-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/bin/extract_tables` & `pdftotree-mercurial-1.2/bin/extract_tables`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/bin/pdftotree` & `pdftotree-mercurial-1.2/bin/pdftotree`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/TreeExtract.py` & `pdftotree-mercurial-1.2/pdftotree/TreeExtract.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             # Set parameters for analysis.
             laparams = LAParams(char_margin=1.0, word_margin=0.1, detect_vertical=True)
             # Create a PDF page aggregator object.
             device = CustomPDFPageAggregator(rsrcmgr, laparams=laparams)
             # Create a PDF interpreter object.
             interpreter = PDFPageInterpreter(rsrcmgr, device)
 
-            pages = PDFPage.create_pages(document)
+            pages = list(PDFPage.create_pages(document))
             pages = pages[int(len(pages) / 2 - 1):]
             # Process each page contained in the document.
             for page_num, page in enumerate(pages):
                 try:
                     interpreter.process_page(page)
                 except OverflowError as oe:
                     log.exception(
```

### Comparing `pdftotree-mercurial-1.1/pdftotree/TreeVisualizer.py` & `pdftotree-mercurial-1.2/pdftotree/TreeVisualizer.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/core.py` & `pdftotree-mercurial-1.2/pdftotree/core.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/ml/TableExtractML.py` & `pdftotree-mercurial-1.2/pdftotree/ml/TableExtractML.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/ml/features.py` & `pdftotree-mercurial-1.2/pdftotree/ml/features.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/bbox_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/display_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/display_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/img_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/img_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/lines_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/lines_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/grid.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/grid.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/layout_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/layout_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/node.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/node.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/pdf_parsers.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/pdf_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/render.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/render.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/utils/pdf/vector_utils.py` & `pdftotree-mercurial-1.2/pdftotree/utils/pdf/vector_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree/visual/visual_utils.py` & `pdftotree-mercurial-1.2/pdftotree/visual/visual_utils.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/PKG-INFO` & `pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftotree-mercurial
-Version: 1.1
+Version: 1.2
 Summary: Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without sklearn in dependencies)
 Home-page: https://github.com/HazyResearch/pdftotree
 Author: Hazy Research
 Author-email: senwu@cs.stanford.edu
 License: MIT
 Project-URL: Tracker, https://github.com/HazyResearch/pdftotree/issues
 Project-URL: Source, https://github.com/HazyResearch/pdftotree
```

### Comparing `pdftotree-mercurial-1.1/pdftotree_mercurial.egg-info/SOURCES.txt` & `pdftotree-mercurial-1.2/pdftotree_mercurial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/setup.py` & `pdftotree-mercurial-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """For pip."""
 from setuptools import find_packages, setup
 
 exec(open("pdftotree/_version.py").read())
 setup(
     name="pdftotree-mercurial",
-    version='1.1',
+    version='1.2',
     description="Convert PDF into hOCR with text, tables, and figures being recognized and preserved. (Without "
                 "sklearn in dependencies)",
     packages=find_packages(),
     install_requires=[
         "IPython",
         "beautifulsoup4",
         "numpy",
```

### Comparing `pdftotree-mercurial-1.1/tests/test_basic.py` & `pdftotree-mercurial-1.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/tests/test_figures.py` & `pdftotree-mercurial-1.2/tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/tests/test_table_detection.py` & `pdftotree-mercurial-1.2/tests/test_table_detection.py`

 * *Files identical despite different names*

### Comparing `pdftotree-mercurial-1.1/tests/test_text.py` & `pdftotree-mercurial-1.2/tests/test_text.py`

 * *Files identical despite different names*

