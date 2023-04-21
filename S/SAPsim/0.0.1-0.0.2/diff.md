# Comparing `tmp/SAPsim-0.0.1.tar.gz` & `tmp/SAPsim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-0.0.1.tar", last modified: Fri Apr 21 18:32:41 2023, max compression
+gzip compressed data, was "SAPsim-0.0.2.tar", last modified: Fri Apr 21 18:48:51 2023, max compression
```

## Comparing `SAPsim-0.0.1.tar` & `SAPsim-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.480839 SAPsim-0.0.1/
--rw-r--r--   0 jesse      (501) staff       (20)     1066 2023-02-23 19:54:52.000000 SAPsim-0.0.1/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)     1252 2023-04-21 18:32:41.480945 SAPsim-0.0.1/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     3098 2023-04-21 18:22:40.000000 SAPsim-0.0.1/README.md
--rw-r--r--   0 jesse      (501) staff       (20)      301 2023-04-21 18:01:43.000000 SAPsim-0.0.1/README_PyPI.md
--rw-r--r--   0 jesse      (501) staff       (20)      908 2023-04-21 17:59:42.000000 SAPsim-0.0.1/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)      728 2023-04-21 18:32:41.481255 SAPsim-0.0.1/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)     1492 2023-04-21 18:00:02.000000 SAPsim-0.0.1/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.474648 SAPsim-0.0.1/src/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.476081 SAPsim-0.0.1/src/SAPsim/
--rw-r--r--   0 jesse      (501) staff       (20)     3547 2023-04-21 18:11:33.000000 SAPsim-0.0.1/src/SAPsim/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.477221 SAPsim-0.0.1/src/SAPsim.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)     1252 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      546 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-02-25 02:12:35.000000 SAPsim-0.0.1/src/SAPsim.egg-info/not-zip-safe
--rw-r--r--   0 jesse      (501) staff       (20)       93 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)       13 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/top_level.txt
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.479302 SAPsim-0.0.1/src/utils/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-03-16 06:39:53.000000 SAPsim-0.0.1/src/utils/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     7460 2023-03-27 00:31:56.000000 SAPsim-0.0.1/src/utils/exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     1704 2023-03-27 00:30:53.000000 SAPsim-0.0.1/src/utils/execute.py
--rw-r--r--   0 jesse      (501) staff       (20)     2078 2023-04-21 17:32:33.000000 SAPsim-0.0.1/src/utils/globs.py
--rw-r--r--   0 jesse      (501) staff       (20)     6729 2023-04-21 17:36:55.000000 SAPsim-0.0.1/src/utils/helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     5861 2023-03-27 00:30:53.000000 SAPsim-0.0.1/src/utils/instructions.py
--rw-r--r--   0 jesse      (501) staff       (20)     3702 2023-04-21 18:11:33.000000 SAPsim-0.0.1/src/utils/parser.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.480600 SAPsim-0.0.1/tests/
--rw-r--r--   0 jesse      (501) staff       (20)     3021 2023-04-21 18:21:50.000000 SAPsim-0.0.1/tests/test_example_progs.py
--rw-r--r--   0 jesse      (501) staff       (20)      689 2023-04-21 18:21:50.000000 SAPsim-0.0.1/tests/test_exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     1336 2023-03-27 00:28:37.000000 SAPsim-0.0.1/tests/test_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     4783 2023-03-27 00:28:31.000000 SAPsim-0.0.1/tests/test_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-21 18:48:42.000000 SAPsim-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-21 18:48:51.240523 SAPsim-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-21 18:48:42.000000 SAPsim-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 18:48:42.000000 SAPsim-0.0.2/README_PyPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 18:48:42.000000 SAPsim-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-21 18:48:51.240523 SAPsim-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-21 18:48:42.000000 SAPsim-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.236523 SAPsim-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 18:48:51.000000 SAPsim-0.0.2/src/SAPsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-21 18:48:42.000000 SAPsim-0.0.2/src/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:48:51.240523 SAPsim-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-21 18:48:42.000000 SAPsim-0.0.2/tests/test_instructions.py
```

### Comparing `SAPsim-0.0.1/LICENSE` & `SAPsim-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/PKG-INFO` & `SAPsim-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/sapsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
```

### Comparing `SAPsim-0.0.1/README.md` & `SAPsim-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/pyproject.toml` & `SAPsim-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/setup.cfg` & `SAPsim-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/setup.py` & `SAPsim-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Version number that appears on PyPI and Test PyPI
-    version="0.0.1",
+    version="0.0.2",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/sapsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-0.0.1/src/SAPsim/__init__.py` & `SAPsim-0.0.2/src/SAPsim/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any
 from src.utils.parser import parse_csv
 import src.utils.helpers as helpers
 import src.utils.globs as globs
 import src.utils.execute as execute
 
 
-def run(prog_path: str, **kwargs) -> dict[str, Any]:
+def run(prog_path: str, **kwargs) -> None:
     r"""Run given .csv program.
 
     :param prog_path:
         .csv file in SAPsim format.
     :type prog_path: ``str``
     :param \**kwargs:
         See below
@@ -86,8 +86,37 @@
         print("Program halted.")
     else:
         execute.execute_full_speed()
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Program halted.")
 
+
+def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
+    r"""Run given .csv program and return final state. Just a wrapper around run() that's used for autograding.
+
+    The rest of the docstring is identical to that of run().
+
+    :param prog_path:
+        .csv file in SAPsim format.
+    :type prog_path: ``str``
+    :param \**kwargs:
+        See below
+
+    :Keyword Arguments:
+        * *debug* (``bool``) --
+            * Whether to run in debug mode (True) or at full speed (False)
+        * *change* (``str``) --
+            * Comma-separated list of changes to RAM
+            * Useful for debugging programs (edit a value without changing CSV)
+            * Also useful for autograding programs (overwrite a reserved instruction/data value)
+            * Format: <addr>:<base-10 value>,<addr>:<base-10 value>, ...
+        * *format* (``str``) --
+            * Table format
+            * Options: https://github.com/astanin/python-tabulate#table-format
+        * *bits* (``int``) --
+            * Number of bits in unsigned registers
+    :return: ``dict`` containing all final values in globs.py, used for autograding
+    :rtype: ``dict``
+    """
+    run(prog_path, **kwargs)
     return helpers.get_state()
```

### Comparing `SAPsim-0.0.1/src/SAPsim.egg-info/PKG-INFO` & `SAPsim-0.0.2/src/SAPsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/sapsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
```

### Comparing `SAPsim-0.0.1/src/SAPsim.egg-info/SOURCES.txt` & `SAPsim-0.0.2/src/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/exceptions.py` & `SAPsim-0.0.2/src/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/execute.py` & `SAPsim-0.0.2/src/utils/execute.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/globs.py` & `SAPsim-0.0.2/src/utils/globs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/helpers.py` & `SAPsim-0.0.2/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/instructions.py` & `SAPsim-0.0.2/src/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/src/utils/parser.py` & `SAPsim-0.0.2/src/utils/parser.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/tests/test_example_progs.py` & `SAPsim-0.0.2/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/tests/test_exceptions.py` & `SAPsim-0.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/tests/test_helpers.py` & `SAPsim-0.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.1/tests/test_instructions.py` & `SAPsim-0.0.2/tests/test_instructions.py`

 * *Files identical despite different names*

