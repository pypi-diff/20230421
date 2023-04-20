# Comparing `tmp/charmr-1.0.6.tar.gz` & `tmp/charmr-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmr-1.0.6.tar", last modified: Wed Apr 19 03:10:30 2023, max compression
+gzip compressed data, was "charmr-1.0.7.tar", last modified: Thu Apr 20 22:04:32 2023, max compression
```

## Comparing `charmr-1.0.6.tar` & `charmr-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.479851 charmr-1.0.6/
--rw-r--r--   0 ronharlev   (501) staff       (20)     3952 2023-04-19 03:10:30.479510 charmr-1.0.6/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)     3694 2023-04-19 02:57:00.000000 charmr-1.0.6/README.md
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.476264 charmr-1.0.6/charmr/
--rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.6/charmr/__init__.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1455 2023-04-19 02:21:55.000000 charmr-1.0.6/charmr/ai.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.6/charmr/alias_manager.py
--rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.6/charmr/load_code.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     2786 2023-04-19 03:07:10.000000 charmr-1.0.6/charmr/main.py
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.479053 charmr-1.0.6/charmr.egg-info/
--rw-r--r--   0 ronharlev   (501) staff       (20)     3952 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/SOURCES.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/dependency_links.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/entry_points.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/requires.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/top_level.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-19 03:10:30.479943 charmr-1.0.6/setup.cfg
--rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-19 03:10:25.000000 charmr-1.0.6/setup.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.024959 charmr-1.0.7/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-20 22:04:32.024472 charmr-1.0.7/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4259 2023-04-20 21:28:46.000000 charmr-1.0.7/README.md
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.021041 charmr-1.0.7/charmr/
+-rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.7/charmr/__init__.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1523 2023-04-20 21:39:35.000000 charmr-1.0.7/charmr/ai.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.7/charmr/alias_manager.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.7/charmr/load_code.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     2756 2023-04-20 22:01:10.000000 charmr-1.0.7/charmr/main.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.023874 charmr-1.0.7/charmr.egg-info/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/SOURCES.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/dependency_links.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/entry_points.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/requires.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/top_level.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-20 22:04:32.025143 charmr-1.0.7/setup.cfg
+-rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-20 21:58:47.000000 charmr-1.0.7/setup.py
```

### Comparing `charmr-1.0.6/PKG-INFO` & `charmr-1.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmr
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Magical AI File Converter
 Home-page: https://github.com/harlev/charmr
 Author: Ron Harlev
 Author-email: harlev@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -55,15 +55,36 @@
 * Adding an `--alias` will save the conversion in a `.charmr` file.  
 * Then you can specify `--alias` without providing `--conversion` to repeat the same conversion.  
 * Define `--view_code_only` will only print out the code without running it. Use this to review generated code for safety. Specifying `--alias` will save it to be reused.
 * Use `--gpt_4` to use GPT-4 to generate code. Default is `gpt-3.5-turbo`
 * Specify `include_input_rows` with number of rows to include in prompt. This can improve code generation.
 
 e.g. `charmr -i input.csv -o output.json -c "convert csv to json"`  
-OR   `charmr -c "convert csv to json" < input.csv > output.json`
+OR   `charmr -c "convert csv to json" < input.csv > output.json`  
+OR a more fluent use
+```
+cat input.csv | charmr -4 -c "convert the csv to json and keep just the first and third columns" | jq .
+[
+  {
+    "a": "1",
+    "c": "3"
+  },
+  {
+    "a": "4",
+    "c": "6"
+  }
+]
+```  
+Emulating the `cut` utility:  
+`cat input.csv | cut -d"," -f2`  
+Same thing with `charmr`  
+`cat input.csv | charmr -4 -c "read the csv and keep only the second column"`  
+
+Then combining transformation and filtering  
+`cat input.csv | charmr -4 -c "read the csv, remove the header row, keep only the second column and output the square of the values"`
 
 ### Examples
 #### Basic conversion
 input `csv`  
 ```
 a, b, c
 1, 2, 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: charmr Version: 1.0.6 Summary: A Magical AI File
+Metadata-Version: 2.1 Name: charmr Version: 1.0.7 Summary: A Magical AI File
 Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
 Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
 version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 [License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
 pepy.tech/project/charmr) This application will convert, transform, filter etc.
 any text based common file format into another file, based on a text
@@ -22,24 +22,31 @@
 file. * Then you can specify `--alias` without providing `--conversion` to
 repeat the same conversion. * Define `--view_code_only` will only print out the
 code without running it. Use this to review generated code for safety.
 Specifying `--alias` will save it to be reused. * Use `--gpt_4` to use GPT-4 to
 generate code. Default is `gpt-3.5-turbo` * Specify `include_input_rows` with
 number of rows to include in prompt. This can improve code generation. e.g.
 `charmr -i input.csv -o output.json -c "convert csv to json"` OR `charmr -
-c "convert csv to json" < input.csv > output.json` ### Examples #### Basic
-conversion input `csv` ``` a, b, c 1, 2, 3 4, 5, 6 ``` conversion `convert csv
-to json` output `json` ```json [{"a": "1", " b": " 2", " c": " 3"}, {"a": "4",
-" b": " 5", " c": " 6"}] ``` #### Column manipulation input `csv` ``` a, b, c
-1, 2, 3 4, 5, 6 ``` conversion `the input file is a CSV with column headers
-a,b,c. the output file is a CSV. create a new column ac with the multiplication
-of a and c` output `csv` ``` a,b,c,ac 1,2,3,3 4,5,6,24 ``` #### Conversion
-Logic input `csv` ``` day,month,year 11,3,2021 2,8,1999 ``` conversion `input a
-csv file with day,month,year column headers. output a JSON file with an extra
-field which is the unix timestamp for the date represented in each row"` output
+c "convert csv to json" < input.csv > output.json` OR a more fluent use ``` cat
+input.csv | charmr -4 -c "convert the csv to json and keep just the first and
+third columns" | jq . [ { "a": "1", "c": "3" }, { "a": "4", "c": "6" } ] ```
+Emulating the `cut` utility: `cat input.csv | cut -d"," -f2` Same thing with
+`charmr` `cat input.csv | charmr -4 -c "read the csv and keep only the second
+column"` Then combining transformation and filtering `cat input.csv | charmr -
+4 -c "read the csv, remove the header row, keep only the second column and
+output the square of the values"` ### Examples #### Basic conversion input
+`csv` ``` a, b, c 1, 2, 3 4, 5, 6 ``` conversion `convert csv to json` output
+`json` ```json [{"a": "1", " b": " 2", " c": " 3"}, {"a": "4", " b": " 5", "
+c": " 6"}] ``` #### Column manipulation input `csv` ``` a, b, c 1, 2, 3 4, 5, 6
+``` conversion `the input file is a CSV with column headers a,b,c. the output
+file is a CSV. create a new column ac with the multiplication of a and c`
+output `csv` ``` a,b,c,ac 1,2,3,3 4,5,6,24 ``` #### Conversion Logic input
+`csv` ``` day,month,year 11,3,2021 2,8,1999 ``` conversion `input a csv file
+with day,month,year column headers. output a JSON file with an extra field
+which is the unix timestamp for the date represented in each row"` output
 `json` ```json [{"day": "11", "month": "3", "year": "2021", "timestamp":
 1615449600}, {"day": "2", "month": "8", "year": "1999", "timestamp":
 933577200}] ``` ### Disclaimer The success of each conversion depends on GPT-
 3.5 generating the correct code for the task. It also depends on the conversion
 string correctly describing the input and the logic of manipulating it. ###
 Security / Safety Input file data never leaves your local machine. Only the
 conversion description is sent to OpenAI to generate the conversion code. Note
```

### Comparing `charmr-1.0.6/README.md` & `charmr-1.0.7/charmr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: charmr
+Version: 1.0.7
+Summary: A Magical AI File Converter
+Home-page: https://github.com/harlev/charmr
+Author: Ron Harlev
+Author-email: harlev@gmail.com
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 # charmr
 #### a Magical AI File Converter
 
 [![PyPI version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 <a href="https://github.com/harlev/charmr/blob/master/LICENSE">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg" target="_blank" />
 </a>
@@ -44,15 +55,36 @@
 * Adding an `--alias` will save the conversion in a `.charmr` file.  
 * Then you can specify `--alias` without providing `--conversion` to repeat the same conversion.  
 * Define `--view_code_only` will only print out the code without running it. Use this to review generated code for safety. Specifying `--alias` will save it to be reused.
 * Use `--gpt_4` to use GPT-4 to generate code. Default is `gpt-3.5-turbo`
 * Specify `include_input_rows` with number of rows to include in prompt. This can improve code generation.
 
 e.g. `charmr -i input.csv -o output.json -c "convert csv to json"`  
-OR   `charmr -c "convert csv to json" < input.csv > output.json`
+OR   `charmr -c "convert csv to json" < input.csv > output.json`  
+OR a more fluent use
+```
+cat input.csv | charmr -4 -c "convert the csv to json and keep just the first and third columns" | jq .
+[
+  {
+    "a": "1",
+    "c": "3"
+  },
+  {
+    "a": "4",
+    "c": "6"
+  }
+]
+```  
+Emulating the `cut` utility:  
+`cat input.csv | cut -d"," -f2`  
+Same thing with `charmr`  
+`cat input.csv | charmr -4 -c "read the csv and keep only the second column"`  
+
+Then combining transformation and filtering  
+`cat input.csv | charmr -4 -c "read the csv, remove the header row, keep only the second column and output the square of the values"`
 
 ### Examples
 #### Basic conversion
 input `csv`  
 ```
 a, b, c
 1, 2, 3
```

#### html2text {}

```diff
@@ -1,33 +1,43 @@
-# charmr #### a Magical AI File Converter [![PyPI version](https://
-badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr) [License:_MIT]
-[![Downloads](https://pepy.tech/badge/charmr)](https://pepy.tech/project/
-charmr) This application will convert, transform, filter etc. any text based
-common file format into another file, based on a text description of the
-required result. It is using GPT-3.5/4 to generate code that will run the
-conversion locally. The actual input data is not being sent outside of the
-local machine. ### Getting Started ```commandline pip install charmr ``` ###
-Set OpenAI API Key ```commandline export OPENAI_API_KEY= ``` ### Usage
-```options: options: -h, --help show this help message and exit --input_file
-INPUT_FILE, -i INPUT_FILE Input file --output_file OUTPUT_FILE, -o OUTPUT_FILE
-Output file --conversion CONVERSION, -c CONVERSION Conversion description --
-alias ALIAS, -a ALIAS Conversion alias, for reuse --view_code_only, -v View
-code without running --gpt_4, -4 Use GPT-4 --include_input_rows
-INCLUDE_INPUT_ROWS, -r INCLUDE_INPUT_ROWS Include N input rows in prompt ``` *
-Define `--input_file`, `--output_file` and `--conversion` for basic
-functionality. * Can also use stdin and/or stdout instead of defining in/out
-path. * Adding an `--alias` will save the conversion in a `.charmr` file. *
-Then you can specify `--alias` without providing `--conversion` to repeat the
-same conversion. * Define `--view_code_only` will only print out the code
-without running it. Use this to review generated code for safety. Specifying `-
--alias` will save it to be reused. * Use `--gpt_4` to use GPT-4 to generate
-code. Default is `gpt-3.5-turbo` * Specify `include_input_rows` with number of
-rows to include in prompt. This can improve code generation. e.g. `charmr -
-i input.csv -o output.json -c "convert csv to json"` OR `charmr -c "convert csv
-to json" < input.csv > output.json` ### Examples #### Basic conversion input
+Metadata-Version: 2.1 Name: charmr Version: 1.0.7 Summary: A Magical AI File
+Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
+Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
+Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
+version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
+[License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
+pepy.tech/project/charmr) This application will convert, transform, filter etc.
+any text based common file format into another file, based on a text
+description of the required result. It is using GPT-3.5/4 to generate code that
+will run the conversion locally. The actual input data is not being sent
+outside of the local machine. ### Getting Started ```commandline pip install
+charmr ``` ### Set OpenAI API Key ```commandline export OPENAI_API_KEY= ``` ###
+Usage ```options: options: -h, --help show this help message and exit --
+input_file INPUT_FILE, -i INPUT_FILE Input file --output_file OUTPUT_FILE, -
+o OUTPUT_FILE Output file --conversion CONVERSION, -c CONVERSION Conversion
+description --alias ALIAS, -a ALIAS Conversion alias, for reuse --
+view_code_only, -v View code without running --gpt_4, -4 Use GPT-4 --
+include_input_rows INCLUDE_INPUT_ROWS, -r INCLUDE_INPUT_ROWS Include N input
+rows in prompt ``` * Define `--input_file`, `--output_file` and `--conversion`
+for basic functionality. * Can also use stdin and/or stdout instead of defining
+in/out path. * Adding an `--alias` will save the conversion in a `.charmr`
+file. * Then you can specify `--alias` without providing `--conversion` to
+repeat the same conversion. * Define `--view_code_only` will only print out the
+code without running it. Use this to review generated code for safety.
+Specifying `--alias` will save it to be reused. * Use `--gpt_4` to use GPT-4 to
+generate code. Default is `gpt-3.5-turbo` * Specify `include_input_rows` with
+number of rows to include in prompt. This can improve code generation. e.g.
+`charmr -i input.csv -o output.json -c "convert csv to json"` OR `charmr -
+c "convert csv to json" < input.csv > output.json` OR a more fluent use ``` cat
+input.csv | charmr -4 -c "convert the csv to json and keep just the first and
+third columns" | jq . [ { "a": "1", "c": "3" }, { "a": "4", "c": "6" } ] ```
+Emulating the `cut` utility: `cat input.csv | cut -d"," -f2` Same thing with
+`charmr` `cat input.csv | charmr -4 -c "read the csv and keep only the second
+column"` Then combining transformation and filtering `cat input.csv | charmr -
+4 -c "read the csv, remove the header row, keep only the second column and
+output the square of the values"` ### Examples #### Basic conversion input
 `csv` ``` a, b, c 1, 2, 3 4, 5, 6 ``` conversion `convert csv to json` output
 `json` ```json [{"a": "1", " b": " 2", " c": " 3"}, {"a": "4", " b": " 5", "
 c": " 6"}] ``` #### Column manipulation input `csv` ``` a, b, c 1, 2, 3 4, 5, 6
 ``` conversion `the input file is a CSV with column headers a,b,c. the output
 file is a CSV. create a new column ac with the multiplication of a and c`
 output `csv` ``` a,b,c,ac 1,2,3,3 4,5,6,24 ``` #### Conversion Logic input
 `csv` ``` day,month,year 11,3,2021 2,8,1999 ``` conversion `input a csv file
```

### Comparing `charmr-1.0.6/charmr/ai.py` & `charmr-1.0.7/charmr/ai.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 
 SYSTEM = """you are a file converter code generator. 
 You will get a description of the source and target files format, and any conversion, manipulation, 
 filtering or transformation to apply on the source to generate the target. 
 You will output a python function.
 The source input is a stream.
+skip empty lines or lines with only whitespace in the input stream.
 The target output is a stream as well.
 The function name will be "file_convert". 
 function signature is "file_convert(input_stream, output_stream)"
 Generate only the code, with no comments. 
 Don't generate any wrapper to the code. 
 The output should be compilable as python code, version 3.8.
 prefer string manipulation over using external packages where possible.
```

### Comparing `charmr-1.0.6/charmr/alias_manager.py` & `charmr-1.0.7/charmr/alias_manager.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.6/charmr/load_code.py` & `charmr-1.0.7/charmr/load_code.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.6/charmr/main.py` & `charmr-1.0.7/charmr/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,32 @@
     parser.add_argument('--view_code_only', '-v', help='View code without running', action='store_true')
     parser.add_argument('--gpt_4', '-4', help='Use GPT-4', action='store_true')
     parser.add_argument('--include_input_rows', '-r', type=int, help='Include N input rows in prompt', required=False)
     args = parser.parse_args()
     return args
 
 
-def read_input_file(file_path):
-    with open(file_path, 'r') as f:
-        file_content = f.read()
-    return file_content
+def read_first_n_lines(in_file, n):
+    if in_file:
+        in_stream = open(in_file, "r")
+    else:
+        in_stream = sys.stdin
 
+    lines = []
+    for i in range(n):
+        line = in_stream.readline()
+        if line:
+            lines.append(line)
+        else:
+            break
 
-def read_first_n_lines(file_path, n):
-    with open(file_path, 'r') as f:
-        lines = []
-        for i in range(n):
-            line = f.readline()
-            if line:
-                lines.append(line)
-            else:
-                break
+    if in_file:
+        in_stream.close()
+    else:
+        in_stream.seek(0)
     return lines
 
 
 def send_stream_to_stdout(stream):
     for line in stream:
         sys.stdout.write(line)
 
@@ -83,12 +86,10 @@
             in_stream.close()
         if args.output_file:
             out_stream.close()
 
     else:
         print(conversion_code)
 
-    # print(result)
-
 
 if __name__ == "__main__":
     main()
```

### Comparing `charmr-1.0.6/charmr.egg-info/PKG-INFO` & `charmr-1.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: charmr
-Version: 1.0.6
-Summary: A Magical AI File Converter
-Home-page: https://github.com/harlev/charmr
-Author: Ron Harlev
-Author-email: harlev@gmail.com
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # charmr
 #### a Magical AI File Converter
 
 [![PyPI version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 <a href="https://github.com/harlev/charmr/blob/master/LICENSE">
     <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-yellow.svg" target="_blank" />
 </a>
@@ -55,15 +44,36 @@
 * Adding an `--alias` will save the conversion in a `.charmr` file.  
 * Then you can specify `--alias` without providing `--conversion` to repeat the same conversion.  
 * Define `--view_code_only` will only print out the code without running it. Use this to review generated code for safety. Specifying `--alias` will save it to be reused.
 * Use `--gpt_4` to use GPT-4 to generate code. Default is `gpt-3.5-turbo`
 * Specify `include_input_rows` with number of rows to include in prompt. This can improve code generation.
 
 e.g. `charmr -i input.csv -o output.json -c "convert csv to json"`  
-OR   `charmr -c "convert csv to json" < input.csv > output.json`
+OR   `charmr -c "convert csv to json" < input.csv > output.json`  
+OR a more fluent use
+```
+cat input.csv | charmr -4 -c "convert the csv to json and keep just the first and third columns" | jq .
+[
+  {
+    "a": "1",
+    "c": "3"
+  },
+  {
+    "a": "4",
+    "c": "6"
+  }
+]
+```  
+Emulating the `cut` utility:  
+`cat input.csv | cut -d"," -f2`  
+Same thing with `charmr`  
+`cat input.csv | charmr -4 -c "read the csv and keep only the second column"`  
+
+Then combining transformation and filtering  
+`cat input.csv | charmr -4 -c "read the csv, remove the header row, keep only the second column and output the square of the values"`
 
 ### Examples
 #### Basic conversion
 input `csv`  
 ```
 a, b, c
 1, 2, 3
```

#### html2text {}

```diff
@@ -1,45 +1,49 @@
-Metadata-Version: 2.1 Name: charmr Version: 1.0.6 Summary: A Magical AI File
-Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
-Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
-Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
-version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
-[License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
-pepy.tech/project/charmr) This application will convert, transform, filter etc.
-any text based common file format into another file, based on a text
-description of the required result. It is using GPT-3.5/4 to generate code that
-will run the conversion locally. The actual input data is not being sent
-outside of the local machine. ### Getting Started ```commandline pip install
-charmr ``` ### Set OpenAI API Key ```commandline export OPENAI_API_KEY= ``` ###
-Usage ```options: options: -h, --help show this help message and exit --
-input_file INPUT_FILE, -i INPUT_FILE Input file --output_file OUTPUT_FILE, -
-o OUTPUT_FILE Output file --conversion CONVERSION, -c CONVERSION Conversion
-description --alias ALIAS, -a ALIAS Conversion alias, for reuse --
-view_code_only, -v View code without running --gpt_4, -4 Use GPT-4 --
-include_input_rows INCLUDE_INPUT_ROWS, -r INCLUDE_INPUT_ROWS Include N input
-rows in prompt ``` * Define `--input_file`, `--output_file` and `--conversion`
-for basic functionality. * Can also use stdin and/or stdout instead of defining
-in/out path. * Adding an `--alias` will save the conversion in a `.charmr`
-file. * Then you can specify `--alias` without providing `--conversion` to
-repeat the same conversion. * Define `--view_code_only` will only print out the
-code without running it. Use this to review generated code for safety.
-Specifying `--alias` will save it to be reused. * Use `--gpt_4` to use GPT-4 to
-generate code. Default is `gpt-3.5-turbo` * Specify `include_input_rows` with
-number of rows to include in prompt. This can improve code generation. e.g.
-`charmr -i input.csv -o output.json -c "convert csv to json"` OR `charmr -
-c "convert csv to json" < input.csv > output.json` ### Examples #### Basic
-conversion input `csv` ``` a, b, c 1, 2, 3 4, 5, 6 ``` conversion `convert csv
-to json` output `json` ```json [{"a": "1", " b": " 2", " c": " 3"}, {"a": "4",
-" b": " 5", " c": " 6"}] ``` #### Column manipulation input `csv` ``` a, b, c
-1, 2, 3 4, 5, 6 ``` conversion `the input file is a CSV with column headers
-a,b,c. the output file is a CSV. create a new column ac with the multiplication
-of a and c` output `csv` ``` a,b,c,ac 1,2,3,3 4,5,6,24 ``` #### Conversion
-Logic input `csv` ``` day,month,year 11,3,2021 2,8,1999 ``` conversion `input a
-csv file with day,month,year column headers. output a JSON file with an extra
-field which is the unix timestamp for the date represented in each row"` output
+# charmr #### a Magical AI File Converter [![PyPI version](https://
+badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr) [License:_MIT]
+[![Downloads](https://pepy.tech/badge/charmr)](https://pepy.tech/project/
+charmr) This application will convert, transform, filter etc. any text based
+common file format into another file, based on a text description of the
+required result. It is using GPT-3.5/4 to generate code that will run the
+conversion locally. The actual input data is not being sent outside of the
+local machine. ### Getting Started ```commandline pip install charmr ``` ###
+Set OpenAI API Key ```commandline export OPENAI_API_KEY= ``` ### Usage
+```options: options: -h, --help show this help message and exit --input_file
+INPUT_FILE, -i INPUT_FILE Input file --output_file OUTPUT_FILE, -o OUTPUT_FILE
+Output file --conversion CONVERSION, -c CONVERSION Conversion description --
+alias ALIAS, -a ALIAS Conversion alias, for reuse --view_code_only, -v View
+code without running --gpt_4, -4 Use GPT-4 --include_input_rows
+INCLUDE_INPUT_ROWS, -r INCLUDE_INPUT_ROWS Include N input rows in prompt ``` *
+Define `--input_file`, `--output_file` and `--conversion` for basic
+functionality. * Can also use stdin and/or stdout instead of defining in/out
+path. * Adding an `--alias` will save the conversion in a `.charmr` file. *
+Then you can specify `--alias` without providing `--conversion` to repeat the
+same conversion. * Define `--view_code_only` will only print out the code
+without running it. Use this to review generated code for safety. Specifying `-
+-alias` will save it to be reused. * Use `--gpt_4` to use GPT-4 to generate
+code. Default is `gpt-3.5-turbo` * Specify `include_input_rows` with number of
+rows to include in prompt. This can improve code generation. e.g. `charmr -
+i input.csv -o output.json -c "convert csv to json"` OR `charmr -c "convert csv
+to json" < input.csv > output.json` OR a more fluent use ``` cat input.csv |
+charmr -4 -c "convert the csv to json and keep just the first and third
+columns" | jq . [ { "a": "1", "c": "3" }, { "a": "4", "c": "6" } ] ```
+Emulating the `cut` utility: `cat input.csv | cut -d"," -f2` Same thing with
+`charmr` `cat input.csv | charmr -4 -c "read the csv and keep only the second
+column"` Then combining transformation and filtering `cat input.csv | charmr -
+4 -c "read the csv, remove the header row, keep only the second column and
+output the square of the values"` ### Examples #### Basic conversion input
+`csv` ``` a, b, c 1, 2, 3 4, 5, 6 ``` conversion `convert csv to json` output
+`json` ```json [{"a": "1", " b": " 2", " c": " 3"}, {"a": "4", " b": " 5", "
+c": " 6"}] ``` #### Column manipulation input `csv` ``` a, b, c 1, 2, 3 4, 5, 6
+``` conversion `the input file is a CSV with column headers a,b,c. the output
+file is a CSV. create a new column ac with the multiplication of a and c`
+output `csv` ``` a,b,c,ac 1,2,3,3 4,5,6,24 ``` #### Conversion Logic input
+`csv` ``` day,month,year 11,3,2021 2,8,1999 ``` conversion `input a csv file
+with day,month,year column headers. output a JSON file with an extra field
+which is the unix timestamp for the date represented in each row"` output
 `json` ```json [{"day": "11", "month": "3", "year": "2021", "timestamp":
 1615449600}, {"day": "2", "month": "8", "year": "1999", "timestamp":
 933577200}] ``` ### Disclaimer The success of each conversion depends on GPT-
 3.5 generating the correct code for the task. It also depends on the conversion
 string correctly describing the input and the logic of manipulating it. ###
 Security / Safety Input file data never leaves your local machine. Only the
 conversion description is sent to OpenAI to generate the conversion code. Note
```

### Comparing `charmr-1.0.6/setup.py` & `charmr-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='charmr',
-    version='1.0.6',
+    version='1.0.7',
     description='A Magical AI File Converter',
     url='https://github.com/harlev/charmr',
     author='Ron Harlev',
     author_email='harlev@gmail.com',
     packages=find_packages(),
     install_requires=[
         'openai',
```

