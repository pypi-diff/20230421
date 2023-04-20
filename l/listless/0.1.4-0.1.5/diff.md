# Comparing `tmp/listless-0.1.4.tar.gz` & `tmp/listless-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "listless-0.1.4.tar", max compression
+gzip compressed data, was "listless-0.1.5.tar", max compression
```

## Comparing `listless-0.1.4.tar` & `listless-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1056 2022-02-11 23:27:58.165586 listless-0.1.4/LICENSE
--rw-r--r--   0        0        0    19482 2023-04-11 21:27:29.161305 listless-0.1.4/listless/__init__.py
--rw-r--r--   0        0        0      381 2023-04-11 21:27:29.161305 listless-0.1.4/listless/__main__.py
--rw-r--r--   0        0        0      209 2023-04-11 21:27:29.162305 listless-0.1.4/listless/_meta.py
--rw-r--r--   0        0        0        0 2022-02-01 20:37:20.181695 listless-0.1.4/listless/py.typed
--rw-r--r--   0        0        0     2156 2023-04-11 21:27:29.162305 listless-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      816 2022-06-02 17:33:59.763392 listless-0.1.4/README.md
--rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 listless-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.425545 listless-0.1.5/LICENSE
+-rw-r--r--   0        0        0      286 2023-04-20 23:19:54.396173 listless-0.1.5/listless/__about__.py
+-rw-r--r--   0        0        0    19493 2023-04-20 22:21:57.270795 listless-0.1.5/listless/__init__.py
+-rw-r--r--   0        0        0      385 2023-04-20 20:51:48.622821 listless-0.1.5/listless/__main__.py
+-rw-r--r--   0        0        0      355 2023-04-20 20:38:23.588328 listless-0.1.5/listless/_meta.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.830952 listless-0.1.5/listless/py.typed
+-rw-r--r--   0        0        0     2154 2023-04-20 23:19:53.075226 listless-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      816 2022-05-03 21:42:21.354967 listless-0.1.5/README.md
+-rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 listless-0.1.5/PKG-INFO
```

### Comparing `listless-0.1.4/LICENSE` & `listless-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `listless-0.1.4/listless/__init__.py` & `listless-0.1.5/listless/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # pyright: reportInvalidTypeVarUse=false
-"""Listless generator utils"""
+"""Listless = generators, iterators, and async iterators, Oh My!"""
 import asyncio
 
 from collections import deque
 from functools import reduce
 from itertools import chain, count, islice, tee, zip_longest
 from operator import iconcat, mul
 from typing import (
@@ -22,15 +22,15 @@
     Tuple,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
-from listless._meta import __version__
+from listless.__about__ import __version__
 
 __all__ = (
     "__version__",
     "aiterable",
     "chunks",
     "enumerate_async",
     "exhaust",
@@ -46,15 +46,14 @@
     "partition",
     "set_async",
     "spliterable",
     "unique",
     "unique_gen",
     "xmap",
     "zip_async",
-    "zip_longest",
 )
 
 _K = TypeVar("_K")
 _T = TypeVar("_T")
 _R = TypeVar("_R")
 AnyIterable = Union[Iterable[_T], AsyncIterable[_T]]
 AnyIterator = Union[Iterator[_T], AsyncIterator[_T]]
@@ -425,25 +424,27 @@
         >>> list(filter_is_none([1, 2, None, 3, 4, None, 5, "a_string???"]))
         [1, 2, 3, 4, 5, 'a_string???']
         >>> list(filter_is_none([-1, 0, 1, '', 's', None, [], ['s'], {}]))
         [-1, 0, 1, '', 's', [], ['s'], {}]
 
 
     """
-    return filter(None.__ne__, it)  # type: ignore[arg-type]
+    return filter(lambda x: x is not None, it)  # type: ignore[arg-type]
 
 
 def flatten(*args: Union[_T, Iterable[_T]], anystr: bool = False) -> Iterable[_T]:
     """Flatten possibly nested iterables of sequences to a flat list
 
     Examples:
         >>> list(flatten("cmd", ["uno", "dos", "tres"]))
         ['cmd', 'uno', 'dos', 'tres']
         >>> list(flatten("cmd", ["uno", "dos", "tres", ["4444", "five"]]))
         ['cmd', 'uno', 'dos', 'tres', '4444', 'five']
+        >>> list(flatten("cmd", ["uno", "dos", "tres", ["4444", "five", 123]]))
+        ['cmd', 'uno', 'dos', 'tres', '4444', 'five', 123]
 
     """
     return chain(
         *(flatten(*arg) if isinstance(arg, (list, tuple)) else (arg,) for arg in args)
     )
 
 
@@ -546,17 +547,15 @@
     """1 generator + True/False-function => 2 generators (True-gen, False-gen)
 
     Args:
         it: iterable to split
         fn: Function to evaluate iterable elements and returns True or False
 
     Returns:
-        tuple of generators. The first generator will yield elements of the
-        original iterable where the conditional-function evaluates True, and
-        the second generator where the conditional-function evaluates to False.
+        tuple of generators: (gen_predicate_true, gen_predicate_false)
 
     Examples:
         >>> is_even = lambda n: n % 2 == 0
         >>> a, b = spliterable(range(10), is_even)
         >>> list(a)
         [0, 2, 4, 6, 8]
         >>> list(b)
```

### Comparing `listless-0.1.4/pyproject.toml` & `listless-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "listless"
-version = "0.1.4"
+version = "0.1.5"
 description = "generator utils; aka listless"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless"
 readme = 'README.md'
 packages = [
@@ -29,36 +29,36 @@
   "typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.0"
+pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = [
   "-ra",
   "--strict-config",
   "--strict-markers",
   "--doctest-modules",
   "--disable-warnings",
+  "--ignore-glob=*/_meta.py",
 ]
 xfail_strict = true
 filterwarnings = [
   "error",
   'ignore:"@coroutine" decorator is deprecated since Python 3\.8, use "async def" instead:DeprecationWarning',
   "ignore::RuntimeWarning",
   "ignore::pytest.PytestUnraisableExceptionWarning",
-  "ignore::DeprecationWarning",
 ]
 markers = [
   "slow: marks tests as slow (deselect with '-m \"not slow\"')",
   "timeout",
 ]
 
 [tool.coverage.run]
```

### Comparing `listless-0.1.4/README.md` & `listless-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `listless-0.1.4/PKG-INFO` & `listless-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: listless
-Version: 0.1.4
+Version: 0.1.5
 Summary: generator utils; aka listless
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless
 License: MIT
 Keywords: generators,itertools,dgpy,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: listless Version: 0.1.4 Summary: generator utils;
+Metadata-Version: 2.1 Name: listless Version: 0.1.5 Summary: generator utils;
 aka listless Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/
 main/libs/listless License: MIT Keywords: generators,itertools,dgpy,typed
 Author: jesse Author-email: jesse@dgi.com Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
```

