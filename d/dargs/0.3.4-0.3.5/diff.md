# Comparing `tmp/dargs-0.3.4.tar.gz` & `tmp/dargs-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-tik549g9/dargs-0.3.4.tar", last modified: Fri Nov 25 04:15:50 2022, max compression
+gzip compressed data, was "/home/runner/work/dargs/dargs/dist/.tmp-ccu11s4g/dargs-0.3.5.tar", last modified: Fri Apr 21 03:59:18 2023, max compression
```

## Comparing `dargs-0.3.4.tar` & `dargs-0.3.5.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      230 2022-11-25 04:15:27.000000 dargs-0.3.4/.github/workflows/mirror_gitee.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2022-11-25 04:15:27.000000 dargs-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)      408 2022-11-25 04:15:27.000000 dargs-0.3.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      676 2022-11-25 04:15:27.000000 dargs-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2022-11-25 04:15:27.000000 dargs-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    10650 2022-11-25 04:15:50.000000 dargs-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2022-11-25 04:15:27.000000 dargs-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-11-25 04:15:27.000000 dargs-0.3.4/dargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    34181 2022-11-25 04:15:27.000000 dargs-0.3.4/dargs/dargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2022-11-25 04:15:27.000000 dargs-0.3.4/dargs/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10650 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      596 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-25 04:15:50.000000 dargs-0.3.4/dargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      602 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     5511 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)       45 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      473 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-25 04:15:27.000000 dargs-0.3.4/docs/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (122)      859 2022-11-25 04:15:27.000000 dargs-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-25 04:15:50.000000 dargs-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:50.000000 dargs-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      110 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (122)    37056 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/dpmdargs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9801 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/test_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     8422 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5085 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/test_docgen.py
--rw-r--r--   0 runner    (1001) docker     (122)     4789 2022-11-25 04:15:27.000000 dargs-0.3.4/tests/test_normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-21 03:58:57.000000 dargs-0.3.5/.github/workflows/mirror_gitee.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 03:58:57.000000 dargs-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-21 03:58:57.000000 dargs-0.3.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-21 03:58:57.000000 dargs-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-21 03:58:57.000000 dargs-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-21 03:58:57.000000 dargs-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-21 03:59:18.000000 dargs-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 03:58:57.000000 dargs-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-21 03:58:57.000000 dargs-0.3.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 03:58:57.000000 dargs-0.3.5/dargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-21 03:58:57.000000 dargs-0.3.5/dargs/dargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-21 03:58:57.000000 dargs-0.3.5/dargs/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 03:59:18.000000 dargs-0.3.5/dargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-21 03:58:57.000000 dargs-0.3.5/docs/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-21 03:58:57.000000 dargs-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:59:18.000000 dargs-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:59:18.000000 dargs-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38859 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/dpmdargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/test_docgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-21 03:58:57.000000 dargs-0.3.5/tests/test_normalizer.py
```

### Comparing `dargs-0.3.4/.github/workflows/python-publish.yml` & `dargs-0.3.5/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 name: Upload Python Package
 
 on:
   release:
     types: [published]
   workflow_dispatch:
-    
+
 
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
```

### Comparing `dargs-0.3.4/.gitignore` & `dargs-0.3.5/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 # Environments
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
-venv.bak/
+venv.bak/
```

### Comparing `dargs-0.3.4/LICENSE` & `dargs-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dargs-0.3.4/PKG-INFO` & `dargs-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -177,27 +177,27 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Argument checking for python programs
 
-This is a minimum version for checking the input argument dict. 
-It would examine argument's type,  as well as keys and types of its sub-arguments. 
+This is a minimum version for checking the input argument dict.
+It would examine argument's type,  as well as keys and types of its sub-arguments.
 
-A special case called *variant* is also handled, 
-where you can determine the items of a dict based the value of on one of its `flag_name` key. 
+A special case called *variant* is also handled,
+where you can determine the items of a dict based the value of on one of its `flag_name` key.
 
 There are three main methods of `Argument` class:
 
 - `check` method that takes a dict and see if its type follows the definition in the class
 - `normalize` method that takes a dict and convert alias and add default value into it
 - `gendoc` method that outputs the defined argument structure and corresponding docs
 
-There are also `check_value` and `normalize_value` that 
+There are also `check_value` and `normalize_value` that
 ignore the leading key comparing to the base version.
 
-When targeting to html rendering, additional anchor can be made for cross reference. 
+When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
```

### Comparing `dargs-0.3.4/README.md` & `dargs-0.3.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Argument checking for python programs
 
-This is a minimum version for checking the input argument dict. 
-It would examine argument's type,  as well as keys and types of its sub-arguments. 
+This is a minimum version for checking the input argument dict.
+It would examine argument's type,  as well as keys and types of its sub-arguments.
 
-A special case called *variant* is also handled, 
-where you can determine the items of a dict based the value of on one of its `flag_name` key. 
+A special case called *variant* is also handled,
+where you can determine the items of a dict based the value of on one of its `flag_name` key.
 
 There are three main methods of `Argument` class:
 
 - `check` method that takes a dict and see if its type follows the definition in the class
 - `normalize` method that takes a dict and convert alias and add default value into it
 - `gendoc` method that outputs the defined argument structure and corresponding docs
 
-There are also `check_value` and `normalize_value` that 
+There are also `check_value` and `normalize_value` that
 ignore the leading key comparing to the base version.
 
-When targeting to html rendering, additional anchor can be made for cross reference. 
+When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
```

### Comparing `dargs-0.3.4/dargs/dargs.py` & `dargs-0.3.5/dargs/dargs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 r"""
 Some (ocaml) pseudo-code here to show the intended type structure::
 
     type args = {key: str; value: data; optional: bool; doc: str} list
-    and  data = 
+    and  data =
            | Arg of dtype
            | Node of args
            | Repeat of args
            | Variant of (str * args) list
 
 In actual implementation, We flatten this structure into on tree-like class
-`Argument` with (optional) attribute `dtype`, `sub_fields`, `repeat` and 
+`Argument` with (optional) attribute `dtype`, `sub_fields`, `repeat` and
 `sub_variants` to mimic the union behavior in the type structure.
 
-Due to the complexity of *Variant* structure, it is implemented into a 
+Due to the complexity of *Variant* structure, it is implemented into a
 separate class `Variant` so that multiple choices can be handled correctly.
 We also need to pay special attention to flat the keys of its choices.
 """
 
 
-from typing import Union, Any, List, Dict, Iterable, Optional, Callable
-from textwrap import indent
+import fnmatch
+import json
+import re
 from copy import deepcopy
 from enum import Enum
-import fnmatch, re
-import json
+from numbers import Real
+from textwrap import indent
+from typing import Any, Callable, Dict, Iterable, List, Optional, Union
 
 
-INDENT = "    " # doc is indented by four spaces
-RAW_ANCHOR = False # whether to use raw html anchors or RST ones
+INDENT = "    "  # doc is indented by four spaces
+RAW_ANCHOR = False  # whether to use raw html anchors or RST ones
 
 # the third argument is the base path
 HookArgKType = Callable[["Argument", dict, List[str]], None]
-HookArgVType = Callable[["Argument", Any,  List[str]], None]
-HookVrntType = Callable[["Variant",  dict, List[str]], None]
-_DUMMYHOOK = lambda a,x,p: None # for doing nothing in traversing
-class _Flags(Enum): NONE = 0 # for no value in dict (when optional)
+HookArgVType = Callable[["Argument", Any, List[str]], None]
+HookVrntType = Callable[["Variant", dict, List[str]], None]
+_DUMMYHOOK = lambda a, x, p: None  # for doing nothing in traversing
+
+
+class _Flags(Enum):
+    NONE = 0  # for no value in dict (when optional)
+    EMPTY_DICT = 1  # for empty dict as default value
 
 
 class ArgumentError(Exception):
     """Base error class for invalid argument values in argchecking."""
 
-    def __init__(self, 
-                 path: Union[None, str, List[str]] = None, 
-                 message: Optional[str] = None):
+    def __init__(
+        self, path: Union[None, str, List[str]] = None, message: Optional[str] = None
+    ):
         super().__init__(message)
         if path is None:
             path = ""
         if not isinstance(path, str):
             path = "/".join(path)
         self.path = path.strip("/")
         self.message = message
-    
+
     def __str__(self) -> str:
-        loc_msg = ("at root location" if not self.path else
-                  f"at location `{self.path}`")
+        loc_msg = "at root location" if not self.path else f"at location `{self.path}`"
         return f"[{loc_msg}] {self.message}"
 
+
 class ArgumentKeyError(ArgumentError):
     """Error class for missing or invalid argument keys"""
+
     pass
 
+
 class ArgumentTypeError(ArgumentError):
     """Error class for invalid argument data types"""
+
     pass
 
+
 class ArgumentValueError(ArgumentError):
     """Error class for missing or invalid argument values"""
+
     pass
 
 
 class Argument:
     """Define possible arguments and their types and properties.
-    
+
     Each `Argument` instance contains a `name` and a `dtype`, that correspond
     to the key and value type of the actual argument. Additionally, it can
     include `sub_fields` and `sub_variants` to deal with nested dict arguments.
 
     Parameters
     ----------
     name : str
@@ -101,64 +112,72 @@
     extra_check: callable
         Additional check to be done on the value of the argument.
         Should be a function that takes the value and returns whether it passes.
     doc: str
         The doc string of the argument, used in doc generation.
     fold_subdoc: bool, optional
         If true, no doc will be generated for sub args.
+    extra_check_errmsg : str
+        The error message if extra_check fails
 
     Examples
     --------
     >>> ca = Argument("base", dict, [Argument("sub", int)])
     >>> ca.check({"base": {"sub1": 1}})
     >>> ca.check_value({"sub1": 1})
 
     for more detailed examples, please check the unit tests.
     """
 
-    def __init__(self, 
-            name: str,
-            dtype: Union[None, type, Iterable[type]],
-            sub_fields: Optional[Iterable["Argument"]] = None,
-            sub_variants: Optional[Iterable["Variant"]] = None,
-            repeat: bool = False,
-            optional: bool = False,
-            default: Any = _Flags.NONE,
-            alias: Optional[Iterable[str]] = None,
-            extra_check: Optional[Callable[[Any], bool]] = None,
-            doc: str = "",
-            fold_subdoc: bool = False):
+    def __init__(
+        self,
+        name: str,
+        dtype: Union[None, type, Iterable[type]],
+        sub_fields: Optional[Iterable["Argument"]] = None,
+        sub_variants: Optional[Iterable["Variant"]] = None,
+        repeat: bool = False,
+        optional: bool = False,
+        default: Any = _Flags.NONE,
+        alias: Optional[Iterable[str]] = None,
+        extra_check: Optional[Callable[[Any], bool]] = None,
+        doc: str = "",
+        fold_subdoc: bool = False,
+        extra_check_errmsg: str = "",
+    ):
         self.name = name
         self.dtype = dtype
-        self.sub_fields : Dict[str, "Argument"] = {}
-        self.sub_variants : Dict[str, "Variant"] = {}
+        self.sub_fields: Dict[str, "Argument"] = {}
+        self.sub_variants: Dict[str, "Variant"] = {}
         self.repeat = repeat
         self.optional = optional
         self.default = default
         self.alias = alias if alias is not None else []
         self.extra_check = extra_check
         self.doc = doc
         self.fold_subdoc = fold_subdoc
+        self.extra_check_errmsg = extra_check_errmsg
         # adding subfields and subvariants
         self.extend_subfields(sub_fields)
         self.extend_subvariants(sub_variants)
         # handle the format of dtype, makeit a tuple
         self._reorg_dtype()
 
     def __eq__(self, other: "Argument") -> bool:
         # do not compare doc and default
         # since they do not enter to the type checking
         fkey = lambda f: f.name
         vkey = lambda v: v.flag_name
-        return (self.name         == other.name 
-            and set(self.dtype)   == set(other.dtype)
-            and self.sub_fields   == other.sub_fields
+        return (
+            self.name == other.name
+            and set(self.dtype) == set(other.dtype)
+            and self.sub_fields == other.sub_fields
             and self.sub_variants == other.sub_variants
-            and self.repeat       == other.repeat
-            and self.optional     == other.optional)
+            and self.repeat == other.repeat
+            and self.optional == other.optional
+        )
 
     def __repr__(self) -> str:
         return f"<Argument {self.name}: {' | '.join(dd.__name__ for dd in self.dtype)}>"
 
     def __getitem__(self, key: str) -> "Argument":
         key = key.lstrip("/")
         if key in ("", "."):
@@ -168,34 +187,34 @@
             if vkey.count("=") == 1:
                 fkey, ckey = vkey.split("=")
             else:
                 [fkey] = self.sub_variants.keys()
                 ckey = vkey
             return self.sub_variants[fkey][ckey][rkey]
         p1, p2 = key.find("/"), key.find("[")
-        if max(p1, p2) < 0: # not found
+        if max(p1, p2) < 0:  # not found
             return self.sub_fields[key]
-        else: # at least one found
-            p = p1 if p2 < 0 or  0 < p1 < p2 else p2
+        else:  # at least one found
+            p = p1 if p2 < 0 or 0 < p1 < p2 else p2
             skey, rkey = key[:p], key[p:]
             return self[skey][rkey]
-    
+
     @property
-    def I(self): 
+    def I(self):
         # return a dummy argument that only has self as a sub field
         # can be used in indexing
         return Argument("_", dict, [self])
 
     def _reorg_dtype(self):
         if isinstance(self.dtype, type) or self.dtype is None:
             self.dtype = [self.dtype]
         # remove duplicate
         self.dtype = {dt if type(dt) is type else type(dt) for dt in self.dtype}
         # check conner cases
-        if self.sub_fields or self.sub_variants: 
+        if self.sub_fields or self.sub_variants:
             self.dtype.add(list if self.repeat else dict)
         if self.optional and self.default is not _Flags.NONE:
             self.dtype.add(type(self.default))
         # and make it compatible with `isinstance`
         self.dtype = tuple(self.dtype)
 
     def set_dtype(self, dtype: Union[None, type, Iterable[type]]):
@@ -203,280 +222,349 @@
         self.dtype = dtype
         self._reorg_dtype()
 
     def set_repeat(self, repeat: bool = True):
         """Change the repeat attribute of the current Argument."""
         self.repeat = repeat
         self._reorg_dtype()
-    
+
     def extend_subfields(self, sub_fields: Optional[Iterable["Argument"]]):
         """Add a list of sub fields to the current Argument."""
         if sub_fields is None:
             return
         assert all(isinstance(s, Argument) for s in sub_fields)
-        update_nodup(self.sub_fields, ((s.name, s) for s in sub_fields),
-            err_msg=f"building Argument `{self.name}`")
+        update_nodup(
+            self.sub_fields,
+            ((s.name, s) for s in sub_fields),
+            err_msg=f"building Argument `{self.name}`",
+        )
         self._reorg_dtype()
 
-    def add_subfield(self, name: Union[str, "Argument"], 
-                     *args, **kwargs) -> "Argument":
+    def add_subfield(self, name: Union[str, "Argument"], *args, **kwargs) -> "Argument":
         """Add a sub field to the current Argument."""
         if isinstance(name, Argument):
             newarg = name
         else:
             newarg = Argument(name, *args, **kwargs)
         self.extend_subfields([newarg])
         return newarg
 
     def extend_subvariants(self, sub_variants: Optional[Iterable["Variant"]]):
         """Add a list of sub variants to the current Argument."""
         if sub_variants is None:
             return
         assert all(isinstance(s, Variant) for s in sub_variants)
-        update_nodup(self.sub_variants, ((s.flag_name, s) for s in sub_variants),
+        update_nodup(
+            self.sub_variants,
+            ((s.flag_name, s) for s in sub_variants),
             exclude=self.sub_fields.keys(),
-            err_msg=f"building Argument `{self.name}`")
+            err_msg=f"building Argument `{self.name}`",
+        )
         self._reorg_dtype()
 
-    def add_subvariant(self, flag_name: Union[str, "Variant"], 
-                       *args, **kwargs) -> "Variant":
+    def add_subvariant(
+        self, flag_name: Union[str, "Variant"], *args, **kwargs
+    ) -> "Variant":
         """Add a sub variant to the current Argument."""
         if isinstance(flag_name, Variant):
             newvrnt = flag_name
         else:
             newvrnt = Variant(flag_name, *args, **kwargs)
         self.extend_subvariants([newvrnt])
         return newvrnt
 
     # above are creation part
     # below are general traverse part
 
     def flatten_sub(self, value: dict, path=None) -> Dict[str, "Argument"]:
         sub_dicts = [self.sub_fields]
-        sub_dicts.extend(vrnt.flatten_sub(value, path) 
-            for vrnt in self.sub_variants.values())
+        sub_dicts.extend(
+            vrnt.flatten_sub(value, path) for vrnt in self.sub_variants.values()
+        )
         flat_subs = {}
-        update_nodup(flat_subs, *sub_dicts, 
-            err_msg=f"flattening variants of {self.name}")
+        update_nodup(
+            flat_subs, *sub_dicts, err_msg=f"flattening variants of {self.name}"
+        )
         return flat_subs
 
-    def traverse(self, argdict: dict, 
-                 key_hook: HookArgKType = _DUMMYHOOK,
-                 value_hook: HookArgVType = _DUMMYHOOK,
-                 sub_hook: HookArgKType = _DUMMYHOOK,
-                 variant_hook: HookVrntType = _DUMMYHOOK, 
-                 path: Optional[List[str]] = None):
+    def traverse(
+        self,
+        argdict: dict,
+        key_hook: HookArgKType = _DUMMYHOOK,
+        value_hook: HookArgVType = _DUMMYHOOK,
+        sub_hook: HookArgKType = _DUMMYHOOK,
+        variant_hook: HookVrntType = _DUMMYHOOK,
+        path: Optional[List[str]] = None,
+    ):
         # first, do something with the key
         # then, take out the vaule and do something with it
-        if path is None: path = []
+        if path is None:
+            path = []
         key_hook(self, argdict, path)
         if self.name in argdict:
             value = argdict[self.name]
             value_hook(self, value, path)
             newpath = [*path, self.name]
             # this is the key step that we traverse into the tree
-            self.traverse_value(value, 
-                key_hook, value_hook, sub_hook, variant_hook, newpath)
-
-    def traverse_value(self, value: Any, 
-                       key_hook: HookArgKType = _DUMMYHOOK,
-                       value_hook: HookArgVType = _DUMMYHOOK,
-                       sub_hook: HookArgKType = _DUMMYHOOK,
-                       variant_hook: HookVrntType = _DUMMYHOOK,
-                       path: Optional[List[str]] = None):
+            self.traverse_value(
+                value, key_hook, value_hook, sub_hook, variant_hook, newpath
+            )
+
+    def traverse_value(
+        self,
+        value: Any,
+        key_hook: HookArgKType = _DUMMYHOOK,
+        value_hook: HookArgVType = _DUMMYHOOK,
+        sub_hook: HookArgKType = _DUMMYHOOK,
+        variant_hook: HookVrntType = _DUMMYHOOK,
+        path: Optional[List[str]] = None,
+    ):
         # this is not private, and can be called directly
         # in the condition where there is no leading key
-        if path is None: path = []
+        if path is None:
+            path = []
         if isinstance(value, dict):
-            self._traverse_sub(value,
-                key_hook, value_hook, sub_hook, variant_hook, path)
+            self._traverse_sub(
+                value, key_hook, value_hook, sub_hook, variant_hook, path
+            )
         if isinstance(value, list) and self.repeat:
             for idx, item in enumerate(value):
-                self._traverse_sub(item,
-                    key_hook, value_hook, sub_hook, variant_hook, [*path, str(idx)])
-
-    def _traverse_sub(self, value: dict, 
-                      key_hook: HookArgKType = _DUMMYHOOK,
-                      value_hook: HookArgVType = _DUMMYHOOK,
-                      sub_hook: HookArgKType = _DUMMYHOOK,
-                      variant_hook: HookVrntType = _DUMMYHOOK,
-                      path: Optional[List[str]] = None):
+                self._traverse_sub(
+                    item,
+                    key_hook,
+                    value_hook,
+                    sub_hook,
+                    variant_hook,
+                    [*path, str(idx)],
+                )
+
+    def _traverse_sub(
+        self,
+        value: dict,
+        key_hook: HookArgKType = _DUMMYHOOK,
+        value_hook: HookArgVType = _DUMMYHOOK,
+        sub_hook: HookArgKType = _DUMMYHOOK,
+        variant_hook: HookVrntType = _DUMMYHOOK,
+        path: Optional[List[str]] = None,
+    ):
         assert isinstance(value, dict)
-        if path is None: path = [self.name]
+        if path is None:
+            path = [self.name]
         sub_hook(self, value, path)
         for subvrnt in self.sub_variants.values():
             variant_hook(subvrnt, value, path)
         for subarg in self.flatten_sub(value, path).values():
-            subarg.traverse(value, 
-                key_hook, value_hook, sub_hook, variant_hook, path)
+            subarg.traverse(value, key_hook, value_hook, sub_hook, variant_hook, path)
 
     # above are general traverse part
     # below are type checking part
 
     def check(self, argdict: dict, strict: bool = False):
         """Check whether `argdict` meets the structure defined in self.
 
-        Will recursively check nested dicts according to 
+        Will recursively check nested dicts according to
         sub_fields and sub_variants. Raise an error if the check fails.
-        
+
         Parameters
         ----------
-        argdict: dict
+        argdict : dict
             The arg dict to be checked
-        strict: bool, optional
+        strict : bool, optional
             If true, only keys defined in `Argument` are allowed.
         """
         if strict and len(argdict) != 1:
-            raise ArgumentKeyError(None,
+            raise ArgumentKeyError(
+                None,
                 "only one single key of arg name is allowed "
                 "for check in strict mode at top level, "
-                "use check_value if you are checking subfields")
-        self.traverse(argdict, 
+                "use check_value if you are checking subfields",
+            )
+        self.traverse(
+            argdict,
             key_hook=Argument._check_exist,
             value_hook=Argument._check_data,
-            sub_hook=Argument._check_strict if strict else _DUMMYHOOK)
+            sub_hook=Argument._check_strict if strict else _DUMMYHOOK,
+        )
 
     def check_value(self, value: Any, strict: bool = False):
         """Check the value without the leading key.
 
-        Same as `check({self.name: value})`. 
+        Same as `check({self.name: value})`.
         Raise an error if the check fails.
-        
+
         Parameters
         ----------
-        value: any value type
+        value : any value type
             The value to be checked
-        strict: bool, optional
+        strict : bool, optional
             If true, only keys defined in `Argument` are allowed.
         """
-        self.traverse_value(value, 
+        self.traverse_value(
+            value,
             key_hook=Argument._check_exist,
             value_hook=Argument._check_data,
-            sub_hook=Argument._check_strict if strict else _DUMMYHOOK)
+            sub_hook=Argument._check_strict if strict else _DUMMYHOOK,
+        )
 
     def _check_exist(self, argdict: dict, path=None):
         if self.optional is True:
             return
         if self.name not in argdict:
-            raise ArgumentKeyError(path,
-                f"key `{self.name}` is required "
-                 "in arguments but not found")
+            raise ArgumentKeyError(
+                path, f"key `{self.name}` is required " "in arguments but not found"
+            )
 
     def _check_data(self, value: Any, path=None):
-        if not isinstance(value, self.dtype):
-            raise ArgumentTypeError(path,
+        if not (
+            isinstance(value, self.dtype)
+            or (float in self.dtype and isinstance(value, Real))
+        ):
+            raise ArgumentTypeError(
+                path,
                 f"key `{self.name}` gets wrong value type, "
                 f"requires <{'|'.join(dd.__name__ for dd in self.dtype)}> "
-                f"but gets <{type(value).__name__}>")
+                f"but gets <{type(value).__name__}>",
+            )
         if self.extra_check is not None and not self.extra_check(value):
-            raise ArgumentValueError(path,
+            raise ArgumentValueError(
+                path,
                 f"key `{self.name}` gets bad value "
-                "that fails to pass its extra checking")
+                "that fails to pass its extra checking. " + self.extra_check_errmsg,
+            )
 
     def _check_strict(self, value: dict, path=None):
         allowed_keys = self.flatten_sub(value, path).keys()
         # curpath = [*path, self.name]
         if not len(allowed_keys):
             # no allowed keys defined, allow any keys
             return
         for name in value.keys():
             if name not in allowed_keys:
-                raise ArgumentKeyError(path,
-                    f"undefined key `{name}` is "
-                     "not allowed in strict mode")
+                raise ArgumentKeyError(
+                    path, f"undefined key `{name}` is " "not allowed in strict mode"
+                )
 
     # above are type checking part
     # below are normalizing part
 
-    def normalize(self, argdict: dict, inplace: bool = False, 
-                  do_default: bool = True, do_alias: bool = True, 
-                  trim_pattern: Optional[str] = None):
+    def normalize(
+        self,
+        argdict: dict,
+        inplace: bool = False,
+        do_default: bool = True,
+        do_alias: bool = True,
+        trim_pattern: Optional[str] = None,
+    ):
         """Modify `argdict` so that it meets the Argument structure
-        
-        Normalization can add default values to optional args, 
+
+        Normalization can add default values to optional args,
         substitute alias by its standard names, and discard unnecessary
         args following given pattern.
 
         Parameters
         ----------
-        argdict: dict
+        argdict : dict
             The arg dict to be normalized.
-        inplace: bool, optional
+        inplace : bool, optional
             If true, modify the given dict. Otherwise return a new one.
-        do_default: bool, optional
+        do_default : bool, optional
             Whether to add default values.
-        do_alias: bool, optional
+        do_alias : bool, optional
             Whether to transform alias names.
-        trim_pattern: str, optional
+        trim_pattern : str, optional
             If given, discard keys that matches the glob pattern.
 
         Returns
         -------
         dict:
             The normalized arg dict.
         """
         if not inplace:
             argdict = deepcopy(argdict)
         if do_alias:
-            self.traverse(argdict, 
+            self.traverse(
+                argdict,
                 key_hook=Argument._convert_alias,
-                variant_hook=Variant._convert_choice_alias)
+                variant_hook=Variant._convert_choice_alias,
+            )
         if do_default:
-            self.traverse(argdict, 
-                key_hook=Argument._assign_default)
+            self.traverse(argdict, key_hook=Argument._assign_default)
+            self.traverse(argdict, key_hook=Argument._handle_empty_dict)
         if trim_pattern is not None:
             trim_by_pattern(argdict, trim_pattern, reserved=[self.name])
-            self.traverse(argdict, sub_hook=lambda a, d, p: 
-                trim_by_pattern(d, trim_pattern, a.flatten_sub(d, p).keys()))
+            self.traverse(
+                argdict,
+                sub_hook=lambda a, d, p: trim_by_pattern(
+                    d, trim_pattern, a.flatten_sub(d, p).keys()
+                ),
+            )
         return argdict
 
-    def normalize_value(self, value: Any, inplace: bool = False, 
-                        do_default: bool = True, do_alias: bool = True, 
-                        trim_pattern: Optional[str] = None):
+    def normalize_value(
+        self,
+        value: Any,
+        inplace: bool = False,
+        do_default: bool = True,
+        do_alias: bool = True,
+        trim_pattern: Optional[str] = None,
+    ):
         """Modify the value so that it meets the Argument structure
-        
+
         Same as `normalize({self.name: value})[self.name]`.
 
         Parameters
         ----------
-        value: any value type
+        value : any value type
             The arg value to be normalized.
-        inplace: bool, optional
+        inplace : bool, optional
             If true, modify the given dict. Otherwise return a new one.
-        do_default: bool, optional
+        do_default : bool, optional
             Whether to add default values.
-        do_alias: bool, optional
+        do_alias : bool, optional
             Whether to transform alias names.
-        trim_pattern: str, optional
+        trim_pattern : str, optional
             If given, discard keys that matches the glob pattern.
 
         Returns
         -------
         value:
             The normalized arg value.
         """
         if not inplace:
             value = deepcopy(value)
         if do_alias:
-            self.traverse_value(value, 
+            self.traverse_value(
+                value,
                 key_hook=Argument._convert_alias,
-                variant_hook=Variant._convert_choice_alias)
+                variant_hook=Variant._convert_choice_alias,
+            )
         if do_default:
-            self.traverse_value(value, 
-                key_hook=Argument._assign_default)
+            self.traverse_value(value, key_hook=Argument._assign_default)
+            self.traverse_value(value, key_hook=Argument._handle_empty_dict)
         if trim_pattern is not None:
-            self.traverse_value(value, sub_hook=lambda a, d, p: 
-                trim_by_pattern(d, trim_pattern, a.flatten_sub(d, p).keys()))
+            self.traverse_value(
+                value,
+                sub_hook=lambda a, d, p: trim_by_pattern(
+                    d, trim_pattern, a.flatten_sub(d, p).keys()
+                ),
+            )
         return value
 
     def _assign_default(self, argdict: dict, path=None):
-        if (self.name not in argdict 
-        and self.optional 
-        and self.default is not _Flags.NONE):
-            argdict[self.name] = self.default
+        if (
+            self.name not in argdict
+            and self.optional
+            and self.default is not _Flags.NONE
+        ):
+            default = self.default if self.default != {} else _Flags.EMPTY_DICT
+            argdict[self.name] = default
+
+    def _handle_empty_dict(self, argdict: dict, path=None):
+        if argdict.get(self.name, None) is _Flags.EMPTY_DICT:
+            argdict[self.name] = {}
 
     def _convert_alias(self, argdict: dict, path=None):
         if self.name not in argdict:
             for alias in self.alias:
                 if alias in argdict:
                     argdict[self.name] = argdict.pop(alias)
                     return
@@ -489,31 +577,31 @@
         # the actual indentation is done here, and ONLY here
         if path is None:
             path = []
         sub_paths = [*path, self.name]
         doc_list = [
             self.gen_doc_head(sub_paths, **kwargs),
             indent(self.gen_doc_path(sub_paths, **kwargs), INDENT),
-            indent(self.gen_doc_body(sub_paths, **kwargs), INDENT)
+            indent(self.gen_doc_body(sub_paths, **kwargs), INDENT),
         ]
         return "\n".join(filter(None, doc_list))
 
     def gen_doc_head(self, path: Optional[List[str]] = None, **kwargs) -> str:
         typesig = "| type: " + " | ".join([f"``{dt.__name__}``" for dt in self.dtype])
         if self.optional:
             typesig += ", optional"
             if self.default == "":
                 typesig += f", default: (empty string)"
             elif self.default is not _Flags.NONE:
                 typesig += f", default: ``{self.default}``"
         if self.alias:
             typesig += f", alias{'es' if len(self.alias) > 1 else ''}: "
-            typesig += ', '.join(f"*{al}*" for al in self.alias)
+            typesig += ", ".join(f"*{al}*" for al in self.alias)
         head = f"{self.name}: "
-        if kwargs.get('use_sphinx_domain', False):
+        if kwargs.get("use_sphinx_domain", False):
             head = f".. dargs:argument:: {self.name}:\n   :path: {'/'.join(path)}\n"
         head += f"\n{indent(typesig, INDENT)}"
         if kwargs.get("make_anchor"):
             head = f"{make_rst_refid(path)}\n" + head
         return head
 
     def gen_doc_path(self, path: Optional[List[str]] = None, **kwargs) -> str:
@@ -524,35 +612,37 @@
 
     def gen_doc_body(self, path: Optional[List[str]] = None, **kwargs) -> str:
         body_list = []
         if self.doc:
             body_list.append(self.doc + "\n")
         if not self.fold_subdoc:
             if self.repeat:
-                body_list.append("This argument takes a list with "
-                                "each element containing the following: \n")
+                body_list.append(
+                    "This argument takes a list with "
+                    "each element containing the following: \n"
+                )
             if self.sub_fields:
                 # body_list.append("") # genetate a blank line
-                # body_list.append("This argument accept the following sub arguments:")                
+                # body_list.append("This argument accept the following sub arguments:")
                 for subarg in self.sub_fields.values():
                     body_list.append(subarg.gen_doc(path, **kwargs))
             if self.sub_variants:
                 showflag = len(self.sub_variants) > 1
                 for subvrnt in self.sub_variants.values():
                     body_list.append(subvrnt.gen_doc(path, showflag, **kwargs))
         body = "\n".join(body_list)
         return body
 
 
 class Variant:
     """Define multiple choices of possible argument sets.
-    
-    Each Variant contains a `flag_name` and a list of choices 
-    that are represented by `Argument`s. The choice is picked if its name 
-    matches the value of `flag_name` in the actual arguments. The actual 
+
+    Each Variant contains a `flag_name` and a list of choices
+    that are represented by `Argument`s. The choice is picked if its name
+    matches the value of `flag_name` in the actual arguments. The actual
     arguments should then be a dict containing `flag_name` and sub fields
     of the picked choice.
 
     Parameters
     ----------
     flag_name: str
         The name of the key to be used as the switching flag.
@@ -567,244 +657,308 @@
         The doc string used in document generation.
 
     Notes
     -----
     This class should only be used in sub variants of the `Argument` class.
     """
 
-    def __init__(self, 
-            flag_name: str,
-            choices: Optional[Iterable["Argument"]] = None,
-            optional: bool = False,
-            default_tag: str = "", # this is indeed necessary in case of optional
-            doc: str = ""):
+    def __init__(
+        self,
+        flag_name: str,
+        choices: Optional[Iterable["Argument"]] = None,
+        optional: bool = False,
+        default_tag: str = "",  # this is indeed necessary in case of optional
+        doc: str = "",
+    ):
         self.flag_name = flag_name
-        self.choice_dict : Dict[str, Argument] = {}
-        self.choice_alias : Dict[str, str] = {}
+        self.choice_dict: Dict[str, Argument] = {}
+        self.choice_alias: Dict[str, str] = {}
         self.extend_choices(choices)
         self.optional = optional
         if optional and not default_tag:
             raise ValueError("default_tag is needed if optional is set to be True")
         self.set_default(default_tag)
         self.doc = doc
 
     def __eq__(self, other: "Variant") -> bool:
-        # do not compare doc 
-        return (self.flag_name == other.flag_name 
+        # do not compare doc
+        return (
+            self.flag_name == other.flag_name
             and self.choice_dict == other.choice_dict
             and self.optional == other.optional
-            and self.default_tag == other.default_tag)
-    
+            and self.default_tag == other.default_tag
+        )
+
     def __repr__(self) -> str:
-        return f"<Variant {self.flag_name} in {{ {', '.join(self.choice_dict.keys())} }}>"
+        return (
+            f"<Variant {self.flag_name} in {{ {', '.join(self.choice_dict.keys())} }}>"
+        )
 
     def __getitem__(self, key: str) -> "Argument":
         return self.choice_dict[key]
 
-    def set_default(self, default_tag : Union[bool, str]):
+    def set_default(self, default_tag: Union[bool, str]):
         """Change the default tag of the current Variant."""
         if not default_tag:
             self.optional = False
             self.default_tag = ""
         else:
             if default_tag not in self.choice_dict:
                 raise ValueError(f"trying to set invalid default_tag `{default_tag}`")
             self.optional = True
             self.default_tag = default_tag
 
     def extend_choices(self, choices: Optional[Iterable["Argument"]]):
         """Add a list of choice Arguments to the current Variant"""
-        # choices is a list of arguments 
+        # choices is a list of arguments
         # whose name is treated as the switch tag
         # we convert it into a dict for better reference
         # and avoid duplicate tags
         if choices is None:
             return
-        update_nodup(self.choice_dict, ((c.name, c) for c in choices),
+        update_nodup(
+            self.choice_dict,
+            ((c.name, c) for c in choices),
             exclude={self.flag_name},
-            err_msg=f"Variant with flag `{self.flag_name}`")
-        update_nodup(self.choice_alias, 
+            err_msg=f"Variant with flag `{self.flag_name}`",
+        )
+        update_nodup(
+            self.choice_alias,
             *[[(a, c.name) for a in c.alias] for c in choices],
             exclude={self.flag_name, *self.choice_dict.keys()},
-            err_msg=f"building alias dict for Variant with flag `{self.flag_name}`")
+            err_msg=f"building alias dict for Variant with flag `{self.flag_name}`",
+        )
 
-    def add_choice(self, tag: Union[str, "Argument"], 
-                   _dtype: Union[None, type, Iterable[type]] = dict,
-                   *args, **kwargs) -> "Argument":
+    def add_choice(
+        self,
+        tag: Union[str, "Argument"],
+        _dtype: Union[None, type, Iterable[type]] = dict,
+        *args,
+        **kwargs,
+    ) -> "Argument":
         """Add a choice Argument to the current Variant"""
         if isinstance(tag, Argument):
             newarg = tag
         else:
             newarg = Argument(tag, _dtype, *args, **kwargs)
         self.extend_choices([newarg])
         return newarg
-    
+
     def dummy_argument(self):
-        return Argument(name=self.flag_name, dtype=str, 
-                        optional=self.optional, default=self.default_tag,
-                        sub_fields=None, sub_variants=None, repeat=False,
-                        alias=None, extra_check=None, 
-                        doc=f"dummy Argument converted from Variant {self.flag_name}")
+        return Argument(
+            name=self.flag_name,
+            dtype=str,
+            optional=self.optional,
+            default=self.default_tag,
+            sub_fields=None,
+            sub_variants=None,
+            repeat=False,
+            alias=None,
+            extra_check=None,
+            doc=f"dummy Argument converted from Variant {self.flag_name}",
+        )
 
     # above are creation part
     # below are helpers for traversing
 
     def get_choice(self, argdict: dict, path=None) -> "Argument":
         if self.flag_name in argdict:
             tag = argdict[self.flag_name]
             if tag in self.choice_dict:
                 return self.choice_dict[tag]
             elif tag in self.choice_alias:
                 return self.choice_dict[self.choice_alias[tag]]
             else:
-                raise ArgumentValueError(path,
-                    f"get invalid choice `{tag}` for flag key `{self.flag_name}`.")
+                raise ArgumentValueError(
+                    path, f"get invalid choice `{tag}` for flag key `{self.flag_name}`."
+                )
         elif self.optional:
             return self.choice_dict[self.default_tag]
         else:
-            raise ArgumentKeyError(path,
+            raise ArgumentKeyError(
+                path,
                 f"key `{self.flag_name}` is required "
-                 "to choose variant but not found.")
+                "to choose variant but not found.",
+            )
 
     def flatten_sub(self, argdict: dict, path=None) -> Dict[str, "Argument"]:
         choice = self.get_choice(argdict, path)
-        fields = {self.flag_name: self.dummy_argument(), # as a placeholder
-                  **choice.flatten_sub(argdict, path)}
+        fields = {
+            self.flag_name: self.dummy_argument(),  # as a placeholder
+            **choice.flatten_sub(argdict, path),
+        }
         return fields
 
     def _convert_choice_alias(self, argdict: dict, path=None):
         if self.flag_name in argdict:
             tag = argdict[self.flag_name]
             if tag not in self.choice_dict and tag in self.choice_alias:
                 argdict[self.flag_name] = self.choice_alias[tag]
 
     # above are traversing part
     # below are doc generation part
 
-    def gen_doc(self, path: Optional[List[str]] = None, 
-                      showflag : bool = False, **kwargs) -> str:
+    def gen_doc(
+        self, path: Optional[List[str]] = None, showflag: bool = False, **kwargs
+    ) -> str:
         body_list = [""]
-        body_list.append(f"Depending on the value of *{self.flag_name}*, "
-                          "different sub args are accepted. \n") 
+        body_list.append(
+            f"Depending on the value of *{self.flag_name}*, "
+            "different sub args are accepted. \n"
+        )
         body_list.append(self.gen_doc_flag(path, showflag=showflag, **kwargs))
         fnstr = f"*{self.flag_name}*"
         if kwargs.get("make_link"):
             if not kwargs.get("make_anchor"):
                 raise ValueError("`make_link` only works with `make_anchor` set")
-            fnstr, target = make_ref_pair(path+[self.flag_name], fnstr, "flag")
+            fnstr, target = make_ref_pair(path + [self.flag_name], fnstr, "flag")
             body_list.append(target + "\n")
         for choice in self.choice_dict.values():
             body_list.append("")
             choice_path = self._make_cpath(choice.name, path, showflag)
             if kwargs.get("make_anchor"):
                 body_list.append(make_rst_refid(choice_path))
-            c_alias = (f" (or its alias{'es' if len(choice.alias) > 1 else ''} "
-                      + ", ".join(f"``{al}``" for al in choice.alias) + ")"
-                      if choice.alias else "")
-            body_list.extend([
-                f"When {fnstr} is set to ``{choice.name}``{c_alias}: \n",
-                choice.gen_doc_body(choice_path, **kwargs), 
-            ])
+            c_alias = (
+                f" (or its alias{'es' if len(choice.alias) > 1 else ''} "
+                + ", ".join(f"``{al}``" for al in choice.alias)
+                + ")"
+                if choice.alias
+                else ""
+            )
+            body_list.extend(
+                [
+                    f"When {fnstr} is set to ``{choice.name}``{c_alias}: \n",
+                    choice.gen_doc_body(choice_path, **kwargs),
+                ]
+            )
         body = "\n".join(body_list)
         return body
 
     def gen_doc_flag(self, path: Optional[List[str]] = None, **kwargs) -> str:
         headdoc = f"{self.flag_name}:"
         typedoc = "| type: ``str`` (flag key)"
         if self.optional:
             typedoc += f", default: ``{self.default_tag}``"
         typedoc = indent(typedoc, INDENT)
         if path is None:
             path = []
         arg_path = [*path, self.flag_name]
-        if kwargs.get('use_sphinx_domain', False):
+        if kwargs.get("use_sphinx_domain", False):
             headdoc = f".. dargs:argument:: {self.flag_name}:\n   :path: {'/'.join(arg_path)}\n"
         pathdoc = indent(f"| argument path: ``{'/'.join(arg_path)}`` ", INDENT)
         if kwargs.get("make_link"):
             if not kwargs.get("make_anchor"):
                 raise ValueError("`make_link` only works with `make_anchor` being set")
-            l_choice, l_target = zip(*(make_ref_pair(
-                    self._make_cpath(c.name, path, kwargs["showflag"]),
-                    text=f"``{c.name}``", prefix="code") 
-                for c in self.choice_dict.values()))
-            targetdoc = indent('\n'.join(l_target) + "\n", INDENT)
+            l_choice, l_target = zip(
+                *(
+                    make_ref_pair(
+                        self._make_cpath(c.name, path, kwargs["showflag"]),
+                        text=f"``{c.name}``",
+                        prefix="code",
+                    )
+                    for c in self.choice_dict.values()
+                )
+            )
+            targetdoc = indent("\n".join(l_target) + "\n", INDENT)
         else:
             l_choice = [c.name for c in self.choice_dict.values()]
             targetdoc = None
         choicedoc = indent("| possible choices: " + ", ".join(l_choice), INDENT)
         realdoc = indent(self.doc + "\n", INDENT) if self.doc else None
         anchor = make_rst_refid(arg_path) if kwargs.get("make_anchor") else None
-        allparts = [anchor, headdoc, typedoc, pathdoc, choicedoc, "", realdoc, targetdoc]
+        allparts = [
+            anchor,
+            headdoc,
+            typedoc,
+            pathdoc,
+            choicedoc,
+            "",
+            realdoc,
+            targetdoc,
+        ]
         return "\n".join(filter(None.__ne__, allparts))
 
-    def _make_cpath(self, cname: str, 
-                    path: Optional[List[str]] = None, 
-                    showflag : bool = False):
+    def _make_cpath(
+        self, cname: str, path: Optional[List[str]] = None, showflag: bool = False
+    ):
         f_str = f"{self.flag_name}=" if showflag else ""
         c_str = f"[{f_str}{cname}]"
-        cpath = [*path[:-1], path[-1]+c_str] if path else [c_str]
+        cpath = [*path[:-1], path[-1] + c_str] if path else [c_str]
         return cpath
 
 
 def make_rst_refid(name):
     if not isinstance(name, str):
-        name = '/'.join(name)
-    return (f'.. _`{name}`: \n' if not RAW_ANCHOR
-            else f'.. raw:: html\n\n   <a id="{name}"></a>')
+        name = "/".join(name)
+    return (
+        f".. _`{name}`: \n"
+        if not RAW_ANCHOR
+        else f'.. raw:: html\n\n   <a id="{name}"></a>'
+    )
 
 
 def make_ref_pair(path, text=None, prefix=None):
     if not isinstance(path, str):
-        path = '/'.join(path)
+        path = "/".join(path)
     tgt = f"`{path}`_" if not RAW_ANCHOR else f"#{path}"
     ref = ("" if not prefix else f"{prefix}:") + path
-    inline = f'`{ref}`_' if not text else f'|{ref}|_'
-    target = f'.. _`{ref}`: {tgt}'
+    inline = f"`{ref}`_" if not text else f"|{ref}|_"
+    target = f".. _`{ref}`: {tgt}"
     if text:
-        target = f'.. |{ref}| replace:: {text}\n' + target
+        target = f".. |{ref}| replace:: {text}\n" + target
     return inline, target
 
 
-def update_nodup(this : dict, 
-                 *others : Union[dict, Iterable[tuple]], 
-                 exclude : Optional[Iterable] = None,
-                 err_msg : Optional[str] = None):
+def update_nodup(
+    this: dict,
+    *others: Union[dict, Iterable[tuple]],
+    exclude: Optional[Iterable] = None,
+    err_msg: Optional[str] = None,
+):
     for pair in others:
         if isinstance(pair, dict):
             pair = pair.items()
         for k, v in pair:
             if k in this or (exclude and k in exclude):
-                raise ValueError(f"duplicate key `{k}` when updating dict"
-                                 +("" if err_msg is None else f"in {err_msg}"))
+                raise ValueError(
+                    f"duplicate key `{k}` when updating dict"
+                    + ("" if err_msg is None else f"in {err_msg}")
+                )
             this[k] = v
     return this
 
 
-def trim_by_pattern(argdict: dict, pattern: str, 
-                    reserved: Optional[List[str]] = None,
-                    use_regex: bool = False):
+def trim_by_pattern(
+    argdict: dict,
+    pattern: str,
+    reserved: Optional[List[str]] = None,
+    use_regex: bool = False,
+):
     rep = fnmatch.translate(pattern) if not use_regex else pattern
     rem = re.compile(rep)
     if reserved:
         conflict = list(filter(rem.match, reserved))
         if conflict:
-            raise ValueError(f"pattern `{pattern}` conflicts with the "
-                                f"following reserved names: {', '.join(conflict)}")
+            raise ValueError(
+                f"pattern `{pattern}` conflicts with the "
+                f"following reserved names: {', '.join(conflict)}"
+            )
     unrequired = list(filter(rem.match, argdict.keys()))
     for key in unrequired:
         argdict.pop(key)
 
 
 class ArgumentEncoder(json.JSONEncoder):
     """Extended JSON Encoder to encode Argument object:
 
     Examples
     --------
     >>> json.dumps(some_arg, cls=ArgumentEncoder)
     """
+
     def default(self, obj) -> Dict[str, Union[str, bool, List]]:
         """Generate a dict containing argument information, making it ready to be encoded
         to JSON string.
 
         Notes
         -----
         All object in the dict should be JSON serializable.
@@ -823,15 +977,15 @@
                 "alias": obj.alias,
                 "doc": obj.doc,
                 "repeat": obj.repeat,
                 "sub_fields": obj.sub_fields,
                 "sub_variants": obj.sub_variants,
             }
             if obj.optional and obj.default is not _Flags.NONE:
-                output['default'] = obj.default
+                output["default"] = obj.default
             return output
         elif isinstance(obj, Variant):
             return {
                 "object": "Variant",
                 "flag_name": obj.flag_name,
                 "optional": obj.optional,
                 "default_tag": obj.default_tag,
```

### Comparing `dargs-0.3.4/dargs/sphinx.py` & `dargs-0.3.5/dargs/sphinx.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 .. code-block:: rst
 
     .. dargs::
        :module: dargs.sphinx
        :func: _test_argument
 
-where `_test_argument` returns an :class:`Argument <dargs.Argument>`. A :class:`list` of :class:`Argument <dargs.Argument>` is also accepted. 
+where `_test_argument` returns an :class:`Argument <dargs.Argument>`. A :class:`list` of :class:`Argument <dargs.Argument>` is also accepted.
 """
 import sys
 from typing import List
 
 from docutils.parsers.rst import Directive
 from docutils.parsers.rst.directives import unchanged
 from sphinx import addnodes
@@ -31,140 +31,166 @@
 from sphinx.util.nodes import make_refnode
 
 from .dargs import Argument, Variant
 
 
 class DargsDirective(Directive):
     """dargs directive"""
+
     has_content = True
     option_spec = dict(
         module=unchanged,
         func=unchanged,
     )
 
-
     def run(self):
-        if 'module' in self.options and 'func' in self.options:
-            module_name = self.options['module']
-            attr_name = self.options['func']
+        if "module" in self.options and "func" in self.options:
+            module_name = self.options["module"]
+            attr_name = self.options["func"]
         else:
-            raise self.error(':module: and :func: should be specified')
+            raise self.error(":module: and :func: should be specified")
 
         try:
             mod = __import__(module_name, globals(), locals(), [attr_name])
         except ImportError:
-            raise self.error(f'Failed to import "{attr_name}" from "{module_name}".\n{sys.exc_info()[1]}')
+            raise self.error(
+                f'Failed to import "{attr_name}" from "{module_name}".\n{sys.exc_info()[1]}'
+            )
 
         if not hasattr(mod, attr_name):
-            raise self.error(('Module "%s" has no attribute "%s"\n' 'Incorrect argparse :module: or :func: values?') % (module_name, attr_name))
+            raise self.error(
+                (
+                    'Module "%s" has no attribute "%s"\n'
+                    "Incorrect argparse :module: or :func: values?"
+                )
+                % (module_name, attr_name)
+            )
         func = getattr(mod, attr_name)
         arguments = func()
 
         if not isinstance(arguments, (list, tuple)):
             arguments = [arguments]
 
         rsts = []
         for argument in arguments:
             if not isinstance(argument, (Argument, Variant)):
                 raise RuntimeError("The function doesn't return Argument")
-            rst = argument.gen_doc(make_anchor=True, make_link=True, use_sphinx_domain=True)
+            rst = argument.gen_doc(
+                make_anchor=True, make_link=True, use_sphinx_domain=True
+            )
             rsts.extend(rst.split("\n"))
-        self.state_machine.insert_input(rsts, "%s:%s" %(module_name, attr_name))
+        self.state_machine.insert_input(rsts, "%s:%s" % (module_name, attr_name))
         return []
 
 
 class DargsObject(ObjectDescription):
     """dargs::argument directive.
-    
+
     This directive creates a signature node for an argument.
     """
+
     option_spec = dict(
         path=unchanged,
     )
 
     def handle_signature(self, sig, signode):
         signode += addnodes.desc_name(sig, sig)
         return sig
 
     def add_target_and_index(self, name, sig, signode):
-        path = self.options['path']
+        path = self.options["path"]
         targetid = "%s:%s" % (self.objtype, path)
         if targetid not in self.state.document.ids:
-            signode['names'].append(targetid)
-            signode['ids'].append(targetid)
-            signode['first'] = (not self.names)
+            signode["names"].append(targetid)
+            signode["ids"].append(targetid)
+            signode["first"] = not self.names
             self.state.document.note_explicit_target(signode)
             # for cross-references
-            inv = self.env.domaindata['dargs']['arguments']
+            inv = self.env.domaindata["dargs"]["arguments"]
             if targetid in inv:
                 self.state.document.reporter.warning(
-                    'Duplicated argument "%s" described in "%s".' %
-                    (targetid, self.env.doc2path(inv[targetid][0])), line=self.lineno)
+                    'Duplicated argument "%s" described in "%s".'
+                    % (targetid, self.env.doc2path(inv[targetid][0])),
+                    line=self.lineno,
+                )
             inv[targetid] = (self.env.docname, self.objtype)
 
-        self.indexnode['entries'].append(('pair', u'%s ; %s (%s) ' % (name, path, self.objtype.title()), targetid, 'main', None))
+        self.indexnode["entries"].append(
+            (
+                "pair",
+                "%s ; %s (%s) " % (name, path, self.objtype.title()),
+                targetid,
+                "main",
+                None,
+            )
+        )
 
 
 class DargsDomain(Domain):
     """Dargs domain.
-    
+
     Includes:
     - dargs::argument directive
     - dargs::argument role
     """
-    name = 'dargs'
-    label = 'dargs'
+
+    name = "dargs"
+    label = "dargs"
     object_types = {
-        'argument': ObjType('argument', 'argument'),
+        "argument": ObjType("argument", "argument"),
     }
     directives = {
-        'argument': DargsObject,
+        "argument": DargsObject,
     }
     roles = {
-        'argument': XRefRole(),
+        "argument": XRefRole(),
     }
 
     initial_data = {
-        'arguments': {},  # fullname -> docname, objtype
+        "arguments": {},  # fullname -> docname, objtype
     }
 
-    def resolve_xref(self, env, fromdocname, builder,
-                     typ, target, node, contnode):
+    def resolve_xref(self, env, fromdocname, builder, typ, target, node, contnode):
         """Resolve cross-references."""
-        targetid = '%s:%s' % (typ, target)
-        obj = self.data['arguments'].get(targetid)
+        targetid = "%s:%s" % (typ, target)
+        obj = self.data["arguments"].get(targetid)
         if obj is None:
             return None
-        return make_refnode(builder, fromdocname, obj[0], targetid,
-                            contnode, target)
+        return make_refnode(builder, fromdocname, obj[0], targetid, contnode, target)
 
 
 def setup(app):
     """Setup sphinx app."""
-    app.add_directive('dargs', DargsDirective)
+    app.add_directive("dargs", DargsDirective)
     app.add_domain(DargsDomain)
-    return {'parallel_read_safe': True}
+    return {"parallel_read_safe": True}
 
 
 def _test_argument() -> Argument:
     """This internal function is used to generate docs of dargs."""
     doc_test = "This argument/variant is only used to test."
-    return Argument(name="test", dtype=str, doc=doc_test,
+    return Argument(
+        name="test",
+        dtype=str,
+        doc=doc_test,
         sub_fields=[
             Argument("test_argument", dtype=str, doc=doc_test, default="test"),
         ],
         sub_variants=[
-            Variant("test_variant", doc=doc_test,
+            Variant(
+                "test_variant",
+                doc=doc_test,
                 choices=[
                     Argument("test_variant_argument", dtype=str, doc=doc_test),
                 ],
             ),
         ],
     )
 
+
 def _test_arguments() -> List[Argument]:
     """Returns a list of arguments."""
     return [
         Argument(name="test1", dtype=int, doc="Argument 1"),
         Argument(name="test2", dtype=[float, None], doc="Argument 2"),
         Argument(name="test3", dtype=list, doc="Argument 3"),
     ]
```

### Comparing `dargs-0.3.4/dargs.egg-info/PKG-INFO` & `dargs-0.3.5/dargs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dargs
-Version: 0.3.4
+Version: 0.3.5
 Summary: Process arguments for the deep modeling project.
 Author: DeepModeling
 Author-email: Yixiao Chen <yixiaoc@princeton.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -177,27 +177,27 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Argument checking for python programs
 
-This is a minimum version for checking the input argument dict. 
-It would examine argument's type,  as well as keys and types of its sub-arguments. 
+This is a minimum version for checking the input argument dict.
+It would examine argument's type,  as well as keys and types of its sub-arguments.
 
-A special case called *variant* is also handled, 
-where you can determine the items of a dict based the value of on one of its `flag_name` key. 
+A special case called *variant* is also handled,
+where you can determine the items of a dict based the value of on one of its `flag_name` key.
 
 There are three main methods of `Argument` class:
 
 - `check` method that takes a dict and see if its type follows the definition in the class
 - `normalize` method that takes a dict and convert alias and add default value into it
 - `gendoc` method that outputs the defined argument structure and corresponding docs
 
-There are also `check_value` and `normalize_value` that 
+There are also `check_value` and `normalize_value` that
 ignore the leading key comparing to the base version.
 
-When targeting to html rendering, additional anchor can be made for cross reference. 
+When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
```

### Comparing `dargs-0.3.4/dargs.egg-info/SOURCES.txt` & `dargs-0.3.5/dargs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
+codecov.yml
 pyproject.toml
 .github/workflows/mirror_gitee.yml
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
 dargs/__init__.py
 dargs/_version.py
 dargs/dargs.py
```

### Comparing `dargs-0.3.4/docs/Makefile` & `dargs-0.3.5/docs/Makefile`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `dargs-0.3.4/docs/conf.py` & `dargs-0.3.5/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,93 +11,94 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 from datetime import date
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'dargs'
-copyright = '2020-%d, DeepModeling ' % date.today().year
-author = 'DeepModeling'
+project = "dargs"
+copyright = "2020-%d, DeepModeling " % date.today().year
+author = "DeepModeling"
 
 # The short X.Y version
-version = '0.0'
+version = "0.0"
 # The full version, including alpha/beta/rc tags
-release = '0.0.0-rc'
+release = "0.0.0-rc"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'deepmodeling_sphinx',
-    'sphinx_rtd_theme',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.intersphinx',
-    'numpydoc',
-    'myst_parser',
-    'dargs.sphinx',
+    "deepmodeling_sphinx",
+    "sphinx_rtd_theme",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.intersphinx",
+    "numpydoc",
+    "myst_parser",
+    "dargs.sphinx",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = ['.rst', '.md']
+source_suffix = [".rst", ".md"]
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-#html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
@@ -105,76 +106,89 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'dargsdoc'
+htmlhelp_basename = "dargsdoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'dargs.tex', 'dargs Documentation',
-     'DeepModeling', 'manual'),
+    (master_doc, "dargs.tex", "dargs Documentation", "DeepModeling", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'dargs', 'dargs Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "dargs", "dargs Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'dargs', 'dargs Documentation',
-     author, 'dargs', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "dargs",
+        "dargs Documentation",
+        author,
+        "dargs",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 def run_apidoc(_):
     from sphinx.ext.apidoc import main
-    sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+    sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
     cur_dir = os.path.abspath(os.path.dirname(__file__))
     module = os.path.join(cur_dir, "..", "dargs")
-    main(['-M', '--tocfile', 'api', '-H', 'API documentation', '-o', os.path.join(cur_dir, "api"), module, '--force'])
+    main(
+        [
+            "-M",
+            "--tocfile",
+            "api",
+            "-H",
+            "API documentation",
+            "-o",
+            os.path.join(cur_dir, "api"),
+            module,
+            "--force",
+        ]
+    )
+
 
 def setup(app):
-    app.connect('builder-inited', run_apidoc)
+    app.connect("builder-inited", run_apidoc)
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/", None),
 }
```

### Comparing `dargs-0.3.4/docs/intro.md` & `dargs-0.3.5/docs/intro.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Argument checking for python programs
 
-This is a minimum version for checking the input argument dict. 
-It would examine argument's type,  as well as keys and types of its sub-arguments. 
+This is a minimum version for checking the input argument dict.
+It would examine argument's type,  as well as keys and types of its sub-arguments.
 
-A special case called *variant* is also handled, 
-where you can determine the items of a dict based the value of on one of its `flag_name` key. 
+A special case called *variant* is also handled,
+where you can determine the items of a dict based the value of on one of its `flag_name` key.
 
 There are three main methods of `Argument` class:
 
 - `check` method that takes a dict and see if its type follows the definition in the class
 - `normalize` method that takes a dict and convert alias and add default value into it
 - `gendoc` method that outputs the defined argument structure and corresponding docs
 
-There are also `check_value` and `normalize_value` that 
+There are also `check_value` and `normalize_value` that
 ignore the leading key comparing to the base version.
 
-When targeting to html rendering, additional anchor can be made for cross reference. 
+When targeting to html rendering, additional anchor can be made for cross reference.
 Set `make_anchor=True` when calling `gendoc` function and use standard ref syntax in rst.
 The id is the same as the argument path. Variant types would be in square brackets.
 
 Please refer to test files for detailed usage.
```

### Comparing `dargs-0.3.4/docs/sphinx.rst` & `dargs-0.3.5/docs/sphinx.rst`

 * *Files identical despite different names*

### Comparing `dargs-0.3.4/pyproject.toml` & `dargs-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dargs-0.3.4/tests/dpmdargs.py` & `dargs-0.3.5/tests/dpmdargs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .context import dargs
 from dargs import dargs, Argument, Variant
 
 ACTIVATION_FN_DICT = {
-    "relu": None, 
+    "relu": None,
     "relu6": None,
     "softplus": None,
     "sigmoid": None,
     "tanh": None,
     "gelu": None,
 }
 
@@ -14,478 +14,711 @@
     "default": None,
     "float16": None,
     "float32": None,
     "float64": None,
 }
 
 
-def list_to_doc (xx):
+def list_to_doc(xx):
     items = []
     for ii in xx:
         if len(items) == 0:
             items.append(f'"{ii}"')
         else:
             items.append(f', "{ii}"')
-    items.append('.')
-    return ''.join(items)
+    items.append(".")
+    return "".join(items)
 
 
-def make_link(content, ref_key) :
-    return f'`{content} <{ref_key}_>`_' if not dargs.RAW_ANCHOR else f'`{content} <#{ref_key}>`_'
-
-
-def descrpt_local_frame_args ():
-    doc_sel_a = 'A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_a[i]` gives the selected number of type-i neighbors. The full relative coordinates of the neighbors are used by the descriptor.'
-    doc_sel_r = 'A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_r[i]` gives the selected number of type-i neighbors. Only relative distance of the neighbors are used by the descriptor. sel_a[i] + sel_r[i] is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius.'
-    doc_rcut = 'The cut-off radius. The default value is 6.0'
-    doc_axis_rule = 'A list of integers. The length should be 6 times of the number of types. \n\n\
+def make_link(content, ref_key):
+    return (
+        f"`{content} <{ref_key}_>`_"
+        if not dargs.RAW_ANCHOR
+        else f"`{content} <#{ref_key}>`_"
+    )
+
+
+def descrpt_local_frame_args():
+    doc_sel_a = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_a[i]` gives the selected number of type-i neighbors. The full relative coordinates of the neighbors are used by the descriptor."
+    doc_sel_r = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_r[i]` gives the selected number of type-i neighbors. Only relative distance of the neighbors are used by the descriptor. sel_a[i] + sel_r[i] is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius."
+    doc_rcut = "The cut-off radius. The default value is 6.0"
+    doc_axis_rule = "A list of integers. The length should be 6 times of the number of types. \n\n\
 - axis_rule[i*6+0]: class of the atom defining the first axis of type-i atom. 0 for neighbors with full coordinates and 1 for neighbors only with relative distance.\n\n\
 - axis_rule[i*6+1]: type of the atom defining the first axis of type-i atom.\n\n\
 - axis_rule[i*6+2]: index of the axis atom defining the first axis. Note that the neighbors with the same class and type are sorted according to their relative distance.\n\n\
 - axis_rule[i*6+3]: class of the atom defining the first axis of type-i atom. 0 for neighbors with full coordinates and 1 for neighbors only with relative distance.\n\n\
 - axis_rule[i*6+4]: type of the atom defining the second axis of type-i atom.\n\n\
-- axis_rule[i*6+5]: class of the atom defining the second axis of type-i atom. 0 for neighbors with full coordinates and 1 for neighbors only with relative distance.'
-    
+- axis_rule[i*6+5]: class of the atom defining the second axis of type-i atom. 0 for neighbors with full coordinates and 1 for neighbors only with relative distance."
+
     return [
-        Argument("sel_a", list, optional = False, doc = doc_sel_a),
-        Argument("sel_r", list, optional = False, doc = doc_sel_r),
-        Argument("rcut", float, optional = True, default = 6.0, doc = doc_rcut),
-        Argument("axis_rule", list, optional = False, doc = doc_axis_rule)
+        Argument("sel_a", list, optional=False, doc=doc_sel_a),
+        Argument("sel_r", list, optional=False, doc=doc_sel_r),
+        Argument("rcut", float, optional=True, default=6.0, doc=doc_rcut),
+        Argument("axis_rule", list, optional=False, doc=doc_axis_rule),
     ]
 
 
 def descrpt_se_a_args():
-    doc_sel = 'A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius.'
-    doc_rcut = 'The cut-off radius.'
-    doc_rcut_smth = 'Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`'
-    doc_neuron = 'Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built.'
-    doc_axis_neuron = 'Size of the submatrix of G (embedding matrix).'
-    doc_activation_function = f'The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
+    doc_sel = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius."
+    doc_rcut = "The cut-off radius."
+    doc_rcut_smth = "Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`"
+    doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
+    doc_axis_neuron = "Size of the submatrix of G (embedding matrix)."
+    doc_activation_function = f"The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_type_one_side = 'Try to build N_types embedding nets. Otherwise, building N_types^2 embedding nets'
-    doc_precision = f'The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
-    doc_trainable = 'If the parameters in the embedding net is trainable'
-    doc_seed = 'Random seed for parameter initialization'
-    doc_exclude_types = 'The Excluded types'
-    doc_set_davg_zero = 'Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used'
-    
-    return [
-        Argument("sel", list, optional = False, doc = doc_sel),
-        Argument("rcut", float, optional = True, default = 6.0, doc = doc_rcut),
-        Argument("rcut_smth", float, optional = True, default = 0.5, doc = doc_rcut_smth),
-        Argument("neuron", list, optional = True, default = [10,20,40], doc = doc_neuron),
-        Argument("axis_neuron", int, optional = True, default = 4, doc = doc_axis_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("resnet_dt", bool, optional = True, default = False, doc = doc_resnet_dt),
-        Argument("type_one_side", bool, optional = True, default = False, doc = doc_type_one_side),
-        Argument("precision", str, optional = True, default = "float64", doc = doc_precision),
-        Argument("trainable", bool, optional = True, default = True, doc = doc_trainable),
-        Argument("seed", [int,None], optional = True, doc = doc_seed),
-        Argument("exclude_types", list, optional = True, default = [], doc = doc_exclude_types),
-        Argument("set_davg_zero", bool, optional = True, default = False, doc = doc_set_davg_zero)
+    doc_type_one_side = "Try to build N_types embedding nets. Otherwise, building N_types^2 embedding nets"
+    doc_precision = f"The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
+    doc_trainable = "If the parameters in the embedding net is trainable"
+    doc_seed = "Random seed for parameter initialization"
+    doc_exclude_types = "The Excluded types"
+    doc_set_davg_zero = "Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used"
+
+    return [
+        Argument("sel", list, optional=False, doc=doc_sel),
+        Argument("rcut", float, optional=True, default=6.0, doc=doc_rcut),
+        Argument("rcut_smth", float, optional=True, default=0.5, doc=doc_rcut_smth),
+        Argument("neuron", list, optional=True, default=[10, 20, 40], doc=doc_neuron),
+        Argument("axis_neuron", int, optional=True, default=4, doc=doc_axis_neuron),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("resnet_dt", bool, optional=True, default=False, doc=doc_resnet_dt),
+        Argument(
+            "type_one_side", bool, optional=True, default=False, doc=doc_type_one_side
+        ),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("trainable", bool, optional=True, default=True, doc=doc_trainable),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+        Argument(
+            "exclude_types", list, optional=True, default=[], doc=doc_exclude_types
+        ),
+        Argument(
+            "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
+        ),
     ]
 
 
 def descrpt_se_a_3be_args():
-    doc_sel = 'A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius.'
-    doc_rcut = 'The cut-off radius.'
-    doc_rcut_smth = 'Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`'
-    doc_neuron = 'Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built.'
-    doc_activation_function = f'The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
+    doc_sel = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius."
+    doc_rcut = "The cut-off radius."
+    doc_rcut_smth = "Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`"
+    doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
+    doc_activation_function = f"The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_precision = f'The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
-    doc_trainable = 'If the parameters in the embedding net is trainable'
-    doc_seed = 'Random seed for parameter initialization'
-    doc_set_davg_zero = 'Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used'
-    
-    return [
-        Argument("sel", list, optional = False, doc = doc_sel),
-        Argument("rcut", float, optional = True, default = 6.0, doc = doc_rcut),
-        Argument("rcut_smth", float, optional = True, default = 0.5, doc = doc_rcut_smth),
-        Argument("neuron", list, optional = True, default = [10,20,40], doc = doc_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("resnet_dt", bool, optional = True, default = False, doc = doc_resnet_dt),
-        Argument("precision", str, optional = True, default = "float64", doc = doc_precision),
-        Argument("trainable", bool, optional = True, default = True, doc = doc_trainable),
-        Argument("seed", [int,None], optional = True, doc = doc_seed),
-        Argument("set_davg_zero", bool, optional = True, default = False, doc = doc_set_davg_zero)
+    doc_precision = f"The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
+    doc_trainable = "If the parameters in the embedding net is trainable"
+    doc_seed = "Random seed for parameter initialization"
+    doc_set_davg_zero = "Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used"
+
+    return [
+        Argument("sel", list, optional=False, doc=doc_sel),
+        Argument("rcut", float, optional=True, default=6.0, doc=doc_rcut),
+        Argument("rcut_smth", float, optional=True, default=0.5, doc=doc_rcut_smth),
+        Argument("neuron", list, optional=True, default=[10, 20, 40], doc=doc_neuron),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("resnet_dt", bool, optional=True, default=False, doc=doc_resnet_dt),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("trainable", bool, optional=True, default=True, doc=doc_trainable),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+        Argument(
+            "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
+        ),
     ]
 
 
-
 def descrpt_se_a_tpe_args():
-    doc_type_nchanl = 'number of channels for type embedding'
-    doc_type_nlayer = 'number of hidden layers of type embedding net'
-    doc_numb_aparam = 'dimension of atomic parameter. if set to a value > 0, the atomic parameters are embedded.'
-
-    return descrpt_se_a_args() + [        
-        Argument("type_nchanl", int, optional = True, default = 4, doc = doc_type_nchanl),
-        Argument("type_nlayer", int, optional = True, default = 2, doc = doc_type_nlayer),
-        Argument("numb_aparam", int, optional = True, default = 0, doc = doc_numb_aparam)
+    doc_type_nchanl = "number of channels for type embedding"
+    doc_type_nlayer = "number of hidden layers of type embedding net"
+    doc_numb_aparam = "dimension of atomic parameter. if set to a value > 0, the atomic parameters are embedded."
+
+    return descrpt_se_a_args() + [
+        Argument("type_nchanl", int, optional=True, default=4, doc=doc_type_nchanl),
+        Argument("type_nlayer", int, optional=True, default=2, doc=doc_type_nlayer),
+        Argument("numb_aparam", int, optional=True, default=0, doc=doc_numb_aparam),
     ]
 
 
 def descrpt_se_r_args():
-    doc_sel = 'A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius.'
-    doc_rcut = 'The cut-off radius.'
-    doc_rcut_smth = 'Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`'
-    doc_neuron = 'Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built.'
-    doc_activation_function = f'The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
+    doc_sel = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius."
+    doc_rcut = "The cut-off radius."
+    doc_rcut_smth = "Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`"
+    doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
+    doc_activation_function = f"The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_type_one_side = 'Try to build N_types embedding nets. Otherwise, building N_types^2 embedding nets'
-    doc_precision = f'The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
-    doc_trainable = 'If the parameters in the embedding net is trainable'
-    doc_seed = 'Random seed for parameter initialization'
-    doc_exclude_types = 'The Excluded types'
-    doc_set_davg_zero = 'Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used'
-    
-    return [
-        Argument("sel", list, optional = False, doc = doc_sel),
-        Argument("rcut", float, optional = True, default = 6.0, doc = doc_rcut),
-        Argument("rcut_smth", float, optional = True, default = 0.5, doc = doc_rcut_smth),
-        Argument("neuron", list, optional = True, default = [10,20,40], doc = doc_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("resnet_dt", bool, optional = True, default = False, doc = doc_resnet_dt),
-        Argument("type_one_side", bool, optional = True, default = False, doc = doc_type_one_side),
-        Argument("precision", str, optional = True, default = "float64", doc = doc_precision),
-        Argument("trainable", bool, optional = True, default = True, doc = doc_trainable),
-        Argument("seed", [int,None], optional = True, doc = doc_seed),
-        Argument("exclude_types", list, optional = True, default = [], doc = doc_exclude_types),
-        Argument("set_davg_zero", bool, optional = True, default = False, doc = doc_set_davg_zero)
+    doc_type_one_side = "Try to build N_types embedding nets. Otherwise, building N_types^2 embedding nets"
+    doc_precision = f"The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
+    doc_trainable = "If the parameters in the embedding net is trainable"
+    doc_seed = "Random seed for parameter initialization"
+    doc_exclude_types = "The Excluded types"
+    doc_set_davg_zero = "Set the normalization average to zero. This option should be set when `atom_ener` in the energy fitting is used"
+
+    return [
+        Argument("sel", list, optional=False, doc=doc_sel),
+        Argument("rcut", float, optional=True, default=6.0, doc=doc_rcut),
+        Argument("rcut_smth", float, optional=True, default=0.5, doc=doc_rcut_smth),
+        Argument("neuron", list, optional=True, default=[10, 20, 40], doc=doc_neuron),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("resnet_dt", bool, optional=True, default=False, doc=doc_resnet_dt),
+        Argument(
+            "type_one_side", bool, optional=True, default=False, doc=doc_type_one_side
+        ),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("trainable", bool, optional=True, default=True, doc=doc_trainable),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+        Argument(
+            "exclude_types", list, optional=True, default=[], doc=doc_exclude_types
+        ),
+        Argument(
+            "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
+        ),
     ]
 
 
 def descrpt_se_ar_args():
-    link = make_link('se_a', 'model/descriptor[se_a]')
-    doc_a = f'The parameters of descriptor {link}'
-    link = make_link('se_r', 'model/descriptor[se_r]')
-    doc_r = f'The parameters of descriptor {link}'
-    
+    link = make_link("se_a", "model/descriptor[se_a]")
+    doc_a = f"The parameters of descriptor {link}"
+    link = make_link("se_r", "model/descriptor[se_r]")
+    doc_r = f"The parameters of descriptor {link}"
+
     return [
-        Argument("a", dict, optional = False, doc = doc_a),
-        Argument("r", dict, optional = False, doc = doc_r),
+        Argument("a", dict, optional=False, doc=doc_a),
+        Argument("r", dict, optional=False, doc=doc_r),
     ]
 
 
 def descrpt_hybrid_args():
-    doc_list = f'A list of descriptor definitions'
-    
+    doc_list = f"A list of descriptor definitions"
+
     return [
-        Argument("list", list, [], [
-            Variant("type", [
-                Argument("loc_frame", dict, descrpt_local_frame_args()),
-                Argument("se_a", dict, descrpt_se_a_args()),
-                Argument("se_r", dict, descrpt_se_r_args()),
-                Argument("se_a_3be", dict, descrpt_se_a_3be_args(), alias = ['se_at']),
-                Argument("se_a_tpe", dict, descrpt_se_a_tpe_args(), alias = ['se_a_ebd'])])],
-            repeat=True, optional = False, doc = doc_list, fold_subdoc=True)
+        Argument(
+            "list",
+            list,
+            [],
+            [
+                Variant(
+                    "type",
+                    [
+                        Argument("loc_frame", dict, descrpt_local_frame_args()),
+                        Argument("se_a", dict, descrpt_se_a_args()),
+                        Argument("se_r", dict, descrpt_se_r_args()),
+                        Argument(
+                            "se_a_3be", dict, descrpt_se_a_3be_args(), alias=["se_at"]
+                        ),
+                        Argument(
+                            "se_a_tpe",
+                            dict,
+                            descrpt_se_a_tpe_args(),
+                            alias=["se_a_ebd"],
+                        ),
+                    ],
+                )
+            ],
+            repeat=True,
+            optional=False,
+            doc=doc_list,
+            fold_subdoc=True,
+        )
     ]
 
 
 def descrpt_variant_type_args():
-    link_lf = make_link('loc_frame', 'model/descriptor[loc_frame]')
-    link_se_a = make_link('se_a', 'model/descriptor[se_a]')
-    link_se_r = make_link('se_r', 'model/descriptor[se_r]')
-    link_se_a_3be = make_link('se_a_3be', 'model/descriptor[se_a_3be]')
-    link_se_a_tpe = make_link('se_a_tpe', 'model/descriptor[se_a_tpe]')
-    link_hybrid = make_link('hybrid', 'model/descriptor[hybrid]')
-    doc_descrpt_type = f'The type of the descritpor. See explanation below. \n\n\
+    link_lf = make_link("loc_frame", "model/descriptor[loc_frame]")
+    link_se_a = make_link("se_a", "model/descriptor[se_a]")
+    link_se_r = make_link("se_r", "model/descriptor[se_r]")
+    link_se_a_3be = make_link("se_a_3be", "model/descriptor[se_a_3be]")
+    link_se_a_tpe = make_link("se_a_tpe", "model/descriptor[se_a_tpe]")
+    link_hybrid = make_link("hybrid", "model/descriptor[hybrid]")
+    doc_descrpt_type = f"The type of the descritpor. See explanation below. \n\n\
 - `loc_frame`: Defines a local frame at each atom, and the compute the descriptor as local coordinates under this frame.\n\n\
 - `se_a`: Used by the smooth edition of Deep Potential. The full relative coordinates are used to construct the descriptor.\n\n\
 - `se_r`: Used by the smooth edition of Deep Potential. Only the distance between atoms is used to construct the descriptor.\n\n\
 - `se_a_3be`: Used by the smooth edition of Deep Potential. The full relative coordinates are used to construct the descriptor. Three-body embedding will be used by this descriptor.\n\n\
 - `se_a_tpe`: Used by the smooth edition of Deep Potential. The full relative coordinates are used to construct the descriptor. Type embedding will be used by this descriptor.\n\n\
-- `hybrid`: Concatenate of a list of descriptors as a new descriptor.'
-    
-    return Variant("type", [
-        Argument("loc_frame", dict, descrpt_local_frame_args()),
-        Argument("se_a", dict, descrpt_se_a_args()),
-        Argument("se_r", dict, descrpt_se_r_args()),
-        Argument("se_a_3be", dict, descrpt_se_a_3be_args(), alias = ['se_at']),
-        Argument("se_a_tpe", dict, descrpt_se_a_tpe_args(), alias = ['se_a_ebd']),
-        Argument("hybrid", dict, descrpt_hybrid_args()),
-    ], doc = doc_descrpt_type)
+- `hybrid`: Concatenate of a list of descriptors as a new descriptor."
+
+    return Variant(
+        "type",
+        [
+            Argument("loc_frame", dict, descrpt_local_frame_args()),
+            Argument("se_a", dict, descrpt_se_a_args()),
+            Argument("se_r", dict, descrpt_se_r_args()),
+            Argument("se_a_3be", dict, descrpt_se_a_3be_args(), alias=["se_at"]),
+            Argument("se_a_tpe", dict, descrpt_se_a_tpe_args(), alias=["se_a_ebd"]),
+            Argument("hybrid", dict, descrpt_hybrid_args()),
+        ],
+        doc=doc_descrpt_type,
+    )
 
 
 def fitting_ener():
-    doc_numb_fparam = 'The dimension of the frame parameter. If set to >0, file `fparam.npy` should be included to provided the input fparams.'
-    doc_numb_aparam = 'The dimension of the atomic parameter. If set to >0, file `aparam.npy` should be included to provided the input aparams.'
-    doc_neuron = 'The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built.'
-    doc_activation_function = f'The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
-    doc_precision = f'The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
+    doc_numb_fparam = "The dimension of the frame parameter. If set to >0, file `fparam.npy` should be included to provided the input fparams."
+    doc_numb_aparam = "The dimension of the atomic parameter. If set to >0, file `aparam.npy` should be included to provided the input aparams."
+    doc_neuron = "The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built."
+    doc_activation_function = f"The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
+    doc_precision = f"The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_trainable = 'Whether the parameters in the fitting net are trainable. This option can be\n\n\
+    doc_trainable = "Whether the parameters in the fitting net are trainable. This option can be\n\n\
 - bool: True if all parameters of the fitting net are trainable, False otherwise.\n\n\
-- list of bool: Specifies if each layer is trainable. Since the fitting net is composed by hidden layers followed by a output layer, the length of tihs list should be equal to len(`neuron`)+1.'
-    doc_rcond = 'The condition number used to determine the inital energy shift for each type of atoms.'
-    doc_seed = 'Random seed for parameter initialization of the fitting net'
-    doc_atom_ener = 'Specify the atomic energy in vacuum for each type'
-
-    return [
-        Argument("numb_fparam", int, optional = True, default = 0, doc = doc_numb_fparam),
-        Argument("numb_aparam", int, optional = True, default = 0, doc = doc_numb_aparam),
-        Argument("neuron", list, optional = True, default = [120,120,120], doc = doc_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("precision", str, optional = True, default = 'float64', doc = doc_precision),
-        Argument("resnet_dt", bool, optional = True, default = True, doc = doc_resnet_dt),
-        Argument("trainable", [list,bool], optional = True, default = True, doc = doc_trainable),
-        Argument("rcond", float, optional = True, default = 1e-3, doc = doc_rcond),
-        Argument("seed", [int,None], optional = True, doc = doc_seed),
-        Argument("atom_ener", list, optional = True, default = [], doc = doc_atom_ener)
+- list of bool: Specifies if each layer is trainable. Since the fitting net is composed by hidden layers followed by a output layer, the length of tihs list should be equal to len(`neuron`)+1."
+    doc_rcond = "The condition number used to determine the inital energy shift for each type of atoms."
+    doc_seed = "Random seed for parameter initialization of the fitting net"
+    doc_atom_ener = "Specify the atomic energy in vacuum for each type"
+
+    return [
+        Argument("numb_fparam", int, optional=True, default=0, doc=doc_numb_fparam),
+        Argument("numb_aparam", int, optional=True, default=0, doc=doc_numb_aparam),
+        Argument(
+            "neuron", list, optional=True, default=[120, 120, 120], doc=doc_neuron
+        ),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("resnet_dt", bool, optional=True, default=True, doc=doc_resnet_dt),
+        Argument(
+            "trainable", [list, bool], optional=True, default=True, doc=doc_trainable
+        ),
+        Argument("rcond", float, optional=True, default=1e-3, doc=doc_rcond),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+        Argument("atom_ener", list, optional=True, default=[], doc=doc_atom_ener),
     ]
 
 
 def fitting_polar():
-    doc_neuron = 'The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built.'
-    doc_activation_function = f'The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
+    doc_neuron = "The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built."
+    doc_activation_function = f"The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_precision = f'The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
-    doc_scale = 'The output of the fitting net (polarizability matrix) will be scaled by ``scale``'
-    doc_diag_shift = 'The diagonal part of the polarizability matrix  will be shifted by ``diag_shift``. The shift operation is carried out after ``scale``.'
-    doc_fit_diag = 'Fit the diagonal part of the rotational invariant polarizability matrix, which will be converted to normal polarizability matrix by contracting with the rotation matrix.'
-    doc_sel_type = 'The atom types for which the atomic polarizability will be provided. If not set, all types will be selected.'
-    doc_seed = 'Random seed for parameter initialization of the fitting net'
-    
-    return [
-        Argument("neuron", list, optional = True, default = [120,120,120], doc = doc_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("resnet_dt", bool, optional = True, default = True, doc = doc_resnet_dt),
-        Argument("precision", str, optional = True, default = 'float64', doc = doc_precision),
-        Argument("fit_diag", bool, optional = True, default = True, doc = doc_fit_diag),
-        Argument("scale", [list,float], optional = True, default = 1.0, doc = doc_scale),
-        Argument("diag_shift", [list,float], optional = True, default = 0.0, doc = doc_diag_shift),
-        Argument("sel_type", [list,int,None], optional = True, doc = doc_sel_type),
-        Argument("seed", [int,None], optional = True, doc = doc_seed)
+    doc_precision = f"The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
+    doc_scale = "The output of the fitting net (polarizability matrix) will be scaled by ``scale``"
+    doc_diag_shift = "The diagonal part of the polarizability matrix  will be shifted by ``diag_shift``. The shift operation is carried out after ``scale``."
+    doc_fit_diag = "Fit the diagonal part of the rotational invariant polarizability matrix, which will be converted to normal polarizability matrix by contracting with the rotation matrix."
+    doc_sel_type = "The atom types for which the atomic polarizability will be provided. If not set, all types will be selected."
+    doc_seed = "Random seed for parameter initialization of the fitting net"
+
+    return [
+        Argument(
+            "neuron", list, optional=True, default=[120, 120, 120], doc=doc_neuron
+        ),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("resnet_dt", bool, optional=True, default=True, doc=doc_resnet_dt),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("fit_diag", bool, optional=True, default=True, doc=doc_fit_diag),
+        Argument("scale", [list, float], optional=True, default=1.0, doc=doc_scale),
+        Argument(
+            "diag_shift", [list, float], optional=True, default=0.0, doc=doc_diag_shift
+        ),
+        Argument("sel_type", [list, int, None], optional=True, doc=doc_sel_type),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
     ]
 
 
 def fitting_global_polar():
     return fitting_polar()
 
 
 def fitting_dipole():
-    doc_neuron = 'The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built.'
-    doc_activation_function = f'The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}'
+    doc_neuron = "The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built."
+    doc_activation_function = f"The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())}"
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_precision = f'The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}'
-    doc_sel_type = 'The atom types for which the atomic dipole will be provided. If not set, all types will be selected.'
-    doc_seed = 'Random seed for parameter initialization of the fitting net'
-    return [
-        Argument("neuron", list, optional = True, default = [120,120,120], doc = doc_neuron),
-        Argument("activation_function", str, optional = True, default = 'tanh', doc = doc_activation_function),
-        Argument("resnet_dt", bool, optional = True, default = True, doc = doc_resnet_dt),
-        Argument("precision", str, optional = True, default = 'float64', doc = doc_precision),
-        Argument("sel_type", [list,int,None], optional = True, doc = doc_sel_type),
-        Argument("seed", [int,None], optional = True, doc = doc_seed)
-    ]    
+    doc_precision = f"The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())}"
+    doc_sel_type = "The atom types for which the atomic dipole will be provided. If not set, all types will be selected."
+    doc_seed = "Random seed for parameter initialization of the fitting net"
+    return [
+        Argument(
+            "neuron", list, optional=True, default=[120, 120, 120], doc=doc_neuron
+        ),
+        Argument(
+            "activation_function",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_activation_function,
+        ),
+        Argument("resnet_dt", bool, optional=True, default=True, doc=doc_resnet_dt),
+        Argument("precision", str, optional=True, default="float64", doc=doc_precision),
+        Argument("sel_type", [list, int, None], optional=True, doc=doc_sel_type),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+    ]
 
 
 def fitting_variant_type_args():
-    doc_descrpt_type = 'The type of the fitting. See explanation below. \n\n\
+    doc_descrpt_type = "The type of the fitting. See explanation below. \n\n\
 - `ener`: Fit an energy model (potential energy surface).\n\n\
 - `dipole`: Fit an atomic dipole model. Atomic dipole labels for all the selected atoms (see `sel_type`) should be provided by `dipole.npy` in each data system. The file has number of frames lines and 3 times of number of selected atoms columns.\n\n\
 - `polar`: Fit an atomic polarizability model. Atomic polarizability labels for all the selected atoms (see `sel_type`) should be provided by `polarizability.npy` in each data system. The file has number of frames lines and 9 times of number of selected atoms columns.\n\n\
-- `global_polar`: Fit a polarizability model. Polarizability labels should be provided by `polarizability.npy` in each data system. The file has number of frames lines and 9 columns.'
-    
-    return Variant("type", [Argument("ener", dict, fitting_ener()),
-                            Argument("dipole", dict, fitting_dipole()),
-                            Argument("polar", dict, fitting_polar()),
-                            Argument("global_polar", dict, fitting_global_polar())], 
-                   optional = True,
-                   default_tag = 'ener',
-                   doc = doc_descrpt_type)
+- `global_polar`: Fit a polarizability model. Polarizability labels should be provided by `polarizability.npy` in each data system. The file has number of frames lines and 9 columns."
+
+    return Variant(
+        "type",
+        [
+            Argument("ener", dict, fitting_ener()),
+            Argument("dipole", dict, fitting_dipole()),
+            Argument("polar", dict, fitting_polar()),
+            Argument("global_polar", dict, fitting_global_polar()),
+        ],
+        optional=True,
+        default_tag="ener",
+        doc=doc_descrpt_type,
+    )
+
 
 def modifier_dipole_charge():
     doc_model_name = "The name of the frozen dipole model file."
     doc_model_charge_map = f"The charge of the WFCC. The list length should be the same as the {make_link('sel_type', 'model/fitting_net[dipole]/sel_type')}. "
     doc_sys_charge_map = f"The charge of real atoms. The list length should be the same as the {make_link('type_map', 'model/type_map')}"
     doc_ewald_h = f"The grid spacing of the FFT grid. Unit is A"
     doc_ewald_beta = f"The splitting parameter of Ewald sum. Unit is A^{-1}"
-    
+
     return [
-        Argument("model_name", str, optional = False, doc = doc_model_name),
-        Argument("model_charge_map", list, optional = False, doc = doc_model_charge_map),
-        Argument("sys_charge_map", list, optional = False, doc = doc_sys_charge_map),
-        Argument("ewald_beta", float, optional = True, default = 0.4, doc = doc_ewald_beta),
-        Argument("ewald_h", float, optional = True, default = 1.0, doc = doc_ewald_h),        
+        Argument("model_name", str, optional=False, doc=doc_model_name),
+        Argument("model_charge_map", list, optional=False, doc=doc_model_charge_map),
+        Argument("sys_charge_map", list, optional=False, doc=doc_sys_charge_map),
+        Argument("ewald_beta", float, optional=True, default=0.4, doc=doc_ewald_beta),
+        Argument("ewald_h", float, optional=True, default=1.0, doc=doc_ewald_h),
     ]
 
+
 def modifier_variant_type_args():
     doc_modifier_type = "The type of modifier. See explanation below.\n\n\
 -`dipole_charge`: Use WFCC to model the electronic structure of the system. Correct the long-range interaction"
-    return Variant("type", 
-                   [
-                       Argument("dipole_charge", dict, modifier_dipole_charge()),
-                   ],
-                   optional = False,
-                   doc = doc_modifier_type)
-
-
-def model_args ():
-    doc_type_map = 'A list of strings. Give the name to each type of atoms.'
-    doc_data_stat_nbatch = 'The model determines the normalization from the statistics of the data. This key specifies the number of `frames` in each `system` used for statistics.'
-    doc_data_stat_protect = 'Protect parameter for atomic energy regression.'
-    doc_descrpt = 'The descriptor of atomic environment.'
-    doc_fitting = 'The fitting of physical properties.'
-    doc_modifier = 'The modifier of model output.'
-    doc_use_srtab = 'The table for the short-range pairwise interaction added on top of DP. The table is a text data file with (N_t + 1) * N_t / 2 + 1 columes. The first colume is the distance between atoms. The second to the last columes are energies for pairs of certain types. For example we have two atom types, 0 and 1. The columes from 2nd to 4th are for 0-0, 0-1 and 1-1 correspondingly.'
-    doc_smin_alpha = 'The short-range tabulated interaction will be swithed according to the distance of the nearest neighbor. This distance is calculated by softmin. This parameter is the decaying parameter in the softmin. It is only required when `use_srtab` is provided.'
-    doc_sw_rmin = 'The lower boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided.'
-    doc_sw_rmax = 'The upper boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided.'
-
-    ca = Argument("model", dict, 
-                  [Argument("type_map", list, optional = True, doc = doc_type_map),
-                   Argument("data_stat_nbatch", int, optional = True, default = 10, doc = doc_data_stat_nbatch),
-                   Argument("data_stat_protect", float, optional = True, default = 1e-2, doc = doc_data_stat_protect),
-                   Argument("use_srtab", str, optional = True, doc = doc_use_srtab),
-                   Argument("smin_alpha", float, optional = True, doc = doc_smin_alpha),
-                   Argument("sw_rmin", float, optional = True, doc = doc_sw_rmin),
-                   Argument("sw_rmax", float, optional = True, doc = doc_sw_rmax),
-                   Argument("descriptor", dict, [], [descrpt_variant_type_args()], doc = doc_descrpt),
-                   Argument("fitting_net", dict, [], [fitting_variant_type_args()], doc = doc_fitting),
-                   Argument("modifier", dict, [], [modifier_variant_type_args()], optional = True, doc = doc_modifier),
-                  ])
+    return Variant(
+        "type",
+        [
+            Argument("dipole_charge", dict, modifier_dipole_charge()),
+        ],
+        optional=False,
+        doc=doc_modifier_type,
+    )
+
+
+def model_args():
+    doc_type_map = "A list of strings. Give the name to each type of atoms."
+    doc_data_stat_nbatch = "The model determines the normalization from the statistics of the data. This key specifies the number of `frames` in each `system` used for statistics."
+    doc_data_stat_protect = "Protect parameter for atomic energy regression."
+    doc_descrpt = "The descriptor of atomic environment."
+    doc_fitting = "The fitting of physical properties."
+    doc_modifier = "The modifier of model output."
+    doc_use_srtab = "The table for the short-range pairwise interaction added on top of DP. The table is a text data file with (N_t + 1) * N_t / 2 + 1 columes. The first colume is the distance between atoms. The second to the last columes are energies for pairs of certain types. For example we have two atom types, 0 and 1. The columes from 2nd to 4th are for 0-0, 0-1 and 1-1 correspondingly."
+    doc_smin_alpha = "The short-range tabulated interaction will be swithed according to the distance of the nearest neighbor. This distance is calculated by softmin. This parameter is the decaying parameter in the softmin. It is only required when `use_srtab` is provided."
+    doc_sw_rmin = "The lower boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided."
+    doc_sw_rmax = "The upper boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided."
+
+    ca = Argument(
+        "model",
+        dict,
+        [
+            Argument("type_map", list, optional=True, doc=doc_type_map),
+            Argument(
+                "data_stat_nbatch",
+                int,
+                optional=True,
+                default=10,
+                doc=doc_data_stat_nbatch,
+            ),
+            Argument(
+                "data_stat_protect",
+                float,
+                optional=True,
+                default=1e-2,
+                doc=doc_data_stat_protect,
+            ),
+            Argument("use_srtab", str, optional=True, doc=doc_use_srtab),
+            Argument("smin_alpha", float, optional=True, doc=doc_smin_alpha),
+            Argument("sw_rmin", float, optional=True, doc=doc_sw_rmin),
+            Argument("sw_rmax", float, optional=True, doc=doc_sw_rmax),
+            Argument(
+                "descriptor", dict, [], [descrpt_variant_type_args()], doc=doc_descrpt
+            ),
+            Argument(
+                "fitting_net", dict, [], [fitting_variant_type_args()], doc=doc_fitting
+            ),
+            Argument(
+                "modifier",
+                dict,
+                [],
+                [modifier_variant_type_args()],
+                optional=True,
+                doc=doc_modifier,
+            ),
+        ],
+    )
     # print(ca.gen_doc())
     return ca
 
 
 def learning_rate_exp():
-    doc_start_lr = 'The learning rate the start of the training.'
-    doc_stop_lr = 'The desired learning rate at the end of the training.'
-    doc_decay_steps = 'The learning rate is decaying every this number of training steps.'
-    
-    args =  [
-        Argument("start_lr", float, optional = True, default = 1e-3, doc = doc_start_lr),
-        Argument("stop_lr", float, optional = True, default = 1e-8, doc = doc_stop_lr),
-        Argument("decay_steps", int, optional = True, default = 5000, doc = doc_decay_steps)
+    doc_start_lr = "The learning rate the start of the training."
+    doc_stop_lr = "The desired learning rate at the end of the training."
+    doc_decay_steps = (
+        "The learning rate is decaying every this number of training steps."
+    )
+
+    args = [
+        Argument("start_lr", float, optional=True, default=1e-3, doc=doc_start_lr),
+        Argument("stop_lr", float, optional=True, default=1e-8, doc=doc_stop_lr),
+        Argument("decay_steps", int, optional=True, default=5000, doc=doc_decay_steps),
     ]
     return args
-    
+
 
 def learning_rate_variant_type_args():
-    doc_lr = 'The type of the learning rate.'
+    doc_lr = "The type of the learning rate."
 
-    return Variant("type", 
-                   [Argument("exp", dict, learning_rate_exp())],
-                   optional = True,
-                   default_tag = 'exp',
-                   doc = doc_lr)
+    return Variant(
+        "type",
+        [Argument("exp", dict, learning_rate_exp())],
+        optional=True,
+        default_tag="exp",
+        doc=doc_lr,
+    )
 
 
 def learning_rate_args():
-    doc_lr = "The definitio of learning rate" 
-    return Argument("learning_rate", dict, [], 
-                    [learning_rate_variant_type_args()],
-                    doc = doc_lr)
+    doc_lr = "The definitio of learning rate"
+    return Argument(
+        "learning_rate", dict, [], [learning_rate_variant_type_args()], doc=doc_lr
+    )
 
 
 def start_pref(item):
-    return f'The prefactor of {item} loss at the start of the training. Should be larger than or equal to 0. If set to none-zero value, the {item} label should be provided by file {item}.npy in each data system. If both start_pref_{item} and limit_pref_{item} are set to 0, then the {item} will be ignored.'
+    return f"The prefactor of {item} loss at the start of the training. Should be larger than or equal to 0. If set to none-zero value, the {item} label should be provided by file {item}.npy in each data system. If both start_pref_{item} and limit_pref_{item} are set to 0, then the {item} will be ignored."
+
 
 def limit_pref(item):
-    return f'The prefactor of {item} loss at the limit of the training, Should be larger than or equal to 0. i.e. the training step goes to infinity.'
+    return f"The prefactor of {item} loss at the limit of the training, Should be larger than or equal to 0. i.e. the training step goes to infinity."
+
 
 def loss_ener():
-    doc_start_pref_e = start_pref('energy')
-    doc_limit_pref_e = limit_pref('energy')
-    doc_start_pref_f = start_pref('force')
-    doc_limit_pref_f = limit_pref('force')
-    doc_start_pref_v = start_pref('virial')
-    doc_limit_pref_v = limit_pref('virial')
-    doc_start_pref_ae = start_pref('atom_ener')
-    doc_start_pref_ae = limit_pref('atom_ener')
-    doc_relative_f = 'If provided, relative force error will be used in the loss. The difference of force will be normalized by the magnitude of the force in the label with a shift given by `relative_f`, i.e. DF_i / ( || F || + relative_f ) with DF denoting the difference between prediction and label and || F || denoting the L2 norm of the label.'
-    return [
-        Argument("start_pref_e", [float,int], optional = True, default = 0.02, doc = doc_start_pref_e),
-        Argument("limit_pref_e", [float,int], optional = True, default = 1.00, doc = doc_limit_pref_e),
-        Argument("start_pref_f", [float,int], optional = True, default = 1000, doc = doc_start_pref_f),
-        Argument("limit_pref_f", [float,int], optional = True, default = 1.00, doc = doc_limit_pref_f),
-        Argument("start_pref_v", [float,int], optional = True, default = 0.00, doc = doc_start_pref_v),
-        Argument("limit_pref_v", [float,int], optional = True, default = 0.00, doc = doc_limit_pref_v),
-        Argument("start_pref_ae", [float,int], optional = True, default = 0.00, doc = doc_start_pref_v),
-        Argument("limit_pref_ae", [float,int], optional = True, default = 0.00, doc = doc_limit_pref_v),
-        Argument("relative_f", [float,None], optional = True, doc = doc_relative_f)
+    doc_start_pref_e = start_pref("energy")
+    doc_limit_pref_e = limit_pref("energy")
+    doc_start_pref_f = start_pref("force")
+    doc_limit_pref_f = limit_pref("force")
+    doc_start_pref_v = start_pref("virial")
+    doc_limit_pref_v = limit_pref("virial")
+    doc_start_pref_ae = start_pref("atom_ener")
+    doc_start_pref_ae = limit_pref("atom_ener")
+    doc_relative_f = "If provided, relative force error will be used in the loss. The difference of force will be normalized by the magnitude of the force in the label with a shift given by `relative_f`, i.e. DF_i / ( || F || + relative_f ) with DF denoting the difference between prediction and label and || F || denoting the L2 norm of the label."
+    return [
+        Argument(
+            "start_pref_e",
+            [float, int],
+            optional=True,
+            default=0.02,
+            doc=doc_start_pref_e,
+        ),
+        Argument(
+            "limit_pref_e",
+            [float, int],
+            optional=True,
+            default=1.00,
+            doc=doc_limit_pref_e,
+        ),
+        Argument(
+            "start_pref_f",
+            [float, int],
+            optional=True,
+            default=1000,
+            doc=doc_start_pref_f,
+        ),
+        Argument(
+            "limit_pref_f",
+            [float, int],
+            optional=True,
+            default=1.00,
+            doc=doc_limit_pref_f,
+        ),
+        Argument(
+            "start_pref_v",
+            [float, int],
+            optional=True,
+            default=0.00,
+            doc=doc_start_pref_v,
+        ),
+        Argument(
+            "limit_pref_v",
+            [float, int],
+            optional=True,
+            default=0.00,
+            doc=doc_limit_pref_v,
+        ),
+        Argument(
+            "start_pref_ae",
+            [float, int],
+            optional=True,
+            default=0.00,
+            doc=doc_start_pref_v,
+        ),
+        Argument(
+            "limit_pref_ae",
+            [float, int],
+            optional=True,
+            default=0.00,
+            doc=doc_limit_pref_v,
+        ),
+        Argument("relative_f", [float, None], optional=True, doc=doc_relative_f),
     ]
 
 
 def loss_variant_type_args():
-    doc_loss = 'The type of the loss. \n\.'
-    
-    return Variant("type", 
-                   [Argument("ener", dict, loss_ener())],
-                   optional = True,
-                   default_tag = 'ener',
-                   doc = doc_loss)
+    doc_loss = "The type of the loss. \n"
+
+    return Variant(
+        "type",
+        [Argument("ener", dict, loss_ener())],
+        optional=True,
+        default_tag="ener",
+        doc=doc_loss,
+    )
+
 
 def loss_args():
-    doc_loss = 'The definition of loss function. The type of the loss depends on the type of the fitting. For fitting type `ener`, the prefactors before energy, force, virial and atomic energy losses may be provided. For fitting type `dipole`, `polar` and `global_polar`, the loss may be an empty `dict` or unset.' 
-    ca = Argument('loss', dict, [], 
-                  [loss_variant_type_args()],
-                  optional = True,
-                  doc = doc_loss)
+    doc_loss = "The definition of loss function. The type of the loss depends on the type of the fitting. For fitting type `ener`, the prefactors before energy, force, virial and atomic energy losses may be provided. For fitting type `dipole`, `polar` and `global_polar`, the loss may be an empty `dict` or unset."
+    ca = Argument(
+        "loss", dict, [], [loss_variant_type_args()], optional=True, doc=doc_loss
+    )
     return ca
 
+
 def training_args():
     link_sys = make_link("systems", "training/systems")
-    doc_systems = 'The data systems. This key can be provided with a listthat specifies the systems, or be provided with a string by which the prefix of all systems are given and the list of the systems is automatically generated.'
-    doc_set_prefix = f'The prefix of the sets in the {link_sys}.'
-    doc_stop_batch = 'Number of training batch. Each training uses one batch of data.'
+    doc_systems = "The data systems. This key can be provided with a listthat specifies the systems, or be provided with a string by which the prefix of all systems are given and the list of the systems is automatically generated."
+    doc_set_prefix = f"The prefix of the sets in the {link_sys}."
+    doc_stop_batch = "Number of training batch. Each training uses one batch of data."
     doc_batch_size = f'This key can be \n\n\
 - list: the length of which is the same as the {link_sys}. The batch size of each system is given by the elements of the list.\n\n\
 - int: all {link_sys} use the same batch size.\n\n\
 - string "auto": automatically determines the batch size so that the batch_size times the number of atoms in the system is no less than 32.\n\n\
 - string "auto:N": automatically determines the batch size so that the batch_size times the number of atoms in the system is no less than N.'
-    doc_seed = 'The random seed for getting frames from the training data set.'
-    doc_disp_file = 'The file for printing learning curve.'
-    doc_disp_freq = 'The frequency of printing learning curve.'
-    doc_numb_test = 'Number of frames used for the test during training.'
-    doc_save_freq = 'The frequency of saving check point.'
-    doc_save_ckpt = 'The file name of saving check point.'
-    doc_disp_training = 'Displaying verbose information during training.'
-    doc_time_training = 'Timing durining training.'
-    doc_profiling = 'Profiling during training.'
-    doc_profiling_file = 'Output file for profiling.'
+    doc_seed = "The random seed for getting frames from the training data set."
+    doc_disp_file = "The file for printing learning curve."
+    doc_disp_freq = "The frequency of printing learning curve."
+    doc_numb_test = "Number of frames used for the test during training."
+    doc_save_freq = "The frequency of saving check point."
+    doc_save_ckpt = "The file name of saving check point."
+    doc_disp_training = "Displaying verbose information during training."
+    doc_time_training = "Timing durining training."
+    doc_profiling = "Profiling during training."
+    doc_profiling_file = "Output file for profiling."
     doc_train_auto_prob_style = 'Determine the probability of systems automatically. The method is assigned by this key and can be\n\n\
 - "prob_uniform"  : the probability all the systems are equal, namely 1.0/self.get_nsystems()\n\n\
 - "prob_sys_size" : the probability of a system is proportional to the number of batches in the system\n\n\
 - "prob_sys_size;stt_idx:end_idx:weight;stt_idx:end_idx:weight;..." : the list of systems is devided into blocks. A block is specified by `stt_idx:end_idx:weight`, where `stt_idx` is the starting index of the system, `end_idx` is then ending (not including) index of the system, the probabilities of the systems in this block sums up to `weight`, and the relatively probabilities within this block is proportional to the number of batches in the system.'
     doc_train_sys_probs = "A list of float, should be of the same length as `train_systems`, specifying the probability of each system."
-    doc_tensorboard = 'Enable tensorboard'
-    doc_tensorboard_log_dir = 'The log directory of tensorboard outputs'
+    doc_tensorboard = "Enable tensorboard"
+    doc_tensorboard_log_dir = "The log directory of tensorboard outputs"
 
     args = [
-        Argument("systems", [list,str], optional = False, doc = doc_systems, alias = ["trn_systems"]),
-        Argument("set_prefix", str, optional = True, default = 'set', doc = doc_set_prefix),
-        Argument("auto_prob", str, optional = True, default = "prob_sys_size", doc = doc_train_auto_prob_style, alias = ["trn_auto_prob", "auto_prob_style"]),
-        Argument("sys_probs", list, optional = True, default = None, doc = doc_train_sys_probs, alias = ["trn_sys_probs"]),
-        Argument("batch_size", [list,int,str], optional = True, default = 'auto', doc = doc_batch_size, alias = ["trn_batch_size"]),
-        Argument("numb_steps", int, optional = False, doc = doc_stop_batch, alias = ["stop_batch"]),
-        Argument("seed", [int,None], optional = True, doc = doc_seed),
-        Argument("disp_file", str, optional = True, default = 'lcueve.out', doc = doc_disp_file),
-        Argument("disp_freq", int, optional = True, default = 1000, doc = doc_disp_freq),
-        Argument("numb_test", [list,int,str], optional = True, default = 1, doc = doc_numb_test),
-        Argument("save_freq", int, optional = True, default = 1000, doc = doc_save_freq),
-        Argument("save_ckpt", str, optional = True, default = 'model.ckpt', doc = doc_save_ckpt),
-        Argument("disp_training", bool, optional = True, default = True, doc = doc_disp_training),
-        Argument("time_training", bool, optional = True, default = True, doc = doc_time_training),
-        Argument("profiling", bool, optional = True, default = False, doc = doc_profiling),
-        Argument("profiling_file", str, optional = True, default = 'timeline.json', doc = doc_profiling_file),
-        Argument("tensorboard", bool, optional = True, default = False, doc = doc_tensorboard),
-        Argument("tensorboard_log_dir", str, optional = True, default = 'log', doc = doc_tensorboard_log_dir),
+        Argument(
+            "systems",
+            [list, str],
+            optional=False,
+            doc=doc_systems,
+            alias=["trn_systems"],
+        ),
+        Argument("set_prefix", str, optional=True, default="set", doc=doc_set_prefix),
+        Argument(
+            "auto_prob",
+            str,
+            optional=True,
+            default="prob_sys_size",
+            doc=doc_train_auto_prob_style,
+            alias=["trn_auto_prob", "auto_prob_style"],
+        ),
+        Argument(
+            "sys_probs",
+            list,
+            optional=True,
+            default=None,
+            doc=doc_train_sys_probs,
+            alias=["trn_sys_probs"],
+        ),
+        Argument(
+            "batch_size",
+            [list, int, str],
+            optional=True,
+            default="auto",
+            doc=doc_batch_size,
+            alias=["trn_batch_size"],
+        ),
+        Argument(
+            "numb_steps", int, optional=False, doc=doc_stop_batch, alias=["stop_batch"]
+        ),
+        Argument("seed", [int, None], optional=True, doc=doc_seed),
+        Argument(
+            "disp_file", str, optional=True, default="lcueve.out", doc=doc_disp_file
+        ),
+        Argument("disp_freq", int, optional=True, default=1000, doc=doc_disp_freq),
+        Argument(
+            "numb_test", [list, int, str], optional=True, default=1, doc=doc_numb_test
+        ),
+        Argument("save_freq", int, optional=True, default=1000, doc=doc_save_freq),
+        Argument(
+            "save_ckpt", str, optional=True, default="model.ckpt", doc=doc_save_ckpt
+        ),
+        Argument(
+            "disp_training", bool, optional=True, default=True, doc=doc_disp_training
+        ),
+        Argument(
+            "time_training", bool, optional=True, default=True, doc=doc_time_training
+        ),
+        Argument("profiling", bool, optional=True, default=False, doc=doc_profiling),
+        Argument(
+            "profiling_file",
+            str,
+            optional=True,
+            default="timeline.json",
+            doc=doc_profiling_file,
+        ),
+        Argument(
+            "tensorboard", bool, optional=True, default=False, doc=doc_tensorboard
+        ),
+        Argument(
+            "tensorboard_log_dir",
+            str,
+            optional=True,
+            default="log",
+            doc=doc_tensorboard_log_dir,
+        ),
     ]
 
-    doc_training = 'The training options'
-    return Argument("training", dict, args, [], doc = doc_training)
+    doc_training = "The training options"
+    return Argument("training", dict, args, [], doc=doc_training)
 
 
 def make_index(keys):
     ret = []
     for ii in keys:
         ret.append(make_link(ii, ii))
-    return ', '.join(ret)
+    return ", ".join(ret)
 
 
 def gen_doc(*, make_anchor=True, make_link=True, **kwargs):
     if make_link:
         make_anchor = True
     ma = model_args()
     lra = learning_rate_args()
@@ -494,18 +727,18 @@
     ptr = []
     ptr.append(ma.gen_doc(make_anchor=make_anchor, make_link=make_link, **kwargs))
     ptr.append(la.gen_doc(make_anchor=make_anchor, make_link=make_link, **kwargs))
     ptr.append(lra.gen_doc(make_anchor=make_anchor, make_link=make_link, **kwargs))
     ptr.append(ta.gen_doc(make_anchor=make_anchor, make_link=make_link, **kwargs))
 
     key_words = []
-    for ii in "\n\n".join(ptr).split('\n'):
-        if 'argument path' in ii:
-            key_words.append(ii.split(':')[1].replace('`','').strip())
-    #ptr.insert(0, make_index(key_words))
+    for ii in "\n\n".join(ptr).split("\n"):
+        if "argument path" in ii:
+            key_words.append(ii.split(":")[1].replace("`", "").strip())
+    # ptr.insert(0, make_index(key_words))
 
     return "\n\n".join(ptr)
 
 
 def check(data):
     ma = model_args()
     lra = learning_rate_args()
@@ -519,25 +752,26 @@
 def normalize(data):
     ma = model_args()
     lra = learning_rate_args()
     la = loss_args()
     ta = training_args()
 
     base = Argument("base", dict, [ma, lra, la, ta])
-    data = base.normalize_value(data, trim_pattern = "_*")
+    data = base.normalize_value(data, trim_pattern="_*")
     base.check_value(data, strict=True)
 
-    return data        
+    return data
+
 
-example_json_str = '''
+example_json_str = """
 {
     "_comment": " model parameters",
     "model": {
         "type_map":	["O", "H"],
-        "descriptor" : { 
+        "descriptor" : {
             "type": "hybrid",
             "list": [{
                 "type":		"se_a",
                 "sel":		[46, 92],
                 "rcut_smth":	5.80,
                 "rcut":		6.00,
                 "neuron":		[25, 50, 100],
@@ -551,28 +785,28 @@
                 "rcut_smth":	5.80,
                 "rcut":		6.00,
                 "neuron":		[25, 50, 100],
                 "resnet_dt":	false,
                 "seed":		1,
                 "_comment":		" that's all"
             }]
-        }, 
+        },
         "fitting_net" : {
             "neuron":		[240, 240, 240],
             "resnet_dt":	true,
             "seed":		1,
             "_comment":		" that's all"
         },
         "_comment":	" that's all"
     },
 
     "learning_rate" :{
         "type":		"exp",
         "decay_steps":	5000,
-        "start_lr":	0.001,	
+        "start_lr":	0.001,
         "stop_lr":	3.51e-8,
         "_comment":	"that's all"
         },
 
         "loss" :{
         "start_pref_e":	0.02,
         "limit_pref_e":	1,
@@ -582,15 +816,15 @@
         "limit_pref_v":	0,
         "_comment":	" that's all"
     },
 
     "_comment": " traing controls",
     "training" : {
         "systems":	["../data/"],
-        "set_prefix":	"set",    
+        "set_prefix":	"set",
         "stop_batch":	1000000,
         "batch_size":	1,
 
         "seed":		1,
 
         "_comment": " display and restart",
         "_comment": " frequencies counted in batch",
@@ -606,13 +840,14 @@
         "profiling":	false,
         "profiling_file":"timeline.json",
         "_comment":	"that's all"
     },
 
     "_comment":		"that's all"
 }
-'''
+"""
 
 if __name__ == "__main__":
     import json
+
     data = json.loads(example_json_str)
     normalize(data)
```

### Comparing `dargs-0.3.4/tests/test_checker.py` & `dargs-0.3.5/tests/test_creation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,268 +1,286 @@
 from .context import dargs
 import unittest
 from dargs import Argument, Variant
-from dargs.dargs import ArgumentKeyError, ArgumentTypeError, ArgumentValueError
 
-class TestChecker(unittest.TestCase):
 
-    def test_name_type(self):
-        # naive
+class TestCreation(unittest.TestCase):
+    def test_dtype(self):
+        ref = Argument("key1", [bool, str, dict])
         ca = Argument("key1", int)
-        ca.check({"key1": 10})
-        # accept multiple types
-        ca = Argument("key1", [int, list, str])
-        ca.check({"key1": 10})
-        ca.check({"key1": [10, 20]})
-        ca.check({"key1": "hello"})
-        # possible error
-        with self.assertRaises(ArgumentKeyError):
-            ca.check({"key2": 1})
-        with self.assertRaises(ArgumentKeyError):
-            ca.check({"key1": 1, "key2": 1}, strict=True)
-        with self.assertRaises(ArgumentTypeError):
-            ca.check({"key1": 1.0})
-        # special handle of None
-        ca = Argument("key1", [int, None])
-        ca.check({"key1": None})
-        # optional case
-        ca = Argument("key1", int, optional=True)
-        ca.check({})
-        # extra checker
-        ca = Argument("key1", int, extra_check=lambda v: v > 0)
-        ca.check({"key1": 1})
-        with self.assertRaises(ArgumentValueError):
-            ca.check({"key1": 0})
-        # check any keywords
-        ca = Argument("kwargs", dict)
-        anydict = {"this": 1, "that": 2, "any": 3}
-        ca.check({"kwargs": anydict}, strict=True)
-        ca.check_value(anydict)
+        ca.set_dtype([bool, str, dict])
+        self.assertTrue(ca == ref)
 
     def test_sub_fields(self):
-        ca = Argument("base", dict, [
-            Argument("sub1", int),
-            Argument("sub2", [str, dict], [
-                Argument("subsub1", int),
-                Argument("subsub2", dict, [
-                    Argument("subsubsub1", int)
-                ])
-            ])
-        ])
-        # short one
-        test_dict1 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "hello"}}
-        self.assertSetEqual(set(ca.flatten_sub(test_dict1["base"]).keys()),
-                            set(test_dict1["base"].keys()))
-        ca.check(test_dict1)
-        ca.check_value(test_dict1["base"])
-        # long one
-        test_dict2 = {
-            "base": {
-                "sub1": 1,
-                "sub2": {
-                    "subsub1": 11,
-                    "subsub2": {
-                        "subsubsub1": 111}}}}
-        ca.check(test_dict2)
-        ca.check_value(test_dict2["base"])
-        # expect error
-        err_dict1 = {
-            "base": {
-                "sub1": 1,
-                "sub2": {
-                    "subsub1": 11,
-                    "subsub2": {
-                        "subsubsub2": 111}}}} # different name here
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1)
-        err_dict1["base"]["sub2"]["subsub2"]["subsubsub1"] = 111
-        ca.check(err_dict1) # now should pass
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1, strict=True) # but should fail when strict
-        err_dict1["base"]["sub2"] = None
-        with self.assertRaises(ArgumentTypeError):
-            ca.check(err_dict1)
-        # make sure no dup keys is allowed
-        with self.assertRaises(ValueError):
-            Argument("base", dict, [
+        ref = Argument(
+            "base",
+            dict,
+            [
                 Argument("sub1", int),
-                Argument("sub1", int)
-            ])
-        
-    def test_sub_repeat(self):
-        ca = Argument("base", dict, [
-            Argument("sub1", int),
-            Argument("sub2", str)
-        ], repeat=True)
-        test_dict1 = {
-            "base": [
-                {"sub1": 10,
-                 "sub2": "hello"},
-                {"sub1": 11,
-                 "sub2": "world"}
-            ]}
-        ca.check(test_dict1)
-        ca.check_value(test_dict1["base"])
-        err_dict1 = {
-            "base": [
-                {"sub1": 10,
-                 "sub2": "hello"},
-                {"sub1": 11,
-                 "sub3": "world"}
-            ]}
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1)
-        err_dict1["base"][1]["sub2"] = "world too"
-        ca.check(err_dict1) # now should pass
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1, strict=True) # but should fail when strict
-        err_dict2 = {
-            "base": [
-                {"sub1": 10,
-                 "sub2": "hello"},
-                {"sub1": 11,
-                 "sub2": None}
-            ]}
-        with self.assertRaises(ArgumentTypeError):
-            ca.check(err_dict2)
+                Argument(
+                    "sub2",
+                    [str, dict],
+                    [
+                        Argument("subsub1", int),
+                        Argument("subsub2", dict, [Argument("subsubsub1", int)]),
+                    ],
+                ),
+            ],
+        )
+        ca = Argument("base", dict)
+        s1 = ca.add_subfield("sub1", int)
+        s2 = ca.add_subfield("sub2", str)
+        ss1 = s2.add_subfield("subsub1", int)
+        ss2 = s2.add_subfield("subsub2", dict)
+        sss1 = ss2.add_subfield("subsubsub1", int)
+        self.assertTrue(ca == ref)
+        ref.set_repeat(True)
+        ca.set_repeat(True)
+        self.assertTrue(ca == ref)
+
+    def test_idx_fields(self):
+        s1 = Argument("sub1", int)
+        vt1 = Argument(
+            "type1",
+            dict,
+            [
+                Argument("shared", str),
+                Argument("vnt1_1", dict, [Argument("vnt1_1_1", int)]),
+            ],
+        )
+        vt2 = Argument(
+            "type2",
+            dict,
+            [
+                Argument("shared", int),
+            ],
+        )
+        v1 = Variant("vnt_flag", [vt1, vt2])
+        ca = Argument("base", dict, [s1], [v1])
+        self.assertTrue(ca[""] is ca)
+        self.assertTrue(ca["."] is ca)
+        self.assertTrue(ca["sub1"] == ca["./sub1"] == s1)
+        with self.assertRaises(KeyError):
+            ca["sub2"]
+        self.assertTrue(ca["[type1]"] is vt1)
+        self.assertTrue(ca["[type1]///"] is vt1)
+        self.assertTrue(ca["[type1]/vnt1_1/vnt1_1_1"] == Argument("vnt1_1_1", int))
+        self.assertTrue(ca["[type2]//shared"] == Argument("shared", int))
+        with self.assertRaises(KeyError):
+            s1["sub1"]
+        self.assertTrue(s1.I["sub1"] is s1)
+        self.assertTrue(ca.I["base[type1]"] is vt1)
+        self.assertTrue(ca.I["base[type2]//shared"] == Argument("shared", int))
 
     def test_sub_variants(self):
-        ca = Argument("base", dict, [
-            Argument("sub1", int),
-            Argument("sub2", str)
-        ], [
-            Variant("vnt_flag", [
-                Argument("type1", dict, [
-                    Argument("shared", int),
-                    Argument("vnt1_1", int),
-                    Argument("vnt1_2", dict, [
-                        Argument("vnt1_1_1", int)
-                    ])
-                ]),
-                Argument("type2", dict, [
-                    Argument("shared", int),
-                    Argument("vnt2_1", int),
-                ], alias=['type2a']),
-                Argument("type3", dict, [
-                    Argument("vnt3_1", int)
-                ], [ # testing cascade variants here
-                    Variant("vnt3_flag1", [
-                        Argument("v3f1t1", dict, [
-                            Argument('v3f1t1_1', int),
-                            Argument('v3f1t1_2', int)
-                        ]),
-                        Argument("v3f1t2", dict, [
-                            Argument('v3f1t2_1', int)
-                        ])
-                    ]),
-                    Variant("vnt3_flag2", [
-                        Argument("v3f2t1", dict, [
-                            Argument('v3f2t1_1', int),
-                            Argument('v3f2t1_2', int)
-                        ]),
-                        Argument("v3f2t2", dict, [
-                            Argument('v3f2t2_1', int)
-                        ])
-                    ])
-                ])
-            ])
-        ])
-        test_dict1 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "a",
-                "vnt_flag" : "type1",
-                "shared": 10,
-                "vnt1_1": 11,
-                "vnt1_2": {
-                    "vnt1_1_1": 111}}}
-        self.assertSetEqual(set(ca.flatten_sub(test_dict1["base"]).keys()),
-                            set(test_dict1["base"].keys()))
-        ca.check(test_dict1)
-        test_dict2 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "a",
-                "vnt_flag" : "type2",
-                "shared": 20,
-                "vnt2_1": 21}}
-        self.assertSetEqual(set(ca.flatten_sub(test_dict2["base"]).keys()),
-                            set(test_dict2["base"].keys()))
-        ca.check(test_dict2, strict=True)
-        test_dict2["base"]["vnt_flag"] = "type2a"
-        ca.check(test_dict2, strict=True)
-        err_dict1 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "a",
-                "vnt_flag" : "type2", # here is wrong
-                "shared": 10,
-                "vnt1_1": 11,
-                "vnt1_2": {
-                    "vnt1_1_1": 111}}}
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1)
-        err_dict1["base"]["vnt_flag"] = "type1"
-        ca.check(err_dict1, strict=True) # no additional should pass
-        err_dict1["base"]["additional"] = "hahaha"
-        ca.check(err_dict1) # without strict should pass
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(err_dict1, strict=True) # but should fail when strict
-        err_dict2 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "a",
-                "vnt_flag" : "badtype", # here is wrong
-                "shared": 20,
-                "vnt2_1": 21}}
-        with self.assertRaises(ArgumentValueError):
-            ca.check(err_dict2)
-        # test optional choice
-        test_dict1["base"].pop("vnt_flag")
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(test_dict1)
-        ca.sub_variants["vnt_flag"].optional = True
-        ca.sub_variants["vnt_flag"].default_tag = "type1"
-        ca.check(test_dict1)
-        # test cascade variants
-        test_dict3 = {
-            "base": {
-                "sub1": 1,
-                "sub2": "a",
-                "vnt_flag" : "type3",
-                "vnt3_1": 31,
-                "vnt3_flag1": "v3f1t1",
-                "vnt3_flag2": "v3f2t2",
-                "v3f1t1_1": 3111,
-                "v3f1t1_2": 3112,
-                "v3f2t2_1": 3221}}
-        self.assertSetEqual(set(ca.flatten_sub(test_dict3["base"]).keys()),
-                            set(test_dict3["base"].keys()))
-        ca.check(test_dict3, strict=True)
-        test_dict3["base"].pop("vnt3_flag2")
-        with self.assertRaises(ArgumentKeyError):
-            ca.check(test_dict3)
-        ca.sub_variants['vnt_flag'].choice_dict["type3"].sub_variants["vnt3_flag2"].optional = True
-        ca.sub_variants['vnt_flag'].choice_dict["type3"].sub_variants["vnt3_flag2"].default_tag = 'v3f2t2'
-        ca.check(test_dict3, strict=True)
-        # make sure duplicate tag is not allowed
-        with self.assertRaises(ValueError):
-            Argument("base", dict, [], [
-                Variant("flag", [
-                    Argument("type1", dict),
-                    Argument("type1", dict)])
-            ])
-        with self.assertRaises(ValueError):
-            Argument("base", dict, [], [
-                Variant("flag", [
-                    Argument("type1", dict)]),
-                Variant("flag", [
-                    Argument("type2", dict)])
-            ])
+        ref = Argument(
+            "base",
+            dict,
+            [Argument("sub1", int), Argument("sub2", str)],
+            [
+                Variant(
+                    "vnt_flag",
+                    [
+                        Argument(
+                            "type1",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt1_1", int),
+                                Argument("vnt1_2", dict, [Argument("vnt1_1_1", int)]),
+                            ],
+                        ),
+                        Argument(
+                            "type2",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt2_1", int),
+                            ],
+                        ),
+                    ],
+                )
+            ],
+        )
+        ca = Argument("base", dict)
+        s1 = ca.add_subfield("sub1", int)
+        s2 = ca.add_subfield("sub2", str)
+        v1 = ca.add_subvariant("vnt_flag")
+        vt1 = v1.add_choice("type1", dict)
+        vt1s0 = vt1.add_subfield("shared", int)
+        vt1s1 = vt1.add_subfield("vnt1_1", int)
+        vt1s2 = vt1.add_subfield("vnt1_2", dict)
+        vt1ss = vt1s2.add_subfield("vnt1_1_1", int)
+        vt2 = v1.add_choice("type2")
+        vt2s0 = vt2.add_subfield("shared", int)
+        vt2s1 = vt2.add_subfield("vnt2_1", int)
+        self.assertTrue(ca == ref)
+        # make sure we can modify the reference
+        ref1 = Argument(
+            "base",
+            dict,
+            [Argument("sub1", int), Argument("sub2", str)],
+            [
+                Variant(
+                    "vnt_flag",
+                    [
+                        Argument(
+                            "type1",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt1_1", int),
+                                Argument("vnt1_2", dict, [Argument("vnt1_1_1", int)]),
+                            ],
+                        ),
+                        Argument(
+                            "type2",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt2_1", int),
+                            ],
+                        ),
+                    ],
+                    optional=True,
+                    default_tag="type1",
+                )
+            ],
+        )
+        v1.set_default("type1")
+        self.assertTrue(ca == ref1)
+        v1.set_default(False)
+        self.assertTrue(ca == ref)
+
+    def test_idx_variants(self):
+        vt1 = Argument(
+            "type1",
+            dict,
+            [
+                Argument("shared", int),
+                Argument("vnt1_1", int),
+                Argument("vnt1_2", dict, [Argument("vnt1_1_1", int)]),
+            ],
+        )
+        vt2 = Argument(
+            "type2",
+            dict,
+            [
+                Argument("shared", int),
+                Argument("vnt2_1", int),
+            ],
+        )
+        vnt = Variant("vnt_flag", [vt1, vt2])
+        self.assertTrue(vnt["type1"] is vt1)
+        self.assertTrue(vnt["type2"] is vt2)
+        with self.assertRaises(KeyError):
+            vnt["type3"]
+
+    def test_complicated(self):
+        ref = Argument(
+            "base",
+            dict,
+            [Argument("sub1", int), Argument("sub2", str)],
+            [
+                Variant(
+                    "vnt_flag",
+                    [
+                        Argument(
+                            "type1",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt1_1", int),
+                                Argument("vnt1_2", dict, [Argument("vnt1_1_1", int)]),
+                            ],
+                        ),
+                        Argument(
+                            "type2",
+                            dict,
+                            [
+                                Argument("shared", int),
+                                Argument("vnt2_1", int),
+                            ],
+                        ),
+                        Argument(
+                            "type3",
+                            dict,
+                            [Argument("vnt3_1", int)],
+                            [  # testing cascade variants here
+                                Variant(
+                                    "vnt3_flag1",
+                                    [
+                                        Argument(
+                                            "v3f1t1",
+                                            dict,
+                                            [
+                                                Argument("v3f1t1_1", int),
+                                                Argument("v3f1t1_2", int),
+                                            ],
+                                        ),
+                                        Argument(
+                                            "v3f1t2", dict, [Argument("v3f1t2_1", int)]
+                                        ),
+                                    ],
+                                ),
+                                Variant(
+                                    "vnt3_flag2",
+                                    [
+                                        Argument(
+                                            "v3f2t1",
+                                            dict,
+                                            [
+                                                Argument("v3f2t1_1", int),
+                                                Argument("v3f2t1_2", int),
+                                            ],
+                                        ),
+                                        Argument(
+                                            "v3f2t2", dict, [Argument("v3f2t2_1", int)]
+                                        ),
+                                    ],
+                                ),
+                            ],
+                        ),
+                    ],
+                )
+            ],
+        )
+        ca = Argument("base", dict)
+        s1 = ca.add_subfield("sub1", int)
+        s2 = ca.add_subfield("sub2", str)
+        v1 = ca.add_subvariant("vnt_flag")
+        vt1 = v1.add_choice("type1", dict)
+        vt1s0 = vt1.add_subfield("shared", int)
+        vt1s1 = vt1.add_subfield("vnt1_1", int)
+        vt1s2 = vt1.add_subfield("vnt1_2", dict)
+        vt1ss = vt1s2.add_subfield("vnt1_1_1", int)
+        vt2 = v1.add_choice("type2")
+        vt2s0 = vt2.add_subfield("shared", int)
+        vt2s1 = vt2.add_subfield("vnt2_1", int)
+        vt3 = v1.add_choice("type3")
+        vt3s1 = vt3.add_subfield("vnt3_1", int)
+        vt3f1 = vt3.add_subvariant("vnt3_flag1")
+        vt3f1t1 = vt3f1.add_choice("v3f1t1")
+        vt3f1t1s1 = vt3f1t1.add_subfield("v3f1t1_1", int)
+        vt3f1t1s2 = vt3f1t1.add_subfield("v3f1t1_2", int)
+        vt3f1t2 = vt3f1.add_choice("v3f1t2")
+        vt3f1t2s1 = vt3f1t2.add_subfield("v3f1t2_1", int)
+        vt3f2 = vt3.add_subvariant("vnt3_flag2")
+        vt3f2t1 = vt3f2.add_choice("v3f2t1")
+        vt3f2t1s1 = vt3f2t1.add_subfield("v3f2t1_1", int)
+        vt3f2t1s2 = vt3f2t1.add_subfield("v3f2t1_2", int)
+        vt3f2t2 = vt3f2.add_choice("v3f2t2")
+        vt3f2t2s1 = vt3f2t2.add_subfield("v3f2t2_1", int)
+        self.assertTrue(ca == ref)
+        self.assertTrue(ca["[type3][vnt3_flag1=v3f1t1]"] is vt3f1t1)
+        self.assertTrue(ca.I["base[type3][vnt3_flag1=v3f1t1]/v3f1t1_2"] is vt3f1t1s2)
+        self.assertTrue(ca.I["base[type3][vnt3_flag1=v3f1t2]/v3f1t2_1"] is vt3f1t2s1)
+        self.assertTrue(ca.I["base[type3][vnt3_flag2=v3f2t1]/v3f2t1_1"] is vt3f2t1s1)
+        self.assertTrue(ca.I["base[type3][vnt3_flag2=v3f2t2]/v3f2t2_1"] is vt3f2t2s1)
+        with self.assertRaises((KeyError, ValueError)):
+            ca.I["base[type3][v3f2t2]"]
+        with self.assertRaises((KeyError, ValueError)):
+            ca.I["base[type3][vnt3_flag3=v3f2t2]/v3f2t2_1"]
 
 
 if __name__ == "__main__":
     unittest.main()
-
```

### Comparing `dargs-0.3.4/tests/test_normalizer.py` & `dargs-0.3.5/tests/test_normalizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from .context import dargs
 import unittest
 from dargs import Argument, Variant
 
 
 class TestNormalizer(unittest.TestCase):
-
     def test_default(self):
         # naive
         ca = Argument("Key1", int, optional=True, default=1)
         beg = {}
         end = ca.normalize(beg)
         ref = {"Key1": 1}
         self.assertDictEqual(end, ref)
         self.assertDictEqual(beg, {})
         self.assertTrue(end is not beg)
         # inplace
         end1 = ca.normalize(beg, inplace=True)
         self.assertDictEqual(end1, ref)
         self.assertTrue(end1 is beg)
-    
+
+    def test_default_dict(self):
+        def make_arguments():
+            arg_foo = Argument("foo", int, optional=True, default=1)
+            arg_bar = Argument("bar", dict, [arg_foo], optional=True, default={})
+            return [arg_bar]
+
+        base = Argument("base", dict, make_arguments())
+        data = base.normalize_value({})
+        self.assertDictEqual(data, {"bar": {}})
+
     def test_alias(self):
         ca = Argument("Key1", int, alias=["Old1", "Old2"])
         beg = {"Old1": 1}
         end = ca.normalize(beg)
         ref = {"Key1": 1}
         self.assertDictEqual(end, ref)
         self.assertDictEqual(beg, {"Old1": 1})
@@ -46,82 +55,142 @@
             ca.normalize(beg, trim_pattern="Key1")
         # inplace
         end1 = ca.normalize(beg, inplace=True, trim_pattern="_*")
         self.assertDictEqual(end1, ref)
         self.assertTrue(end1 is beg)
 
     def test_combined(self):
-        ca = Argument("base", dict, [
-            Argument("sub1", int, optional=True, default=1, alias=["sub1a"]),
-            Argument("sub2", str, optional=True, default="haha", alias=["sub2a"])
-        ])
-        beg1 = {"base":{}}
-        ref1 = {"base":{"sub1":1, "sub2": "haha"}}
+        ca = Argument(
+            "base",
+            dict,
+            [
+                Argument("sub1", int, optional=True, default=1, alias=["sub1a"]),
+                Argument("sub2", str, optional=True, default="haha", alias=["sub2a"]),
+            ],
+        )
+        beg1 = {"base": {}}
+        ref1 = {"base": {"sub1": 1, "sub2": "haha"}}
         self.assertDictEqual(ca.normalize(beg1), ref1)
         self.assertDictEqual(ca.normalize_value(beg1["base"]), ref1["base"])
-        beg2 = {"base":{"sub1a": 2, "sub2a": "hoho", "_comment": None}}
-        ref2 = {"base":{"sub1": 2, "sub2": "hoho"}}
+        beg2 = {"base": {"sub1a": 2, "sub2a": "hoho", "_comment": None}}
+        ref2 = {"base": {"sub1": 2, "sub2": "hoho"}}
         self.assertDictEqual(ca.normalize(beg2, trim_pattern="_*"), ref2)
-        self.assertDictEqual(ca.normalize_value(beg2["base"], trim_pattern="_*"), ref2["base"])
+        self.assertDictEqual(
+            ca.normalize_value(beg2["base"], trim_pattern="_*"), ref2["base"]
+        )
 
     def test_complicated(self):
-        ca = Argument("base", dict, [
-            Argument("sub1", int, optional=True, default=1, alias=["sub1a"]),
-            Argument("sub2", list, [
-                Argument("ss1", int, optional=True, default=21, alias=["ss1a"])
-            ], repeat=True, alias=["sub2a"])
-        ], [
-            Variant("vnt_flag", [
-                Argument("type1", dict, [
-                    Argument("shared", int, optional=True, default=-1, alias=["shareda"]),
-                    Argument("vnt1", int, optional=True, default=111, alias=["vnt1a"]),
-                ]),
-                Argument("type2", dict, [
-                    Argument("shared", int, optional=True, default=-2, alias=["sharedb"]),
-                    Argument("vnt2", int, optional=True, default=222, alias=["vnt2a"]),
-                ], alias = ['type3'])
-            ], optional=True, default_tag="type1")
-        ])
+        ca = Argument(
+            "base",
+            dict,
+            [
+                Argument("sub1", int, optional=True, default=1, alias=["sub1a"]),
+                Argument(
+                    "sub2",
+                    list,
+                    [Argument("ss1", int, optional=True, default=21, alias=["ss1a"])],
+                    repeat=True,
+                    alias=["sub2a"],
+                ),
+            ],
+            [
+                Variant(
+                    "vnt_flag",
+                    [
+                        Argument(
+                            "type1",
+                            dict,
+                            [
+                                Argument(
+                                    "shared",
+                                    int,
+                                    optional=True,
+                                    default=-1,
+                                    alias=["shareda"],
+                                ),
+                                Argument(
+                                    "vnt1",
+                                    int,
+                                    optional=True,
+                                    default=111,
+                                    alias=["vnt1a"],
+                                ),
+                            ],
+                        ),
+                        Argument(
+                            "type2",
+                            dict,
+                            [
+                                Argument(
+                                    "shared",
+                                    int,
+                                    optional=True,
+                                    default=-2,
+                                    alias=["sharedb"],
+                                ),
+                                Argument(
+                                    "vnt2",
+                                    int,
+                                    optional=True,
+                                    default=222,
+                                    alias=["vnt2a"],
+                                ),
+                            ],
+                            alias=["type3"],
+                        ),
+                    ],
+                    optional=True,
+                    default_tag="type1",
+                )
+            ],
+        )
         beg1 = {"base": {"sub2": [{}, {}]}}
         ref1 = {
-            'base': {
-                'sub1': 1,
-                'sub2': [{'ss1': 21}, {'ss1': 21}], 
-                'vnt_flag': "type1",
-                'shared': -1, 
-                'vnt1': 111}
+            "base": {
+                "sub1": 1,
+                "sub2": [{"ss1": 21}, {"ss1": 21}],
+                "vnt_flag": "type1",
+                "shared": -1,
+                "vnt1": 111,
+            }
         }
         self.assertDictEqual(ca.normalize(beg1), ref1)
         self.assertDictEqual(ca.normalize_value(beg1["base"]), ref1["base"])
         beg2 = {
             "base": {
                 "sub1a": 2,
-                "sub2a": [{"ss1a":22}, {"_comment1": None}],
+                "sub2a": [{"ss1a": 22}, {"_comment1": None}],
                 "vnt_flag": "type3",
                 "sharedb": -3,
                 "vnt2a": 223,
-                "_comment2": None}
+                "_comment2": None,
+            }
         }
+        print(ca.normalize(beg2, do_default=False, trim_pattern="_*"))
         ref2 = {
-            'base': {
-                'sub1': 2,
-                'sub2': [{'ss1': 22}, {'ss1': 21}], 
+            "base": {
+                "sub1": 2,
+                "sub2": [{"ss1": 22}, {"ss1": 21}],
                 "vnt_flag": "type2",
-                'shared': -3, 
-                'vnt2': 223}
+                "shared": -3,
+                "vnt2": 223,
+            }
         }
         self.assertDictEqual(ca.normalize(beg2, trim_pattern="_*"), ref2)
-        self.assertDictEqual(ca.normalize_value(beg2["base"], trim_pattern="_*"), ref2["base"])
+        self.assertDictEqual(
+            ca.normalize_value(beg2["base"], trim_pattern="_*"), ref2["base"]
+        )
         with self.assertRaises(ValueError):
             ca.normalize(beg2, trim_pattern="sub*")
         with self.assertRaises(ValueError):
             ca.normalize(beg2, trim_pattern="vnt*")
 
     def test_dpmd(self):
         import json
         from .dpmdargs import normalize, example_json_str
+
         data = json.loads(example_json_str)
         normalize(data)
 
+
 if __name__ == "__main__":
     unittest.main()
-
```

