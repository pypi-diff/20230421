# Comparing `tmp/easyhist-0.2.1.tar.gz` & `tmp/easyhist-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyhist-0.2.1.tar", last modified: Mon Dec 12 17:01:14 2022, max compression
+gzip compressed data, was "easyhist-0.2.2.tar", last modified: Thu Apr 20 22:50:47 2023, max compression
```

## Comparing `easyhist-0.2.1.tar` & `easyhist-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2022-12-12 17:01:14.310219 easyhist-0.2.1/
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2635 2022-12-12 17:01:14.310219 easyhist-0.2.1/PKG-INFO
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2291 2022-12-05 06:07:28.000000 easyhist-0.2.1/README.md
-drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2022-12-12 17:01:14.310219 easyhist-0.2.1/easyhist/
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)       20 2022-12-05 06:07:28.000000 easyhist-0.2.1/easyhist/__init__.py
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     9598 2022-12-05 06:07:28.000000 easyhist-0.2.1/easyhist/hist.py
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     6122 2022-12-12 16:27:47.000000 easyhist-0.2.1/easyhist/plot.py
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2709 2022-12-05 06:07:28.000000 easyhist-0.2.1/easyhist/utilities.py
-drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2022-12-12 17:01:14.310219 easyhist-0.2.1/easyhist.egg-info/
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2635 2022-12-12 17:01:14.000000 easyhist-0.2.1/easyhist.egg-info/PKG-INFO
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)      223 2022-12-12 17:01:14.000000 easyhist-0.2.1/easyhist.egg-info/SOURCES.txt
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)        1 2022-12-12 17:01:14.000000 easyhist-0.2.1/easyhist.egg-info/dependency_links.txt
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)        9 2022-12-12 17:01:14.000000 easyhist-0.2.1/easyhist.egg-info/top_level.txt
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)       38 2022-12-12 17:01:14.310219 easyhist-0.2.1/setup.cfg
--rw-rw-r--   0 pranphy   (1000) pranphy   (1000)      771 2022-12-12 16:55:01.000000 easyhist-0.2.1/setup.py
+drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2023-04-20 22:50:47.425365 easyhist-0.2.2/
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2582 2023-04-20 22:50:47.425365 easyhist-0.2.2/PKG-INFO
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2291 2022-12-05 06:07:28.000000 easyhist-0.2.2/README.md
+drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2023-04-20 22:50:47.425365 easyhist-0.2.2/easyhist/
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)       20 2023-04-20 22:50:30.000000 easyhist-0.2.2/easyhist/__init__.py
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     9598 2023-04-20 22:50:30.000000 easyhist-0.2.2/easyhist/hist.py
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     6122 2023-04-20 22:50:30.000000 easyhist-0.2.2/easyhist/plot.py
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2709 2023-04-20 22:50:30.000000 easyhist-0.2.2/easyhist/utilities.py
+drwxrwxr-x   0 pranphy   (1000) pranphy   (1000)        0 2023-04-20 22:50:47.425365 easyhist-0.2.2/easyhist.egg-info/
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)     2582 2023-04-20 22:50:47.000000 easyhist-0.2.2/easyhist.egg-info/PKG-INFO
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)      223 2023-04-20 22:50:47.000000 easyhist-0.2.2/easyhist.egg-info/SOURCES.txt
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)        1 2023-04-20 22:50:47.000000 easyhist-0.2.2/easyhist.egg-info/dependency_links.txt
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)        9 2023-04-20 22:50:47.000000 easyhist-0.2.2/easyhist.egg-info/top_level.txt
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)       38 2023-04-20 22:50:47.425365 easyhist-0.2.2/setup.cfg
+-rw-rw-r--   0 pranphy   (1000) pranphy   (1000)      771 2023-04-20 22:49:33.000000 easyhist-0.2.2/setup.py
```

### Comparing `easyhist-0.2.1/PKG-INFO` & `easyhist-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: easyhist
-Version: 0.2.1
-Summary: UNKNOWN
+Version: 0.2.2
 Home-page: https://github.com/pranphy/easyhist
 Author: Prakash Gautam
 Author-email: pranphy@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Easy Histogram
 This is a very small python package used to make histograms in python, and optionally plot them with `matplotlib`. The underlying histogramming tool is from `numpy`. This provides a very handy wrappers around them to easily make common histograms in 1d and 2d and plot with nice labels.
 
@@ -94,8 +91,7 @@
 fig,ax= plt.subplots(1,1,figsize=(12,6))
 h2d.plot(ax,steps=True,ebar=False,filled=True,xlabel='x (unit)',ylabel='y(unit)',title='Test',cbarlabel='Colorbar',aspect='auto',cmin=1)
 ```
 
 ![](images/gaussian-hist-05.png)
 
 There are a lot of othe nice useful features which can be found in the documentation.
-
```

### Comparing `easyhist-0.2.1/README.md` & `easyhist-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `easyhist-0.2.1/easyhist/hist.py` & `easyhist-0.2.2/easyhist/hist.py`

 * *Files identical despite different names*

### Comparing `easyhist-0.2.1/easyhist/plot.py` & `easyhist-0.2.2/easyhist/plot.py`

 * *Files identical despite different names*

### Comparing `easyhist-0.2.1/easyhist/utilities.py` & `easyhist-0.2.2/easyhist/utilities.py`

 * *Files identical despite different names*

### Comparing `easyhist-0.2.1/easyhist.egg-info/PKG-INFO` & `easyhist-0.2.2/easyhist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: easyhist
-Version: 0.2.1
-Summary: UNKNOWN
+Version: 0.2.2
 Home-page: https://github.com/pranphy/easyhist
 Author: Prakash Gautam
 Author-email: pranphy@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Easy Histogram
 This is a very small python package used to make histograms in python, and optionally plot them with `matplotlib`. The underlying histogramming tool is from `numpy`. This provides a very handy wrappers around them to easily make common histograms in 1d and 2d and plot with nice labels.
 
@@ -94,8 +91,7 @@
 fig,ax= plt.subplots(1,1,figsize=(12,6))
 h2d.plot(ax,steps=True,ebar=False,filled=True,xlabel='x (unit)',ylabel='y(unit)',title='Test',cbarlabel='Colorbar',aspect='auto',cmin=1)
 ```
 
 ![](images/gaussian-hist-05.png)
 
 There are a lot of othe nice useful features which can be found in the documentation.
-
```

### Comparing `easyhist-0.2.1/setup.py` & `easyhist-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 long_description = None
 
 with open("README.md",'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easyhist",
-    version="0.2.1",
+    version="0.2.2",
     author="Prakash Gautam",
     author_email="pranphy@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     #install_requres['numpy','matplotlib'],
 
     url='https://github.com/pranphy/easyhist',
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
-
 )
+
```

