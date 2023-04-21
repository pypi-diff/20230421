# Comparing `tmp/ledes-parser-1.0.1.tar.gz` & `tmp/ledes-parser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledes-parser-1.0.1.tar", last modified: Sun Apr 16 20:38:03 2023, max compression
+gzip compressed data, was "ledes-parser-1.0.3.tar", last modified: Fri Apr 21 17:43:12 2023, max compression
```

## Comparing `ledes-parser-1.0.1.tar` & `ledes-parser-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:38:03.424297 ledes-parser-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 20:38:03.424297 ledes-parser-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:38:03.420297 ledes-parser-1.0.1/ledes_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/base_ledes_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/ledes_1998BIV2_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/ledes_1998BI_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/ledes_1998B_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/ledes_dynamic_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:38:03.420297 ledes-parser-1.0.1/ledes_parser/typings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/typings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/ledes_parser/typings/invoice_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:38:03.420297 ledes-parser-1.0.1/ledes_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 20:38:03.000000 ledes-parser-1.0.1/ledes_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-16 20:38:03.000000 ledes-parser-1.0.1/ledes_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:38:03.000000 ledes-parser-1.0.1/ledes_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 20:38:03.000000 ledes-parser-1.0.1/ledes_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 20:38:03.424297 ledes-parser-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:38:03.424297 ledes-parser-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/tests/test_dynamic_ledes_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/tests/test_ledes_1998B_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 20:37:48.000000 ledes-parser-1.0.1/tests/test_parse_leads_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:43:12.434146 ledes-parser-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-21 17:43:12.434146 ledes-parser-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:43:12.430146 ledes-parser-1.0.3/ledes_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-21 17:42:47.000000 ledes-parser-1.0.3/ledes_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/base_ledes_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/ledes_1998BIV2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/ledes_1998BI_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/ledes_1998B_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/ledes_dynamic_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:43:12.430146 ledes-parser-1.0.3/ledes_parser/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/ledes_parser/typings/invoice_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:43:12.430146 ledes-parser-1.0.3/ledes_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-21 17:43:12.000000 ledes-parser-1.0.3/ledes_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 17:43:12.000000 ledes-parser-1.0.3/ledes_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:43:12.000000 ledes-parser-1.0.3/ledes_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 17:43:12.000000 ledes-parser-1.0.3/ledes_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:43:12.434146 ledes-parser-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:43:12.434146 ledes-parser-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/tests/test_dynamic_ledes_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/tests/test_ledes_1998B_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 17:42:46.000000 ledes-parser-1.0.3/tests/test_parse_leads_file.py
```

### Comparing `ledes-parser-1.0.1/LICENSE` & `ledes-parser-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ledes-parser-1.0.1/README.md` & `ledes-parser-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pip install ledes-parser
 ```
 # Example Usage
 ```python
 from ledes_parser import parse_ledes_file
 
 with open('path/to/the/ledes_file.txt', 'r') as f:
-    invoices = parse_ledes_file(f, "1998")
+    invoices = parse_ledes_file(f, "1998B")
     print(invoices)
 ```
 
 # LEDES File Formats
 This package supports the following LEDES file formats:
 
 * LEDES98B
@@ -27,8 +27,8 @@
 * (TBD) LEDESXML20
 * (TBD) LEDESXML21
 
 # Contributing
 Fork the repository on GitHub.
 Create a new branch with your changes.
 Commit your changes and push them to your fork.
-Create a pull request against the main branch of the original repository.
+Create a pull request against the main branch of the original repository.
```

### Comparing `ledes-parser-1.0.1/ledes_parser/__init__.py` & `ledes-parser-1.0.3/ledes_parser/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, TextIO
 
 from ledes_parser.ledes_1998B_parser import Ledes1998BParser
 from ledes_parser.ledes_1998BI_parser import Ledes1998BIParser
 
 from .typings.invoice_types import Invoice
 
+__version__ = "1.0.3"
 
 def parse_ledes_file(file: TextIO, ledes_format: str) -> List[Invoice]:
     """
     Parses a LEDES file based on the provided format and returns a list of Invoice objects.
 
     :param file: A file-like object (TextIO) containing the LEDES data to parse.
     :param ledes_format: A string specifying the LEDES format of the input data.
```

### Comparing `ledes-parser-1.0.1/ledes_parser/ledes_1998BIV2_parser.py` & `ledes-parser-1.0.3/ledes_parser/ledes_1998BIV2_parser.py`

 * *Files identical despite different names*

### Comparing `ledes-parser-1.0.1/ledes_parser/ledes_dynamic_parser.py` & `ledes-parser-1.0.3/ledes_parser/ledes_dynamic_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import json
-from typing import List, TextIO
+from typing import Iterable, List
 
 from .typings.invoice_types import Invoice
 
 field_to_property_map = {
-  'INVOICE_DATE': 'invoice_date'
+    'INVOICE_DATE': 'invoice_date'
 }
 
+
 class DynamicLEDESParser:
     def __init__(self, format_file: str):
         with open(format_file, 'r') as f:
             self.format_data = json.load(f)
-        self.field_codes = [field["code"] for field in self.format_data["fields"]]
+        self.field_codes = [field["code"]
+                            for field in self.format_data["fields"]]
 
-    def parse(self, input_data: TextIO) -> List[Invoice]:
+    def parse(self, csv_data: Iterable[str]) -> List[Invoice]:
         invoices = []
-        for line in input_data:
+        for line in csv_data:
             line_parts = line.strip().split('\t')
             invoice_data = {}
             for idx, field_code in enumerate(self.field_codes):
                 invoice_data[field_code] = line_parts[idx]
             invoices.append(Invoice(**invoice_data))
         return invoices
-
-# Usage example
-parser = DynamicLEDESParser('path/to/ledes_1998.json')
-
-with open('path/to/ledes_file.txt', 'r') as file:
-    invoices = parser.parse(file)
-
-print(invoices)
```

### Comparing `ledes-parser-1.0.1/ledes_parser/typings/invoice_types.py` & `ledes-parser-1.0.3/ledes_parser/typings/invoice_types.py`

 * *Files identical despite different names*

### Comparing `ledes-parser-1.0.1/ledes_parser.egg-info/SOURCES.txt` & `ledes-parser-1.0.3/ledes_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ledes-parser-1.0.1/tests/test_dynamic_ledes_parser.py` & `ledes-parser-1.0.3/tests/test_dynamic_ledes_parser.py`

 * *Files identical despite different names*

### Comparing `ledes-parser-1.0.1/tests/test_ledes_1998B_parser.py` & `ledes-parser-1.0.3/tests/test_ledes_1998B_parser.py`

 * *Files identical despite different names*

