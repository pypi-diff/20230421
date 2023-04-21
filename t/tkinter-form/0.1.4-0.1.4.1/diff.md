# Comparing `tmp/tkinter_form-0.1.4.tar.gz` & `tmp/tkinter_form-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_form-0.1.4.tar", last modified: Fri Apr 21 09:20:49 2023, max compression
+gzip compressed data, was "tkinter_form-0.1.4.1.tar", last modified: Fri Apr 21 09:27:22 2023, max compression
```

## Comparing `tkinter_form-0.1.4.tar` & `tkinter_form-0.1.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.806831 tkinter_form-0.1.4/
--rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2744 2023-04-21 09:20:49.805829 tkinter_form-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 09:20:49.806831 tkinter_form-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-21 09:20:32.000000 tkinter_form-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.787826 tkinter_form-0.1.4/tkinter_form/
--rw-rw-rw-   0        0        0       44 2023-04-21 09:19:56.000000 tkinter_form-0.1.4/tkinter_form/__init__.py
--rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.4/tkinter_form/tkinter_form.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.803829 tkinter_form-0.1.4/tkinter_form.egg-info/
--rw-rw-rw-   0        0        0     2744 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.199248 tkinter_form-0.1.4.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2809 2023-04-21 09:27:22.198248 tkinter_form-0.1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:27:22.199248 tkinter_form-0.1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-04-21 09:26:56.000000 tkinter_form-0.1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.180244 tkinter_form-0.1.4.1/tkinter_form/
+-rw-rw-rw-   0        0        0       44 2023-04-21 09:19:56.000000 tkinter_form-0.1.4.1/tkinter_form/__init__.py
+-rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.4.1/tkinter_form/tkinter_form.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:27:22.197248 tkinter_form-0.1.4.1/tkinter_form.egg-info/
+-rw-rw-rw-   0        0        0     2809 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 09:27:22.000000 tkinter_form-0.1.4.1/tkinter_form.egg-info/top_level.txt
```

### Comparing `tkinter_form-0.1.4/LICENSE` & `tkinter_form-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.4/PKG-INFO` & `tkinter_form-0.1.4.1/tkinter_form.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: tkinter_form
-Version: 0.1.4
+Name: tkinter-form
+Version: 0.1.4.1
 Summary: form for tkinter
+Home-page: https://github.com/JohanEstebanCuervo/tkinter_form
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tkinter_form-0.1.4/setup.py` & `tkinter_form-0.1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "readme.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.4"
+VERSION = "0.1.4.1"
 DESCRIPTION = "form for tkinter"
 LONG_DESCRIPTION = "create a form for tkinter from a base dictionary"
 
 # Setting up
 setup(
     name="tkinter_form",
     version=VERSION,
@@ -36,8 +36,9 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     license="MIT",
+    url="https://github.com/JohanEstebanCuervo/tkinter_form",
 )
```

### Comparing `tkinter_form-0.1.4/tkinter_form/tkinter_form.py` & `tkinter_form-0.1.4.1/tkinter_form/tkinter_form.py`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.4/tkinter_form.egg-info/PKG-INFO` & `tkinter_form-0.1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
-Name: tkinter-form
-Version: 0.1.4
+Name: tkinter_form
+Version: 0.1.4.1
 Summary: form for tkinter
+Home-page: https://github.com/JohanEstebanCuervo/tkinter_form
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

