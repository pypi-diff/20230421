# Comparing `tmp/proxyorderedset-0.3.1.tar.gz` & `tmp/proxyorderedset-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyorderedset-0.3.1.tar", last modified: Wed Aug  3 14:24:22 2022, max compression
+gzip compressed data, was "proxyorderedset-0.3.2.tar", last modified: Fri Apr 21 13:49:53 2023, max compression
```

## Comparing `proxyorderedset-0.3.1.tar` & `proxyorderedset-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-03 14:24:22.926048 proxyorderedset-0.3.1/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1211 2021-12-21 10:52:02.000000 proxyorderedset-0.3.1/LICENSE
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2022-08-03 14:24:22.926149 proxyorderedset-0.3.1/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      552 2022-08-03 14:10:17.000000 proxyorderedset-0.3.1/README.md
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      815 2022-08-03 14:24:05.000000 proxyorderedset-0.3.1/pyproject.toml
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1071 2022-08-03 14:24:22.926770 proxyorderedset-0.3.1/setup.cfg
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:03:26.000000 proxyorderedset-0.3.1/setup.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-03 14:24:22.922416 proxyorderedset-0.3.1/src/
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-03 14:24:22.924462 proxyorderedset-0.3.1/src/orderedset/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      119 2022-08-03 14:24:00.000000 proxyorderedset-0.3.1/src/orderedset/__init__.py
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     8364 2022-05-23 04:18:31.000000 proxyorderedset-0.3.1/src/orderedset/orderedset.py
-drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2022-08-03 14:24:22.925836 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2022-08-03 14:24:22.000000 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/PKG-INFO
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      321 2022-08-03 14:24:22.000000 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/SOURCES.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2022-08-03 14:24:22.000000 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/dependency_links.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)      191 2022-08-03 14:24:22.000000 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/requires.txt
--rw-r--r--   0 dsteinhoefel   (501) staff       (20)       11 2022-08-03 14:24:22.000000 proxyorderedset-0.3.1/src/proxyorderedset.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.186386 proxyorderedset-0.3.2/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1211 2021-12-21 10:52:02.000000 proxyorderedset-0.3.2/LICENSE
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-21 13:49:53.186540 proxyorderedset-0.3.2/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      552 2022-08-03 14:10:17.000000 proxyorderedset-0.3.2/README.md
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      815 2023-04-21 13:48:32.000000 proxyorderedset-0.3.2/pyproject.toml
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     1071 2023-04-21 13:49:53.186985 proxyorderedset-0.3.2/setup.cfg
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       69 2022-08-03 14:03:26.000000 proxyorderedset-0.3.2/setup.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.181514 proxyorderedset-0.3.2/src/
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.184102 proxyorderedset-0.3.2/src/orderedset/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      119 2023-04-21 13:48:36.000000 proxyorderedset-0.3.2/src/orderedset/__init__.py
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     9988 2023-04-21 13:48:24.000000 proxyorderedset-0.3.2/src/orderedset/orderedset.py
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.185740 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     2774 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/PKG-INFO
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      346 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/SOURCES.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)        1 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/dependency_links.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)      191 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/requires.txt
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)       11 2023-04-21 13:49:53.000000 proxyorderedset-0.3.2/src/proxyorderedset.egg-info/top_level.txt
+drwxr-xr-x   0 dsteinhoefel   (501) staff       (20)        0 2023-04-21 13:49:53.186022 proxyorderedset-0.3.2/tests/
+-rw-r--r--   0 dsteinhoefel   (501) staff       (20)     5172 2022-08-03 14:14:09.000000 proxyorderedset-0.3.2/tests/test_orderedset.py
```

### Comparing `proxyorderedset-0.3.1/LICENSE` & `proxyorderedset-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.1/PKG-INFO` & `proxyorderedset-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyorderedset
-Version: 0.3.1
+Version: 0.3.2
 Summary: A simple implementation of ordered sets as a proxy to Python's standard dict class.
 Home-page: https://github.com/rindPHI/proxyorderedset
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `proxyorderedset-0.3.1/README.md` & `proxyorderedset-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.1/pyproject.toml` & `proxyorderedset-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxyorderedset"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Dominic Steinhöfel", email="dominic.steinhoefel@cispa.de" },
 ]
 description = "A simple implementation of ordered sets as a proxy to Python's standard dict class."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `proxyorderedset-0.3.1/setup.cfg` & `proxyorderedset-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `proxyorderedset-0.3.1/src/orderedset/orderedset.py` & `proxyorderedset-0.3.2/src/orderedset/orderedset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 from collections.abc import Set, Iterator, Iterable
 from typing import TypeVar, Generic, Optional, Any, Dict, Union
 
 from frozendict import frozendict
 
 T = TypeVar("T")
 S = TypeVar("S")
@@ -29,27 +30,86 @@
 
     def __str__(self) -> str:
         return "{" + ", ".join(list(map(str, self.the_dict))) + "}"
 
     def __repr__(self) -> str:
         return f"OrderedSet({repr(self.the_dict)})"
 
-    def __getitem__(self, item: int) -> T:
-        assert isinstance(item, int)
-        if item >= len(self):
-            raise IndexError('list index out of range')
-
-        idx = 0
-        for elem in iter(self):
-            if idx == item:
-                return elem
+    def __getitem__(self, item: int | slice) -> T | 'OrderedSet[T]':
+        """
+        Returns the indexed item or subset.
 
-            idx += 1
+        Example:
 
-        assert False
+        >>> s = OrderedSet([1, 2, 3, 4, 5])
+
+        We can access individual elements of the list, starting from index 0.
+
+        >>> s[1]
+        2
+
+        Negative indices work, too, just as for Python lists.
+
+        >>> s[-2]
+        4
+
+        If we access an item with a too high index, we receive and error.
+
+        >>> s[5]
+        Traceback (most recent call last):
+        ...
+        IndexError: list index out of range
+
+        Slices work, too:
+
+        >>> s[1:3]
+        OrderedSet({2: None, 3: None})
+
+        Their semantics is the same as for ordinary lists.
+
+        >>> list(s)[1:3] == list(s[1:3])
+        True
+
+        High indices are fine:
+
+        >>> s[1:700]
+        OrderedSet({2: None, 3: None, 4: None, 5: None})
+
+        However, negative indices are not allowed (this is different for lists!):
+
+        >>> s[-1:700]
+        Traceback (most recent call last):
+        ...
+        ValueError: Indices for islice() must be None or an integer: 0 <= x <= sys.maxsize.
+
+        :param item: An item index or a slice defining what item(s) to return.
+        :return: The indexed item or subset.
+        """
+        assert isinstance(item, int) or isinstance(item, slice)
+        if isinstance(item, int):
+            if item < 0:
+                item = len(self) + item
+
+            if item < 0 or item >= len(self):
+                raise IndexError("list index out of range")
+
+            idx = 0
+            for elem in iter(self):
+                if idx == item:
+                    return elem
+
+                idx += 1
+
+            assert False
+        else:
+            start = item.start or 0
+            stop = item.stop or 0
+            step = item.step or 1
+
+            return OrderedSet(itertools.islice(iter(self), start, stop, step))
 
     def add(self, element: T) -> None:
         self.the_dict = {**self.the_dict, **{element: None}}
 
     def clear(self) -> None:
         self.the_dict.clear()
```

### Comparing `proxyorderedset-0.3.1/src/proxyorderedset.egg-info/PKG-INFO` & `proxyorderedset-0.3.2/src/proxyorderedset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxyorderedset
-Version: 0.3.1
+Version: 0.3.2
 Summary: A simple implementation of ordered sets as a proxy to Python's standard dict class.
 Home-page: https://github.com/rindPHI/proxyorderedset
 Author: Dominic Steinhöfel
 Author-email: Dominic Steinhöfel <dominic.steinhoefel@cispa.de>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

