# Comparing `tmp/jittok-0.0.4.tar.gz` & `tmp/jittok-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jittok-0.0.4.tar", last modified: Fri Mar 17 12:59:18 2023, max compression
+gzip compressed data, was "jittok-0.0.5.tar", last modified: Fri Apr 21 15:07:01 2023, max compression
```

## Comparing `jittok-0.0.4.tar` & `jittok-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.547117 jittok-0.0.4/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1073 2022-10-23 11:33:34.000000 jittok-0.0.4/LICENSE
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      767 2023-03-17 12:59:18.547117 jittok-0.0.4/PKG-INFO
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      465 2023-02-24 15:16:15.000000 jittok-0.0.4/README.md
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.543117 jittok-0.0.4/jittok/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2023-03-17 12:59:03.000000 jittok-0.0.4/jittok/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       30 2023-02-14 13:34:36.000000 jittok-0.0.4/jittok/__main__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      497 2023-02-14 13:34:36.000000 jittok-0.0.4/jittok/cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2022-11-08 13:52:24.000000 jittok-0.0.4/jittok/core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       36 2022-11-08 13:52:24.000000 jittok-0.0.4/jittok/exceptions.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.547117 jittok-0.0.4/jittok/jpdatetime/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       51 2023-03-16 13:16:33.000000 jittok-0.0.4/jittok/jpdatetime/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1832 2023-03-16 13:16:33.000000 jittok-0.0.4/jittok/jpdatetime/core.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.547117 jittok-0.0.4/jittok/jptext/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      303 2023-03-02 13:14:13.000000 jittok-0.0.4/jittok/jptext/__init__.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      422 2023-02-14 13:34:36.000000 jittok-0.0.4/jittok/jptext/cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     6196 2023-03-16 11:12:43.000000 jittok-0.0.4/jittok/jptext/core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      146 2023-02-13 12:57:35.000000 jittok-0.0.4/jittok/jptext/exceptions.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        0 2023-02-15 00:21:42.000000 jittok-0.0.4/jittok/py.typed
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.547117 jittok-0.0.4/jittok.egg-info/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      767 2023-03-17 12:59:18.000000 jittok-0.0.4/jittok.egg-info/PKG-INFO
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      491 2023-03-17 12:59:18.000000 jittok-0.0.4/jittok.egg-info/SOURCES.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        1 2023-03-17 12:59:18.000000 jittok-0.0.4/jittok.egg-info/dependency_links.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       81 2023-03-17 12:59:18.000000 jittok-0.0.4/jittok.egg-info/requires.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)        7 2023-03-17 12:59:18.000000 jittok-0.0.4/jittok.egg-info/top_level.txt
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       38 2023-03-17 12:59:18.547117 jittok-0.0.4/setup.cfg
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      886 2023-03-17 12:59:03.000000 jittok-0.0.4/setup.py
-drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-03-17 12:59:18.547117 jittok-0.0.4/tests/
--rw-rw-r--   0 osoken    (1000) osoken    (1000)     1600 2023-02-14 13:34:36.000000 jittok-0.0.4/tests/test_cli.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)      253 2023-02-14 13:34:36.000000 jittok-0.0.4/tests/test_core.py
--rw-rw-r--   0 osoken    (1000) osoken    (1000)       98 2022-10-31 11:27:53.000000 jittok-0.0.4/tests/test_package.py
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1073 2022-10-23 11:33:34.000000 jittok-0.0.5/LICENSE
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1369 2023-04-21 15:07:01.189279 jittok-0.0.5/PKG-INFO
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1067 2023-03-20 14:04:49.000000 jittok-0.0.5/README.md
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2023-04-21 15:05:21.000000 jittok-0.0.5/jittok/__init__.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       30 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/__main__.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      497 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/cli.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      233 2022-11-08 13:52:24.000000 jittok-0.0.5/jittok/core.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       36 2022-11-08 13:52:24.000000 jittok-0.0.5/jittok/exceptions.py
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/jpaddress/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      123 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/__init__.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     6525 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/core.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      150 2023-03-24 14:39:08.000000 jittok-0.0.5/jittok/jpaddress/exceptions.py
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok/jpdatetime/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       51 2023-03-20 14:04:49.000000 jittok-0.0.5/jittok/jpdatetime/__init__.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1832 2023-03-20 14:04:49.000000 jittok-0.0.5/jittok/jpdatetime/core.py
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/jittok/jptext/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      303 2023-03-02 13:14:13.000000 jittok-0.0.5/jittok/jptext/__init__.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      422 2023-02-14 13:34:36.000000 jittok-0.0.5/jittok/jptext/cli.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     6389 2023-04-21 15:02:22.000000 jittok-0.0.5/jittok/jptext/core.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      146 2023-02-13 12:57:35.000000 jittok-0.0.5/jittok/jptext/exceptions.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)        0 2023-02-15 00:21:42.000000 jittok-0.0.5/jittok/py.typed
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.185279 jittok-0.0.5/jittok.egg-info/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1369 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/PKG-INFO
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      576 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/SOURCES.txt
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)        1 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/dependency_links.txt
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       81 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/requires.txt
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)        7 2023-04-21 15:07:01.000000 jittok-0.0.5/jittok.egg-info/top_level.txt
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       38 2023-04-21 15:07:01.189279 jittok-0.0.5/setup.cfg
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1164 2023-03-24 15:17:43.000000 jittok-0.0.5/setup.py
+drwxrwxr-x   0 osoken    (1000) osoken    (1000)        0 2023-04-21 15:07:01.189279 jittok-0.0.5/tests/
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)     1600 2023-02-14 13:34:36.000000 jittok-0.0.5/tests/test_cli.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)      253 2023-02-14 13:34:36.000000 jittok-0.0.5/tests/test_core.py
+-rw-rw-r--   0 osoken    (1000) osoken    (1000)       98 2022-10-31 11:27:53.000000 jittok-0.0.5/tests/test_package.py
```

### Comparing `jittok-0.0.4/LICENSE` & `jittok-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jittok-0.0.4/PKG-INFO` & `jittok-0.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittok
-Version: 0.0.4
+Version: 0.0.5
 Summary: Swiss Army Knife-like toolbox for data processing
 Home-page: https://github.com/osoken/jittok
 Author: osoken
 Author-email: osoken.devel@outlook.jp
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -35,7 +35,27 @@
 #### parsing Japanese numeric string
 
 ```
 >>> from jittok import jptext
 >>> jptext.to_numeric("一二,三四五億2百十万987")
 1234502100987
 ```
+
+### `jpdatetime` - Japanese datetime related functions
+
+#### parsing Japanese "wareki" string
+
+```
+>>> from jittok import jpdatetime
+>>> jpdatetime.strptime("令和元年10月3日", "%Y年%m月%d日")
+datetime.datetime(2019, 10, 3, 0, 0)
+>>> jpdatetime.strptime("昭和64年1月1日", "%Y年%m月%d日")
+datetime.datetime(1989, 1, 1, 0, 0)
+```
+
+It parses `"明治"`, `"大正"`, `"昭和"`, `"平成"`, `"令和"` and does not support consistency check:
+
+```
+>>> from jittok import jpdatetime
+>>> jpdatetime.strptime("大正90年10月3日", "%Y年%m月%d日")
+datetime.datetime(2001, 10, 3, 0, 0)
+```
```

### Comparing `jittok-0.0.4/jittok/jpdatetime/core.py` & `jittok-0.0.5/jittok/jpdatetime/core.py`

 * *Files identical despite different names*

### Comparing `jittok-0.0.4/jittok/jptext/core.py` & `jittok-0.0.5/jittok/jptext/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 
 def guess_encoding(x: bytes, hint: Optional[Union[str, PatternT]] = None) -> str:
     if hint is None:
         return guess_encoding(
             x,
             regex.compile(
-                r'[\p{Script=Han}\u3041-\u309F\u30A1-\u30FF\uFF01-\uFF0F\uFF1A-\uFF20'
-                r'\uFF3B-\uFF40\uFF5B-\uFF65\u3000-\u303F]+'
+                r"[\p{Script=Han}\u3041-\u309F\u30A1-\u30FF\uFF01-\uFF0F\uFF1A-\uFF20"
+                r"\uFF3B-\uFF40\uFF5B-\uFF65\u3000-\u303F]+"
             ),
         )
     if isinstance(hint, str):
         return guess_encoding(x, re.compile(hint))
     for c in codec_list:
         try:
             buf = x.decode(c)
@@ -55,28 +55,28 @@
 
 def decode(x: bytes) -> str:
     return x.decode(guess_encoding(x))
 
 
 _basic_number_string = r"(?:(?:(?:[0-9]{0,3})(?:,[0-9]{3})+)|(?:[0-9]*))(?:\.[0-9]+)?"
 _four_digits_string_regex_str = (
-    fr"^((?P<千>{_basic_number_string})千)?"
-    fr"((?P<百>{_basic_number_string})百)?"
-    fr"((?P<十>{_basic_number_string})十)?"
-    fr"((?P<一>{_basic_number_string}))?$"
+    rf"^((?P<千>{_basic_number_string})千)?"
+    rf"((?P<百>{_basic_number_string})百)?"
+    rf"((?P<十>{_basic_number_string})十)?"
+    rf"((?P<一>{_basic_number_string}))?$"
 )
 
 numeric_string_regex = re.compile(
     r"^(?P<minus>-)?"
     + "".join(
         (
-            fr"(?:(?P<{dig}>({_basic_number_string}千)?"
-            fr"({_basic_number_string}百)?"
-            fr"({_basic_number_string}十)?"
-            fr"({_basic_number_string})?)?{dig})?"
+            rf"(?:(?P<{dig}>({_basic_number_string}千)?"
+            rf"({_basic_number_string}百)?"
+            rf"({_basic_number_string}十)?"
+            rf"({_basic_number_string})?)?{dig})?"
             for dig in [
                 "無量大数",
                 "不可思議",
                 "那由他",
                 "阿僧祇",
                 "恒河沙",
                 "極",
@@ -91,18 +91,18 @@
                 "兆",
                 "億",
                 "万",
             ]
         )
     )
     + (
-        fr"(?P<一>({_basic_number_string}千)?"
-        fr"({_basic_number_string}百)?"
-        fr"({_basic_number_string}十)?"
-        fr"({_basic_number_string})?)?$"
+        rf"(?P<一>({_basic_number_string}千)?"
+        rf"({_basic_number_string}百)?"
+        rf"({_basic_number_string}十)?"
+        rf"({_basic_number_string})?)?$"
     )
 )
 
 _four_digits_string_regex = re.compile(_four_digits_string_regex_str)
 trans_map = str.maketrans(
     {
         "１": "1",
@@ -204,33 +204,40 @@
         "⁻": "-",
         "₋": "-",
         "−": "-",
         "　": " ",
         "\u200b": " ",
         "\ufeff": " ",
         "\t": " ",
-        "“": "\"",
-        "”": "\"",
+        "“": '"',
+        "”": '"',
         "‘": "'",
         "’": "'",
     }
 )
 
 parentheses_left = re.compile(r"([^\s(])\(")
 parentheses_right = re.compile(r"\)([^\s)])")
 
 
-def normalize(x: str, newline_to_space: bool = False, remove_multiple_spaces: bool = False) -> str:
+def normalize(
+    x: str,
+    newline_to_space: bool = False,
+    remove_multiple_spaces: bool = False,
+    remove_variation_selectors: bool = False,
+) -> str:
     normalized_string = parentheses_right.sub(
         r") \1", parentheses_left.sub(r"\1 (", unicodedata.normalize("NFKC", x).translate(normalize_trans_map))
     )
     if newline_to_space:
         normalized_string = re.sub(r"[\n\r]", " ", normalized_string)
     if remove_multiple_spaces:
-        return re.sub(r" +", " ", normalized_string)
+        normalized_string = re.sub(r" +", " ", normalized_string)
+    if remove_variation_selectors:
+        normalized_string = re.sub(r"[\U000e0100-\U000e01ef]", "", normalized_string)
     return normalized_string
 
 
 def kanji_to_kana(x: str) -> str:
     return "".join(d["kana"] for d in kks.convert(x))
```

### Comparing `jittok-0.0.4/jittok.egg-info/PKG-INFO` & `jittok-0.0.5/jittok.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jittok
-Version: 0.0.4
+Version: 0.0.5
 Summary: Swiss Army Knife-like toolbox for data processing
 Home-page: https://github.com/osoken/jittok
 Author: osoken
 Author-email: osoken.devel@outlook.jp
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -35,7 +35,27 @@
 #### parsing Japanese numeric string
 
 ```
 >>> from jittok import jptext
 >>> jptext.to_numeric("一二,三四五億2百十万987")
 1234502100987
 ```
+
+### `jpdatetime` - Japanese datetime related functions
+
+#### parsing Japanese "wareki" string
+
+```
+>>> from jittok import jpdatetime
+>>> jpdatetime.strptime("令和元年10月3日", "%Y年%m月%d日")
+datetime.datetime(2019, 10, 3, 0, 0)
+>>> jpdatetime.strptime("昭和64年1月1日", "%Y年%m月%d日")
+datetime.datetime(1989, 1, 1, 0, 0)
+```
+
+It parses `"明治"`, `"大正"`, `"昭和"`, `"平成"`, `"令和"` and does not support consistency check:
+
+```
+>>> from jittok import jpdatetime
+>>> jpdatetime.strptime("大正90年10月3日", "%Y年%m月%d日")
+datetime.datetime(2001, 10, 3, 0, 0)
+```
```

### Comparing `jittok-0.0.4/tests/test_cli.py` & `jittok-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

