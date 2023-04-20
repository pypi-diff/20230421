# Comparing `tmp/wtfl-1.1.0.tar.gz` & `tmp/wtfl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtfl-1.1.0.tar", max compression
+gzip compressed data, was "wtfl-1.2.0.tar", max compression
```

## Comparing `wtfl-1.1.0.tar` & `wtfl-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-19 04:40:07.624410 wtfl-1.1.0/LICENSE
--rw-r--r--   0        0        0     9891 2023-04-19 04:40:07.624410 wtfl-1.1.0/README.md
--rw-r--r--   0        0        0      578 2023-04-19 04:40:07.624410 wtfl-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/__init__.py
--rw-r--r--   0        0        0     5035 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/grammar.py
--rw-r--r--   0        0        0     2789 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/internal_types.py
--rw-r--r--   0        0        0     6190 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/parser.py
--rw-r--r--   0        0        0     6899 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/reader.py
--rw-r--r--   0        0        0     4557 2023-04-19 04:40:07.624410 wtfl-1.1.0/wtfl/writer.py
--rw-r--r--   0        0        0    10730 1970-01-01 00:00:00.000000 wtfl-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-20 22:33:19.586953 wtfl-1.2.0/LICENSE
+-rw-r--r--   0        0        0     9899 2023-04-20 22:33:19.586953 wtfl-1.2.0/README.md
+-rw-r--r--   0        0        0      578 2023-04-20 22:33:19.586953 wtfl-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/__init__.py
+-rw-r--r--   0        0        0     5035 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/grammar.py
+-rw-r--r--   0        0        0     2789 2023-04-20 22:33:19.586953 wtfl-1.2.0/wtfl/internal_types.py
+-rw-r--r--   0        0        0     6349 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/parser.py
+-rw-r--r--   0        0        0     6899 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/reader.py
+-rw-r--r--   0        0        0     4557 2023-04-20 22:33:19.590953 wtfl-1.2.0/wtfl/writer.py
+-rw-r--r--   0        0        0    10738 1970-01-01 00:00:00.000000 wtfl-1.2.0/PKG-INFO
```

### Comparing `wtfl-1.1.0/LICENSE` & `wtfl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfl-1.1.0/README.md` & `wtfl-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     *,
     parse_float, # function for float parsing, `float` used by default
     parse_int, # function for integer parsing (only unprefixed decimal), `int` used by default
     parse_roman, # function for roman numerals parsing, accepts whole literal as a string (0r...)
     parse_numbers, # function for integer literals parsing (0b..., 0o..., and so on)
 ) -> 
 ```
-read an object from a file (same argument meaning as `.loads`):
+read an object from a file (same argument meaning as `.loads`):    
 `wtfl.load(file, *, parse_float, parse_int, parse_roman, parse_numbers)` 
 
 dump an object into a string:
 ```python
 def wtfl.dumps(
     obj: object, # object to dump
     *,
@@ -64,15 +64,15 @@
     # if current value is not serializable and skipkeys=False, tries to serialize the result of default(value)
     default: Callable[[object], str] | None = None, 
     
     # if True, sorts object keys
     sort_keys: bool = False,
 )
 ```
-dump an object into a file (same argument meaning as `.dumps()`):
+dump an object into a file (same argument meaning as `.dumps()`):    
 `wtfl.dump(file, obj, *, skipkeys, ensure_ascii, indent, default, sort_keys)`
 
 # Reserved keywords
 
 It is very important to know all the keywords of WTFL, since all those keywords are important.    
 
 Here's a list (keywords in the same list entry are equivalent and used interchangeably in the spec):
```

### Comparing `wtfl-1.1.0/pyproject.toml` & `wtfl-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wtfl"
-version = "1.1.0"
+version = "1.2.0"
 description = "Well-designed Text-based Friendly Language"
 authors = ["Dmitry Gritsenko <k01419q45@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/evtn/wtfl"
 homepage = "https://github.com/evtn/wtfl"
 keywords = ["markup", "config"]
```

### Comparing `wtfl-1.1.0/wtfl/grammar.py` & `wtfl-1.2.0/wtfl/grammar.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.1.0/wtfl/internal_types.py` & `wtfl-1.2.0/wtfl/internal_types.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.1.0/wtfl/parser.py` & `wtfl-1.2.0/wtfl/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
             else:
                 result += part_value
             current = [digit_value, 1]
     return result + current[0] * current[1]
 
 
 def parse_numbers(s: str) -> PythonValue:
+    if s[1] == "u":
+        return len(s) - 2
+
     bases = {
         "b": 2,
         "o": 8,
         "d": 10,
         "z": 12,
         "v": 20,
     }
@@ -113,15 +116,15 @@
         s = tokens[0]
 
         if "." in s:
             return WTFLTransformer.parse_float(s)
         return WTFLTransformer.parse_int(s)
 
     def integer(self, tokens):
-        return int(tokens[0])
+        return WTFLTransformer.parse_int(tokens[0])
 
     def negative(self, tokens):
         return -tokens[1]
 
     def roman(self, tokens):
         return WTFLTransformer.parse_roman(tokens[0])
 
@@ -136,14 +139,17 @@
 
     def duodecimal(self, tokens):
         return WTFLTransformer.parse_numbers(tokens[0])
 
     def vigesimal(self, tokens):
         return WTFLTransformer.parse_numbers(tokens[0])
 
+    def unary_int(self, tokens):
+        return WTFLTransformer.parse_numbers(tokens[0])
+
     def string(self, tokens):
         decoder = codecs.getdecoder("unicode_escape")
         return decoder(tokens[0][1:-1])[0]
 
     def object(self, tokens):
         [_, *pairs, _] = tokens
         return Object(pairs)
```

### Comparing `wtfl-1.1.0/wtfl/reader.py` & `wtfl-1.2.0/wtfl/reader.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.1.0/wtfl/writer.py` & `wtfl-1.2.0/wtfl/writer.py`

 * *Files identical despite different names*

### Comparing `wtfl-1.1.0/PKG-INFO` & `wtfl-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtfl
-Version: 1.1.0
+Version: 1.2.0
 Summary: Well-designed Text-based Friendly Language
 Home-page: https://github.com/evtn/wtfl
 License: MIT
 Keywords: markup,config
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.7,<4.0
@@ -62,15 +62,15 @@
     *,
     parse_float, # function for float parsing, `float` used by default
     parse_int, # function for integer parsing (only unprefixed decimal), `int` used by default
     parse_roman, # function for roman numerals parsing, accepts whole literal as a string (0r...)
     parse_numbers, # function for integer literals parsing (0b..., 0o..., and so on)
 ) -> 
 ```
-read an object from a file (same argument meaning as `.loads`):
+read an object from a file (same argument meaning as `.loads`):    
 `wtfl.load(file, *, parse_float, parse_int, parse_roman, parse_numbers)` 
 
 dump an object into a string:
 ```python
 def wtfl.dumps(
     obj: object, # object to dump
     *,
@@ -87,15 +87,15 @@
     # if current value is not serializable and skipkeys=False, tries to serialize the result of default(value)
     default: Callable[[object], str] | None = None, 
     
     # if True, sorts object keys
     sort_keys: bool = False,
 )
 ```
-dump an object into a file (same argument meaning as `.dumps()`):
+dump an object into a file (same argument meaning as `.dumps()`):    
 `wtfl.dump(file, obj, *, skipkeys, ensure_ascii, indent, default, sort_keys)`
 
 # Reserved keywords
 
 It is very important to know all the keywords of WTFL, since all those keywords are important.    
 
 Here's a list (keywords in the same list entry are equivalent and used interchangeably in the spec):
```

