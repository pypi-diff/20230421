# Comparing `tmp/catprompt-0.0.3.tar.gz` & `tmp/catprompt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.0.3.tar", last modified: Sat Apr 15 14:52:44 2023, max compression
+gzip compressed data, was "catprompt-0.0.4.tar", last modified: Fri Apr 21 11:04:04 2023, max compression
```

## Comparing `catprompt-0.0.3.tar` & `catprompt-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.154076 catprompt-0.0.3/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.0.3/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-15 14:52:44.153770 catprompt-0.0.3/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     4141 2023-04-15 09:03:27.000000 catprompt-0.0.3/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.149858 catprompt-0.0.3/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.0.3/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     1967 2023-04-15 14:46:38.000000 catprompt-0.0.3/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.152243 catprompt-0.0.3/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-15 14:52:44.000000 catprompt-0.0.3/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-15 14:51:03.000000 catprompt-0.0.3/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-15 14:52:44.154163 catprompt-0.0.3/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.0.3/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-15 14:52:44.152766 catprompt-0.0.3/test/
--rw-r--r--   0 juanre     (501) staff       (20)     1458 2023-04-15 09:03:27.000000 catprompt-0.0.3/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857942 catprompt-0.0.4/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-15 09:03:27.000000 catprompt-0.0.4/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     6136 2023-04-21 11:04:04.857839 catprompt-0.0.4/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     4509 2023-04-21 10:59:07.000000 catprompt-0.0.4/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.856885 catprompt-0.0.4/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-15 09:03:27.000000 catprompt-0.0.4/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     2601 2023-04-21 11:00:22.000000 catprompt-0.0.4/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857579 catprompt-0.0.4/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     6136 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-21 11:04:04.000000 catprompt-0.0.4/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      832 2023-04-21 11:02:41.000000 catprompt-0.0.4/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-21 11:04:04.857978 catprompt-0.0.4/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-15 09:03:27.000000 catprompt-0.0.4/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-21 11:04:04.857698 catprompt-0.0.4/test/
+-rw-r--r--   0 juanre     (501) staff       (20)     2230 2023-04-21 10:50:54.000000 catprompt-0.0.4/test/test_prompter.py
```

### Comparing `catprompt-0.0.3/LICENSE` & `catprompt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.3/PKG-INFO` & `catprompt-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -70,28 +70,29 @@
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
+- Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
 
 ### Example
 
 Let's consider the following example with three files:
 
 **main_prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
 += sub_prompt_1.txt
-+= code_snippet.py
++- code_snippet.py The snippet of code
 
 This is the end of the main prompt.
 ```
 
 **sub_prompt_1.txt**
 
 ```
@@ -111,16 +112,19 @@
 ```
 
 When running `catprompt main_prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
+The snippet of code follows delimited by +-----
++-----
 def example_function():
     return "This is an example code snippet."
++-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
 
@@ -128,15 +132,15 @@
 - Including code snippets in your prompts;
 - Organizing prompt files as part of a project;
 - Using prompt files as the seed for documentation.
 
 ## Developing
 
 ```
-mkdir ~/venv/catp && python3.9 -m venv ~/venv/catp
+mkdir ~/venv/catp && python -m venv ~/venv/catp
 source ~/venv/catp/bin/activate
 pip install --upgrade pip
 pip install -e .
 pip install ".[dev]"
 ```
 
 ## Author
```

### Comparing `catprompt-0.0.3/README.md` & `catprompt-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,28 +37,29 @@
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
+- Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
 
 ### Example
 
 Let's consider the following example with three files:
 
 **main_prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
 += sub_prompt_1.txt
-+= code_snippet.py
++- code_snippet.py The snippet of code
 
 This is the end of the main prompt.
 ```
 
 **sub_prompt_1.txt**
 
 ```
@@ -78,16 +79,19 @@
 ```
 
 When running `catprompt main_prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
+The snippet of code follows delimited by +-----
++-----
 def example_function():
     return "This is an example code snippet."
++-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
 
@@ -95,15 +99,15 @@
 - Including code snippets in your prompts;
 - Organizing prompt files as part of a project;
 - Using prompt files as the seed for documentation.
 
 ## Developing
 
 ```
-mkdir ~/venv/catp && python3.9 -m venv ~/venv/catp
+mkdir ~/venv/catp && python -m venv ~/venv/catp
 source ~/venv/catp/bin/activate
 pip install --upgrade pip
 pip install -e .
 pip install ".[dev]"
 ```
 
 ## Author
```

### Comparing `catprompt-0.0.3/catprompt/prompter.py` & `catprompt-0.0.4/catprompt/prompter.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,40 @@
 import tiktoken
 
 
 # pylint: disable=inconsistent-return-statements
 def process_line(line, base_dir, processed_lines):
     if line.startswith('++'):
         return
-
     if line.startswith('+='):
         file_to_include = line[2:].strip()
         file_path = base_dir / file_to_include
         if not file_path.is_file():
             file_path = Path(file_to_include)
         if file_path.is_file():
             print(f'Including {str(file_path)}')
             process_file(file_path, processed_lines)
         else:
             raise RuntimeError(f'Cannot find {file_to_include}')
+    elif line.startswith('+-'):
+        file_to_include, description = line[2:].strip().split(maxsplit=1)
+        file_path = base_dir / file_to_include
+        if not file_path.is_file():
+            file_path = Path(file_to_include)
+        if file_path.is_file():
+            with file_path.open(encoding='utf-8') as f:
+                content = f.read().strip()
+            processed_lines.extend([
+                f"{description} follows delimited by +-----",
+                "+-----",
+                content,
+                "+-----"
+            ])
+        else:
+            raise RuntimeError(f'Cannot find {file_to_include}')
     elif line.startswith('+#'):
         return False
     else:
         processed_lines.append(line)
 
 
 def process_file(file_path, processed_lines=None):
```

### Comparing `catprompt-0.0.3/catprompt.egg-info/PKG-INFO` & `catprompt-0.0.4/catprompt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -70,28 +70,29 @@
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
 
 ## Prompt file format
 
 - Lines starting with `++` are ignored
 - Lines starting with `+=` should be followed by the name of a file to include. The file will be searched for in the directory of the original file, or in the working directory if not found there. The named file will be read, processed, and its content will replace the current line.
+- Lines starting with `+-` should be followed by the name of a file to include, and a description. The file will processed as above, and its content prefaced by a line saying "[description] follows delimited by +-----" and another line with just +-----, and followed by a line with +-----
 - Lines starting with `+#` will cause the current line and all following lines in the file being processed to be ignored
 
 ### Example
 
 Let's consider the following example with three files:
 
 **main_prompt.txt**
 
 ```
 This is the main prompt.
 
 ++ This is a comment and will be ignored.
 += sub_prompt_1.txt
-+= code_snippet.py
++- code_snippet.py The snippet of code
 
 This is the end of the main prompt.
 ```
 
 **sub_prompt_1.txt**
 
 ```
@@ -111,16 +112,19 @@
 ```
 
 When running `catprompt main_prompt.txt`, the processed content will be:
 
 ```
 This is the main prompt.
 This is the sub-prompt 1.
+The snippet of code follows delimited by +-----
++-----
 def example_function():
     return "This is an example code snippet."
++-----
 This is the end of the main prompt.
 ```
 
 This processed content will be copied to your clipboard, ready for use with ChatGPT.
 
 ## Use cases
 
@@ -128,15 +132,15 @@
 - Including code snippets in your prompts;
 - Organizing prompt files as part of a project;
 - Using prompt files as the seed for documentation.
 
 ## Developing
 
 ```
-mkdir ~/venv/catp && python3.9 -m venv ~/venv/catp
+mkdir ~/venv/catp && python -m venv ~/venv/catp
 source ~/venv/catp/bin/activate
 pip install --upgrade pip
 pip install -e .
 pip install ".[dev]"
 ```
 
 ## Author
```

### Comparing `catprompt-0.0.3/pyproject.toml` & `catprompt-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.0.3"
+version = "0.0.4"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
```

### Comparing `catprompt-0.0.3/test/test_prompter.py` & `catprompt-0.0.4/test/test_prompter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os
 from pathlib import Path
 from catprompt.prompter import process_and_copy_to_clipboard
 import clipboard
 
 
 def test_process_file():
     # Prepare test data
     test_data_dir = Path(__file__).parent / "data"
     input_file = test_data_dir / "input.txt"
-    expected_output_file = test_data_dir / "expected_output.txt"
+    expected_output_file = test_data_dir / "expected-output.txt"
 
     # Run process_file
     processed_content = process_and_copy_to_clipboard(input_file)
 
     # Compare the processed content with the expected output
     with expected_output_file.open() as f:
         expected_output = f.read().rstrip()
@@ -22,21 +21,42 @@
     clipboard_content = clipboard.paste()
     assert processed_content == clipboard_content
 
 
 def test_process_file_with_stop():
     # Prepare test data
     test_data_dir = Path(__file__).parent / "data"
-    input_file = test_data_dir / "input_with_stop.txt"
-    expected_output_file = test_data_dir / "expected_output_with_stop.txt"
+    input_file = test_data_dir / "input-with-stop.txt"
+    expected_output_file = test_data_dir / "expected-output-with-stop.txt"
 
     # Run process_and_copy_to_clipboard
     processed_content = process_and_copy_to_clipboard(input_file)
 
     # Compare the processed content with the expected output
     with expected_output_file.open() as f:
         expected_output = f.read().rstrip()
     assert processed_content == expected_output
 
     # Check if processed content was copied to clipboard
     clipboard_content = clipboard.paste()
     assert processed_content == clipboard_content
+
+
+def test_process_file_with_inline_content():
+    # Prepare test data
+    test_data_dir = Path(__file__).parent / "data"
+    input_file = test_data_dir / "input-with-inline-content.txt"
+    expected_output_file = test_data_dir / "expected-output-with-inline-content.txt"
+
+    # Run process_and_copy_to_clipboard
+    processed_content = process_and_copy_to_clipboard(input_file)
+
+    # Compare the processed content with the expected output
+    with expected_output_file.open() as f:
+        expected_output = f.read().rstrip()
+    print(processed_content)
+    print(expected_output)
+    assert processed_content == expected_output
+
+    # Check if processed content was copied to clipboard
+    clipboard_content = clipboard.paste()
+    assert processed_content == clipboard_content
```

