# Comparing `tmp/fmts-0.1.4.tar.gz` & `tmp/fmts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmts-0.1.4.tar", max compression
+gzip compressed data, was "fmts-0.1.5.tar", max compression
```

## Comparing `fmts-0.1.4.tar` & `fmts-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    46138 2022-09-19 18:35:17.072113 fmts-0.1.4/fmts/__init__.py
--rw-r--r--   0        0        0      229 2022-02-08 18:01:19.714971 fmts-0.1.4/fmts/__main__.py
--rw-r--r--   0        0        0      200 2022-09-19 18:35:17.073113 fmts-0.1.4/fmts/_meta.py
--rw-r--r--   0        0        0        0 2022-02-08 18:01:19.714971 fmts-0.1.4/fmts/py.typed
--rw-r--r--   0        0        0     2256 2022-09-19 18:35:17.073113 fmts-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      765 2022-08-17 14:07:03.986595 fmts-0.1.4/README.md
--rw-r--r--   0        0        0     1406 1970-01-01 00:00:00.000000 fmts-0.1.4/setup.py
--rw-r--r--   0        0        0     1889 1970-01-01 00:00:00.000000 fmts-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      277 2023-04-20 23:19:54.396173 fmts-0.1.5/fmts/__about__.py
+-rw-r--r--   0        0        0    49718 2023-04-20 20:51:48.605177 fmts-0.1.5/fmts/__init__.py
+-rw-r--r--   0        0        0      473 2023-04-20 20:51:48.622821 fmts-0.1.5/fmts/__main__.py
+-rw-r--r--   0        0        0      343 2023-04-20 20:38:23.577137 fmts-0.1.5/fmts/_meta.py
+-rw-r--r--   0        0        0        0 2022-02-08 18:01:19.714971 fmts-0.1.5/fmts/py.typed
+-rw-r--r--   0        0        0     2535 2023-04-20 23:43:39.971887 fmts-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      765 2022-08-17 14:07:03.986595 fmts-0.1.5/README.md
+-rw-r--r--   0        0        0     1890 1970-01-01 00:00:00.000000 fmts-0.1.5/PKG-INFO
```

### Comparing `fmts-0.1.4/fmts/__init__.py` & `fmts-0.1.5/fmts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
-from fmts._meta import __version__
+from fmts.__about__ import __version__
 
 # END IMPORTS
 
 _R = TypeVar("_R")
 
 # characters strings
 CAMEL_CHARACTERS: str = ascii_letters + digits + "_"  # also works for pascal case
@@ -802,17 +802,17 @@
     filelines = string.splitlines(keepends=False)
     comment_re = re.compile(r'(?:"(?:[^"\\]|\\.)*"|[^"#])*(#|$)')
 
     def _strip_comments_line(line: str) -> str:
         comment_re_match = comment_re.match(line)
         if comment_re_match:
             return line[: comment_re_match.start(1)]
-        return line
+        return line  # pragma: no cover
 
-    return "\n".join((_strip_comments_line(line) for line in filelines))
+    return "\n".join(_strip_comments_line(line) for line in filelines)
 
 
 def multi_replace(
     string: str,
     replacements: Union[
         List[Tuple[str, str]], List[List[str]], Dict[str, str], ItemsView[str, str]
     ],
@@ -841,14 +841,21 @@
 
         Works with a dictionary where all keys and values are strings!
 
         >>> replacements = {'hello': 'goodbye', 'world': 'earth'}
         >>> multi_replace('hello, world', replacements)
         'goodbye, earth'
 
+        >>> replacements = [['hello', 'goodbye'], ['world', 'this', 'will', 'fail']]
+        >>> try:
+        ...     multi_replace('hello, world', replacements)
+        ... except ValueError:
+        ...     print('ValueError raised')
+        ValueError raised
+
     """
     if isinstance(replacements, dict):
         return multi_replace(string, replacements.items())
     for rep in replacements:
         if isinstance(rep, list):
             if len(rep) != 2:
                 raise ValueError("Replacement must be a list of length 2")
@@ -972,24 +979,38 @@
     _n = longest_line(string)
     return "\n".join(["_" * _n, string, "^" * _n])
 
 
 def truncate_string(
     string: str, maxlines: int = 120, max_characters: int = 4096
 ) -> str:
-    """Truncate a string at either a max number of lines or characters
+    r"""Truncate a string at either a max number of lines or characters
 
     Args:
         string: String to truncate
         maxlines: Max number of lines the truncated string can have; default is 120
         max_characters: Max number of characters the string can have; default is 4096
 
     Returns:
         Truncated string
 
+    Examples:
+        >>> truncate_string('a')
+        'a'
+        >>> print(truncate_string('a\n' * 10, maxlines=5))
+        a
+        a
+        a
+        a
+        a
+        ---------------------------
+        ... Truncated @ 5 lines...
+        ---------------------------
+
+
     """
     string_lines = string.replace("\r\n", "\n").split("\n")
     if len(string_lines) > maxlines:
         string_lines = string_lines[:maxlines]
         line_lengths = [len(line) for line in string_lines]
         total_characters = sum(line_lengths)
         if total_characters < max_characters:
@@ -1063,17 +1084,17 @@
     )
 
 
 def striterable(string: str) -> Iterable[str]:
     r"""Yield 'clean' sub-strings from an input string
 
     This method takes a string (like the string that would be a dat file) and
-    yields strings from that string separated by some delimeter.
+    yields strings from that string separated by some delimiter.
 
-    Delimeters:
+    Delimiters:
         - <space>
         - <tab>
         - <new-line> (unix AND dos!)
 
     Args:
         string (str): string to be turned into a striterable
 
@@ -1142,77 +1163,119 @@
         >>> string_sanitize('question????,')
         'question'
 
     """
     return strip_non_ascii(re.sub(r"[()\"/;:<>{}`=~|!?,]", "", string).strip("."))
 
 
-def longest_line(string: str) -> int:
-    """Return the length of the longest line in a string
+def longest_line(string: Union[str, bytes]) -> int:
+    r"""Return the length of the longest line in a string
 
     Args:
         string (str): String that has either one or more lines
 
     Returns:
         int: The length of the longest line in the string
 
+    Examples:
+        >>> longest_line('hello\nworld')
+        5
+        >>> longest_line(b'hello\nworld')
+        5
+        >>> longest_line('hello world')
+        11
+        >>> longest_line(b'hello world')
+        11
+
     """
+    if isinstance(string, bytes):
+        if b"\n" in string:
+            return max(len(line) for line in string.splitlines(keepends=False))
+        return len(string)
+
     if "\n" in string:
         return max(len(line) for line in string.splitlines(keepends=False))
     return len(string)
 
 
 def rm_multilines(string: str) -> str:
-    """Remove blank lines from a string
+    r"""Remove blank lines from a string
 
     Args:
         string: string possibly containing blank lines
 
     Returns:
         string without blank lines
 
+    Examples:
+        >>> rm_multilines('hello\n\nworld')
+        'hello\nworld'
+
     """
     return "\n".join(
-        (ll.rstrip() for ll in string.replace("\r\n", "\n").split("\n") if ll.strip())
+        ll.rstrip() for ll in string.replace("\r\n", "\n").split("\n") if ll.strip()
     )
 
 
-def ensure_utf8(string: AnyStr) -> str:
+def ensure_utf8(string: Union[str, bytes]) -> str:
     """Return a string that ensured to be utf-8.
 
     This is often needed for those rare cases where some weird non-unicode
     character or escape sequence is present within a string; This method
     protects against the possibility of a UnicodeDecodeError.
 
     Args:
         string: A string which you/one would like the unicode version of
 
     Returns:
         The unicode-encoded version of a string
 
+    Examples:
+        >>> ensure_utf8('hello')
+        'hello'
+        >>> ensure_utf8(b'hello')
+        'hello'
+        >>> latin_bytes_with_weird_characters = b'hello\\xc3\\xa9'
+        >>> latin_string = ensure_utf8(latin_bytes_with_weird_characters)
+        >>> latin_string
+        'helloé'
+        >>> problem_bytes = b'hello\\x00'
+        >>> problem_bytes_utf8 = ensure_utf8(problem_bytes)
+        >>> problem_bytes_utf8
+        'hello\\x00'
+        >>> ensure_utf8('hello\\x00')
+        'hello\\x00'
+        >>> ensure_utf8(b'hello\\x00')
+        'hello\\x00'
+
     """
     if isinstance(string, bytes):
         try:
             return str(string, encoding="utf-8")
         except UnicodeDecodeError:
-            return str(string, encoding="latin2")
+            return str(string, encoding="utf-8", errors="ignore")
         except TypeError:
             pass
     return str(string)
 
 
 def body_contents(html_string: str) -> List[str]:
-    """Parse the innertext for body tags in an html string
+    r"""Parse the innertext for body tags in an html string
 
     Args:
         html_string (str): html to parse
 
     Returns:
         str: the inner text for the body tags
 
+    Examples:
+        >>> html_string = '<html><body>hello</body></html>'
+        >>> body_contents(html_string)
+        ['hello']
+
     """
     return re.findall("<body>(.*?)</body>", html_string, re.DOTALL)
 
 
 class pstr(str):
     """Pretty-string subclass"""
 
@@ -1257,14 +1320,16 @@
         >>> print(indent(s))
             this is a
             multiline string
         >>> s = "this is a\nmultiline string"
         >>> print(indent(s, '  '))
           this is a
           multiline string
+        >>> indent(b'this is a string')
+        b'    this is a string'
 
     """
     if isinstance(string, bytes):
         return indent(string.decode("utf-8"), prefix, predicate).encode("utf-8")
     return _indent(string, prefix, predicate)
 
 
@@ -1272,15 +1337,15 @@
 def dedent(string: str) -> str:
     r"""Dedent a string
 
     Args:
         string: Input string to dedent
 
     Returns:
-        Dedented string
+        Unindented string
 
     Examples:
         >>> s = '    this is a string'
         >>> dedent(s)
         'this is a string'
         >>> s = '        this is a string'
         >>> dedent(s)
@@ -1590,23 +1655,56 @@
         raise ValueError(
             "bytes given instead of string;\n"
             "tried to decode but got UnicodeDecodeError:\n{}".format(str(ude))
         )
     return f'<img src="data:image/jpeg;base64,{str(b64_string)}">'
 
 
-def enum_strings(strings: List[str]) -> Iterable[str]:
-    """Return a generator with enumerated strings"""
+def enum_strings(strings: List[str], numsep: str = ")") -> Iterable[str]:
+    """Return a generator with enumerated strings
+
+    Returns:
+        Generator[str]: Generator with enumerated strings
+
+    Examples:
+        >>> list(enum_strings(list(map(str, range(5)))))
+        ['1) 0', '2) 1', '3) 2', '4) 3', '5) 4']
+
+    """
     _count = len(str(len(strings)))
-    return (f"{str(ix).zfill(_count)}) {s}" for ix, s in enumerate(strings, start=1))
+    return (
+        f"{str(ix).zfill(_count)}{numsep} {s}" for ix, s in enumerate(strings, start=1)
+    )
+
+
+def space_pad_strings(strings: List[str], justify: str = "left") -> List[str]:
+    """Space pads strings to match the string with the max length
+
+    Returns:
+        List[str]: List of space-padded strings
 
+    Examples:
+        >>> space_pad_strings(["a", "bb", "ccc"])
+        ['a  ', 'bb ', 'ccc']
+        >>> space_pad_strings(["a", "bb", "ccc"], justify='right')
+        ['  a', ' bb', 'ccc']
+        >>> space_pad_strings(["a", "bb", "ccc"], justify='center')
+        Traceback (most recent call last):
+        ...
+        ValueError: justify must be 'left' or 'right', not center; case-insensitive
 
-def space_pad_strings(strings: List[str]) -> List[str]:
-    """Space pads strings to match the string with the max length"""
+    """
+    _justify = justify.lower()
+    if _justify not in ["left", "right"]:
+        raise ValueError(
+            f"justify must be 'left' or 'right', not {justify}; case-insensitive"
+        )
     _max_len = max(len(s) for s in strings)
+    if _justify == "right":
+        return [s.rjust(_max_len) for s in strings]
     return [s.ljust(_max_len) for s in strings]
 
 
 def t9_mapping() -> Dict[str, int]:
     return {
         " ": 0,
         ",": 1,
@@ -1716,22 +1814,30 @@
 
     """
     return int(t9_str(string))
 
 
 @anystr
 def str_is_identifier(string: str) -> bool:
-    """
+    """Return True if a string is a valid python identifier; False otherwise
 
     Args:
-        string ():
+        string (str): String (likely to be used as a key) to check
 
     Returns:
+        bool: True if is an identifier
+
+    Examples:
+        >>> str_is_identifier("howdy")
+        True
+        >>> str_is_identifier("class")
+        False
 
     """
+    return string.isidentifier() and not iskeyword(string)
     if not string.isidentifier():
         return False
     if iskeyword(string):
         return False
     return True
 
 
@@ -1798,14 +1904,33 @@
         >>> isidentifier(123)
         False
 
     """
     return is_identifier(string)
 
 
+def is_dunder(string: str) -> bool:
+    """Return True if a string is 'dunder' (starts and ends with '__')
+
+    Args:
+        string (str): String to check
+
+    Returns:
+        bool: True if is a dunder
+
+    Examples:
+        >>> is_dunder("__dunder__")
+        True
+        >>> is_dunder("not_dunder")
+        False
+
+    """
+    return string.startswith("__") and string.endswith("__")
+
+
 __all__ = (
     "ALL_CAP_RE",
     "CAMEL_CHARACTERS",
     "FIRST_CAP_RE",
     "HTML",
     "KEBAB_CHARACTERS",
     "SNAKE_CHARACTERS",
```

### Comparing `fmts-0.1.4/pyproject.toml` & `fmts-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [project]
 name = "fmts"
-version = "0.1.4"
+version = "0.1.5"
 description = "str transformation utils"
 authors = [
   { name = "jesse", email = "jessekrubin@gmail.com" },
   { name = "jesse", email = "jesse@dgi.com" },
 ]
 dependencies = []
 requires-python = ">=3.6.2,<4.0"
 license = { text = "MIT" }
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Typing :: Typed",
 ]
 keywords = ["str", "utils", "dgpy", "vanilla", "typed"]
@@ -27,62 +26,76 @@
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/fmts"
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 
 [tool.pdm]
 includes = ["./fmts"]
 
 [tool.pdm.dev-dependencies]
-dev = [
-  "pytest<7.0.0,>=6.2.2",
-]
+dev = ["pytest<7.0.0,>=6.2.2"]
 
 [tool.poetry]
 name = "fmts"
-version = "0.1.4"
+version = "0.1.5"
 description = "str transformation utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/fmts"
 readme = 'README.md'
-packages = [
-  { include = "fmts", from = "." },
-]
+packages = [{ include = "fmts", from = "." }]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Typing :: Typed",
 ]
-keywords = [
-  "str",
-  "utils",
-  "dgpy",
-  "vanilla",
-  "typed",
-]
+keywords = ["str", "utils", "dgpy", "vanilla", "typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["pdm-pep517"]
 build-backend = "pdm.pep517.api"
 
 # POETRY BUILD SYSTEM
 # [build-system]
 # requires = ["poetry-core>=1.0.0"]
 # build-backend = "poetry.core.masonry.api"
 
 # PDM BUILD SYSTEM
 # [build-system]
 # requires = ["pdm-pep517"]
 # build-backend = "pdm.pep517.api"
+
+[tool.coverage.run]
+source = ['fmts']
+branch = true
+context = '${CONTEXT}'
+
+[tool.coverage.report]
+show_missing = true
+precision = 2
+omit = []
+exclude_lines = [
+  'pragma: no cover',
+  'raise NotImplementedError',
+  'if TYPE_CHECKING:',
+  '@overload',
+  '\(Protocol\):$',
+  'if 0:',
+  'if False:',
+]
+
+[tool.coverage.paths]
+source = ['fmts/']
+
+[tool.ruff]
+extend = "../../pyproject.toml"
```

### Comparing `fmts-0.1.4/README.md` & `fmts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fmts-0.1.4/PKG-INFO` & `fmts-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmts
-Version: 0.1.4
+Version: 0.1.5
 Summary: str transformation utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/fmts
 License: MIT
 Keywords: str,utils,dgpy,vanilla,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
@@ -13,16 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: fmts Version: 0.1.4 Summary: str transformation
+Metadata-Version: 2.1 Name: fmts Version: 0.1.5 Summary: str transformation
 utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/
 libs/fmts License: MIT Keywords: str,utils,dgpy,vanilla,typed Author: jesse
 Author-email: jesse@dgi.com Requires-Python: >=3.7,<4.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Typing :: Typed Project-URL: Repository, https://github.com/dynamic-graphics-
 inc/dgpy-libs Description-Content-Type: text/markdown [drawing] # fmts [!
 [Wheel](https://img.shields.io/pypi/wheel/fmts.svg)](https://img.shields.io/
 pypi/wheel/fmts.svg) [![Version](https://img.shields.io/pypi/v/fmts.svg)]
 (https://img.shields.io/pypi/v/fmts.svg) [![py_versions](https://
```

