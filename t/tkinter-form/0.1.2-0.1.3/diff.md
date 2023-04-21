# Comparing `tmp/tkinter_form-0.1.2.tar.gz` & `tmp/tkinter_form-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinter_form-0.1.2.tar", last modified: Fri Apr 21 09:08:23 2023, max compression
+gzip compressed data, was "tkinter_form-0.1.3.tar", last modified: Fri Apr 21 09:16:33 2023, max compression
```

## Comparing `tkinter_form-0.1.2.tar` & `tkinter_form-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:23.081860 tkinter_form-0.1.2/
--rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2780 2023-04-21 09:08:23.080860 tkinter_form-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 09:08:23.081860 tkinter_form-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-21 09:05:26.000000 tkinter_form-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:23.061857 tkinter_form-0.1.2/tkinter_form/
--rw-rw-rw-   0        0        0       21 2023-04-21 08:41:30.000000 tkinter_form-0.1.2/tkinter_form/__init__.py
--rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.2/tkinter_form/tkinter_form.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:23.078861 tkinter_form-0.1.2/tkinter_form.egg-info/
--rw-rw-rw-   0        0        0     2780 2023-04-21 09:08:22.000000 tkinter_form-0.1.2/tkinter_form.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-21 09:08:23.000000 tkinter_form-0.1.2/tkinter_form.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:08:22.000000 tkinter_form-0.1.2/tkinter_form.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2023-04-21 09:08:22.000000 tkinter_form-0.1.2/tkinter_form.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 09:08:22.000000 tkinter_form-0.1.2/tkinter_form.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.914230 tkinter_form-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 08:09:26.000000 tkinter_form-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2744 2023-04-21 09:16:33.913229 tkinter_form-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:16:33.914230 tkinter_form-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-04-21 09:14:18.000000 tkinter_form-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.890224 tkinter_form-0.1.3/tkinter_form/
+-rw-rw-rw-   0        0        0       39 2023-04-21 09:14:06.000000 tkinter_form-0.1.3/tkinter_form/__init__.py
+-rw-rw-rw-   0        0        0     7506 2023-04-21 07:44:03.000000 tkinter_form-0.1.3/tkinter_form/tkinter_form.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:16:33.911229 tkinter_form-0.1.3/tkinter_form.egg-info/
+-rw-rw-rw-   0        0        0     2744 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 09:16:33.000000 tkinter_form-0.1.3/tkinter_form.egg-info/top_level.txt
```

### Comparing `tkinter_form-0.1.2/LICENSE` & `tkinter_form-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.2/PKG-INFO` & `tkinter_form-0.1.3/tkinter_form.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tkinter_form
-Version: 0.1.2
+Name: tkinter-form
+Version: 0.1.3
 Summary: form for tkinter
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -30,65 +30,53 @@
 
 ### Fast Example
 
 ```python
 import tkinter as tk
 from tkinter_form import Form
 
-
 class App(tk.Tk):
     def __init__(self) -> None:
         super().__init__()
-
         estruct = {
             "high": 1.0,
             "width": 1.0,
             "round": False,
             "type of calculation": ["calculate area", "calculate perimeter"],
             "result": "",
         }
-
         self.form = Form(
             self,
             name_form="calculations of a rectangle",
             form_dict=estruct,
             name_config="calculate",
             button=True
         )
         self.form.pack()
-
         self.button = self.form.button
 
         self.button.config(command=self.calculate)
         self.mainloop()
-
     def calculate(self):
         """
         Calculate values rectangle
         """
         dict_vals = self.form.get()
-
         if dict_vals["type of calculation"] == "calculate area":
             value = dict_vals["high"] * dict_vals["width"]
         elif dict_vals["type of calculation"] == "calculate perimeter":
             value = 2 * dict_vals["high"] + 2 * dict_vals["width"]
         else:
             value = 0
-
         if dict_vals["round"]:
             value = round(value)
-
         result = {"result": str(value)}
-
         self.form.set(result)
-
-
 if __name__ == "__main__":
     App()
-
 ```
 
 With these lines we create the interface that performs the calculations of area and perimeter of a rectangle. This frees us the declaration of the labels and other objects returning a ttk.LabelFrame with the additional methods set(), get() and the attributes widgets and button.
 
 
 
 ![example](src\example.png)
```

### Comparing `tkinter_form-0.1.2/setup.py` & `tkinter_form-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "readme.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 DESCRIPTION = "form for tkinter"
 LONG_DESCRIPTION = "create a form for tkinter from a base dictionary"
 
 # Setting up
 setup(
     name="tkinter_form",
     version=VERSION,
```

### Comparing `tkinter_form-0.1.2/tkinter_form/tkinter_form.py` & `tkinter_form-0.1.3/tkinter_form/tkinter_form.py`

 * *Files identical despite different names*

### Comparing `tkinter_form-0.1.2/tkinter_form.egg-info/PKG-INFO` & `tkinter_form-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tkinter-form
-Version: 0.1.2
+Name: tkinter_form
+Version: 0.1.3
 Summary: form for tkinter
 Author: JohanEstebanCuervo
 Author-email: <jecuervoch@unal.edu.co>
 License: MIT
 Keywords: tkinter,form,form tkinter,tkinter interface,simple tkinter,tkform,tk form
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -30,65 +30,53 @@
 
 ### Fast Example
 
 ```python
 import tkinter as tk
 from tkinter_form import Form
 
-
 class App(tk.Tk):
     def __init__(self) -> None:
         super().__init__()
-
         estruct = {
             "high": 1.0,
             "width": 1.0,
             "round": False,
             "type of calculation": ["calculate area", "calculate perimeter"],
             "result": "",
         }
-
         self.form = Form(
             self,
             name_form="calculations of a rectangle",
             form_dict=estruct,
             name_config="calculate",
             button=True
         )
         self.form.pack()
-
         self.button = self.form.button
 
         self.button.config(command=self.calculate)
         self.mainloop()
-
     def calculate(self):
         """
         Calculate values rectangle
         """
         dict_vals = self.form.get()
-
         if dict_vals["type of calculation"] == "calculate area":
             value = dict_vals["high"] * dict_vals["width"]
         elif dict_vals["type of calculation"] == "calculate perimeter":
             value = 2 * dict_vals["high"] + 2 * dict_vals["width"]
         else:
             value = 0
-
         if dict_vals["round"]:
             value = round(value)
-
         result = {"result": str(value)}
-
         self.form.set(result)
-
-
 if __name__ == "__main__":
     App()
-
 ```
 
 With these lines we create the interface that performs the calculations of area and perimeter of a rectangle. This frees us the declaration of the labels and other objects returning a ttk.LabelFrame with the additional methods set(), get() and the attributes widgets and button.
 
 
 
 ![example](src\example.png)
```

