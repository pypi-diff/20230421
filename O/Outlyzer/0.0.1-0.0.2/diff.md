# Comparing `tmp/Outlyzer-0.0.1.tar.gz` & `tmp/Outlyzer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Outlyzer-0.0.1.tar", last modified: Fri Apr 21 18:34:52 2023, max compression
+gzip compressed data, was "dist\Outlyzer-0.0.2.tar", last modified: Fri Apr 21 18:42:36 2023, max compression
```

## Comparing `Outlyzer-0.0.1.tar` & `Outlyzer-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:09:30.000000 Outlyzer-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/Outlyzer/
--rw-rw-rw-   0        0        0        0 2023-04-21 18:31:57.000000 Outlyzer-0.0.1/Outlyzer/__init__.py
--rw-rw-rw-   0        0        0      835 2023-04-21 18:13:33.000000 Outlyzer-0.0.1/Outlyzer/iqr.py
--rw-rw-rw-   0        0        0      982 2023-04-21 18:22:27.000000 Outlyzer-0.0.1/Outlyzer/visual.py
--rw-rw-rw-   0        0        0      644 2023-04-21 18:33:47.000000 Outlyzer-0.0.1/Outlyzer/zscore.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/Outlyzer.egg-info/
--rw-rw-rw-   0        0        0      621 2023-04-21 18:34:51.000000 Outlyzer-0.0.1/Outlyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/Outlyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:34:51.000000 Outlyzer-0.0.1/Outlyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-21 18:34:51.000000 Outlyzer-0.0.1/Outlyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 18:34:51.000000 Outlyzer-0.0.1/Outlyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      621 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-04-21 18:09:30.000000 Outlyzer-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 18:34:52.000000 Outlyzer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-21 18:32:25.000000 Outlyzer-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:09:30.000000 Outlyzer-0.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer/
+-rw-rw-rw-   0        0        0        0 2023-04-21 18:31:57.000000 Outlyzer-0.0.2/Outlyzer/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-04-21 18:13:33.000000 Outlyzer-0.0.2/Outlyzer/iqr.py
+-rw-rw-rw-   0        0        0      982 2023-04-21 18:22:27.000000 Outlyzer-0.0.2/Outlyzer/visual.py
+-rw-rw-rw-   0        0        0      644 2023-04-21 18:33:47.000000 Outlyzer-0.0.2/Outlyzer/zscore.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer.egg-info/
+-rw-rw-rw-   0        0        0     1509 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/Outlyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 18:42:35.000000 Outlyzer-0.0.2/Outlyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1509 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-04-21 18:09:30.000000 Outlyzer-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:42:36.000000 Outlyzer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1839 2023-04-21 18:42:19.000000 Outlyzer-0.0.2/setup.py
```

### Comparing `Outlyzer-0.0.1/LICENSE` & `Outlyzer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.1/Outlyzer/iqr.py` & `Outlyzer-0.0.2/Outlyzer/iqr.py`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.1/Outlyzer/visual.py` & `Outlyzer-0.0.2/Outlyzer/visual.py`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.1/Outlyzer/zscore.py` & `Outlyzer-0.0.2/Outlyzer/zscore.py`

 * *Files identical despite different names*

### Comparing `Outlyzer-0.0.1/setup.py` & `Outlyzer-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,44 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Outlier detection'
-LONG_DESCRIPTION = 'A Python package to detect outliers in a dataset'
+LONG_DESCRIPTION = '''
+
+A Python package to detect outliers in a dataset
+
+Outlyzer: A Python library for outlier detection
+
+Outlyzer is a Python library that provides various methods for detecting outliers in a dataset. It includes implementation of Z-score, IQR, and Mahalanobis distance methods for identifying outliers, as well as visualization-based methods using scatter plots, box plots, and other types of visualizations.
+
+Usage:
+    - Import the desired method from the library, e.g.:
+        from Outlyzer.zscore import detect_outliers_zscore
+        from Outlyzer.iqr import detect_outliers_iqr
+
+    - Pass your dataset or data series to the respective function, e.g.:
+        outliers_zscore = detect_outliers_zscore(data)
+        outliers_iqr = detect_outliers_iqr(data)
+
+    - The functions will return a boolean array indicating whether each data point is an outlier (True) or not (False).
+
+'''
 
 # Setting up
 setup(
     name="Outlyzer",
     version=VERSION,
     author="Devendra Parihar",
     author_email="devendraparihar340@gmail.com",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['numpy', 'scipy', 'pandas', 'matplotlib'],
-    keywords=['outliers', 'outlier-detection', 'data-science', 'machine-learning'],
+    keywords=['outliers', 'outlier-detection', 'data-science', 'machine-learning', 'statistics', 'zscore', 'iqr', 'visualization'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

