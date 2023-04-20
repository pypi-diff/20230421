# Comparing `tmp/xtyping-0.6.2.tar.gz` & `tmp/xtyping-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtyping-0.6.2.tar", max compression
+gzip compressed data, was "xtyping-0.6.3.tar", max compression
```

## Comparing `xtyping-0.6.2.tar` & `xtyping-0.6.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2022-07-19 01:47:39.087430 xtyping-0.6.2/LICENSE
--rw-r--r--   0        0        0    26157 2022-11-08 18:10:21.929246 xtyping-0.6.2/README.md
--rw-r--r--   0        0        0     1105 2023-02-17 18:56:01.946776 xtyping-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7522 2023-02-17 18:54:41.402048 xtyping-0.6.2/xtyping/__init__.py
--rw-r--r--   0        0        0      235 2022-07-19 01:47:39.087430 xtyping-0.6.2/xtyping/__main__.py
--rw-r--r--   0        0        0      215 2023-02-17 18:56:14.776905 xtyping-0.6.2/xtyping/_meta.py
--rw-r--r--   0        0        0      521 2022-07-19 01:47:39.087430 xtyping-0.6.2/xtyping/npt.py
--rw-r--r--   0        0        0        0 2022-07-19 01:47:39.087430 xtyping-0.6.2/xtyping/py.typed
--rw-r--r--   0        0        0    12138 2023-02-17 18:55:43.834958 xtyping-0.6.2/xtyping/shed.py
--rw-r--r--   0        0        0    28249 1970-01-01 00:00:00.000000 xtyping-0.6.2/setup.py
--rw-r--r--   0        0        0    27396 1970-01-01 00:00:00.000000 xtyping-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.435638 xtyping-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1444 2023-04-20 23:19:54.332585 xtyping-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    26157 2022-09-19 18:35:16.988296 xtyping-0.6.3/README.md
+-rw-r--r--   0        0        0      292 2023-04-20 23:19:54.396173 xtyping-0.6.3/xtyping/__about__.py
+-rw-r--r--   0        0        0     7526 2023-04-20 20:51:48.608506 xtyping-0.6.3/xtyping/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-20 20:51:48.649242 xtyping-0.6.3/xtyping/__main__.py
+-rw-r--r--   0        0        0      352 2023-04-20 20:38:23.594410 xtyping-0.6.3/xtyping/_meta.py
+-rw-r--r--   0        0        0      521 2022-02-04 21:32:32.223150 xtyping-0.6.3/xtyping/npt.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.851951 xtyping-0.6.3/xtyping/py.typed
+-rw-r--r--   0        0        0    12138 2023-02-24 22:45:12.455620 xtyping-0.6.3/xtyping/shed.py
+-rw-r--r--   0        0        0    27396 1970-01-01 00:00:00.000000 xtyping-0.6.3/PKG-INFO
```

### Comparing `xtyping-0.6.2/LICENSE` & `xtyping-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtyping-0.6.2/README.md` & `xtyping-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `xtyping-0.6.2/xtyping/__init__.py` & `xtyping-0.6.3/xtyping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     get_origin,
     get_type_hints,
     overload,
     runtime,
     runtime_checkable,
 )
 
-from xtyping._meta import __version__
+from xtyping.__about__ import __version__
 from xtyping.shed import (
     _DT,
     _KT,
     _R,
     _RT,
     _T,
     _VT,
```

### Comparing `xtyping-0.6.2/xtyping/npt.py` & `xtyping-0.6.3/xtyping/npt.py`

 * *Files identical despite different names*

### Comparing `xtyping-0.6.2/xtyping/shed.py` & `xtyping-0.6.3/xtyping/shed.py`

 * *Files identical despite different names*

### Comparing `xtyping-0.6.2/PKG-INFO` & `xtyping-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtyping
-Version: 0.6.2
+Version: 0.6.3
 Summary: xtyping = typing + typing_extensions
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/xtyping
 License: MIT
 Keywords: typing,dgpy,typed,types
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xtyping Version: 0.6.2 Summary: xtyping = typing +
+Metadata-Version: 2.1 Name: xtyping Version: 0.6.3 Summary: xtyping = typing +
 typing_extensions Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/
 tree/main/libs/xtyping License: MIT Keywords: typing,dgpy,typed,types Author:
 jesse Author-email: jesse@dgi.com Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

