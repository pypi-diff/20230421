# Comparing `tmp/samarium-0.5.1.tar.gz` & `tmp/samarium-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samarium-0.5.1.tar", max compression
+gzip compressed data, was "samarium-0.5.2.tar", max compression
```

## Comparing `samarium-0.5.1.tar` & `samarium-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1059 2023-04-02 20:20:07.460871 samarium-0.5.1/LICENSE
--rw-r--r--   0        0        0     2304 2023-04-02 22:14:04.461419 samarium-0.5.1/README.md
--rw-r--r--   0        0        0      681 2023-04-07 22:18:25.805970 samarium-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1424 2023-04-02 20:20:07.478242 samarium-0.5.1/src/samarium/__init__.py
--rw-r--r--   0        0        0       70 2023-01-19 17:08:28.384405 samarium-0.5.1/src/samarium/__main__.py
--rw-r--r--   0        0        0     2852 2023-04-02 20:20:07.478578 samarium-0.5.1/src/samarium/builtins.py
--rw-r--r--   0        0        0      674 2023-04-02 20:20:07.478901 samarium-0.5.1/src/samarium/classes/__init__.py
--rw-r--r--   0        0        0    33210 2023-04-07 21:00:46.672638 samarium-0.5.1/src/samarium/classes/base.py
--rw-r--r--   0        0        0     6092 2023-04-02 20:20:07.479723 samarium-0.5.1/src/samarium/classes/fileio.py
--rw-r--r--   0        0        0     2883 2023-04-02 20:20:07.480066 samarium-0.5.1/src/samarium/core.py
--rw-r--r--   0        0        0     4142 2023-04-02 20:20:07.480371 samarium-0.5.1/src/samarium/exceptions.py
--rw-r--r--   0        0        0     3471 2023-04-02 20:20:07.480686 samarium-0.5.1/src/samarium/imports.py
--rw-r--r--   0        0        0     6354 2023-04-02 20:20:07.481371 samarium-0.5.1/src/samarium/modules/collections.sm
--rw-r--r--   0        0        0     4198 2023-04-02 20:20:07.481761 samarium-0.5.1/src/samarium/modules/datetime.sm
--rw-r--r--   0        0        0     1618 2023-04-02 20:20:07.482061 samarium-0.5.1/src/samarium/modules/io.sm
--rw-r--r--   0        0        0     3925 2023-04-02 20:20:07.482459 samarium-0.5.1/src/samarium/modules/iter.sm
--rw-r--r--   0        0        0     2123 2023-04-02 20:20:07.482978 samarium-0.5.1/src/samarium/modules/math.sm
--rw-r--r--   0        0        0      646 2023-01-19 17:08:28.381214 samarium-0.5.1/src/samarium/modules/operator.sm
--rw-r--r--   0        0        0      169 2023-04-02 20:20:07.483436 samarium-0.5.1/src/samarium/modules/pystd.py
--rw-r--r--   0        0        0      711 2023-04-02 20:20:07.483957 samarium-0.5.1/src/samarium/modules/random.sm
--rw-r--r--   0        0        0     6975 2023-04-02 20:20:07.484269 samarium-0.5.1/src/samarium/modules/string.sm
--rw-r--r--   0        0        0     2378 2023-04-02 20:20:07.484856 samarium-0.5.1/src/samarium/modules/types.sm
--rw-r--r--   0        0        0     3157 2023-04-02 20:20:07.485169 samarium-0.5.1/src/samarium/python.py
--rw-r--r--   0        0        0       40 2023-01-19 17:08:28.377552 samarium-0.5.1/src/samarium/runtime.py
--rw-r--r--   0        0        0     1174 2023-04-02 20:20:07.485455 samarium-0.5.1/src/samarium/shell.py
--rw-r--r--   0        0        0      492 2023-04-02 20:20:07.485672 samarium-0.5.1/src/samarium/template.py
--rw-r--r--   0        0        0     1285 2023-04-02 20:20:07.485907 samarium-0.5.1/src/samarium/tokenizer.py
--rw-r--r--   0        0        0     2180 2023-01-19 17:08:28.373894 samarium-0.5.1/src/samarium/tokens.py
--rw-r--r--   0        0        0    27167 2023-04-07 21:19:04.255490 samarium-0.5.1/src/samarium/transpiler.py
--rw-r--r--   0        0        0     3050 2023-04-07 22:18:24.791295 samarium-0.5.1/src/samarium/utils.py
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 samarium-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-21 03:42:28.355286 samarium-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2304 2023-04-21 03:42:28.355376 samarium-0.5.2/README.md
+-rw-r--r--   0        0        0      681 2023-04-21 03:43:02.453014 samarium-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1424 2023-04-21 03:42:28.359480 samarium-0.5.2/src/samarium/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-21 03:42:28.359539 samarium-0.5.2/src/samarium/__main__.py
+-rw-r--r--   0        0        0     2852 2023-04-21 03:42:28.359628 samarium-0.5.2/src/samarium/builtins.py
+-rw-r--r--   0        0        0      674 2023-04-21 03:42:28.359737 samarium-0.5.2/src/samarium/classes/__init__.py
+-rw-r--r--   0        0        0    33210 2023-04-21 03:42:28.359987 samarium-0.5.2/src/samarium/classes/base.py
+-rw-r--r--   0        0        0     6092 2023-04-21 03:42:28.360083 samarium-0.5.2/src/samarium/classes/fileio.py
+-rw-r--r--   0        0        0     2883 2023-04-21 03:42:28.360162 samarium-0.5.2/src/samarium/core.py
+-rw-r--r--   0        0        0     4142 2023-04-21 03:42:28.360239 samarium-0.5.2/src/samarium/exceptions.py
+-rw-r--r--   0        0        0     3471 2023-04-21 03:42:28.360315 samarium-0.5.2/src/samarium/imports.py
+-rw-r--r--   0        0        0     6354 2023-04-21 03:42:28.360431 samarium-0.5.2/src/samarium/modules/collections.sm
+-rw-r--r--   0        0        0     4198 2023-04-21 03:42:28.360515 samarium-0.5.2/src/samarium/modules/datetime.sm
+-rw-r--r--   0        0        0     1618 2023-04-21 03:42:28.360579 samarium-0.5.2/src/samarium/modules/io.sm
+-rw-r--r--   0        0        0     3925 2023-04-21 03:42:28.360655 samarium-0.5.2/src/samarium/modules/iter.sm
+-rw-r--r--   0        0        0     2123 2023-04-21 03:42:28.360722 samarium-0.5.2/src/samarium/modules/math.sm
+-rw-r--r--   0        0        0      646 2023-04-21 03:42:28.360786 samarium-0.5.2/src/samarium/modules/operator.sm
+-rw-r--r--   0        0        0      169 2023-04-21 03:42:28.360845 samarium-0.5.2/src/samarium/modules/pystd.py
+-rw-r--r--   0        0        0      711 2023-04-21 03:42:28.360905 samarium-0.5.2/src/samarium/modules/random.sm
+-rw-r--r--   0        0        0     6975 2023-04-21 03:42:28.360984 samarium-0.5.2/src/samarium/modules/string.sm
+-rw-r--r--   0        0        0     2378 2023-04-21 03:42:28.361045 samarium-0.5.2/src/samarium/modules/types.sm
+-rw-r--r--   0        0        0     3157 2023-04-21 03:42:28.361123 samarium-0.5.2/src/samarium/python.py
+-rw-r--r--   0        0        0       40 2023-04-21 03:42:28.361180 samarium-0.5.2/src/samarium/runtime.py
+-rw-r--r--   0        0        0     1174 2023-04-21 03:42:28.361249 samarium-0.5.2/src/samarium/shell.py
+-rw-r--r--   0        0        0      492 2023-04-21 03:42:28.361311 samarium-0.5.2/src/samarium/template.py
+-rw-r--r--   0        0        0     1285 2023-04-21 03:42:28.361371 samarium-0.5.2/src/samarium/tokenizer.py
+-rw-r--r--   0        0        0     2180 2023-04-21 03:42:28.361441 samarium-0.5.2/src/samarium/tokens.py
+-rw-r--r--   0        0        0    27167 2023-04-21 03:42:28.361614 samarium-0.5.2/src/samarium/transpiler.py
+-rw-r--r--   0        0        0     3050 2023-04-21 03:43:24.675294 samarium-0.5.2/src/samarium/utils.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 samarium-0.5.2/PKG-INFO
```

### Comparing `samarium-0.5.1/LICENSE` & `samarium-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/README.md` & `samarium-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/pyproject.toml` & `samarium-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "samarium"
-version = "0.5.1"
+version = "0.5.2"
 description = "The Samarium Programming Language"
 authors = ["trag1c <trag1cdev@yahoo.com>"]
 license = "MIT"
 documentation = "https://samarium-lang.github.io/Samarium/"
 repository = "https://github.com/samarium-lang/Samarium"
 readme = "README.md"
```

### Comparing `samarium-0.5.1/src/samarium/__init__.py` & `samarium-0.5.2/src/samarium/__init__.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/builtins.py` & `samarium-0.5.2/src/samarium/builtins.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/classes/__init__.py` & `samarium-0.5.2/src/samarium/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/classes/base.py` & `samarium-0.5.2/src/samarium/classes/base.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/classes/fileio.py` & `samarium-0.5.2/src/samarium/classes/fileio.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/core.py` & `samarium-0.5.2/src/samarium/core.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/exceptions.py` & `samarium-0.5.2/src/samarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/imports.py` & `samarium-0.5.2/src/samarium/imports.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/collections.sm` & `samarium-0.5.2/src/samarium/modules/collections.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/datetime.sm` & `samarium-0.5.2/src/samarium/modules/datetime.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/io.sm` & `samarium-0.5.2/src/samarium/modules/io.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/iter.sm` & `samarium-0.5.2/src/samarium/modules/iter.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/math.sm` & `samarium-0.5.2/src/samarium/modules/math.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/operator.sm` & `samarium-0.5.2/src/samarium/modules/operator.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/random.sm` & `samarium-0.5.2/src/samarium/modules/random.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/string.sm` & `samarium-0.5.2/src/samarium/modules/string.sm`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/modules/types.sm` & `samarium-0.5.2/src/samarium/modules/types.sm`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Array: []?!;
-Integer: \?!;
+Number: \?!;
 Null: (||)?!;
 Slice: <<>>?!;
 String: ""?!;
 Table: {{}}?!;
 Zip: ("" >< "")?!;
 
 
@@ -107,8 +107,8 @@
     ->? element * { * element ->? '#val; }
     ... * { ... i ->? '#val { ** i; } }
     <<>> index * { * '#val<<index>>; }
     >< other * { * '#val >< other; }
     :: other * { * '#val :: other.#val; }
     ? * { * / ? '#val ,, \; }
     $ * { * '#val$; }
-}
+}
```

### Comparing `samarium-0.5.1/src/samarium/python.py` & `samarium-0.5.2/src/samarium/python.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/shell.py` & `samarium-0.5.2/src/samarium/shell.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/tokenizer.py` & `samarium-0.5.2/src/samarium/tokenizer.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/tokens.py` & `samarium-0.5.2/src/samarium/tokens.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/transpiler.py` & `samarium-0.5.2/src/samarium/transpiler.py`

 * *Files identical despite different names*

### Comparing `samarium-0.5.1/src/samarium/utils.py` & `samarium-0.5.2/src/samarium/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Callable
 from re import sub
 from typing import Any, TypeVar
 
 from .exceptions import SamariumTypeError, SamariumValueError
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 T = TypeVar("T")
 
 
 KT = TypeVar("KT")
 VT = TypeVar("VT")
```

### Comparing `samarium-0.5.1/PKG-INFO` & `samarium-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samarium
-Version: 0.5.1
+Version: 0.5.2
 Summary: The Samarium Programming Language
 Home-page: https://github.com/samarium-lang/Samarium
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

