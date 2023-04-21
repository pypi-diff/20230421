# Comparing `tmp/byu_pytest_utils-0.5.3.tar.gz` & `tmp/byu_pytest_utils-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.5.3.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.6.0.tar", max compression
```

## Comparing `byu_pytest_utils-0.5.3.tar` & `byu_pytest_utils-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-03-04 23:37:17.850707 byu_pytest_utils-0.5.3/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0      714 2022-03-14 21:00:52.263812 byu_pytest_utils-0.5.3/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0     8150 2023-03-04 23:37:17.851768 byu_pytest_utils-0.5.3/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.5.3/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0    10828 2023-03-04 23:37:17.854014 byu_pytest_utils-0.5.3/byu_pytest_utils/io_checker.py
--rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.5.3/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3428 2023-03-04 23:37:17.857403 byu_pytest_utils-0.5.3/byu_pytest_utils/test_utils.py
--rw-r--r--   0        0        0      562 2023-03-06 23:45:28.525003 byu_pytest_utils-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      784 2023-03-06 23:45:55.576367 byu_pytest_utils-0.5.3/setup.py
--rw-r--r--   0        0        0      550 2023-03-06 23:45:55.576642 byu_pytest_utils-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 21:42:09.303677 byu_pytest_utils-0.6.0/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0      714 2022-03-14 21:00:52.263812 byu_pytest_utils-0.6.0/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0     9871 2023-04-21 21:40:40.002962 byu_pytest_utils-0.6.0/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3088 2023-03-04 23:37:17.852701 byu_pytest_utils-0.6.0/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3595 2023-03-06 23:42:26.126776 byu_pytest_utils-0.6.0/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.6.0/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2023-04-21 21:37:59.023625 byu_pytest_utils-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.6.0/PKG-INFO
```

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import inspect
 from pathlib import Path
 import pytest
 
 pytest.register_assert_rewrite("byu_pytest_utils.io_checker")
 pytest.register_assert_rewrite("byu_pytest_utils.dialog")
 
-from .test_utils import compare_files, run_python, with_import
+from .utils import run_python_script, with_import, ensure_missing
 from .decorators import max_score, visibility, tags
-from .io_checker import check_io
 from .dialog import dialog
 
 # Type stubs to make these variables discoverable
 # Actual values are supplied by __getattr__
 this_folder: Path
 test_files: Path
```

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/dialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-import math
+import argparse
 import re
 import runpy
 import sys
 import traceback
 from functools import wraps
+from pathlib import Path
 
 from byu_pytest_utils.edit_dist import edit_dist
 
 
-def dialog(dialog_file, script, *script_args):
-    checker = DialogChecker(dialog_file, echo_output=True)
+def dialog(dialog_file, script, *script_args, output_file=None):
     try:
-        group_stats = checker.run_script(script, *script_args)
+        # Ensure the output file isn't leftover from a previous run
+        if output_file is not None:
+            if isinstance(output_file, str):
+                output_file = Path(output_file)
+            output_file.unlink(missing_ok=True)
+
+        # Run the script
+        group_stats = DialogChecker(dialog_file, echo_output=True) \
+            .run_script(script, *script_args, output_file=output_file)
 
     except Exception as ex:
         group_stats = {
+            'load-tests': {
                 'group_name': 'load-tests',
                 'expected': '',
                 'observed': traceback.format_exc(),
                 'score': 0,
                 'max_score': 1,
                 'passed': False,
             }
+        }
 
     def decorator(func):
-        # func should have empty (pass) body
-        @wraps(func)
+        # func should have empty (pass) body and no arguments
         def new_func(group_name):
             group_stat = group_stats[group_name]
             if not group_stat['passed']:
                 assert group_stat['observed'] == group_stat['expected']
 
         new_func._group_stats = group_stats
         return new_func
@@ -103,17 +112,17 @@
         group_weights[DialogChecker.DEFAULT_GROUP] = 100 - total
 
         # Then remove the groups from the dialog contents
         dialog_contents = re.sub(r'``(.*?);(.+?);(\d+?)``', r'\1', dialog_contents, flags=re.DOTALL)
 
         return group_weights, group_names, group_sequence, dialog_contents
 
-    def _score_output(self):
+    def _score_output(self, observed_output):
         _, obs, exp = edit_dist(
-            self.observed_output,
+            observed_output,
             self.expected_output,
             GAP=DialogChecker.GAP
         )
 
         # insert gaps (i.e. DEFAULT_GROUP) into self.groups to match exp
         # then iterate over obs, exp, and groups
         # to compute rate of matches per group
@@ -194,15 +203,15 @@
     @wraps(print)
     def _print(self, *values, **kwargs):
         sep = kwargs.get('sep', ' ')
         end = kwargs.get('end', '\n')
         res = sep.join(str(t) for t in values) + end
         self._consume_output(res)
 
-    def run_script(self, script_name, *args, module='__main__'):
+    def run_script(self, script_name, *args, output_file=None, module='__main__'):
         # Intercept input, print, and sys.argv
         sys.argv = [script_name, *(str(a) for a in args)]
         _globals = {
             'input': self._input,
             'print': self._print,
             'sys': sys
         }
@@ -213,10 +222,50 @@
 
         except Exception as ex:
             # get stack trace as string
             self._consume_output(f'\nException: {ex}\n')
             self._consume_output(traceback.format_exc())
 
         # Final assertion of observed and expected output
-        group_stats = self._score_output()
+        if output_file is not None:
+            with open(output_file) as output:
+                group_stats = self._score_output(output.read())
+        else:
+            group_stats = self._score_output(self.observed_output)
 
         return group_stats
+
+
+def record_script(dialog_file, script_name, *script_args):
+    # Intercept input, print, and sys.argv
+    sys.argv = [script_name, *(str(a) for a in script_args)]
+    with open(dialog_file, 'w') as file:
+        def _input(prompt):
+            file.write(prompt)
+            response = input(prompt)
+            file.write(f'<<{response}>>\n')
+            return response
+
+        def _print(*args, **kwargs):
+            print(*args, **kwargs)
+            print(*args, **kwargs, file=file)
+
+        _globals = {
+            'input': _input,
+            'print': _print,
+            'sys': sys
+        }
+
+        # Run script as __main__
+        result = runpy.run_path(script_name, _globals, '__main__')
+
+    return result
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('dialog_file', help='Dialog file to write')
+    parser.add_argument('python_script', help='Python script to run')
+    parser.add_argument('script_args', nargs='*', help='Arguments to the python script (if any)')
+    args = parser.parse_args()
+
+    record_script(args.dialog_file, args.python_script, *args.script_args)
```

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.5.3/byu_pytest_utils/test_utils.py` & `byu_pytest_utils-0.6.0/byu_pytest_utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 import importlib
 import os.path
-import subprocess
+import runpy
 from functools import wraps
 from pathlib import Path
 import inspect
+from typing import Union
+
 import pytest
 import sys
 
 
-def compare_files(file_1, file_2):
-    with open(file_1) as f1:
-        with open(file_2) as f2:
-            expected = f1.read().strip()
-            observed = f2.read().strip()
-            assert observed == expected
-
-
-def run_python(*command, stdin=None):
-    for token in command:
-        missing = None
-        if isinstance(token, str) and token.endswith('.py') and not os.path.exists(token):
-            missing = os.path.basename(token)
-        elif isinstance(token, Path) and token.name.endswith('.py') and not token.exists():
-            missing = token.name
-
-        if missing:
-            print(f'Missing: {token}')
-            pytest.fail(f'The file {missing} does not exist. Did you submit it?')
-
-    input_bytes = stdin.encode() if stdin else None
-
-    _command = [sys.executable]
-    _command.extend((str(c) for c in command))
-    proc = subprocess.run(_command, input=input_bytes, capture_output=True)
-    if proc.returncode != 0:
-        pytest.fail(f'The command {" ".join(_command)} failed with exit code {proc.returncode}. '
-                    f'{proc.stderr.decode()}')
-    return proc.stdout.decode().replace('\r','')
+def run_python_script(script, *args, module='__main__'):
+    """
+    Run the python script with arguments
+
+    If the script expects STDIN, use the dialog framework instead
+
+    :param script: Python script to run
+    :param args: Arguments to the python script
+    :param module: Defaults to '__main__'
+    :return: Namespace as a result of running the script
+    """
+    if not os.path.exists(script):
+        pytest.fail(f'The file {script} does not exist. Did you submit it?')
+
+    def _input(*args):
+        raise Exception("input function not supported for this test")
+
+    sys.argv = [script, *(str(a) for a in args)]
+    _globals = {
+        'sys': sys,
+        'input': _input
+    }
+    return runpy.run_path(script, _globals, module)
+
+
+def ensure_missing(file: Union[Path, str]):
+    """
+    Use the decorator to ensure the provided file is always missing
+    when the test starts
+    """
+    if isinstance(file, str):
+        file = Path(file)
+    def decorator(func):
+        @wraps(func)
+        def new_func(*args, **kwargs):
+            file.unlink(missing_ok=True)
+            return func(*args, **kwargs)
+
+        return new_func
+
+    return decorator
 
 
 def with_import(module_name=None, function_name=None):
     # Create a decorator
     def decorator(test_function):
         # Import function_name from module_name, then run function
         # with function_name passed in as first arg
```

### Comparing `byu_pytest_utils-0.5.3/pyproject.toml` & `byu_pytest_utils-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.5.3"
+version = "0.6.0"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.5.3/PKG-INFO` & `byu_pytest_utils-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.5.3
+Version: 0.6.0
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.0.1,<8.0.0)
```

