# Comparing `tmp/pynometrics-0.1.2.tar.gz` & `tmp/pynometrics-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynometrics-0.1.2.tar", last modified: Fri Apr 21 08:21:08 2023, max compression
+gzip compressed data, was "pynometrics-0.1.3.tar", last modified: Fri Apr 21 08:55:30 2023, max compression
```

## Comparing `pynometrics-0.1.2.tar` & `pynometrics-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.625345 pynometrics-0.1.2/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-02 14:08:08.000000 pynometrics-0.1.2/LICENSE.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-02 14:08:08.000000 pynometrics-0.1.2/MANIFEST.in
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:21:08.625134 pynometrics-0.1.2/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-02 14:08:08.000000 pynometrics-0.1.2/README.md
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.622260 pynometrics-0.1.2/examples/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.2/examples/example_01.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.2/examples/example_02.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 08:21:08.625419 pynometrics-0.1.2/setup.cfg
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-04-21 08:19:17.000000 pynometrics-0.1.2/setup.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.622591 pynometrics-0.1.2/src/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.2/src/.DS_Store
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.623118 pynometrics-0.1.2/src/pynometrics/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 pynometrics-0.1.2/src/pynometrics/__init__.py
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16158 2023-04-21 08:19:11.000000 pynometrics-0.1.2/src/pynometrics/pynometrics.py
-drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:21:08.624850 pynometrics-0.1.2/src/pynometrics.egg-info/
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/PKG-INFO
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/SOURCES.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/dependency_links.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.2/src/pynometrics.egg-info/not-zip-safe
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/requires.txt
--rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-04-21 08:21:08.000000 pynometrics-0.1.2/src/pynometrics.egg-info/top_level.txt
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:55:30.312418 pynometrics-0.1.3/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1068 2023-04-02 14:08:08.000000 pynometrics-0.1.3/LICENSE.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       65 2023-04-02 14:08:08.000000 pynometrics-0.1.3/MANIFEST.in
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:55:30.312216 pynometrics-0.1.3/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      544 2023-04-02 14:08:08.000000 pynometrics-0.1.3/README.md
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:55:30.308602 pynometrics-0.1.3/examples/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      624 2023-04-01 18:56:30.000000 pynometrics-0.1.3/examples/example_01.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      656 2023-04-01 18:56:30.000000 pynometrics-0.1.3/examples/example_02.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       38 2023-04-21 08:55:30.312495 pynometrics-0.1.3/setup.cfg
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     1171 2023-04-21 08:53:44.000000 pynometrics-0.1.3/setup.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:55:30.309070 pynometrics-0.1.3/src/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)     6148 2023-04-01 21:01:41.000000 pynometrics-0.1.3/src/.DS_Store
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:55:30.309754 pynometrics-0.1.3/src/pynometrics/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-02 14:08:08.000000 pynometrics-0.1.3/src/pynometrics/__init__.py
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)    16098 2023-04-21 08:53:35.000000 pynometrics-0.1.3/src/pynometrics/pynometrics.py
+drwxr-xr-x   0 geofrey.wanyama   (503) staff       (20)        0 2023-04-21 08:55:30.311898 pynometrics-0.1.3/src/pynometrics.egg-info/
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      852 2023-04-21 08:55:30.000000 pynometrics-0.1.3/src/pynometrics.egg-info/PKG-INFO
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)      393 2023-04-21 08:55:30.000000 pynometrics-0.1.3/src/pynometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-21 08:55:30.000000 pynometrics-0.1.3/src/pynometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)        1 2023-04-01 20:54:02.000000 pynometrics-0.1.3/src/pynometrics.egg-info/not-zip-safe
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       42 2023-04-21 08:55:30.000000 pynometrics-0.1.3/src/pynometrics.egg-info/requires.txt
+-rw-r--r--   0 geofrey.wanyama   (503) staff       (20)       12 2023-04-21 08:55:30.000000 pynometrics-0.1.3/src/pynometrics.egg-info/top_level.txt
```

### Comparing `pynometrics-0.1.2/LICENSE.txt` & `pynometrics-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.2/PKG-INFO` & `pynometrics-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.2
+Version: 0.1.3
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `pynometrics-0.1.2/README.md` & `pynometrics-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.2/examples/example_01.py` & `pynometrics-0.1.3/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.2/examples/example_02.py` & `pynometrics-0.1.3/examples/example_02.py`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.2/setup.py` & `pynometrics-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("/Users/geofrey.wanyama/Desktop/wg/projects/package_dev/pyeconometrics/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     # name that will be imported, can be different from code file name
     name='pynometrics',
 
-    version='0.1.2',
+    version='0.1.3',
 
     description='Includes functions for performing econometrics tasks',
 
     # code file name without file extension
     packages=['pynometrics'],
 
     # directory in which code file is stored
```

### Comparing `pynometrics-0.1.2/src/.DS_Store` & `pynometrics-0.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pynometrics-0.1.2/src/pynometrics/pynometrics.py` & `pynometrics-0.1.3/src/pynometrics/pynometrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,30 +207,27 @@
                 errors = lambda X: X['coef'] - self.mdl.conf_int().iloc[:,0].values,
                 pvalues = self.mdl.pvalues.values,
                 Significant = lambda X: X['pvalues'] < 0.05)
             .query("var != 'Intercept'")
         )
 
         
-    def plot(self, figsize=None):
+    def plot(self, figsize=(12,5)):
         """
         Function to generate plot for chosen diagnostic check for linear regression
         
         Args:
             None
         
         Returns
             Matplotlib plot: Plot of chosen diagnostic check
         """
         
         sns.set_style('whitegrid')
         
-        if not figsize:
-            figsize = (12,5)
-        
         params = {
             "figure.figsize":figsize,
             "text.color":"#162871",
             "axes.titlesize":16,
             "axes.labelsize":14,
             "axes.labelcolor": "#162871",
             "axes.edgecolor": "#162871",
```

### Comparing `pynometrics-0.1.2/src/pynometrics.egg-info/PKG-INFO` & `pynometrics-0.1.3/src/pynometrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynometrics
-Version: 0.1.2
+Version: 0.1.3
 Summary: Includes functions for performing econometrics tasks
 Home-page: https://github.com/G-Geofrey/econometric_package.git
 Author: Geofrey Wanyama
 Author-email: wanyamag17@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

