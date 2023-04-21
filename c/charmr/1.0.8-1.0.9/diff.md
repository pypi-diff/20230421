# Comparing `tmp/charmr-1.0.8.tar.gz` & `tmp/charmr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmr-1.0.8.tar", last modified: Fri Apr 21 01:24:09 2023, max compression
+gzip compressed data, was "charmr-1.0.9.tar", last modified: Fri Apr 21 02:02:29 2023, max compression
```

## Comparing `charmr-1.0.8.tar` & `charmr-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.280459 charmr-1.0.8/
--rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 01:24:09.279880 charmr-1.0.8/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)     4259 2023-04-20 21:28:46.000000 charmr-1.0.8/README.md
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.274304 charmr-1.0.8/charmr/
--rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.8/charmr/__init__.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1523 2023-04-20 21:39:35.000000 charmr-1.0.8/charmr/ai.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.8/charmr/alias_manager.py
--rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.8/charmr/load_code.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     3071 2023-04-21 01:18:52.000000 charmr-1.0.8/charmr/main.py
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 01:24:09.279136 charmr-1.0.8/charmr.egg-info/
--rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/SOURCES.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/dependency_links.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/entry_points.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/requires.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-21 01:24:09.000000 charmr-1.0.8/charmr.egg-info/top_level.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-21 01:24:09.280604 charmr-1.0.8/setup.cfg
--rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-21 01:22:26.000000 charmr-1.0.8/setup.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 02:02:29.055742 charmr-1.0.9/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 02:02:29.055142 charmr-1.0.9/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4259 2023-04-20 21:28:46.000000 charmr-1.0.9/README.md
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 02:02:29.051224 charmr-1.0.9/charmr/
+-rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.9/charmr/__init__.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1523 2023-04-20 21:39:35.000000 charmr-1.0.9/charmr/ai.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.9/charmr/alias_manager.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.9/charmr/load_code.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     3080 2023-04-21 02:01:55.000000 charmr-1.0.9/charmr/main.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-21 02:02:29.054280 charmr-1.0.9/charmr.egg-info/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     4517 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/SOURCES.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/dependency_links.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/entry_points.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/requires.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-21 02:02:28.000000 charmr-1.0.9/charmr.egg-info/top_level.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-21 02:02:29.055970 charmr-1.0.9/setup.cfg
+-rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-21 02:02:25.000000 charmr-1.0.9/setup.py
```

### Comparing `charmr-1.0.8/PKG-INFO` & `charmr-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmr
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: charmr Version: 1.0.8 Summary: A Magical AI File
+Metadata-Version: 2.1 Name: charmr Version: 1.0.9 Summary: A Magical AI File
 Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
 Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
 version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 [License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
 pepy.tech/project/charmr) This application will convert, transform, filter etc.
 any text based common file format into another file, based on a text
```

### Comparing `charmr-1.0.8/README.md` & `charmr-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `charmr-1.0.8/charmr/ai.py` & `charmr-1.0.9/charmr/ai.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.8/charmr/alias_manager.py` & `charmr-1.0.9/charmr/alias_manager.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.8/charmr/load_code.py` & `charmr-1.0.9/charmr/load_code.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.8/charmr/main.py` & `charmr-1.0.9/charmr/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,57 +21,61 @@
     return args
 
 
 def get_seekable_stream(stream):
     if stream.seekable():
         return stream
     else:
-        with tempfile.TemporaryFile() as temp_file:
-            temp_file.write(stream.read())
+        temp_file = tempfile.TemporaryFile()
+        temp_file.write(stream.read().encode())
 
-            temp_file.seek(0)
+        temp_file.seek(0)
 
-            return io.BufferedReader(temp_file)
+        return io.BufferedReader(temp_file)
 
 
-def read_first_n_lines(in_file, n):
-    if in_file:
-        in_stream = open(in_file, "r")
-    else:
-        in_stream = get_seekable_stream(sys.stdin)
-
+def read_first_n_lines(in_stream, n):
     lines = []
-    for i in range(n):
-        line = in_stream.readline()
+    count = 0
+    for line in in_stream:
+        count += 1
         if line:
             lines.append(line)
         else:
             break
+        if count == int(n):
+            break
 
-    if in_file:
-        in_stream.close()
-    else:
-        in_stream.seek(0)
     return lines
 
 
 def send_stream_to_stdout(stream):
     for line in stream:
         sys.stdout.write(line)
 
 
 def main():
     load_dotenv()
     args = parse_arguments()
 
+    if args.input_file:
+        in_stream = open(args.input_file, "r")
+    else:
+        in_stream = get_seekable_stream(sys.stdin)
+
     if args.include_input_rows:
-        first_lines = read_first_n_lines(args.input_file, args.include_input_rows)
+        first_lines = read_first_n_lines(in_stream, args.include_input_rows)
     else:
         first_lines = None
 
+    if args.input_file:
+        in_stream.close()
+    else:
+        in_stream.seek(0)
+
     if args.gpt_4:
         model_name = "gpt-4"
     else:
         model_name = "gpt-3.5-turbo"
 
     if args.conversion:
         conversion_code = ai.get_code(args.conversion, model=model_name, header_rows=first_lines)
@@ -83,16 +87,14 @@
             raise Exception("Alias must be provided when no conversion defined")
         else:
             conversion_code = alias_manager.load_code(args.alias)
 
     if not args.view_code_only:
         if args.input_file:
             in_stream = open(args.input_file, "r")
-        else:
-            in_stream = sys.stdin
 
         if args.output_file:
             out_stream = open(args.output_file, "w")
         else:
             out_stream = sys.stdout
 
         run_function(conversion_code, in_stream, out_stream)
@@ -102,8 +104,8 @@
             out_stream.close()
 
     else:
         print(conversion_code)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `charmr-1.0.8/charmr.egg-info/PKG-INFO` & `charmr-1.0.9/charmr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmr
-Version: 1.0.8
+Version: 1.0.9
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
-Metadata-Version: 2.1 Name: charmr Version: 1.0.8 Summary: A Magical AI File
+Metadata-Version: 2.1 Name: charmr Version: 1.0.9 Summary: A Magical AI File
 Converter Home-page: https://github.com/harlev/charmr Author: Ron Harlev
 Author-email: harlev@gmail.com License: MIT Requires-Python: >=3.8 Description-
 Content-Type: text/markdown # charmr #### a Magical AI File Converter [![PyPI
 version](https://badge.fury.io/py/charmr.svg)](https://badge.fury.io/py/charmr)
 [License:_MIT] [![Downloads](https://pepy.tech/badge/charmr)](https://
 pepy.tech/project/charmr) This application will convert, transform, filter etc.
 any text based common file format into another file, based on a text
```

### Comparing `charmr-1.0.8/setup.py` & `charmr-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='charmr',
-    version='1.0.8',
+    version='1.0.9',
     description='A Magical AI File Converter',
     url='https://github.com/harlev/charmr',
     author='Ron Harlev',
     author_email='harlev@gmail.com',
     packages=find_packages(),
     install_requires=[
         'openai',
```

