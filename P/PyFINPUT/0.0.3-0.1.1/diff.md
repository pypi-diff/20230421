# Comparing `tmp/PyFINPUT-0.0.3.tar.gz` & `tmp/PyFINPUT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFINPUT-0.0.3.tar", last modified: Thu Apr 20 19:31:52 2023, max compression
+gzip compressed data, was "PyFINPUT-0.1.1.tar", last modified: Fri Apr 21 13:40:09 2023, max compression
```

## Comparing `PyFINPUT-0.0.3.tar` & `PyFINPUT-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/
--rw-r--r--   0 ben       (1000) ben       (1000)    35149 2023-04-17 15:44:18.000000 PyFINPUT-0.0.3/LICENSE
--rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)     1493 2023-04-19 00:30:49.000000 PyFINPUT-0.0.3/README.md
--rw-r--r--   0 ben       (1000) ben       (1000)      103 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/setup.cfg
--rw-r--r--   0 ben       (1000) ben       (1000)      664 2023-04-20 19:29:41.000000 PyFINPUT-0.0.3/setup.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.975690 PyFINPUT-0.0.3/src/
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.986523 PyFINPUT-0.0.3/src/PyFINPUT/
--rw-r--r--   0 ben       (1000) ben       (1000)     9062 2023-04-20 19:26:14.000000 PyFINPUT-0.0.3/src/PyFINPUT/PyFINPUT.py
--rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-04-19 00:26:22.000000 PyFINPUT-0.0.3/src/PyFINPUT/__init__.py
--rw-r--r--   0 ben       (1000) ben       (1000)      964 2023-04-18 19:15:02.000000 PyFINPUT-0.0.3/src/PyFINPUT/utils.py
-drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-20 19:31:51.997357 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/
--rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) ben       (1000)      252 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        9 2023-04-20 19:31:51.000000 PyFINPUT-0.0.3/src/PyFINPUT.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-21 13:40:09.780706 PyFINPUT-0.1.1/
+-rw-r--r--   0 ben       (1000) ben       (1000)    35149 2023-04-17 15:44:18.000000 PyFINPUT-0.1.1/LICENSE
+-rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-21 13:40:09.780706 PyFINPUT-0.1.1/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)     1555 2023-04-21 13:39:29.000000 PyFINPUT-0.1.1/README.md
+-rw-r--r--   0 ben       (1000) ben       (1000)      103 2023-04-21 13:40:09.780706 PyFINPUT-0.1.1/setup.cfg
+-rw-r--r--   0 ben       (1000) ben       (1000)      673 2023-04-21 13:38:57.000000 PyFINPUT-0.1.1/setup.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-21 13:40:09.750706 PyFINPUT-0.1.1/src/
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-21 13:40:09.780706 PyFINPUT-0.1.1/src/PyFINPUT/
+-rw-r--r--   0 ben       (1000) ben       (1000)     9062 2023-04-20 19:26:14.000000 PyFINPUT-0.1.1/src/PyFINPUT/PyFINPUT.py
+-rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-04-19 00:26:22.000000 PyFINPUT-0.1.1/src/PyFINPUT/__init__.py
+-rw-r--r--   0 ben       (1000) ben       (1000)      964 2023-04-18 19:15:02.000000 PyFINPUT-0.1.1/src/PyFINPUT/utils.py
+drwxr-xr-x   0 ben       (1000) ben       (1000)        0 2023-04-21 13:40:09.780706 PyFINPUT-0.1.1/src/PyFINPUT.egg-info/
+-rw-r--r--   0 ben       (1000) ben       (1000)      473 2023-04-21 13:40:09.000000 PyFINPUT-0.1.1/src/PyFINPUT.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) ben       (1000)      252 2023-04-21 13:40:09.000000 PyFINPUT-0.1.1/src/PyFINPUT.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-21 13:40:09.000000 PyFINPUT-0.1.1/src/PyFINPUT.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) ben       (1000)        1 2023-04-21 13:40:09.000000 PyFINPUT-0.1.1/src/PyFINPUT.egg-info/top_level.txt
```

### Comparing `PyFINPUT-0.0.3/LICENSE` & `PyFINPUT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFINPUT-0.0.3/README.md` & `PyFINPUT-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ### Python File INPUT
 At times, repeatedly using 20 command line arguments is frustrating.
 
 Why not use an input file?
 
 Import like this (I need to fix this...)
 
-`pip install PyFINPUT==0.0.1`
+`pip install PyFINPUT==0.0.3`
 
 `from PyFINPUT import pyfinput`
 
 ### 1. First, initiliase the input file class with the following arguments:
 
 * `parser = pyfinput.input_file(...)`
 
@@ -23,15 +23,16 @@
 * `assigner: str` (optional, def.: "=")
 
     Character(s) to divide the keywords from their values: str
 * `comment: str` (optional, def.: "#")
         
    Character(s) to identify the beginning of comment strings
 
-### 2. Keywords can be added to the input_file object with the `add_keyword()` function:
+### 2. Keywords can be added to the input_file object with the `add_keyword()` function,
+### and blocks can be added with the `add_block()` function.
 
 * `name: str` (required)
    
    Name of keyword
 * `kw_type: type` (optional, def.: str)
    
    Type of the keyword value(s)
@@ -47,8 +48,8 @@
 
 
 ### 3. Finally, parse the file with the parse_file() function on the input_file object:
     returns:
         dict
         The returned dict contains the keywords as keys as strings,
         and their values as the dictionary values, with the defined
-        type.
+        type.
```

### Comparing `PyFINPUT-0.0.3/setup.py` & `PyFINPUT-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyFINPUT',
-    version='0.0.3',
+    version='0.1.1',
     license='GNU General Public License v3.0',
     author="Benedict Saunders",
     author_email='benedictsaunders@gmail.com',
-    packages=find_packages('src'),
+    packages=find_packages('src/PyFINPUT'),
     package_dir={'': 'src'},
     url='https://github.com/benedictsaunders/PyFINPUT',
     keywords='input, file, keywords',
     install_requires=[],
     description = "A simple parser for a file input, akin to the format of argparse",
     long_description="""# PyFINPUT!\n\n  ## A small package to use a file to input multiple arguments to a script.\n\n""",
     long_description_content_type='text/markdown',
```

### Comparing `PyFINPUT-0.0.3/src/PyFINPUT/PyFINPUT.py` & `PyFINPUT-0.1.1/src/PyFINPUT/PyFINPUT.py`

 * *Files identical despite different names*

### Comparing `PyFINPUT-0.0.3/src/PyFINPUT/utils.py` & `PyFINPUT-0.1.1/src/PyFINPUT/utils.py`

 * *Files identical despite different names*

