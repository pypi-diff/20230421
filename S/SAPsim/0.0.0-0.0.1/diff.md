# Comparing `tmp/SAPsim-0.0.0.tar.gz` & `tmp/SAPsim-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-0.0.0.tar", last modified: Fri Apr 21 17:51:58 2023, max compression
+gzip compressed data, was "SAPsim-0.0.1.tar", last modified: Fri Apr 21 18:32:41 2023, max compression
```

## Comparing `SAPsim-0.0.0.tar` & `SAPsim-0.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.274736 SAPsim-0.0.0/
--rw-r--r--   0 jesse      (501) staff       (20)     1066 2023-02-23 19:54:52.000000 SAPsim-0.0.0/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)     4051 2023-04-21 17:51:58.274813 SAPsim-0.0.0/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     3100 2023-04-21 17:51:06.000000 SAPsim-0.0.0/README.md
--rw-r--r--   0 jesse      (501) staff       (20)      903 2023-04-21 16:55:41.000000 SAPsim-0.0.0/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)      728 2023-04-21 17:51:58.275103 SAPsim-0.0.0/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)     1492 2023-04-21 17:51:46.000000 SAPsim-0.0.0/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.269265 SAPsim-0.0.0/src/
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.270377 SAPsim-0.0.0/src/SAPsim/
--rw-r--r--   0 jesse      (501) staff       (20)     3383 2023-04-21 17:38:27.000000 SAPsim-0.0.0/src/SAPsim/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.271543 SAPsim-0.0.0/src/SAPsim.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)     4051 2023-04-21 17:51:58.000000 SAPsim-0.0.0/src/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      531 2023-04-21 17:51:58.000000 SAPsim-0.0.0/src/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-21 17:51:58.000000 SAPsim-0.0.0/src/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-02-25 02:12:35.000000 SAPsim-0.0.0/src/SAPsim.egg-info/not-zip-safe
--rw-r--r--   0 jesse      (501) staff       (20)       93 2023-04-21 17:51:58.000000 SAPsim-0.0.0/src/SAPsim.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)       13 2023-04-21 17:51:58.000000 SAPsim-0.0.0/src/SAPsim.egg-info/top_level.txt
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.273280 SAPsim-0.0.0/src/utils/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-03-16 06:39:53.000000 SAPsim-0.0.0/src/utils/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     7460 2023-03-27 00:31:56.000000 SAPsim-0.0.0/src/utils/exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     1704 2023-03-27 00:30:53.000000 SAPsim-0.0.0/src/utils/execute.py
--rw-r--r--   0 jesse      (501) staff       (20)     2078 2023-04-21 17:32:33.000000 SAPsim-0.0.0/src/utils/globs.py
--rw-r--r--   0 jesse      (501) staff       (20)     6729 2023-04-21 17:36:55.000000 SAPsim-0.0.0/src/utils/helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     5861 2023-03-27 00:30:53.000000 SAPsim-0.0.0/src/utils/instructions.py
--rw-r--r--   0 jesse      (501) staff       (20)     5046 2023-04-21 16:44:05.000000 SAPsim-0.0.0/src/utils/parser.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 17:51:58.274496 SAPsim-0.0.0/tests/
--rw-r--r--   0 jesse      (501) staff       (20)     2981 2023-03-22 18:52:46.000000 SAPsim-0.0.0/tests/test_example_progs.py
--rw-r--r--   0 jesse      (501) staff       (20)      688 2023-03-27 00:28:37.000000 SAPsim-0.0.0/tests/test_exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     1336 2023-03-27 00:28:37.000000 SAPsim-0.0.0/tests/test_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     4783 2023-03-27 00:28:31.000000 SAPsim-0.0.0/tests/test_instructions.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.480839 SAPsim-0.0.1/
+-rw-r--r--   0 jesse      (501) staff       (20)     1066 2023-02-23 19:54:52.000000 SAPsim-0.0.1/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)     1252 2023-04-21 18:32:41.480945 SAPsim-0.0.1/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     3098 2023-04-21 18:22:40.000000 SAPsim-0.0.1/README.md
+-rw-r--r--   0 jesse      (501) staff       (20)      301 2023-04-21 18:01:43.000000 SAPsim-0.0.1/README_PyPI.md
+-rw-r--r--   0 jesse      (501) staff       (20)      908 2023-04-21 17:59:42.000000 SAPsim-0.0.1/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)      728 2023-04-21 18:32:41.481255 SAPsim-0.0.1/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)     1492 2023-04-21 18:00:02.000000 SAPsim-0.0.1/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.474648 SAPsim-0.0.1/src/
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.476081 SAPsim-0.0.1/src/SAPsim/
+-rw-r--r--   0 jesse      (501) staff       (20)     3547 2023-04-21 18:11:33.000000 SAPsim-0.0.1/src/SAPsim/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.477221 SAPsim-0.0.1/src/SAPsim.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)     1252 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      546 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-02-25 02:12:35.000000 SAPsim-0.0.1/src/SAPsim.egg-info/not-zip-safe
+-rw-r--r--   0 jesse      (501) staff       (20)       93 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       13 2023-04-21 18:32:41.000000 SAPsim-0.0.1/src/SAPsim.egg-info/top_level.txt
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.479302 SAPsim-0.0.1/src/utils/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-03-16 06:39:53.000000 SAPsim-0.0.1/src/utils/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     7460 2023-03-27 00:31:56.000000 SAPsim-0.0.1/src/utils/exceptions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1704 2023-03-27 00:30:53.000000 SAPsim-0.0.1/src/utils/execute.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2078 2023-04-21 17:32:33.000000 SAPsim-0.0.1/src/utils/globs.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6729 2023-04-21 17:36:55.000000 SAPsim-0.0.1/src/utils/helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5861 2023-03-27 00:30:53.000000 SAPsim-0.0.1/src/utils/instructions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3702 2023-04-21 18:11:33.000000 SAPsim-0.0.1/src/utils/parser.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-21 18:32:41.480600 SAPsim-0.0.1/tests/
+-rw-r--r--   0 jesse      (501) staff       (20)     3021 2023-04-21 18:21:50.000000 SAPsim-0.0.1/tests/test_example_progs.py
+-rw-r--r--   0 jesse      (501) staff       (20)      689 2023-04-21 18:21:50.000000 SAPsim-0.0.1/tests/test_exceptions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1336 2023-03-27 00:28:37.000000 SAPsim-0.0.1/tests/test_helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4783 2023-03-27 00:28:31.000000 SAPsim-0.0.1/tests/test_instructions.py
```

### Comparing `SAPsim-0.0.0/LICENSE` & `SAPsim-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/PKG-INFO` & `SAPsim-0.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,22 @@
-Metadata-Version: 2.1
-Name: SAPsim
-Version: 0.0.0
-Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
-Home-page: https://github.com/jesse-wei/sapsim
-Download-URL: https://github.com/jesse-wei/SAPsim/releases
-Author: Jesse Wei
-Author-email: Jesse Wei <jesse@cs.unc.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
-Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
-Keywords: SAP,SAPsim,UNC,COMP311
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 ![Tests](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 
 # SAPsim
 
 > Simulation of [SAP (Simple As Possible) computer](img/SAP.png) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
 
 ## How to program
 
 Write a SAP program in the format given in [`template.csv`](template.csv). Also see [`example.csv`](tests/public_prog/example.csv) ([output full speed](tests/data/public_prog/example_full_speed.txt)) ([output debug mode](tests/data/public_prog/example_debug.txt)).
 
-You may edit the `.csv` files in Microsoft Excel. Pass the path to your SAP program as a CLI argument. It'll then be run in debug mode (default). Alternatively, apply the `-s` option to run at full <ins>s</ins>peed.
+You may edit the `.csv` files in Microsoft Excel. You will pass the path to your SAP program as an argument. It'll then be run at full speed (default). There is also a debug (step) mode, explained [below](#usage).
 
 ## Install
 
-Your Python version needs to be 3.7+. Check with `python --version`. If you normally use `python3`, then use that.
+Your Python version needs to be 3.9+. Check with `python --version`. If you normally use `python3`, then use that.
 
 Next, install SAPsim.
 
 ```sh
 pip install SAPsim
 ```
```

### Comparing `SAPsim-0.0.0/pyproject.toml` & `SAPsim-0.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "SAPsim"
 authors = [
     { name="Jesse Wei", email="jesse@cs.unc.edu" },
 ]
 description = "Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC"
-readme = "README.md"
+readme = "README_PyPI.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `SAPsim-0.0.0/setup.cfg` & `SAPsim-0.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/setup.py` & `SAPsim-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Version number that appears on PyPI and Test PyPI
-    version="0.0.0",
+    version="0.0.1",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/sapsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
```

### Comparing `SAPsim-0.0.0/src/SAPsim/__init__.py` & `SAPsim-0.0.1/src/SAPsim/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,55 +30,64 @@
             * Options: https://github.com/astanin/python-tabulate#table-format
         * *bits* (``int``) --
             * Number of bits in unsigned registers
     :return: ``dict`` containing all final values in globs.py, used for autograding
     :rtype: ``dict``
     """
     path: Path = Path(prog_path)
-    assert path.suffix == '.csv'
+    assert path.suffix == ".csv"
     helpers.setup_8bit()
     parse_csv(path)
     if "bits" in kwargs:
         assert int(kwargs["bits"]) > 1
         globs.NUM_BITS_IN_REGISTERS = int(kwargs["bits"])
-        globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2 ** globs.NUM_BITS_IN_REGISTERS - 1
+        globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**globs.NUM_BITS_IN_REGISTERS - 1
     if "change" in kwargs:
-        changes = kwargs["change"].split(',')
+        changes = kwargs["change"].split(",")
         for change in changes:
-            if change.count(':') != 1:
-                print("Invalid syntax for --c option, correct format is <addr>:<base-10 value>,<addr>:<base-10 value>, ...")
+            if change.count(":") != 1:
+                print(
+                    "Invalid syntax for --c option, correct format is <addr>:<base-10 value>,<addr>:<base-10 value>, ..."
+                )
                 exit(1)
-            colon_position = change.find(':')
+            colon_position = change.find(":")
             addr = int(change[:colon_position])
             if addr not in globs.RAM:
-                print(f"You can apply a change only to an address that's already mapped (not skipped). Address {addr} is not mapped.")
+                print(
+                    f"You can apply a change only to an address that's already mapped (not skipped). Address {addr} is not mapped."
+                )
                 exit(1)
-            value = int(change[colon_position+1:])
+            value = int(change[colon_position + 1 :])
             if value < 0 or value > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
-                print(f"Invalid base-10 value for change: {value}. Negative or overflows registers.")
+                print(
+                    f"Invalid base-10 value for change: {value}. Negative or overflows registers."
+                )
                 exit(1)
             globs.RAM[addr] = value
     if "format" in kwargs:
         globs.table_fmt = kwargs["format"]
     if "debug" in kwargs and kwargs["debug"]:
         print("Initial state of simulation.")
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Debug mode: press Enter to execute next instruction ( > ).")
         input()
         while globs.EXECUTING:
             # Special case so that you don't have to press Enter twice to halt on a HLT instruction
-            if globs.PC in globs.RAM and helpers.parse_opcode(globs.RAM[globs.PC]) == 0xF:
+            if (
+                globs.PC in globs.RAM
+                and helpers.parse_opcode(globs.RAM[globs.PC]) == 0xF
+            ):
                 execute.execute_next()
                 break
             execute.execute_next()
             helpers.print_RAM(dispPC=True)
             helpers.print_info()
             input()
         print("Program halted.")
     else:
         execute.execute_full_speed()
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Program halted.")
 
-    return helpers.get_state()
+    return helpers.get_state()
```

### Comparing `SAPsim-0.0.0/src/SAPsim.egg-info/SOURCES.txt` & `SAPsim-0.0.1/src/SAPsim.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+README_PyPI.md
 pyproject.toml
 setup.cfg
 setup.py
 src/SAPsim/__init__.py
 src/SAPsim.egg-info/PKG-INFO
 src/SAPsim.egg-info/SOURCES.txt
 src/SAPsim.egg-info/dependency_links.txt
```

### Comparing `SAPsim-0.0.0/src/utils/exceptions.py` & `SAPsim-0.0.1/src/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/src/utils/execute.py` & `SAPsim-0.0.1/src/utils/execute.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/src/utils/globs.py` & `SAPsim-0.0.1/src/utils/globs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/src/utils/helpers.py` & `SAPsim-0.0.1/src/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/src/utils/instructions.py` & `SAPsim-0.0.1/src/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/tests/test_example_progs.py` & `SAPsim-0.0.1/tests/test_example_progs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Test example programs.
-This code is the same as the code that autogrades Lab 4.
+This code should be the same (or mostly the same, in case it's updated) as the code that autogrades Lab 4.
 If you have any questions about RESERVED/RETURN VALUE, they can be answered by reading through this.
 If you don't know the test cases your program is failing, you can very easily write a function to check it yourself. It'd probably be exactly the same as what I wrote.
 """
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
-import src.utils.global_vars as globs
+import src.utils.globs as globs
 from src.utils import parser
 from src.utils.execute import execute_full_speed
 from src.utils.helpers import setup_8bit
 
 
 def clone_dict(dict):
     """Returns a deep clone of `dict`. Used to clone `RAM`."""
@@ -24,15 +24,15 @@
     """Test ex1.csv.
     RESERVED:
         14: Input 0 to 255
     RETURN VALUE:
         15: 1 if x == 3 else 0
     """
     setup_8bit()
-    parser.parse_csv('tests/public_prog/ex1.csv')
+    parser.parse_csv("tests/public_prog/ex1.csv")
     # Clone student's program
     ram_copy = clone_dict(globs.RAM)
     for num in range(256):
         setup_8bit()
         globs.RAM = clone_dict(ram_copy)
         # Overwrite RESERVED address with test input
         globs.RAM[14] = num
@@ -55,31 +55,33 @@
     """Test ex2.csv.
     RESERVED:
         15: Input 0 to 255
     RETURN VALUE:
         Register A: See ex2_rv() function
     """
     setup_8bit()
-    parser.parse_csv('tests/public_prog/ex2.csv')
+    parser.parse_csv("tests/public_prog/ex2.csv")
     # Clone student's program
     ram_copy = clone_dict(globs.RAM)
     for num in range(256):
         setup_8bit()
         globs.RAM = clone_dict(ram_copy)
         # Overwrite RESERVED address with test input
         globs.RAM[15] = num
         try:
             execute_full_speed()
         except Exception:
             # Note when an Exception occurs, the rest of the tests don't run. The break is for performance reasons.
             break
         # The autograder has a tests_passed variable and adds 1 to it if the RETURN VALUE is correct
         assert ex2_rv(num) == globs.A
-        
+
     # score = tests_passed / total_tests
 
+
 def ex2_rv(X):
     """Helper function for testing ex2.csv. Just the example pseudocode to be replicated.
-    Can make it not use a loop and instead use an if < 16 and then a mod operation but I don't have time for that."""
+    Can make it not use a loop and instead use an if < 16 and then a mod operation but I don't have time for that.
+    """
     while X >= 31:
-        X = X - 3;
-    return X;
+        X = X - 3
+    return X
```

### Comparing `SAPsim-0.0.0/tests/test_exceptions.py` & `SAPsim-0.0.1/tests/test_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from src.utils.execute import execute_full_speed, execute_next
 from src.utils.helpers import check_state, check_state_all, print_RAM, print_info
 from src.utils.exceptions import *
 from src.utils.helpers import setup_4bit, setup_8bit, reset_globals
 from src.utils import parser
 import pytest
 
+
 def test_16MappedAddresses():
     setup_8bit()
-    parser.parse_csv('tests/malformed_csv/16_mapped_addresses.csv')
+    parser.parse_csv("tests/malformed_csv/16_mapped_addresses.csv")
+
 
-def test_17MappedAddresses():
+def test_19MappedAddresses():
     setup_8bit()
     with pytest.raises(MoreThan16MappedAddresses):
-        parser.parse_csv('tests/malformed_csv/17_mapped_addresses.csv')
-
+        parser.parse_csv("tests/malformed_csv/19_mapped_addresses.csv")
```

### Comparing `SAPsim-0.0.0/tests/test_helpers.py` & `SAPsim-0.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-0.0.0/tests/test_instructions.py` & `SAPsim-0.0.1/tests/test_instructions.py`

 * *Files identical despite different names*

