# Comparing `tmp/tkinter_form-0.1.3.tar.gz` & `tmp/tkinter_form-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_form-0.1.3.tar", last modified: Fri Apr 21 09:16:33 2023, max compression
+gzip compressed data, was "tkinter_form-0.1.4.tar", last modified: Fri Apr 21 09:20:49 2023, max compression
```

## Comparing `tkinter_form-0.1.3.tar` & `tkinter_form-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.914230 tkinter_form-0.1.3/
--rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2744 2023-04-21 09:16:33.913229 tkinter_form-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 09:16:33.914230 tkinter_form-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-21 09:14:18.000000 tkinter_form-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.890224 tkinter_form-0.1.3/tkinter_form/
--rw-rw-rw-   0        0        0       39 2023-04-21 09:14:06.000000 tkinter_form-0.1.3/tkinter_form/__init__.py
--rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.3/tkinter_form/tkinter_form.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.911229 tkinter_form-0.1.3/tkinter_form.egg-info/
--rw-rw-rw-   0        0        0     2744 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.806831 tkinter_form-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2744 2023-04-21 09:20:49.805829 tkinter_form-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:20:49.806831 tkinter_form-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-04-21 09:20:32.000000 tkinter_form-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.787826 tkinter_form-0.1.4/tkinter_form/
+-rw-rw-rw-   0        0        0       44 2023-04-21 09:19:56.000000 tkinter_form-0.1.4/tkinter_form/__init__.py
+-rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.4/tkinter_form/tkinter_form.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:20:49.803829 tkinter_form-0.1.4/tkinter_form.egg-info/
+-rw-rw-rw-   0        0        0     2744 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 09:20:49.000000 tkinter_form-0.1.4/tkinter_form.egg-info/top_level.txt
```

### Comparing `tkinter_form-0.1.3/LICENSE` & `tkinter_form-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.3/PKG-INFO` & `tkinter_form-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinter_form
-Version: 0.1.3
+Version: 0.1.4
 Summary: form for tkinter
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tkinter_form-0.1.3/setup.py` & `tkinter_form-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "readme.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 DESCRIPTION = "form for tkinter"
 LONG_DESCRIPTION = "create a form for tkinter from a base dictionary"
 
 # Setting up
 setup(
     name="tkinter_form",
     version=VERSION,
```

### Comparing `tkinter_form-0.1.3/tkinter_form/tkinter_form.py` & `tkinter_form-0.1.4/tkinter_form/tkinter_form.py`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.3/tkinter_form.egg-info/PKG-INFO` & `tkinter_form-0.1.4/tkinter_form.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkinter-form
-Version: 0.1.3
+Version: 0.1.4
 Summary: form for tkinter
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

