# Comparing `tmp/vutils-yaml-0.1.2.tar.gz` & `tmp/vutils-yaml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-yaml-0.1.2.tar", last modified: Mon Mar  6 11:43:59 2023, max compression
+gzip compressed data, was "vutils-yaml-0.1.3.tar", last modified: Thu Apr 20 22:25:30 2023, max compression
```

## Comparing `vutils-yaml-0.1.2.tar` & `vutils-yaml-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.423262 vutils-yaml-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-06 11:43:59.423262 vutils-yaml-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-06 11:43:59.423262 vutils-yaml-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.419262 vutils-yaml-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.419262 vutils-yaml-0.1.2/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.419262 vutils-yaml-0.1.2/src/vutils/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/load.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/src/vutils/yaml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.419262 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 11:43:59.000000 vutils-yaml-0.1.2/src/vutils_yaml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.419262 vutils-yaml-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:43:59.423262 vutils-yaml-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-03-06 11:43:45.000000 vutils-yaml-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/src/vutils/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/src/vutils/yaml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 22:25:30.000000 vutils-yaml-0.1.3/src/vutils_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.482668 vutils-yaml-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:25:30.486668 vutils-yaml-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tests/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-20 22:25:14.000000 vutils-yaml-0.1.3/tox.ini
```

### Comparing `vutils-yaml-0.1.2/LICENSE` & `vutils-yaml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.2/PKG-INFO` & `vutils-yaml-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-yaml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Working with YAML format
 Home-page: https://github.com/i386x/vutils-yaml
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-yaml/issues
 Project-URL: Source, https://github.com/i386x/vutils-yaml
```

### Comparing `vutils-yaml-0.1.2/README.md` & `vutils-yaml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.2/pyproject.toml` & `vutils-yaml-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.2/setup.cfg` & `vutils-yaml-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 metadata = True
 restructuredtext = False
 strict = True
 
 [sdist]
 formats = zip, gztar
 
+[coverage:report]
+exclude_lines = 
+	^if TYPE_CHECKING:$
+
 [flake8]
 filename = *.py,*.pyi,*.pyw
 select = E,F,W,C,G,Y
 enable-extensions = G,Y
 max-line-length = 79
 max-doc-length = 79
 extend-ignore = E203, E302, W503
```

### Comparing `vutils-yaml-0.1.2/src/vutils/yaml/__init__.pyi` & `vutils-yaml-0.1.3/src/vutils/yaml/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vutils-yaml-0.1.2/src/vutils/yaml/load.py` & `vutils-yaml-0.1.3/src/vutils/yaml/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,13 +72,14 @@
 
 
 def load_yaml(stream: "StreamType") -> YamlDataType:
     """
     Load YAML from the stream.
 
     :param stream: The stream
+    :return: the YAML document object
     """
     loader: AnnotateLoader = AnnotateLoader(stream)
     try:
         return cast(YamlDataType, loader.get_single_data())
     finally:
         cast("Callable[[], None]", loader.dispose)()
```

### Comparing `vutils-yaml-0.1.2/src/vutils/yaml/utils.py` & `vutils-yaml-0.1.3/src/vutils/yaml/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 # File:    ./src/vutils/yaml/utils.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-23 21:40:39 +0200
 # Project: vutils-yaml: Working with YAML format
 #
 # SPDX-License-Identifier: MIT
 #
-"""Miscellaneous utilities."""
+"""
+Miscellaneous utilities.
+
+:const ANNOTATION_SLOT: The name of the slot that holds an annotation
+:const KEYLOC_SLOT: The name of the slot that holds the location of a key
+:const TYPEMAP: The mapping between type and its annotation-friendly wrapper
+"""
 
 import datetime
-from typing import TYPE_CHECKING, Iterator, cast
+from typing import TYPE_CHECKING, cast
 
 import yaml
 from vutils.python.objects import merge_data
 from vutils.validator.value import Location
 
 if TYPE_CHECKING:
     from collections.abc import Callable
+    from typing import Iterator
 
     from vutils.yaml import (
         CtorDecorType,
         CtorFuncType,
         CtorSpecType,
         CtorType,
         MarkType,
@@ -39,16 +46,21 @@
     new_datetime = datetime.datetime.__new__
 
 ANNOTATION_SLOT: str = "__yaml_annotation__"
 KEYLOC_SLOT: str = "__yaml_keyloc__"
 
 
 class Annotation:
-    """Holds YAML values annotation."""
+    """
+    Holds YAML values annotation.
 
+    :ivar location: The value's location
+    """
+
+    location: Location
     __slots__ = ("location",)
 
     def __init__(self, location: "Location | None" = None) -> None:
         """
         Initialize annotation object.
 
         :param location: The YAML value's location
@@ -62,34 +74,36 @@
     """Base class for annotated YAML objects."""
 
     __slots__ = ()
 
 
 class NullType(YamlDataType):
     """
-    A null (`None`) type.
+    A null (:obj:`None`) type.
 
-    Since `None` has a special meaning it cannot be annotated nor it is
+    Since :obj:`None` has a special meaning it cannot be annotated nor it is
     possible to inherit from its type. This workaround is used to store
     annotation alongside with ``null``.
     """
 
     def __bool__(self) -> bool:
         """
-        Convert `NullType` object to the `bool` object.
+        Convert :class:`.NullType` object to the :class:`bool` object.
 
-        :return: always `False`
+        :return: always :obj:`False`
         """
         return False
 
     def __eq__(self, other: object) -> bool:
         """
-        Test the equality of this and the other object.
+        Test the equality of this and the :arg:`other` object.
 
-        :return: `True` if this and the other object are considered equal
+        :param other: The other object
+        :return: :obj:`True` if this and the :arg:`other` object are considered
+            equal
         """
         return other is None or isinstance(other, type(self))
 
     def __hash__(self) -> int:
         """
         Return the object hash.
 
@@ -98,40 +112,44 @@
         return hash(None)
 
 
 class BoolType(YamlDataType):
     """
     Represent a Boolean type.
 
-    Since `bool` is not an acceptable base class this workaround is used to
-    store annotation alongside with Boolean values.
+    Since :class:`bool` is not an acceptable base class this workaround is used
+    to store annotation alongside with Boolean values.
     """
 
+    __value: bool
+
     def __init__(self, value: bool) -> None:
         """
-        Initialize the `bool`-like object.
+        Initialize the :class:`bool`-like object.
 
         :param value: The value
         """
         YamlDataType.__init__(self)
         self.__value = value
 
     def __bool__(self) -> bool:
         """
-        Convert this object to `bool` object.
+        Convert this object to :class:`bool` object.
 
         :return: the kept value
         """
         return self.__value
 
     def __eq__(self, other: object) -> bool:
         """
-        Test the equality of this and the other object.
+        Test the equality of this and the :arg:`other` object.
 
-        :return: `True` if this and the other objects are considered equal
+        :param other: The other object
+        :return: :obj:`True` if this and the :arg:`other` object are considered
+            equal
         """
         if isinstance(other, (bool, BoolType)):
             return bool(self) is bool(other)
         if isinstance(other, (int, float)):
             return int(bool(self)) == other
         return False
 
@@ -142,102 +160,103 @@
         :return: the hash of this object
         """
         return hash(bool(self))
 
 
 class IntType(int, YamlDataType):
     """
-    Wrap the `int` type.
+    Wrap the :class:`int` type.
 
     Needed to store annotation.
     """
 
 
 class FloatType(float, YamlDataType):
     """
-    Wrap the `float` type.
+    Wrap the :class:`float` type.
 
     Needed to store annotation.
     """
 
 
 class StrType(str, YamlDataType):
     """
-    Wrap the `str` type.
+    Wrap the :class:`str` type.
 
     Needed to store annotation.
     """
 
 
 class BytesType(bytes, YamlDataType):
     """
-    Wrap the `bytes` type.
+    Wrap the :class:`bytes` type.
 
     Needed to store annotation.
     """
 
 
 class ListType(PyList, YamlDataType):
     """
-    Wrap the `list` type.
+    Wrap the :class:`list` type.
 
     Needed to store annotation.
     """
 
 
 class SetType(PySet, YamlDataType):
     """
-    Wrap the `set` type.
+    Wrap the :class:`set` type.
 
     Needed to store annotation.
     """
 
 
 class DictType(PyDict, YamlDataType):
     """
-    Wrap the `dict` type.
+    Wrap the :class:`dict` type.
 
     Needed to store annotation.
     """
 
 
 class DateType(datetime.date, YamlDataType):
     """
-    Wrap the `datetime.date` type.
+    Wrap the :class:`datetime.date` type.
 
     Needed to store annotation.
     """
 
     def __new__(cls, *args: object) -> "DateType":
         """
         Create the date object.
 
-        :param args: Either `datetime.date` object or `datetime.date` arguments
+        :param args: Either :class:`datetime.date` object or
+            :class:`datetime.date`'s positional arguments
         :return: the date object
         """
         if isinstance(args[0], datetime.date):
             date: datetime.date = args[0]
             return datetime.date.__new__(cls, date.year, date.month, date.day)
         return new_date(cls, *args)
 
 
 class DateTimeType(datetime.datetime, YamlDataType):
     """
-    Wrap the `datetime.datetime` type.
+    Wrap the :class:`datetime.datetime` type.
 
     Needed to store annotation.
     """
 
     def __new__(cls, *args: object, **kwargs: object) -> "DateTimeType":
         """
         Create the datetime object.
 
-        :param args: Either `datetime.datetime` object or `datetime.datetime`
-            arguments
-        :param kwargs: Key-word arguments to `datetime.datetime`
+        :param args: Either :class:`datetime.datetime` object or
+            :class:`datetime.datetime`'s positional arguments
+        :param kwargs: Key-value arguments to :class:`datetime.datetime`
         :return: the datetime object
         """
         if isinstance(args[0], datetime.datetime):
             stamp: datetime.datetime = args[0]
             return datetime.datetime.__new__(
                 cls,
                 stamp.year,
@@ -349,16 +368,16 @@
         inst: "CtorType", node: "NodeType", *args: object, **kwargs: object
     ) -> object:
         """
         Construct an annotated YAML object.
 
         :param inst: The YAML constructor class instance
         :param node: The node
-        :param args: Additional arguments
-        :param kwargs: Additional keyword arguments
+        :param args: Additional positional arguments
+        :param kwargs: Additional key-value arguments
         :return: the annotated YAML object
         """
         base_ctor: "CtorFuncType" = cast(
             "CtorFuncType", getattr(base_cls, name)
         )
         data: object = base_ctor(inst, node, *args, **kwargs)
         return annotate(data, node)
@@ -373,31 +392,31 @@
     :param name: The constructor name
     :param base_cls: The base of the constructor class
     :return: the constructor generator
     """
 
     def gctor(
         inst: "CtorType", node: "NodeType", *args: object, **kwargs: object
-    ) -> Iterator[object]:
+    ) -> "Iterator[object]":
         """
         Generate an annotated YAML object.
 
         :param inst: The YAML constructor class instance
         :param node: The node
-        :param args: Additional arguments
-        :param kwargs: Additional keyword arguments
+        :param args: Additional positional arguments
+        :param kwargs: Additional key-value arguments
         :return: the annotated YAML object
         """
         data: object = annotate(newc(name, args), node)
         yield data
         base_ctor: "CtorFuncType" = cast(
             "CtorFuncType", getattr(base_cls, name)
         )
-        generator: Iterator[object] = cast(
-            Iterator[object], base_ctor(inst, node, *args, **kwargs)
+        generator: "Iterator[object]" = cast(
+            "Iterator[object]", base_ctor(inst, node, *args, **kwargs)
         )
         gdata: object = {}
         for item in generator:
             gdata = item
         merge_data(data, gdata)
 
     return gctor
@@ -406,16 +425,16 @@
 def annotate_constructed_objects(*spec: "CtorSpecType") -> "CtorDecorType":
     """
     Annotate constructed YAML objects with their location.
 
     :param spec: Each argument is a triple holding constructor name, tag, and
         a Boolean value, respectively, saying whether the constructor is a
         generator or not. Constructor name specifies the constructor involved
-        in annotating YAML object during its construction, tag is a tag
-        associated with the constructor or `None`
+        in annotating a YAML object during its construction, tag is a tag
+        associated with the constructor or :obj:`None`
     :return: the decorator function that patches the class
     """
 
     def patch_constructors(cls: "type[CtorType]") -> "type[CtorType]":
         """
         Patch YAML object constructors.
 
@@ -454,15 +473,15 @@
     ).location
 
 
 def keyloc(obj: DictType, kobj: object) -> Location:
     """
     Get the location of the key object.
 
-    :param obj: The annotated `dict` object
+    :param obj: The annotated :class:`dict` object
     :param kobj: The key
     :return: the location of the key
     """
     if not hasattr(obj, KEYLOC_SLOT):
         key2loc: "dict[YamlDataType, Location]" = {}
         for key in obj:
             key2loc[cast(YamlDataType, key)] = getloc(cast(YamlDataType, key))
@@ -473,20 +492,20 @@
 
 
 def is_null(obj: YamlDataType) -> bool:
     """
     Test whether the object is null.
 
     :param obj: The annotated object
-    :return: `True` if *obj* is null
+    :return: :obj:`True` if :arg:`obj` is null
     """
     return isinstance(obj, NullType)
 
 
 def is_bool(obj: YamlDataType) -> bool:
     """
     Test whether the object has Boolean type.
 
     :param obj: The annotated object
-    :return: `True` if *obj* has Boolean type
+    :return: :obj:`True` if :arg:`obj` has Boolean type
     """
     return isinstance(obj, BoolType)
```

### Comparing `vutils-yaml-0.1.2/src/vutils_yaml.egg-info/PKG-INFO` & `vutils-yaml-0.1.3/src/vutils_yaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-yaml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Working with YAML format
 Home-page: https://github.com/i386x/vutils-yaml
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-yaml/issues
 Project-URL: Source, https://github.com/i386x/vutils-yaml
```

### Comparing `vutils-yaml-0.1.2/tests/unit/test_load.py` & `vutils-yaml-0.1.3/tests/unit/test_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 # File:    ./tests/unit/test_load.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-07-07 15:36:46 +0200
 # Project: vutils-yaml: Working with YAML format
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.yaml.load` module."""
+"""
+Test :mod:`vutils.yaml.load` module.
+
+:const YAML_STREAM: The auxiliary YAML data stream
+:const YAML_STREAM_NAME: The name of the auxiliary YAML data stream
+
+.. |load_yaml| replace:: :func:`~vutils.yaml.load.load_yaml`
+"""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.yaml.load import load_yaml
 from vutils.yaml.utils import (
     BoolType,
     BytesType,
@@ -51,15 +58,15 @@
     - b: 2
     - c: 3
 """
 YAML_STREAM_NAME = "<unicode string>"
 
 
 class LoadYamlTestCase(TestCase):
-    """Test case for `load_yaml`."""
+    """Test case for |load_yaml|."""
 
     __slots__ = ()
 
     def check_location(self, obj, name, line, column):
         """
         Check whether the object location matches the expectation.
 
@@ -74,15 +81,15 @@
         self.assertEqual(loc.column, column)
 
     def do_test_data_are_annotated(self, obj, klass, line, column=3):
         """
         Check the data annotation.
 
         :param obj: The data object
-        :param klass: The data type class
+        :param klass: The expected type of the data object
         :param line: The expected line of the data location
         :param column: The expected column of the data location
         """
         self.assertIsInstance(obj, klass)
         self.check_location(obj, YAML_STREAM_NAME, line, column)
 
     def test_loaded_data_are_annotated(self):
```

### Comparing `vutils-yaml-0.1.2/tests/unit/test_utils.py` & `vutils-yaml-0.1.3/tests/unit/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,46 @@
 # File:    ./tests/unit/test_utils.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-07-07 15:36:27 +0200
 # Project: vutils-yaml: Working with YAML format
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.yaml.utils` module."""
+"""
+Test :mod:`vutils.yaml.utils` module.
+
+.. |Annotation| replace:: :class:`~vutils.yaml.utils.Annotation`
+.. |NullType| replace:: :class:`~vutils.yaml.utils.NullType`
+.. |NullType.__hash__| replace:: :meth:`NullType.__hash__
+       <vutils.yaml.utils.NullType.__hash__>`
+.. |NullType.__eq__| replace:: :meth:`NullType.__eq__
+       <vutils.yaml.utils.NullType.__eq__>`
+.. |BoolType| replace:: :class:`~vutils.yaml.utils.BoolType`
+.. |BoolType.__hash__| replace:: :meth:`BoolType.__hash__
+       <vutils.yaml.utils.BoolType.__hash__>`
+.. |BoolType.__eq__| replace:: :meth:`BoolType.__eq__
+       <vutils.yaml.utils.BoolType.__eq__>`
+.. |YamlDataType| replace:: :class:`~vutils.yaml.utils.YamlDataType`
+.. |IntType| replace:: :class:`~vutils.yaml.utils.IntType`
+.. |FloatType| replace:: :class:`~vutils.yaml.utils.FloatType`
+.. |StrType| replace:: :class:`~vutils.yaml.utils.StrType`
+.. |BytesType| replace:: :class:`~vutils.yaml.utils.BytesType`
+.. |ListType| replace:: :class:`~vutils.yaml.utils.ListType`
+.. |SetType| replace:: :class:`~vutils.yaml.utils.SetType`
+.. |DictType| replace:: :class:`~vutils.yaml.utils.DictType`
+.. |DateType| replace:: :class:`~vutils.yaml.utils.DateType`
+.. |DateTimeType| replace:: :class:`~vutils.yaml.utils.DateTimeType`
+.. |obj2xobj| replace:: :func:`~vutils.yaml.utils.obj2xobj`
+.. |newc| replace:: :func:`~vutils.yaml.utils.newc`
+.. |annotate| replace:: :func:`~vutils.yaml.utils.annotate`
+.. |getloc| replace:: :func:`~vutils.yaml.utils.getloc`
+.. |keyloc| replace:: :func:`~vutils.yaml.utils.keyloc`
+.. |is_null| replace:: :func:`~vutils.yaml.utils.is_null`
+.. |is_bool| replace:: :func:`~vutils.yaml.utils.is_bool`
+"""
 
 import datetime
 
 import yaml
 from vutils.testing.mock import make_mock
 from vutils.testing.testcase import TestCase
 from vutils.testing.utils import make_type
@@ -35,60 +66,60 @@
     is_bool,
     is_null,
     keyloc,
     newc,
     obj2xobj,
 )
 
-from .common import SLOT, VALUE
+from .utils import SLOT, VALUE
 
 
 class AnnotationTestCase(TestCase):
-    """Test case for `Annotation`."""
+    """Test case for |Annotation|."""
 
     __slots__ = ()
 
     def test_annotation_initialization(self):
-        """Test `Annotation` initialization."""
+        """Test |Annotation| initialization."""
         location = Location("./foo.yml", 1, 2)
 
         self.assertEqual(f"{Annotation().location}", "")
         self.assertIs(Annotation(location).location, location)
 
 
 class NullTypeTestCase(TestCase):
-    """Test case for `NullType`."""
+    """Test case for |NullType|."""
 
     __slots__ = ()
 
     def test_null_type_behaves_like_false(self):
-        """Test whether `NullType` object behaves like `False`."""
+        """Test whether |NullType| object behaves like :obj:`False`."""
         self.assertFalse(NullType())
 
     def test_hashing_and_equality(self):
-        """Test `__hash__` and `__eq__`."""
+        """Test |NullType.__hash__| and |NullType.__eq__|."""
         self.assertEqual(hash(NullType()), hash(None))
 
         self.assertEqual(NullType(), None)
         self.assertEqual(NullType(), NullType())
         self.assertNotEqual(NullType(), 0)
 
 
 class BoolTypeTestCase(TestCase):
-    """Test case for `BoolType`."""
+    """Test case for |BoolType|."""
 
     __slots__ = ()
 
     def test_bool_type_can_hold_value(self):
-        """Test whether a `BoolType` object can hold a Boolean value."""
+        """Test whether a |BoolType| object can hold a Boolean value."""
         self.assertTrue(BoolType(True))
         self.assertFalse(BoolType(False))
 
     def test_hashing_and_equality(self):
-        """Test `__hash__` and `__eq__`."""
+        """Test |BoolType.__hash__| and |BoolType.__eq__|."""
         self.assertEqual(hash(BoolType(False)), hash(False))
         self.assertEqual(hash(BoolType(True)), hash(True))
 
         self.assertEqual(BoolType(False), BoolType(False))
         self.assertEqual(BoolType(False), False)
         self.assertEqual(BoolType(True), BoolType(True))
         self.assertEqual(BoolType(True), True)
@@ -111,15 +142,15 @@
         self.assertNotEqual(BoolType(True), 2.0)
 
         self.assertNotEqual(BoolType(False), [])
         self.assertNotEqual(BoolType(True), [])
 
 
 class YamlDataTypeTestCase(TestCase):
-    """Test case for `YamlDataType` and its subclasses."""
+    """Test case for |YamlDataType| and its subclasses."""
 
     __slots__ = ()
 
     def do_arithmetic_check(self, cls, zero, unit):
         """
         Test arithmetic types.
 
@@ -144,15 +175,15 @@
         self.assertEqual(cls(sequence), sequence)
         self.assertEqual(cls(sequence)[0], sequence[0])
         self.assertTrue(cls(sequence))
         self.assertFalse(cls(empty))
 
     def do_extensibility_check(self, obj):
         """
-        Test whether *obj* is extensible.
+        Test whether :arg:`obj` is extensible.
 
         :param obj: The YAML data object
         """
         self.assertFalse(hasattr(obj, SLOT))
         setattr(obj, SLOT, VALUE)
         self.assertTrue(hasattr(obj, SLOT))
         self.assertEqual(getattr(obj, SLOT), VALUE)
@@ -160,24 +191,24 @@
     @staticmethod
     def make_key(klass, key):
         """
         Make the key object.
 
         :param klass: The YAML data type
         :param key: The key
-        :return: the *key* as instance of *klass*
+        :return: the :arg:`key` as the instance of :arg:`klass`
         """
         return NullType() if klass is NullType else klass(key)
 
     def do_hashability_check(self, cls, key):
         """
-        Test whether *cls* objects are hashable.
+        Test whether :arg:`cls` objects are hashable.
 
         :param cls: The YAML data type
-        :param key1: The key
+        :param key: The key
         """
         key1 = self.make_key(cls, key)
         key2 = self.make_key(cls, key)
         val1 = 1
         val2 = 2
         dobj = DictType({})
 
@@ -189,187 +220,187 @@
         self.assertEqual(dobj[key1], dobj[key2])
         self.assertEqual(len(dobj), 1)
         for kobj in dobj:
             self.assertIs(kobj, key1)
 
 
 class IntTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `IntType`."""
+    """Test case for |IntType|."""
 
     __slots__ = ()
 
     def test_int_type_mimics_int(self):
-        """Test whether `IntType` mimics `int`."""
+        """Test whether |IntType| mimics :class:`int`."""
         self.do_arithmetic_check(IntType, 0, 1)
 
     def test_int_type_is_extensible(self):
-        """Test whether `IntType` can be extended."""
+        """Test whether |IntType| can be extended."""
         self.do_extensibility_check(IntType(42))
 
 
 class FloatTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `FloatType`."""
+    """Test case for |FloatType|."""
 
     __slots__ = ()
 
     def test_float_type_mimics_float(self):
-        """Test whether `FloatType` mimics `float`."""
+        """Test whether |FloatType| mimics :class:`float`."""
         self.do_arithmetic_check(FloatType, 0.0, 1.0)
 
     def test_float_type_is_extensible(self):
-        """Test whether `FloatType` can be extended."""
+        """Test whether |FloatType| can be extended."""
         self.do_extensibility_check(FloatType(0.5))
 
 
 class StrTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `StrType`."""
+    """Test case for |StrType|."""
 
     __slots__ = ()
 
     def test_str_type_mimics_str(self):
-        """Test whether `StrType` mimics `str`."""
+        """Test whether |StrType| mimics :class:`str`."""
         self.do_sequence_check(StrType, "abc", "")
 
     def test_str_type_is_extensible(self):
-        """Test whether `StrType` can be extended."""
+        """Test whether |StrType| can be extended."""
         self.do_extensibility_check(StrType("abc"))
 
 
 class BytesTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `BytesType`."""
+    """Test case for |BytesType|."""
 
     __slots__ = ()
 
     def test_bytes_type_mimics_bytes(self):
-        """Test whether `BytesType` mimics `byte`."""
+        """Test whether |BytesType| mimics :class:`byte`."""
         self.do_sequence_check(BytesType, b"abc", b"")
 
     def test_bytes_type_is_extensible(self):
-        """Test whether `BytesType` can be extended."""
+        """Test whether |BytesType| can be extended."""
         self.do_extensibility_check(BytesType(b"\0"))
 
 
 class ListTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `ListType`."""
+    """Test case for |ListType|."""
 
     __slots__ = ()
 
     def test_list_type_mimics_list(self):
-        """Test whether `ListType` mimics `List`."""
+        """Test whether |ListType| mimics :class:`list`."""
         self.do_sequence_check(ListType, [1, 2, 3], [])
 
     def test_list_type_is_extensible(self):
-        """Test whether `ListType` can be extended."""
+        """Test whether |ListType| can be extended."""
         self.do_extensibility_check(ListType([1, 2, 3]))
 
 
 class SetTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `SetType`."""
+    """Test case for |SetType|."""
 
     __slots__ = ()
 
     def test_set_type_mimics_set(self):
-        """Test whether `SetType` mimics `set`."""
+        """Test whether |SetType| mimics :class:`set`."""
         self.assertEqual(SetType({1, 2.5, "a"}), {"a", 1, 2.5})
         self.assertIn("a", SetType({"a"}))
         self.assertFalse(SetType(set()))
         self.assertTrue(SetType({2}))
 
     def test_set_type_is_extensible(self):
-        """Test whether `SetType` can be extended."""
+        """Test whether |SetType| can be extended."""
         self.do_extensibility_check(SetType({"a"}))
 
 
 class DictTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `DictType`."""
+    """Test case for |DictType|."""
 
     __slots__ = ()
 
     def test_dict_type_mimics_dict(self):
-        """Test whether `DictType` mimics `dict`."""
+        """Test whether |DictType| mimics :class:`dict`."""
         self.assertEqual(DictType({"a": 1}), {"a": 1})
         self.assertIn("a", DictType({"a": "b"}))
         self.assertEqual(DictType({"a": "b"})["a"], "b")
         self.assertFalse(DictType({}))
         self.assertTrue(DictType({"a": 1}))
 
     def test_dict_type_is_extensible(self):
-        """Test whether `DictType` can be extended."""
+        """Test whether |DictType| can be extended."""
         self.do_extensibility_check(DictType({"a": 3.14}))
 
     def test_null_type_is_hashable(self):
-        """Test whether `NullType` is hashable."""
+        """Test whether |NullType| is hashable."""
         self.do_hashability_check(NullType, None)
 
     def test_bool_type_is_hashable(self):
-        """Test whether `BoolType` is hashable."""
+        """Test whether |BoolType| is hashable."""
         self.do_hashability_check(BoolType, True)
         self.do_hashability_check(BoolType, False)
 
     def test_int_type_is_hashable(self):
-        """Test whether `IntType` is hashable."""
+        """Test whether |IntType| is hashable."""
         self.do_hashability_check(IntType, 1)
 
     def test_float_type_is_hashable(self):
-        """Test whether `FloatType` is hashable."""
+        """Test whether |FloatType| is hashable."""
         self.do_hashability_check(FloatType, 1.6)
 
     def test_str_type_is_hashable(self):
-        """Test whether `StrType` is hashable."""
+        """Test whether |StrType| is hashable."""
         self.do_hashability_check(StrType, "abc")
 
     def test_bytes_type_is_hashable(self):
-        """Test whether `BytesType` is hashable."""
+        """Test whether |BytesType| is hashable."""
         self.do_hashability_check(BytesType, b"\xff")
 
     def test_date_type_is_hashable(self):
-        """Test whether `DateType` is hashable."""
+        """Test whether |DateType| is hashable."""
         self.do_hashability_check(DateType, datetime.date(2008, 1, 1))
 
     def test_datetime_type_is_hashable(self):
-        """Test whether `DateTimeType` is hashable."""
+        """Test whether |DateTimeType| is hashable."""
         self.do_hashability_check(DateTimeType, datetime.datetime(2008, 1, 1))
 
 
 class DateTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `DateType`."""
+    """Test case for |DateType|."""
 
     __slots__ = ()
 
     def test_date_type_mimics_date(self):
-        """Test whether `DateType` mimics `datetime.date`."""
+        """Test whether |DateType| mimics :class:`datetime.date`."""
         date_a = datetime.date(2008, 7, 8)
         date_b = DateType(2008, 7, 8)
         date_c = DateType(date_a)
 
         self.assertEqual(date_b, date_a)
         self.assertEqual(date_b, date_c)
 
     def test_date_type_is_extensible(self):
-        """Test whether `DateType` can be extended."""
+        """Test whether |DateType| can be extended."""
         self.do_extensibility_check(DateType(2008, 1, 1))
 
 
 class DateTimeTypeTestCase(YamlDataTypeTestCase):
-    """Test case for `DateTimeType`."""
+    """Test case for |DateTimeType|."""
 
     __slots__ = ()
 
     def test_datetime_type_mimics_datetime(self):
-        """Test whether `DateTimeType` mimics `datetime.datetime`."""
+        """Test whether |DateTimeType| mimics :class:`datetime.datetime`."""
         tzinfo = datetime.tzinfo(datetime.timedelta(hours=2, minutes=0))
         dt_a = datetime.datetime(2008, 7, 8, 13, 17, 21, 476, tzinfo, fold=1)
         dt_b = DateTimeType(2008, 7, 8, 13, 17, 21, 476, tzinfo, fold=1)
         dt_c = DateTimeType(dt_a)
 
         self.assertEqual(dt_b, dt_a)
         self.assertEqual(dt_b, dt_c)
 
     def test_datetime_type_is_extensible(self):
-        """Test whether `DateTimeType` can be extended."""
+        """Test whether |DateTimeType| can be extended."""
         self.do_extensibility_check(
             DateTimeType(
                 2008,
                 1,
                 1,
                 13,
                 0,
@@ -378,31 +409,31 @@
                 datetime.tzinfo(datetime.timedelta(hours=1)),
                 fold=0,
             )
         )
 
 
 class Obj2XObjTestCase(TestCase):
-    """Test case for `obj2xobj`."""
+    """Test case for |obj2xobj|."""
 
     __slots__ = ()
 
     def do_test_obj2xobj(self, klass, obj):
         """
-        Do the `obj2xobj` test.
+        Do the |obj2xobj| test.
 
-        :param klass: The subclass of `YamlDataType`
+        :param klass: The subclass of |YamlDataType|
         :param obj: The object
         """
         xobj = obj2xobj(obj)
         self.assertIsInstance(xobj, klass)
         self.assertEqual(xobj, obj)
 
     def test_obj2xobj(self):
-        """Test `obj2xobj`."""
+        """Test |obj2xobj|."""
         self.do_test_obj2xobj(NullType, None)
         self.do_test_obj2xobj(BoolType, False)
         self.do_test_obj2xobj(IntType, 1)
         self.do_test_obj2xobj(FloatType, 1.25)
         self.do_test_obj2xobj(StrType, "abc")
         self.do_test_obj2xobj(BytesType, b"\12")
         self.do_test_obj2xobj(ListType, [1, 2])
@@ -415,53 +446,58 @@
         self.assertEqual(
             ctx.exception.args[0],
             "<class 'function'> object cannot be made extensible",
         )
 
 
 class NewCTestCase(TestCase):
-    """Test case for `newc`."""
+    """Test case for |newc|."""
 
     __slots__ = ()
 
     def do_test_newc(self, ctor, obj, *args):
         """
-        Do the `newc` test.
+        Do the |newc| test.
 
         :param ctor: The name of the constructor
         :param obj: The object to be used for comparison
-        :param args: Additional arguments to `newc`
+        :param args: Additional positional arguments to |newc|
         """
         cobj = newc(ctor, args)
         self.assertIs(type(cobj), type(obj))
         self.assertEqual(cobj, obj)
 
     def test_newc(self):
-        """Test `newc`."""
+        """Test |newc|."""
 
         def eqfn(inst, other):
             """
             Equality test.
 
             :param inst: The instance of the owner object
             :param other: The instance of the other object
-            :return: `True` if the two objects are equal
+            :return: :obj:`True` if the two objects are equal
             """
             return isinstance(other, type(inst)) and inst.foo == other.foo
 
         tcls = make_type("TestType", members={"foo": 42, "__eq__": eqfn})
 
         self.do_test_newc("construct_yaml_set", set())
         self.do_test_newc("construct_yaml_map", {})
         self.do_test_newc("construct_yaml_object", tcls(), tcls)
         self.do_test_newc("construct_yaml_seq", [])
 
 
 class AnnotateTestCase(TestCase):
-    """Test case for `annotate`."""
+    """
+    Test case for |annotate|.
+
+    :ivar mark: The mock of :class:`yaml.error.Mark` instance
+    :ivar node: The mock of :class:`yaml.nodes.Node` instance
+    """
 
     __slots__ = ("mark", "node")
 
     def setUp(self):
         """Set up the test."""
         mark = make_mock()
         mark.name = "./foo.yml"
@@ -471,15 +507,15 @@
         node = make_mock()
         node.start_mark = mark
 
         self.mark = mark
         self.node = node
 
     def test_annotate(self):
-        """Test `annotate`."""
+        """Test |annotate|."""
         obj = annotate({}, self.node)
         loc = getloc(obj)
 
         self.assertEqual(loc.path, self.mark.name)
         self.assertEqual(loc.line, self.mark.line + 1)
         self.assertEqual(loc.column, self.mark.column + 1)
 
@@ -492,46 +528,46 @@
                 "<class 'vutils.validator.value.Location'>"
                 " object cannot be made extensible"
             ),
         )
 
 
 class GetLocTestCase(TestCase):
-    """Test case for `getloc`."""
+    """Test case for |getloc|."""
 
     __slots__ = ()
 
     def test_getloc(self):
-        """Test `getloc`."""
+        """Test |getloc|."""
         data = load_yaml("a: b")
         loc = getloc(data)
 
         self.assertEqual(loc.path, "<unicode string>")
         self.assertEqual(loc.line, 1)
         self.assertEqual(loc.column, 1)
 
 
 class KeyLocTestCase(TestCase):
-    """Test case for `keyloc`."""
+    """Test case for |keyloc|."""
 
     __slots__ = ()
 
     def test_keyloc(self):
-        """Test `keyloc`."""
+        """Test |keyloc|."""
         data = load_yaml("{a: 1, b: 2, a: 3}")
 
         self.assertEqual(keyloc(data, "a").column, 2)
         self.assertEqual(keyloc(data, "b").column, 8)
 
 
 class IsXTestCase(TestCase):
-    """Test case for `is_null` and `is_bool`."""
+    """Test case for |is_null| and |is_bool|."""
 
     __slots__ = ()
 
     def test_isx(self):
-        """Test `is_null` and `is_bool`."""
+        """Test |is_null| and |is_bool|."""
         self.assertTrue(is_null(NullType()))
         self.assertFalse(is_null(BoolType(False)))
 
         self.assertTrue(is_bool(BoolType(True)))
         self.assertFalse(is_bool(IntType(0)))
```

### Comparing `vutils-yaml-0.1.2/tests/unit/test_version.py` & `vutils-yaml-0.1.3/tests/unit/test_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # File:    ./tests/unit/test_version.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-23 10:01:39 +0200
 # Project: vutils-yaml: Working with YAML format
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.yaml.version` module."""
+"""Test :mod:`vutils.yaml.version` module."""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.yaml.version import __version__
 
 
 class VersionTestCase(TestCase):
```

### Comparing `vutils-yaml-0.1.2/tox.ini` & `vutils-yaml-0.1.3/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # Project: vutils-yaml: Working with YAML format
 # Brief:   Configuration for tox
 #
 # SPDX-License-Identifier: MIT
 #
 
 [tox]
+requires =
+    pip >= 19.2
+    setuptools >= 65.5.1
+    wheel >= 0.38.1
 envlist =
     py{37,38,39,310}, linters
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
-    pip >= 19.2
-    setuptools >= 65.5.1
-    wheel >= 0.38.1
     safety
     pytest
     pytest-cov
-    pytest-order
     vutils-python
     vutils-validator
     vutils-testing
     coveralls
 commands =
     safety check --full-report
     pytest -v --cov=vutils.yaml --cov-report=term-missing tests
```

