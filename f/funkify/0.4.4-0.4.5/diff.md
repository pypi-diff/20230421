# Comparing `tmp/funkify-0.4.4.tar.gz` & `tmp/funkify-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funkify-0.4.4.tar", max compression
+gzip compressed data, was "funkify-0.4.5.tar", max compression
```

## Comparing `funkify-0.4.4.tar` & `funkify-0.4.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1878 2022-02-17 21:55:28.115836 funkify-0.4.4/funkify/__init__.py
--rw-r--r--   0        0        0      235 2022-02-04 21:32:32.125998 funkify-0.4.4/funkify/__main__.py
--rw-r--r--   0        0        0      220 2022-02-17 21:56:05.923520 funkify-0.4.4/funkify/_meta.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.798952 funkify-0.4.4/funkify/py.typed
--rw-r--r--   0        0        0     1056 2022-02-10 18:00:47.310332 funkify-0.4.4/LICENSE
--rw-r--r--   0        0        0     1477 2022-02-17 21:56:01.520000 funkify-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      657 2022-02-17 21:58:30.407961 funkify-0.4.4/setup.py
--rw-r--r--   0        0        0      912 2022-02-17 21:58:30.408949 funkify-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      297 2023-04-20 23:19:54.396173 funkify-0.4.5/funkify/__about__.py
+-rw-r--r--   0        0        0     1929 2023-04-20 22:34:10.186904 funkify-0.4.5/funkify/__init__.py
+-rw-r--r--   0        0        0      479 2023-04-20 20:51:48.622821 funkify-0.4.5/funkify/__main__.py
+-rw-r--r--   0        0        0      352 2023-04-20 20:38:23.579136 funkify-0.4.5/funkify/_meta.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.798952 funkify-0.4.5/funkify/py.typed
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.417483 funkify-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1768 2023-04-20 23:19:51.337090 funkify-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1158 2022-09-19 18:35:16.981212 funkify-0.4.5/README.md
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 funkify-0.4.5/PKG-INFO
```

### Comparing `funkify-0.4.4/funkify/__init__.py` & `funkify-0.4.5/funkify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
 """`funkify` ~ make modules callable"""
 import sys
 
 from types import ModuleType
 from typing import Any, Callable, Optional, TypeVar, cast
 
-from funkify._meta import __version__
+from funkify import __about__
+from funkify.__about__ import __version__
 
 T = TypeVar("T")
 
 __all__ = (
+    "__about__",
     "__version__",
     "default_export",
     "funkify",
 )
 
 
 def default_export(
```

### Comparing `funkify-0.4.4/LICENSE` & `funkify-0.4.5/LICENSE`

 * *Files identical despite different names*

