# Comparing `tmp/wordflow-0.2.0.tar.gz` & `tmp/wordflow-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordflow-0.2.0.tar", max compression
+gzip compressed data, was "wordflow-0.2.1.tar", max compression
```

## Comparing `wordflow-0.2.0.tar` & `wordflow-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0     2385 2023-04-21 19:41:03.285518 wordflow-0.2.0/README.md
--rw-r--r--   0        0        0      648 2023-04-21 21:07:46.503074 wordflow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 13:18:55.609572 wordflow-0.2.0/wordflow/__init__.py
--rw-r--r--   0        0        0    12288 2023-04-21 20:43:33.006934 wordflow-0.2.0/wordflow/cli/.length.py.swp
--rw-r--r--   0        0        0    12288 2023-04-21 21:03:50.557231 wordflow-0.2.0/wordflow/cli/.lessthan.py.swp
--rw-r--r--   0        0        0    12288 2023-04-21 20:46:37.677071 wordflow-0.2.0/wordflow/cli/.max.py.swp
--rw-r--r--   0        0        0    12288 2023-04-21 21:07:42.372669 wordflow-0.2.0/wordflow/cli/.put.py.swp
--rw-r--r--   0        0        0      101 2023-04-21 13:58:45.274489 wordflow-0.2.0/wordflow/cli/count.py
--rw-r--r--   0        0        0      541 2023-04-21 16:04:45.838288 wordflow-0.2.0/wordflow/cli/frequency.py
--rw-r--r--   0        0        0      514 2023-04-21 16:04:13.879276 wordflow-0.2.0/wordflow/cli/length.py
--rw-r--r--   0        0        0     1299 2023-04-21 21:03:38.425773 wordflow-0.2.0/wordflow/cli/lessthan.py
--rw-r--r--   0        0        0      555 2023-04-21 16:02:22.444874 wordflow-0.2.0/wordflow/cli/match.py
--rw-r--r--   0        0        0      579 2023-04-21 18:14:10.862835 wordflow-0.2.0/wordflow/cli/max.py
--rw-r--r--   0        0        0      580 2023-04-21 18:14:01.345739 wordflow-0.2.0/wordflow/cli/min.py
--rw-r--r--   0        0        0      996 2023-04-21 16:11:10.563267 wordflow-0.2.0/wordflow/cli/order.py
--rw-r--r--   0        0        0      425 2023-04-21 16:03:46.266136 wordflow-0.2.0/wordflow/cli/pluck.py
--rw-r--r--   0        0        0      499 2023-04-21 21:06:30.615593 wordflow-0.2.0/wordflow/cli/put.py
--rw-r--r--   0        0        0       26 2023-04-21 13:46:51.770583 wordflow-0.2.0/wordflow/cli/reverse.py
--rw-r--r--   0        0        0      559 2023-04-21 20:41:40.966713 wordflow-0.2.0/wordflow/cli/unique.py
--rw-r--r--   0        0        0      787 2023-04-21 16:12:58.723877 wordflow-0.2.0/wordflow/pipe_guard.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 wordflow-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-04-21 21:17:11.493442 wordflow-0.2.1/README.md
+-rw-r--r--   0        0        0      682 2023-04-21 21:12:18.934280 wordflow-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 13:18:55.609572 wordflow-0.2.1/wordflow/__init__.py
+-rw-r--r--   0        0        0    12288 2023-04-21 21:11:13.430618 wordflow-0.2.1/wordflow/cli/.lessthan.py.swp
+-rw-r--r--   0        0        0      101 2023-04-21 13:58:45.274489 wordflow-0.2.1/wordflow/cli/count.py
+-rw-r--r--   0        0        0     1138 2023-04-21 21:11:42.865172 wordflow-0.2.1/wordflow/cli/equal.py
+-rw-r--r--   0        0        0      541 2023-04-21 16:04:45.838288 wordflow-0.2.1/wordflow/cli/frequency.py
+-rw-r--r--   0        0        0      514 2023-04-21 16:04:13.879276 wordflow-0.2.1/wordflow/cli/length.py
+-rw-r--r--   0        0        0     1299 2023-04-21 21:03:38.425773 wordflow-0.2.1/wordflow/cli/lessthan.py
+-rw-r--r--   0        0        0      555 2023-04-21 16:02:22.444874 wordflow-0.2.1/wordflow/cli/match.py
+-rw-r--r--   0        0        0      579 2023-04-21 18:14:10.862835 wordflow-0.2.1/wordflow/cli/max.py
+-rw-r--r--   0        0        0      580 2023-04-21 18:14:01.345739 wordflow-0.2.1/wordflow/cli/min.py
+-rw-r--r--   0        0        0      996 2023-04-21 16:11:10.563267 wordflow-0.2.1/wordflow/cli/order.py
+-rw-r--r--   0        0        0      425 2023-04-21 16:03:46.266136 wordflow-0.2.1/wordflow/cli/pluck.py
+-rw-r--r--   0        0        0      499 2023-04-21 21:06:30.615593 wordflow-0.2.1/wordflow/cli/put.py
+-rw-r--r--   0        0        0       26 2023-04-21 13:46:51.770583 wordflow-0.2.1/wordflow/cli/reverse.py
+-rw-r--r--   0        0        0      559 2023-04-21 20:41:40.966713 wordflow-0.2.1/wordflow/cli/unique.py
+-rw-r--r--   0        0        0      787 2023-04-21 16:12:58.723877 wordflow-0.2.1/wordflow/pipe_guard.py
+-rw-r--r--   0        0        0     3172 1970-01-01 00:00:00.000000 wordflow-0.2.1/PKG-INFO
```

### Comparing `wordflow-0.2.0/README.md` & `wordflow-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -33,28 +33,38 @@
 ```
 $ cat words.txt | match "a" | match "e" | match "i" | match "o" | match "u" | length | order | head
 ```
 
 ## What are the most common ten-letter words? 
 
 ```
-$ cat words.txt | length | max 10 | min 10 | frequency 1 | order -r | pluck 2 | head
+$ cat words.txt | length | put 10 | equal | frequency 2 | order -r | pluck 3 | head
+```
+
+## What's the longest word which contains no repeated letters? 
+
+```
+$ cat words.txt | length | unique 1 | length | lessthan 0 1 -e | lessthan 1 0 -e | 
 ```
 
 ### Filter
 
 - **match [pattern] [position=0]**: Allows lines where the specified word matches
   regular expression `pattern`. Regular expressions often need to be in quotation marks.
-- **max [value] [position=0]**: Allows lines where the specified number is no 
-  greater than `value`.
+- **lessthan [position0=0] [position1=1] [--equal]**: Allows lines where the number at 
+  position 0 is less than the number at position 1. When `--equal`, lines are also 
+  allowed when the two numbers are equal.
+- **equal [position0] [position1]**: Allows lines where the number at position 0 
+  is equal to the number at position 1.
 - **min [value] [position=0]**: Allows lines where the specified number is no 
   less than `value`.
 
 ### Map 
 
+- **put [value]** Prepends the value to each line.
 - **length [position=0]** Prepends the length of the specified word to the line.
 - **frequency [position=0]** Prepends the frequency of the specified word 
   (approximate number of occurrences per billion words) to the line. 
 - **pluck [position=0]** Replaces each line with the specified token.
 
 ### Sort
```

### Comparing `wordflow-0.2.0/pyproject.toml` & `wordflow-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordflow"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Chris Proctor <github.com@accounts.chrisproctor.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 wordfreq = "^3.0.3"
@@ -12,14 +12,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 match = "wordflow.cli.match:main"
 lessthan = "wordflow.cli.lessthan:main"
+equal = "wordflow.cli.equal:main"
 order = "wordflow.cli.order:main"
 pluck = "wordflow.cli.pluck:main"
 length = "wordflow.cli.length:main"
 frequency = "wordflow.cli.frequency:main"
 count = "wordflow.cli.count:main"
 unique = "wordflow.cli.unique:main"
 put = "wordflow.cli.put:main"
```

### Comparing `wordflow-0.2.0/wordflow/cli/frequency.py` & `wordflow-0.2.1/wordflow/cli/frequency.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/length.py` & `wordflow-0.2.1/wordflow/cli/length.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/lessthan.py` & `wordflow-0.2.1/wordflow/cli/lessthan.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/match.py` & `wordflow-0.2.1/wordflow/cli/match.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/max.py` & `wordflow-0.2.1/wordflow/cli/max.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/min.py` & `wordflow-0.2.1/wordflow/cli/min.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/order.py` & `wordflow-0.2.1/wordflow/cli/order.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/cli/unique.py` & `wordflow-0.2.1/wordflow/cli/unique.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/wordflow/pipe_guard.py` & `wordflow-0.2.1/wordflow/pipe_guard.py`

 * *Files identical despite different names*

### Comparing `wordflow-0.2.0/PKG-INFO` & `wordflow-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordflow
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Chris Proctor
 Author-email: github.com@accounts.chrisproctor.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: wordfreq (>=3.0.3,<4.0.0)
@@ -45,28 +45,38 @@
 ```
 $ cat words.txt | match "a" | match "e" | match "i" | match "o" | match "u" | length | order | head
 ```
 
 ## What are the most common ten-letter words? 
 
 ```
-$ cat words.txt | length | max 10 | min 10 | frequency 1 | order -r | pluck 2 | head
+$ cat words.txt | length | put 10 | equal | frequency 2 | order -r | pluck 3 | head
+```
+
+## What's the longest word which contains no repeated letters? 
+
+```
+$ cat words.txt | length | unique 1 | length | lessthan 0 1 -e | lessthan 1 0 -e | 
 ```
 
 ### Filter
 
 - **match [pattern] [position=0]**: Allows lines where the specified word matches
   regular expression `pattern`. Regular expressions often need to be in quotation marks.
-- **max [value] [position=0]**: Allows lines where the specified number is no 
-  greater than `value`.
+- **lessthan [position0=0] [position1=1] [--equal]**: Allows lines where the number at 
+  position 0 is less than the number at position 1. When `--equal`, lines are also 
+  allowed when the two numbers are equal.
+- **equal [position0] [position1]**: Allows lines where the number at position 0 
+  is equal to the number at position 1.
 - **min [value] [position=0]**: Allows lines where the specified number is no 
   less than `value`.
 
 ### Map 
 
+- **put [value]** Prepends the value to each line.
 - **length [position=0]** Prepends the length of the specified word to the line.
 - **frequency [position=0]** Prepends the frequency of the specified word 
   (approximate number of occurrences per billion words) to the line. 
 - **pluck [position=0]** Replaces each line with the specified token.
 
 ### Sort
```

