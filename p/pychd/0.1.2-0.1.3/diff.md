# Comparing `tmp/pychd-0.1.2.tar.gz` & `tmp/pychd-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychd-0.1.2.tar", max compression
+gzip compressed data, was "pychd-0.1.3.tar", max compression
```

## Comparing `pychd-0.1.2.tar` & `pychd-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.2/LICENSE
--rw-r--r--   0        0        0    19431 2023-04-21 03:53:19.623020 pychd-0.1.2/README.md
--rw-r--r--   0        0        0      791 2023-04-21 03:54:41.397613 pychd-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.2/src/pychd/__init__.py
--rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.2/src/pychd/compile.py
--rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.2/src/pychd/decompile.py
--rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.2/src/pychd/logging.conf.template
--rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.2/src/pychd/main.py
--rw-r--r--   0        0        0    20246 1970-01-01 00:00:00.000000 pychd-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.3/LICENSE
+-rw-r--r--   0        0        0    19426 2023-04-21 04:13:06.795036 pychd-0.1.3/README.md
+-rw-r--r--   0        0        0      791 2023-04-21 04:14:32.525484 pychd-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.3/src/pychd/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.3/src/pychd/compile.py
+-rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.3/src/pychd/decompile.py
+-rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.3/src/pychd/logging.conf.template
+-rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.3/src/pychd/main.py
+-rw-r--r--   0        0        0    20241 1970-01-01 00:00:00.000000 pychd-0.1.3/PKG-INFO
```

### Comparing `pychd-0.1.2/LICENSE` & `pychd-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pychd-0.1.2/README.md` & `pychd-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 ```bash
 pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
 ```
 
 ## Examples
 
-You can find examples in `example` directory or below (decompiled code is generated by `pychd`).
+You can find examples in `example` directory or below (decompiled code is generated by `pychd` from Python-3.10-compiled `.pyc` code).
 
 ### Variables
 
 original
 
 ```python
 # Assigning values to variables
@@ -253,34 +253,26 @@
 ```
 
 ### List comprehensions
 
 original
 
 ```python
-# Using a for loop to iterate through a list
-fruits = ["apple", "banana", "orange", "grape"]
-for fruit in fruits:
-    print(f"Current fruit: {fruit}")
-
-# Using a for loop with the range function
-for i in range(5):
-    print(f"Current value of i: {i}")
-
-# Using a while loop
-count = 0
-while count < 5:
-    print(f"Current count: {count}")
-    count += 1
+# Basic list comprehension
+squares = [x**2 for x in range(1, 6)]
+print(squares)  # Output: [1, 4, 9, 16, 25]
 
-# Using a nested loop
-for i in range(3):
-    print(f"Outer loop, i: {i}")
-    for j in range(2):
-        print(f"  Inner loop, j: {j}")
+# List comprehension with a condition
+even_squares = [x**2 for x in range(1, 6) if x % 2 == 0]
+print(even_squares)  # Output: [4, 16]
+
+# Nested list comprehension
+matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
+transpose = [[row[i] for row in matrix] for i in range(len(matrix))]
+print(transpose)  # Output: [[1, 4, 7], [2, 5, 8], [3, 6, 9]]
 
 ```
 
 decompiled
 
 ```python
 squares = [x**2 for x in range(1, 6)]
```

### Comparing `pychd-0.1.2/pyproject.toml` & `pychd-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities"
 keywords = ["decompiler", "python", "poetry", "bytecode"]
 license = "MIT"
 name = "pychd"
 packages = [{include = "src/pychd"}]
 readme = "README.md"
 repository = "https://github.com/diohabara/pychd"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 openai = "^0.27.4"
 pytest = "^7.3.1"
 python = ">=3.8, <3.11"
 pytype = "^2023.4.18"
```

### Comparing `pychd-0.1.2/src/pychd/compile.py` & `pychd-0.1.3/src/pychd/compile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.2/src/pychd/decompile.py` & `pychd-0.1.3/src/pychd/decompile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.2/src/pychd/main.py` & `pychd-0.1.3/src/pychd/main.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.2/PKG-INFO` & `pychd-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychd
-Version: 0.1.2
+Version: 0.1.3
 Summary: The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 Home-page: https://github.com/diohabara/pychd
 License: MIT
 Keywords: decompiler,python,poetry,bytecode
 Author: 卍diohabara卍
 Author-email: diohabara@gmail.com
 Requires-Python: >=3.8,<3.11
@@ -62,15 +62,15 @@
 
 ```bash
 pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
 ```
 
 ## Examples
 
-You can find examples in `example` directory or below (decompiled code is generated by `pychd`).
+You can find examples in `example` directory or below (decompiled code is generated by `pychd` from Python-3.10-compiled `.pyc` code).
 
 ### Variables
 
 original
 
 ```python
 # Assigning values to variables
@@ -274,34 +274,26 @@
 ```
 
 ### List comprehensions
 
 original
 
 ```python
-# Using a for loop to iterate through a list
-fruits = ["apple", "banana", "orange", "grape"]
-for fruit in fruits:
-    print(f"Current fruit: {fruit}")
-
-# Using a for loop with the range function
-for i in range(5):
-    print(f"Current value of i: {i}")
-
-# Using a while loop
-count = 0
-while count < 5:
-    print(f"Current count: {count}")
-    count += 1
+# Basic list comprehension
+squares = [x**2 for x in range(1, 6)]
+print(squares)  # Output: [1, 4, 9, 16, 25]
 
-# Using a nested loop
-for i in range(3):
-    print(f"Outer loop, i: {i}")
-    for j in range(2):
-        print(f"  Inner loop, j: {j}")
+# List comprehension with a condition
+even_squares = [x**2 for x in range(1, 6) if x % 2 == 0]
+print(even_squares)  # Output: [4, 16]
+
+# Nested list comprehension
+matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
+transpose = [[row[i] for row in matrix] for i in range(len(matrix))]
+print(transpose)  # Output: [[1, 4, 7], [2, 5, 8], [3, 6, 9]]
 
 ```
 
 decompiled
 
 ```python
 squares = [x**2 for x in range(1, 6)]
```

