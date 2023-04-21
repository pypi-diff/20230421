# Comparing `tmp/pycutils-0.0.9.tar.gz` & `tmp/pycutils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutils-0.0.9.tar", last modified: Tue Mar 28 16:19:06 2023, max compression
+gzip compressed data, was "pycutils-0.1.0.tar", last modified: Fri Apr 21 15:45:33 2023, max compression
```

## Comparing `pycutils-0.0.9.tar` & `pycutils-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-28 16:19:06.026562 pycutils-0.0.9/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-03-28 16:19:06.026738 pycutils-0.0.9/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      552 2023-03-27 19:00:47.000000 pycutils-0.0.9/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      238 2023-03-27 19:00:47.000000 pycutils-0.0.9/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      660 2023-03-28 16:19:06.027511 pycutils-0.0.9/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-28 16:19:06.019169 pycutils-0.0.9/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-28 16:19:06.023358 pycutils-0.0.9/src/cutils/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       27 2023-03-27 19:00:48.000000 pycutils-0.0.9/src/cutils/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8056 2023-03-28 16:15:05.000000 pycutils-0.0.9/src/cutils/cutils.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2022-04-12 16:00:10.000000 pycutils-0.0.9/src/cutils/py.typed
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-28 16:19:06.025570 pycutils-0.0.9/src/pycutils.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-03-28 16:19:06.000000 pycutils-0.0.9/src/pycutils.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-03-28 16:19:06.000000 pycutils-0.0.9/src/pycutils.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-03-28 16:19:06.000000 pycutils-0.0.9/src/pycutils.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        7 2023-03-28 16:19:06.000000 pycutils-0.0.9/src/pycutils.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-03-28 16:19:06.026099 pycutils-0.0.9/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1565 2023-03-27 19:00:48.000000 pycutils-0.0.9/tests/test_cutils.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.437397 pycutils-0.1.0/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-04-21 15:45:33.437681 pycutils-0.1.0/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      552 2023-04-19 15:24:24.000000 pycutils-0.1.0/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      238 2023-04-19 15:24:24.000000 pycutils-0.1.0/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      660 2023-04-21 15:45:33.438733 pycutils-0.1.0/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.429602 pycutils-0.1.0/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.433644 pycutils-0.1.0/src/cutils/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       27 2023-04-19 15:24:25.000000 pycutils-0.1.0/src/cutils/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8373 2023-04-21 15:41:26.000000 pycutils-0.1.0/src/cutils/cutils.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2022-04-12 16:00:10.000000 pycutils-0.1.0/src/cutils/py.typed
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.435997 pycutils-0.1.0/src/pycutils.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        7 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.436689 pycutils-0.1.0/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1754 2023-04-21 15:44:37.000000 pycutils-0.1.0/tests/test_cutils.py
```

### Comparing `pycutils-0.0.9/PKG-INFO` & `pycutils-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutils
-Version: 0.0.9
+Version: 0.1.0
 Summary: A list of python utilities
 Home-page: https://github.com/CangyuanLi/cutils
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/cutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycutils-0.0.9/README.md` & `pycutils-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pycutils-0.0.9/setup.cfg` & `pycutils-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pycutils
-version = 0.0.9
+version = 0.1.0
 author = Cangyuan Li
 author_email = everest229@gmail.com
 description = A list of python utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CangyuanLi/cutils
 project_urls =
```

### Comparing `pycutils-0.0.9/src/cutils/cutils.py` & `pycutils-0.1.0/src/cutils/cutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # Imports
 
+import abc
 from collections.abc import Callable, Generator, Iterable, MutableMapping, Sequence
 from dataclasses import dataclass
 import functools
 import math
 import random
 import re
 import statistics
 import time
 import threading
-from typing import Any, Union
+from typing import Any, Protocol, TypeVar, Union
 
 # Types
 
 Real = Union[int, float]
 
 
+class Comparable(Protocol):
+    @abc.abstractmethod
+    def __lt__(self, other) -> bool:
+        pass
+
+
 @dataclass
 class TimeFuncRes:
     avg: Real
     median: Real
     min: Real
     max: Real
     sd: Real
@@ -69,14 +76,23 @@
     """
     if n <= 0:
         raise ValueError("chunk size must be a positive integer")
 
     return list(_chunk_seq(seq, n))
 
 
+def clamp(num: Comparable, min: Comparable, max: Comparable) -> Comparable:
+    if num > max:
+        return max
+    elif num < min:
+        return min
+    else:
+        return num
+
+
 def _random_chunk_seq(seq: Sequence, min: int, max: int):
     i = 0
     while i < len(seq):
         chunk_size = random.randint(min, max)
         yield seq[i : i + chunk_size]
 
         i += chunk_size
@@ -270,16 +286,16 @@
     if avg_elapsed < 0.1:
         avg_display = f"{avg_elapsed * 1_000_000:.3f} microseconds"
     else:
         avg_display = f"{avg_elapsed:.2f} seconds"
 
     if quiet is False:
         result = (
-            f"{func_name} ran {iterations:,} times and completed in {display_time(total)} "
-            f"for an average time of {avg_display} per run"
+            f"{func_name} ran {iterations:,} times and completed in"
+            f" {display_time(total)} for an average time of {avg_display} per run"
         )
 
         print(result)
 
     res = TimeFuncRes(
         avg=avg_elapsed,
         median=median_elapsed,
```

### Comparing `pycutils-0.0.9/src/pycutils.egg-info/PKG-INFO` & `pycutils-0.1.0/src/pycutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycutils
-Version: 0.0.9
+Version: 0.1.0
 Summary: A list of python utilities
 Home-page: https://github.com/CangyuanLi/cutils
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/cutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycutils-0.0.9/tests/test_cutils.py` & `pycutils-0.1.0/tests/test_cutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,62 @@
+import pytest
+
 from cutils import cutils
 
+
 def test_contains():
     assert cutils.contains("a", "bce") is False
     assert cutils.contains("a", "alde") is True
     assert cutils.contains([2, 3, 4], [3, 4]) is True
     assert cutils.contains(list(range(0, 100000)), {9, 100}) is True
     assert cutils.contains({9, 100}, list(range(0, 100000))) is True
     assert cutils.contains("abcdefg", "hijk") is False
     assert cutils.contains("abcdefg", "a") is True
 
+
 def test_chunk_seq():
     test_list = [1, 2, 3, 4, 5, 6, 7]
     assert cutils.chunk_seq(test_list, 2) == [[1, 2], [3, 4], [5, 6], [7]]
     assert cutils.chunk_seq([], 2) == []
     assert cutils.chunk_seq("abcdefgh", 4) == ["abcd", "efgh"]
 
+
+def test_clamp():
+    assert cutils.clamp(5, 1, 2) == 2
+    assert cutils.clamp(0, 1, 2) == 1
+
+
 def test_random_chunk_seq():
     test_list = [1, 2, 3, 4, 5, 6, 7, 9, 10]
     assert cutils.flatten(cutils.random_chunk_seq(test_list, 2, 5)) == test_list
 
+
 def test_even_split():
     test_list = [1, 2, 3, 4, 5]
     assert cutils.even_split(test_list, 6) == [[1], [2], [3], [4], [5], []]
     assert cutils.even_split((1, 2, 3), 3) == [(1,), (2,), (3,)]
 
+
 def test_find_last_index():
     test_list = [4, 2, 4, 4, 2]
     assert cutils.find_last_index(test_list, 2) == 4
-    assert cutils.find_last_index(test_list, 3) is None
+
+    with pytest.raises(ValueError):
+        cutils.find_last_index(test_list, 3)
+
 
 def test_flatten():
     test_list = [[1], [2], "ab", 3]
     assert cutils.flatten(test_list) == [1, 2, "ab", 3]
 
+
 def test_get_factors():
     assert cutils.get_factors(10) == {2, 5, 1, 10}
 
+
 def test_ordered_unique():
     assert cutils.ordered_unique("abbcb") == ["a", "b", "c"]
 
+
 def test_strip_blanks():
     assert cutils.strip_blanks("a   bc\u2009") == "abc"
+    assert cutils.strip_blanks("a") == "a"
```

