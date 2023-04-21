# Comparing `tmp/bacteria-0.0.1.tar.gz` & `tmp/bacteria-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacteria-0.0.1.tar", last modified: Fri Apr 21 10:55:33 2023, max compression
+gzip compressed data, was "bacteria-0.0.2.tar", last modified: Fri Apr 21 11:07:54 2023, max compression
```

## Comparing `bacteria-0.0.1.tar` & `bacteria-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:55:33.794000 bacteria-0.0.1/
--rw-rw-rw-   0        0        0      606 2023-04-21 10:55:33.648000 bacteria-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 10:55:33.213000 bacteria-0.0.1/bacteria/
--rw-rw-rw-   0        0        0      646 2023-04-21 10:41:12.000000 bacteria-0.0.1/bacteria/__init__.py
--rw-rw-rw-   0        0        0   163931 2023-04-21 10:50:06.000000 bacteria-0.0.1/bacteria/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:55:33.607000 bacteria-0.0.1/bacteria.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-21 10:55:32.000000 bacteria-0.0.1/bacteria.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-21 10:55:32.000000 bacteria-0.0.1/bacteria.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:55:32.000000 bacteria-0.0.1/bacteria.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-04-21 10:55:32.000000 bacteria-0.0.1/bacteria.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 10:55:32.000000 bacteria-0.0.1/bacteria.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 10:55:33.756000 bacteria-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-04-21 10:54:44.000000 bacteria-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.931000 bacteria-0.0.2/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:07:54.821000 bacteria-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 10:36:49.000000 bacteria-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.345000 bacteria-0.0.2/bacteria/
+-rw-rw-rw-   0        0        0      646 2023-04-21 10:41:12.000000 bacteria-0.0.2/bacteria/__init__.py
+-rw-rw-rw-   0        0        0   163931 2023-04-21 10:50:06.000000 bacteria-0.0.2/bacteria/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:07:54.791000 bacteria-0.0.2/bacteria.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 11:07:53.000000 bacteria-0.0.2/bacteria.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 11:07:54.892000 bacteria-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1119 2023-04-21 11:07:48.000000 bacteria-0.0.2/setup.py
```

### Comparing `bacteria-0.0.1/PKG-INFO` & `bacteria-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.1
+Version: 0.0.2
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.1/bacteria/__init__.py` & `bacteria-0.0.2/bacteria/__init__.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.1/bacteria/functions.py` & `bacteria-0.0.2/bacteria/functions.py`

 * *Files identical despite different names*

### Comparing `bacteria-0.0.1/bacteria.egg-info/PKG-INFO` & `bacteria-0.0.2/bacteria.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacteria
-Version: 0.0.1
+Version: 0.0.2
 Summary: Super Segger Analysis in Python.
 Home-page: https://github.com/tuliofalmeida/bacteria
 License: MIT
 Download-URL: https://github.com/tuliofalmeida/bacteria
 Keywords: Data analysis,Cell analysis,Bacteria,SuperSegger
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bacteria-0.0.1/setup.py` & `bacteria-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,30 @@
  
 with open("README.md", "r") as fh:
     long_description = fh.read()
   
 setuptools.setup(
     name = 'bacteria',         
     packages = ['bacteria'],   
-    version = '0.0.1',      
+    version = '0.0.2',      
     license='MIT',       
     description = 'Super Segger Analysis in Python.',
     long_description_content_type="text/markdown",
     url = 'https://github.com/tuliofalmeida/bacteria',  
     download_url = 'https://github.com/tuliofalmeida/bacteria',    
     keywords = ['Data analysis', 'Cell analysis', 'Bacteria', 'SuperSegger'],   
     install_requires=[           
             'numpy',
             'pandas',
             'graphviz',
             'scikit-learn',
             'seaborn',
             'natsort',
             'anytree',
-            'matlabengine',
+            # 'matlabengine',
             'scipy'
         ],
     classifiers=[
       'Development Status :: 4 - Beta',      
       'Intended Audience :: Developers',      
       'Topic :: Software Development :: Build Tools',
       'License :: OSI Approved :: MIT License',
```

