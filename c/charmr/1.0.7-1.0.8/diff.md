# Comparing `tmp/charmr-1.0.7.tar.gz` & `tmp/charmr-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmr-1.0.7.tar", last modified: Thu Apr 20 22:04:32 2023, max compression
+gzip compressed data, was "charmr-1.0.8.tar", last modified: Fri Apr 21 01:24:09 2023, max compression
```

## Comparing `charmr-1.0.7.tar` & `charmr-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.024959 charmr-1.0.7/
--rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-20 22:04:32.024472 charmr-1.0.7/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)     4259 2023-04-20 21:28:46.000000 charmr-1.0.7/README.md
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.021041 charmr-1.0.7/charmr/
--rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.7/charmr/__init__.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1523 2023-04-20 21:39:35.000000 charmr-1.0.7/charmr/ai.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.7/charmr/alias_manager.py
--rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.7/charmr/load_code.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     2756 2023-04-20 22:01:10.000000 charmr-1.0.7/charmr/main.py
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-20 22:04:32.023874 charmr-1.0.7/charmr.egg-info/
--rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/SOURCES.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/dependency_links.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/entry_points.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/requires.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-20 22:04:31.000000 charmr-1.0.7/charmr.egg-info/top_level.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-20 22:04:32.025143 charmr-1.0.7/setup.cfg
--rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-20 21:58:47.000000 charmr-1.0.7/setup.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.280459 charmr-1.0.8/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 01:24:09.279880 charmr-1.0.8/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4259 2023-04-20 21:28:46.000000 charmr-1.0.8/README.md
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.274304 charmr-1.0.8/charmr/
+-rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.8/charmr/__init__.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1523 2023-04-20 21:39:35.000000 charmr-1.0.8/charmr/ai.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.8/charmr/alias_manager.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.8/charmr/load_code.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     3071 2023-04-21 01:18:52.000000 charmr-1.0.8/charmr/main.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.279136 charmr-1.0.8/charmr.egg-info/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/SOURCES.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/dependency_links.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/entry_points.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/requires.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/top_level.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-21 01:24:09.280604 charmr-1.0.8/setup.cfg
+-rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-21 01:22:26.000000 charmr-1.0.8/setup.py
```

### Comparing `charmr-1.0.7/PKG-INFO` & `charmr-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmr
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Magical AI File Converter
 Home-page: https://github.com/harlev/charmr
 Author: Ron Harlev
 Author-email: harlev@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: charmr Version: 1.0.7 Summary: A Magical AI File
+Metadata-Version: 2.1 Name: charmr Version: 1.0.8 Summary: A Magical AI File
 Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
 Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
 version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 [License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
 pepy.tech/project/charmr) This application will convert, transform, filter etc.
 any text based common file format into another file, based on a text
```

### Comparing `charmr-1.0.7/README.md` & `charmr-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `charmr-1.0.7/charmr/ai.py` & `charmr-1.0.8/charmr/ai.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.7/charmr/alias_manager.py` & `charmr-1.0.8/charmr/alias_manager.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.7/charmr/load_code.py` & `charmr-1.0.8/charmr/load_code.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.7/charmr/main.py` & `charmr-1.0.8/charmr/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import sys
+import io
+import tempfile
 from dotenv import load_dotenv
 from charmr import ai
 import argparse
 from charmr.load_code import run_function
 from charmr import alias_manager
 
 
@@ -15,19 +17,31 @@
     parser.add_argument('--view_code_only', '-v', help='View code without running', action='store_true')
     parser.add_argument('--gpt_4', '-4', help='Use GPT-4', action='store_true')
     parser.add_argument('--include_input_rows', '-r', type=int, help='Include N input rows in prompt', required=False)
     args = parser.parse_args()
     return args
 
 
+def get_seekable_stream(stream):
+    if stream.seekable():
+        return stream
+    else:
+        with tempfile.TemporaryFile() as temp_file:
+            temp_file.write(stream.read())
+
+            temp_file.seek(0)
+
+            return io.BufferedReader(temp_file)
+
+
 def read_first_n_lines(in_file, n):
     if in_file:
         in_stream = open(in_file, "r")
     else:
-        in_stream = sys.stdin
+        in_stream = get_seekable_stream(sys.stdin)
 
     lines = []
     for i in range(n):
         line = in_stream.readline()
         if line:
             lines.append(line)
         else:
```

### Comparing `charmr-1.0.7/charmr.egg-info/PKG-INFO` & `charmr-1.0.8/charmr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmr
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Magical AI File Converter
 Home-page: https://github.com/harlev/charmr
 Author: Ron Harlev
 Author-email: harlev@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: charmr Version: 1.0.7 Summary: A Magical AI File
+Metadata-Version: 2.1 Name: charmr Version: 1.0.8 Summary: A Magical AI File
 Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
 Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
 version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 [License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
 pepy.tech/project/charmr) This application will convert, transform, filter etc.
 any text based common file format into another file, based on a text
```

### Comparing `charmr-1.0.7/setup.py` & `charmr-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='charmr',
-    version='1.0.7',
+    version='1.0.8',
     description='A Magical AI File Converter',
     url='https://github.com/harlev/charmr',
     author='Ron Harlev',
     author_email='harlev@gmail.com',
     packages=find_packages(),
     install_requires=[
         'openai',
```

