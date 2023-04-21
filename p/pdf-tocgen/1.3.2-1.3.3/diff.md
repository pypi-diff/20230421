# Comparing `tmp/pdf_tocgen-1.3.2.tar.gz` & `tmp/pdf_tocgen-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_tocgen-1.3.2.tar", max compression
+gzip compressed data, was "pdf_tocgen-1.3.3.tar", max compression
```

## Comparing `pdf_tocgen-1.3.2.tar` & `pdf_tocgen-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.2/LICENSE
--rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.2/LICENSE_AGPL
--rw-r--r--   0        0        0    13650 2021-05-09 08:08:57.010536 pdf_tocgen-1.3.2/README.md
--rw-r--r--   0        0        0      274 2023-04-20 06:06:03.536966 pdf_tocgen-1.3.2/fitzutils/__init__.py
--rw-r--r--   0        0        0     2875 2023-04-20 06:05:46.873633 pdf_tocgen-1.3.2/fitzutils/fitzutils.py
--rw-r--r--   0        0        0       87 2023-04-20 07:11:03.110161 pdf_tocgen-1.3.2/pdftocgen/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocgen/__main__.py
--rw-r--r--   0        0        0     4880 2023-04-20 06:15:48.496945 pdf_tocgen-1.3.2/pdftocgen/app.py
--rw-r--r--   0        0        0     5395 2021-11-10 10:51:01.789897 pdf_tocgen-1.3.2/pdftocgen/filter.py
--rw-r--r--   0        0        0     4963 2021-11-10 19:31:24.999892 pdf_tocgen-1.3.2/pdftocgen/recipe.py
--rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocgen/tocgen.py
--rw-r--r--   0        0        0       73 2023-04-20 07:11:06.263494 pdf_tocgen-1.3.2/pdftocio/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocio/__main__.py
--rw-r--r--   0        0        0     5563 2023-04-20 06:18:07.596940 pdf_tocgen-1.3.2/pdftocio/app.py
--rw-r--r--   0        0        0      481 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdftocio/tocio.py
--rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf_tocgen-1.3.2/pdftocio/tocparser.py
--rw-r--r--   0        0        0      148 2023-04-20 07:11:09.396827 pdf_tocgen-1.3.2/pdfxmeta/__init__.py
--rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.2/pdfxmeta/__main__.py
--rw-r--r--   0        0        0     4212 2023-04-20 06:10:42.420289 pdf_tocgen-1.3.2/pdfxmeta/app.py
--rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf_tocgen-1.3.2/pdfxmeta/pdfxmeta.py
--rw-r--r--   0        0        0      970 2023-04-20 07:11:22.273494 pdf_tocgen-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    14648 1970-01-01 00:00:00.000000 pdf_tocgen-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.3/LICENSE
+-rw-r--r--   0        0        0    34523 2021-01-12 05:43:12.956399 pdf_tocgen-1.3.3/LICENSE_AGPL
+-rw-r--r--   0        0        0    13746 2023-04-20 21:09:30.179886 pdf_tocgen-1.3.3/README.md
+-rw-r--r--   0        0        0      274 2023-04-20 06:06:03.536966 pdf_tocgen-1.3.3/fitzutils/__init__.py
+-rw-r--r--   0        0        0     2875 2023-04-20 06:05:46.873633 pdf_tocgen-1.3.3/fitzutils/fitzutils.py
+-rw-r--r--   0        0        0       87 2023-04-20 22:09:23.189993 pdf_tocgen-1.3.3/pdftocgen/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.3/pdftocgen/__main__.py
+-rw-r--r--   0        0        0     4880 2023-04-20 06:15:48.496945 pdf_tocgen-1.3.3/pdftocgen/app.py
+-rw-r--r--   0        0        0     5399 2023-04-20 21:17:12.859870 pdf_tocgen-1.3.3/pdftocgen/filter.py
+-rw-r--r--   0        0        0     4977 2023-04-20 21:23:03.039858 pdf_tocgen-1.3.3/pdftocgen/recipe.py
+-rw-r--r--   0        0        0      454 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.3/pdftocgen/tocgen.py
+-rw-r--r--   0        0        0       73 2023-04-20 22:09:26.476659 pdf_tocgen-1.3.3/pdftocio/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.3/pdftocio/__main__.py
+-rw-r--r--   0        0        0     5797 2023-04-20 21:03:39.533232 pdf_tocgen-1.3.3/pdftocio/app.py
+-rw-r--r--   0        0        0      583 2023-04-20 20:50:27.753260 pdf_tocgen-1.3.3/pdftocio/tocio.py
+-rw-r--r--   0        0        0     1274 2021-02-06 20:25:15.540000 pdf_tocgen-1.3.3/pdftocio/tocparser.py
+-rw-r--r--   0        0        0      148 2023-04-20 22:09:30.056659 pdf_tocgen-1.3.3/pdfxmeta/__init__.py
+-rw-r--r--   0        0        0       61 2021-01-12 05:43:12.959732 pdf_tocgen-1.3.3/pdfxmeta/__main__.py
+-rw-r--r--   0        0        0     4212 2023-04-20 06:10:42.420289 pdf_tocgen-1.3.3/pdfxmeta/app.py
+-rw-r--r--   0        0        0     4728 2021-11-10 19:23:48.759908 pdf_tocgen-1.3.3/pdfxmeta/pdfxmeta.py
+-rw-r--r--   0        0        0      970 2023-04-20 22:09:11.433326 pdf_tocgen-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0    14744 1970-01-01 00:00:00.000000 pdf_tocgen-1.3.3/PKG-INFO
```

### Comparing `pdf_tocgen-1.3.2/LICENSE` & `pdf_tocgen-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/LICENSE_AGPL` & `pdf_tocgen-1.3.3/LICENSE_AGPL`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/README.md` & `pdf_tocgen-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,20 @@
 ```console
 $ pdftocio -o out.pdf doc.pdf < toc
 ```
 
 To copy the table of contents from `doc1.pdf` to `doc2.pdf`:
 
 ```console
-$ pdftocio doc1.pdf | pdftocio doc2.pdf
+$ pdftocio -v doc1.pdf | pdftocio doc2.pdf
 ```
 
+Note that the `-v` flag helps preserve the vertical
+positions of headings during the copy.
+
 To print the table of contents for reading:
 
 ```console
 $ pdftocio -H doc.pdf
 Level 1 heading 1 ··· 1
     Level 2 heading 1 ··· 1
         Level 3 heading 1 ··· 2
@@ -214,15 +217,15 @@
 
 ### `pdftocgen`
 
 If you have obtained an existing recipe `rcp.toml` for `doc.pdf`, you could
 apply it and print the outline to `stdout` by
 
 ```console
-$ pdftocio doc.pdf < rcp.toml
+$ pdftocgen doc.pdf < rcp.toml
 "Level 1 heading 1" 1
     "Level 2 heading 1" 1
         "Level 3 heading 1" 2
         "Level 3 heading 2" 3
     "Level 2 heading 2" 4
 "Level 1 heading 2" 5
 ```
```

### Comparing `pdf_tocgen-1.3.2/fitzutils/fitzutils.py` & `pdf_tocgen-1.3.3/fitzutils/fitzutils.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/pdftocgen/app.py` & `pdf_tocgen-1.3.3/pdftocgen/app.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/pdftocgen/filter.py` & `pdf_tocgen-1.3.3/pdftocgen/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,21 +134,22 @@
     # When set, the filter will be more *greedy* and extract all the text in a
     # block even when at least one match occurs
     greedy: bool
     font: FontFilter
     bbox: BoundingBoxFilter
 
     def __init__(self, fltr_dict: dict):
-        self.level = fltr_dict.get('level')
+        lvl = fltr_dict.get('level')
 
-        if self.level is None:
+        if lvl is None:
             raise ValueError("filter's 'level' is not set")
-        if self.level < 1:
+        if lvl < 1:
             raise ValueError("filter's 'level' must be >= 1")
 
+        self.level = lvl
         self.greedy = fltr_dict.get('greedy', False)
         self.font = FontFilter(fltr_dict.get('font', {}))
         self.bbox = BoundingBoxFilter(fltr_dict.get('bbox', {}))
 
     def admits(self, spn: dict) -> bool:
         """Check if the filter admits the span
```

### Comparing `pdf_tocgen-1.3.2/pdftocgen/recipe.py` & `pdf_tocgen-1.3.3/pdftocgen/recipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Iterator
 from .filter import ToCFilter
 from fitzutils import ToCEntry
 from itertools import chain
 from collections import defaultdict
 from fitz import Document
 
 
@@ -40,15 +40,15 @@
 @dataclass
 class Fragment:
     """A fragment of the extracted heading"""
     text: str
     level: int
 
 
-def concatFrag(frags: List[Optional[Fragment]], sep: str = " ") -> Dict[int, str]:
+def concatFrag(frags: Iterator[Optional[Fragment]], sep: str = " ") -> Dict[int, str]:
     """Concatenate fragments to strings
 
     Returns
       a dictionary (level -> title) that contains the title for each level.
     """
     # accumulate a list of strings for each level of heading
     acc = defaultdict(list)
```

### Comparing `pdf_tocgen-1.3.2/pdftocio/app.py` & `pdf_tocgen-1.3.3/pdftocio/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 options
   -h, --help            show help
   -t, --toc=toc         path to the table of contents generated by
                         pdftocgen. if this option is not given, the
                         default is stdin, but if no input is piped or
                         redirected to stdin, this program will instead
                         print the existing ToC of the PDF file
+  -v, --vpos            if this flag is set, the vertical position of
+                        each heading will be dumped to the output
   -p, --print           when flag is set, print the existing ToC in
                         the input PDF file. this flag is usually not
                         necessary, since it is the default behavior
                         when no input is given
   -H, --human-readable  print the toc in a readable format
   -o, --out=file.pdf    path to the output file. if this flag is not
                         specified, the default is {input}_out.pdf
@@ -80,33 +82,36 @@
 
 
 def main():
     # parse arguments
     try:
         opts, args = getopt.gnu_getopt(
             sys.argv[1:],
-            "ht:pHo:gV",
-            ["help", "toc=", "print", "human-readable", "out=", "debug", "version"]
+            "hvt:pHo:gV",
+            ["help", "vpos", "toc=", "print", "human-readable", "out=", "debug", "version"]
         )
     except GetoptError as e:
         print(e, file=sys.stderr)
         print(usage_s, file=sys.stderr)
         sys.exit(2)
 
     toc_file: TextIO = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8', errors='ignore')
     print_toc: bool = False
     readable: bool = False
     out: Optional[str] = None
+    vpos: bool = False
     debug: bool = False
 
     for o, a in opts:
         if o in ("-H", "--human-readable"):
             readable = True
         elif o in ("-p", "--print"):
             print_toc = True
+        elif o in ("-v", "--vpos"):
+            vpos = True
         elif o in ("-t", "--toc"):
             try:
                 toc_file = open(a, "r", encoding=get_file_encoding(a))
             except IOError as e:
                 print("error: can't open file for reading", file=sys.stderr)
                 print(e, file=sys.stderr)
                 sys.exit(1)
@@ -140,15 +145,15 @@
                     sys.exit(1)
 
                 stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8', errors='ignore')
 
                 if readable:
                     print(pprint_toc(toc), file=stdout)
                 else:
-                    print(dump_toc(toc), end="", file=stdout)
+                    print(dump_toc(toc, vpos), end="", file=stdout)
                 sys.exit(0)
 
             # an input is given, so switch to input mode
             toc = parse_toc(toc_file)
             write_toc(doc, toc)
 
             if out is None:
```

### Comparing `pdf_tocgen-1.3.2/pdftocio/tocparser.py` & `pdf_tocgen-1.3.3/pdftocio/tocparser.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/pdfxmeta/app.py` & `pdf_tocgen-1.3.3/pdfxmeta/app.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/pdfxmeta/pdfxmeta.py` & `pdf_tocgen-1.3.3/pdfxmeta/pdfxmeta.py`

 * *Files identical despite different names*

### Comparing `pdf_tocgen-1.3.2/pyproject.toml` & `pdf_tocgen-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf.tocgen"
-version = "1.3.2"
+version = "1.3.3"
 description = "Automatically generate table of contents for pdf files"
 authors = ["krasjet"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://krasjet.com/voice/pdf.tocgen/"
 repository = "https://github.com/Krasjet/pdf.tocgen"
 keywords = ["pdf", "cli"]
```

### Comparing `pdf_tocgen-1.3.2/PKG-INFO` & `pdf_tocgen-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-tocgen
-Version: 1.3.2
+Version: 1.3.3
 Summary: Automatically generate table of contents for pdf files
 Home-page: https://krasjet.com/voice/pdf.tocgen/
 License: GPL-3.0-or-later
 Keywords: pdf,cli
 Author: krasjet
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -218,17 +218,20 @@
 ```console
 $ pdftocio -o out.pdf doc.pdf < toc
 ```
 
 To copy the table of contents from `doc1.pdf` to `doc2.pdf`:
 
 ```console
-$ pdftocio doc1.pdf | pdftocio doc2.pdf
+$ pdftocio -v doc1.pdf | pdftocio doc2.pdf
 ```
 
+Note that the `-v` flag helps preserve the vertical
+positions of headings during the copy.
+
 To print the table of contents for reading:
 
 ```console
 $ pdftocio -H doc.pdf
 Level 1 heading 1 ··· 1
     Level 2 heading 1 ··· 1
         Level 3 heading 1 ··· 2
@@ -239,15 +242,15 @@
 
 ### `pdftocgen`
 
 If you have obtained an existing recipe `rcp.toml` for `doc.pdf`, you could
 apply it and print the outline to `stdout` by
 
 ```console
-$ pdftocio doc.pdf < rcp.toml
+$ pdftocgen doc.pdf < rcp.toml
 "Level 1 heading 1" 1
     "Level 2 heading 1" 1
         "Level 3 heading 1" 2
         "Level 3 heading 2" 3
     "Level 2 heading 2" 4
 "Level 1 heading 2" 5
 ```
```

