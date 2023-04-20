# Comparing `tmp/ib110hw-0.1.3.tar.gz` & `tmp/ib110hw-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpx5zacmh7\ib110hw-0.1.3.tar", last modified: Mon Apr 17 11:02:44 2023, max compression
+gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmptxq5pl5a\ib110hw-0.1.4.tar", last modified: Thu Apr 20 22:37:21 2023, max compression
```

## Comparing `ib110hw-0.1.3.tar` & `ib110hw-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    26734 2023-04-17 11:02:44.000000 ib110hw-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    26293 2023-04-17 08:42:12.000000 ib110hw-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 11:02:44.000000 ib110hw-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-17 11:00:05.000000 ib110hw-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw/
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.3/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8286 2023-04-17 08:04:31.000000 ib110hw-0.1.3/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.3/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.3/src/ib110hw/automaton/utils.py
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.3/src/ib110hw/automaton/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw/turing/
--rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.3/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.3/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.3/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.3/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     1246 2023-04-17 08:14:21.000000 ib110hw-0.1.3/src/ib110hw/turing/utils.py
--rw-rw-rw-   0        0        0     5031 2023-04-17 08:11:17.000000 ib110hw-0.1.3/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.3/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.3/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    26734 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 11:02:44.000000 ib110hw-0.1.3/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 11:02:44.000000 ib110hw-0.1.3/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.3/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.3/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.3/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.3/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    26734 2023-04-20 22:37:21.000000 ib110hw-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    26293 2023-04-17 08:42:12.000000 ib110hw-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 22:37:21.000000 ib110hw-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-04-20 22:33:40.000000 ib110hw-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.4/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.4/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.4/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.4/src/ib110hw/automaton/utils.py
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.4/src/ib110hw/automaton/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.4/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.4/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.4/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.4/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     1246 2023-04-17 08:14:21.000000 ib110hw-0.1.4/src/ib110hw/turing/utils.py
+-rw-rw-rw-   0        0        0     5031 2023-04-17 08:11:17.000000 ib110hw-0.1.4/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.4/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.4/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    26734 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 22:37:21.000000 ib110hw-0.1.4/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 22:37:21.000000 ib110hw-0.1.4/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.4/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.4/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.4/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.4/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.3/LICENSE` & `ib110hw-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/PKG-INFO` & `ib110hw-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.3
+Version: 0.1.4
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ib110hw-0.1.3/README.md` & `ib110hw-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/setup.py` & `ib110hw-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.3",
+    version="0.1.4",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.1.3/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.4/src/ib110hw/automaton/dfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         states: Set[str] = None,
         alphabet: Set[str] = None,
         initial_state: str = None,
         final_states: Set[str] = None,
         transitions: DFATransitions = None,
     ) -> None:
         if transitions:
-            states = states or set(transitions.keys())
+            states = states if states is not None else set(transitions.keys())
 
         super().__init__(states, alphabet, initial_state, final_states)
-        self.transitions = transitions or {}
+        self.transitions = transitions if transitions is not None else {}
 
     def __repr__(self) -> str:
         return super().__repr__() + "\n" + self.__repr_transitions__()
 
     def __repr_transitions__(self) -> str:
         def get_max_cell_width() -> int:
             max_cell_width = 5
```

### Comparing `ib110hw-0.1.3/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.4/src/ib110hw/automaton/nfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         states: Set[str] = None,
         alphabet: Set[str] = None,
         initial_state: str = None,
         final_states: Set[str] = None,
         transitions: NFATransitions = None,
     ) -> None:
         if transitions:
-            states = states or set(transitions.keys())
+            states = states if states is not None else set(transitions.keys())
 
         super().__init__(states, alphabet, initial_state, final_states)
-        self.transitions = transitions or {}
+        self.transitions = transitions if transitions is not None else {}
 
     def __repr__(self) -> str:
         return super().__repr__() + "\n" + self.__repr_transitions__()
 
     def __repr_transitions__(self) -> str:
         def get_max_cell_width():
             max_cell_width = 5
```

### Comparing `ib110hw-0.1.3/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.4/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/base.py` & `ib110hw-0.1.4/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.4/src/ib110hw/turing/dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/mtm.py` & `ib110hw-0.1.4/src/ib110hw/turing/mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/tape.py` & `ib110hw-0.1.4/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/utils.py` & `ib110hw-0.1.4/src/ib110hw/turing/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw/turing/_helpers.py` & `ib110hw-0.1.4/src/ib110hw/turing/_helpers.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.4/src/ib110hw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.3
+Version: 0.1.4
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ib110hw-0.1.3/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.4/src/ib110hw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/tests/test_dfa.py` & `ib110hw-0.1.4/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/tests/test_dtm.py` & `ib110hw-0.1.4/tests/test_dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/tests/test_mtm.py` & `ib110hw-0.1.4/tests/test_mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.3/tests/test_nfa.py` & `ib110hw-0.1.4/tests/test_nfa.py`

 * *Files identical despite different names*

