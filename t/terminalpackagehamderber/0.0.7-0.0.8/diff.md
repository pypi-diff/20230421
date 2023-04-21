# Comparing `tmp/terminalpackagehamderber-0.0.7.tar.gz` & `tmp/terminalpackagehamderber-0.0.8.tar.gz`

## Comparing `terminalpackagehamderber-0.0.7.tar` & `terminalpackagehamderber-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/.gitattributes
--rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/run.cmd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/terminalpackagehamderber/__init__.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/terminalpackagehamderber/command_handler.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/terminalpackagehamderber/terminal.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/terminalpackagehamderber/terminal_settings.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/LICENSE
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/README.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/.gitattributes
+-rwxr-xr-x   0        0        0       49 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/run.cmd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/terminalpackagehamderber/__init__.py
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/terminalpackagehamderber/command_handler.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/terminalpackagehamderber/terminal.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/terminalpackagehamderber/terminal_settings.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/LICENSE
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 terminalpackagehamderber-0.0.8/PKG-INFO
```

### Comparing `terminalpackagehamderber-0.0.7/terminalpackagehamderber/command_handler.py` & `terminalpackagehamderber-0.0.8/terminalpackagehamderber/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def get_user_input(input_prompt="Default prompt: "):
     """
     Takes the user's input and drops it to lowercase and submits it to the command parser
     :param input_prompt:
     """
-    user_input = str.lower(input(input_prompt))
+    user_input = input(input_prompt)
     command_parser(user_input)
 
 
 def run_command(text, args=None):
     try:
         command_dict[str.lower(text)].command(args)
     except KeyError:
```

### Comparing `terminalpackagehamderber-0.0.7/terminalpackagehamderber/terminal.py` & `terminalpackagehamderber-0.0.8/terminalpackagehamderber/terminal.py`

 * *Files identical despite different names*

### Comparing `terminalpackagehamderber-0.0.7/.gitignore` & `terminalpackagehamderber-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `terminalpackagehamderber-0.0.7/LICENSE` & `terminalpackagehamderber-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalpackagehamderber-0.0.7/pyproject.toml` & `terminalpackagehamderber-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "terminalpackagehamderber"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Hamderber", email="hamderber@gmail.com" },
 ]
 description = "Terminal package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `terminalpackagehamderber-0.0.7/PKG-INFO` & `terminalpackagehamderber-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: terminalpackagehamderber
-Version: 0.0.7
+Version: 0.0.8
 Summary: Terminal package
 Project-URL: Homepage, https://github.com/Hamderber/TerminalPackageHamderber
 Project-URL: Bug Tracker, https://github.com/Hamderber/TerminalPackageHamderber/issues
 Author-email: Hamderber <hamderber@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# KevTerminal
+# TerminalPackageHamderber
 
 How to add custom commands:
 
 Define a function that has an args parameter with its default as None.
 ex:
     def testcmd(args=None):
         print("test worked")
```

