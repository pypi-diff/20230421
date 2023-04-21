# Comparing `tmp/wasabicli-3.0.2.tar.gz` & `tmp/wasabicli-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasabicli-3.0.2.tar", last modified: Tue Mar  7 03:09:01 2023, max compression
+gzip compressed data, was "wasabicli-4.0.0.tar", last modified: Fri Apr 21 09:28:15 2023, max compression
```

## Comparing `wasabicli-3.0.2.tar` & `wasabicli-4.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.157198 wasabicli-3.0.2/
--rw-rw-rw-   0        0        0      181 2023-03-07 00:15:29.000000 wasabicli-3.0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     3682 2023-03-07 00:15:29.000000 wasabicli-3.0.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-03-07 00:15:29.000000 wasabicli-3.0.2/HISTORY.rst
--rw-rw-rw-   0        0        0     1617 2023-03-07 00:15:29.000000 wasabicli-3.0.2/LICENSE
--rw-rw-rw-   0        0        0      273 2023-03-07 00:15:29.000000 wasabicli-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1949 2023-03-07 03:09:01.157198 wasabicli-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-03-07 02:25:19.000000 wasabicli-3.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.109862 wasabicli-3.0.2/docs/
--rw-rw-rw-   0        0        0      630 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/authors.rst
--rw-rw-rw-   0        0        0     4990 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/history.rst
--rw-rw-rw-   0        0        0      326 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/index.rst
--rw-rw-rw-   0        0        0     1189 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/installation.rst
--rwxrwxrwx   0        0        0      807 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/readme.rst
--rw-rw-rw-   0        0        0       80 2023-03-07 00:15:29.000000 wasabicli-3.0.2/docs/usage.rst
--rw-rw-rw-   0        0        0      404 2023-03-07 03:09:01.157198 wasabicli-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1458 2023-03-07 03:08:54.000000 wasabicli-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.109862 wasabicli-3.0.2/tests/
--rw-rw-rw-   0        0        0       40 2023-03-07 00:15:29.000000 wasabicli-3.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      899 2023-03-07 00:15:29.000000 wasabicli-3.0.2/tests/test_wasabicli.py
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.125517 wasabicli-3.0.2/wasabicli/
--rw-rw-rw-   0        0        0      218 2023-03-07 02:25:19.000000 wasabicli-3.0.2/wasabicli/__init__.py
--rw-rw-rw-   0        0        0    13998 2023-03-07 03:08:54.000000 wasabicli-3.0.2/wasabicli/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.141549 wasabicli-3.0.2/wasabicli/utils/
--rw-rw-rw-   0        0        0      218 2023-03-07 02:23:26.000000 wasabicli-3.0.2/wasabicli/utils/__init__.py
--rw-rw-rw-   0        0        0      257 2023-03-07 00:17:08.000000 wasabicli-3.0.2/wasabicli/utils/formatter.py
--rw-rw-rw-   0        0        0    10827 2023-03-07 02:23:26.000000 wasabicli-3.0.2/wasabicli/wasabicli.py
-drwxrwxrwx   0        0        0        0 2023-03-07 03:09:01.141549 wasabicli-3.0.2/wasabicli.egg-info/
--rw-rw-rw-   0        0        0     1949 2023-03-07 03:09:00.000000 wasabicli-3.0.2/wasabicli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-03-07 03:09:01.000000 wasabicli-3.0.2/wasabicli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 03:09:00.000000 wasabicli-3.0.2/wasabicli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-03-07 03:09:00.000000 wasabicli-3.0.2/wasabicli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 00:47:29.000000 wasabicli-3.0.2/wasabicli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-03-07 03:09:00.000000 wasabicli-3.0.2/wasabicli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-07 03:09:00.000000 wasabicli-3.0.2/wasabicli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:15.082114 wasabicli-4.0.0/
+-rw-rw-rw-   0        0        0      181 2023-03-07 00:15:29.000000 wasabicli-4.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3682 2023-03-07 00:15:29.000000 wasabicli-4.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-03-07 00:15:29.000000 wasabicli-4.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1617 2023-03-07 00:15:29.000000 wasabicli-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-03-07 00:15:29.000000 wasabicli-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2022 2023-04-21 09:28:15.082114 wasabicli-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1082 2023-03-07 11:41:57.000000 wasabicli-4.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:14.998999 wasabicli-4.0.0/docs/
+-rw-rw-rw-   0        0        0      630 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     4990 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/history.rst
+-rw-rw-rw-   0        0        0      326 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1189 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      807 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-03-07 00:15:29.000000 wasabicli-4.0.0/docs/readme.rst
+-rw-rw-rw-   0        0        0      241 2023-03-07 11:49:51.000000 wasabicli-4.0.0/docs/usage.rst
+-rw-rw-rw-   0        0        0      404 2023-04-21 09:28:15.085115 wasabicli-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1458 2023-04-21 09:07:31.000000 wasabicli-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:15.020991 wasabicli-4.0.0/tests/
+-rw-rw-rw-   0        0        0       40 2023-03-07 00:15:29.000000 wasabicli-4.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      899 2023-03-07 00:15:29.000000 wasabicli-4.0.0/tests/test_wasabicli.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:15.034328 wasabicli-4.0.0/wasabicli/
+-rw-rw-rw-   0        0        0      218 2023-03-07 02:25:19.000000 wasabicli-4.0.0/wasabicli/__init__.py
+-rw-rw-rw-   0        0        0    13998 2023-03-07 03:08:54.000000 wasabicli-4.0.0/wasabicli/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:15.081114 wasabicli-4.0.0/wasabicli/utils/
+-rw-rw-rw-   0        0        0      218 2023-03-07 02:23:26.000000 wasabicli-4.0.0/wasabicli/utils/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-03-07 00:17:08.000000 wasabicli-4.0.0/wasabicli/utils/formatter.py
+-rw-rw-rw-   0        0        0    10827 2023-03-07 02:23:26.000000 wasabicli-4.0.0/wasabicli/wasabicli.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:28:15.069592 wasabicli-4.0.0/wasabicli.egg-info/
+-rw-rw-rw-   0        0        0     2022 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 00:47:29.000000 wasabicli-4.0.0/wasabicli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 09:28:14.000000 wasabicli-4.0.0/wasabicli.egg-info/top_level.txt
```

### Comparing `wasabicli-3.0.2/CONTRIBUTING.rst` & `wasabicli-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/LICENSE` & `wasabicli-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/PKG-INFO` & `wasabicli-4.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasabicli
-Version: 3.0.2
+Version: 4.0.0
 Summary: CLI application for management of versioned Wasabi S3 buckets
 Home-page: https://github.com/salimdason/wasabicli
 Author: Mohammed Salim Dason
 Author-email: salimdason@outlook.com
 License: GNU General Public License v3
 Keywords: wasabicli
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,27 +38,29 @@
 
 .. image:: https://pyup.io/repos/github/salimdason/wasabicli/shield.svg
      :target: https://pyup.io/repos/github/salimdason/wasabicli/
      :alt: Updates
 
 
 
-CLI application for management of versioned Wasabi S3 buckets
+CLI application for management of versioned Wasabi S3 buckets. This should also in theory work for AWS S3 buckets.
+
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://wasabi-cli.readthedocs.io/en/latest/index.html
 
 
+
 Features
 --------
 1. Delete only non-current objects
 2. Delete both current and non-current objects
 3. Purge delete markers from bucket
-4. Delete bucket (after running above commands to ensure it's empty)
+4. Delete bucket (Runs all commands above to ensure bucket is empty before deletion)
 
 
 
 =======
 History
 =======
```

### Comparing `wasabicli-3.0.2/README.rst` & `wasabicli-4.0.0/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 
 .. image:: https://pyup.io/repos/github/salimdason/wasabicli/shield.svg
      :target: https://pyup.io/repos/github/salimdason/wasabicli/
      :alt: Updates
 
 
 
-CLI application for management of versioned Wasabi S3 buckets
+CLI application for management of versioned Wasabi S3 buckets. This should also in theory work for AWS S3 buckets.
+
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://wasabi-cli.readthedocs.io/en/latest/index.html
 
 
+
 Features
 --------
 1. Delete only non-current objects
 2. Delete both current and non-current objects
 3. Purge delete markers from bucket
-4. Delete bucket (after running above commands to ensure it's empty)
+4. Delete bucket (Runs all commands above to ensure bucket is empty before deletion)
```

### Comparing `wasabicli-3.0.2/docs/Makefile` & `wasabicli-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/docs/conf.py` & `wasabicli-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/docs/installation.rst` & `wasabicli-4.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/docs/make.bat` & `wasabicli-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/setup.py` & `wasabicli-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='wasabicli',
     name='wasabicli',
     packages=find_packages(include=['wasabicli', 'wasabicli.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/salimdason/wasabicli',
-    version='3.0.2',
+    version='4.0.0',
     zip_safe=False,
 )
```

### Comparing `wasabicli-3.0.2/tests/test_wasabicli.py` & `wasabicli-4.0.0/tests/test_wasabicli.py`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/wasabicli/cli.py` & `wasabicli-4.0.0/wasabicli/cli.py`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/wasabicli/wasabicli.py` & `wasabicli-4.0.0/wasabicli/wasabicli.py`

 * *Files identical despite different names*

### Comparing `wasabicli-3.0.2/wasabicli.egg-info/PKG-INFO` & `wasabicli-4.0.0/wasabicli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasabicli
-Version: 3.0.2
+Version: 4.0.0
 Summary: CLI application for management of versioned Wasabi S3 buckets
 Home-page: https://github.com/salimdason/wasabicli
 Author: Mohammed Salim Dason
 Author-email: salimdason@outlook.com
 License: GNU General Public License v3
 Keywords: wasabicli
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,27 +38,29 @@
 
 .. image:: https://pyup.io/repos/github/salimdason/wasabicli/shield.svg
      :target: https://pyup.io/repos/github/salimdason/wasabicli/
      :alt: Updates
 
 
 
-CLI application for management of versioned Wasabi S3 buckets
+CLI application for management of versioned Wasabi S3 buckets. This should also in theory work for AWS S3 buckets.
+
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://wasabi-cli.readthedocs.io/en/latest/index.html
 
 
+
 Features
 --------
 1. Delete only non-current objects
 2. Delete both current and non-current objects
 3. Purge delete markers from bucket
-4. Delete bucket (after running above commands to ensure it's empty)
+4. Delete bucket (Runs all commands above to ensure bucket is empty before deletion)
 
 
 
 =======
 History
 =======
```

### Comparing `wasabicli-3.0.2/wasabicli.egg-info/SOURCES.txt` & `wasabicli-4.0.0/wasabicli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

