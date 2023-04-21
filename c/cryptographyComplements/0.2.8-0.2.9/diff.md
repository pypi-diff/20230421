# Comparing `tmp/cryptographyComplements-0.2.8.tar.gz` & `tmp/cryptographyComplements-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.8.tar", last modified: Thu Apr 20 23:51:16 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.9.tar", last modified: Fri Apr 21 00:20:29 2023, max compression
```

## Comparing `cryptographyComplements-0.2.8.tar` & `cryptographyComplements-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.808192 cryptographyComplements-0.2.8/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-20 23:51:16.807218 cryptographyComplements-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.804448 cryptographyComplements-0.2.8/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.8/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.8/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.8/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     3307 2023-04-20 23:46:09.000000 cryptographyComplements-0.2.8/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     3292 2023-04-20 23:48:10.000000 cryptographyComplements-0.2.8/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.806217 cryptographyComplements-0.2.8/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-20 23:51:16.000000 cryptographyComplements-0.2.8/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 23:51:16.808192 cryptographyComplements-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-20 23:51:11.000000 cryptographyComplements-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.354103 cryptographyComplements-0.2.9/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-21 00:20:29.354103 cryptographyComplements-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.9/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.349404 cryptographyComplements-0.2.9/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.9/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.9/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    10528 2023-04-21 00:19:12.000000 cryptographyComplements-0.2.9/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     3307 2023-04-20 23:46:09.000000 cryptographyComplements-0.2.9/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3292 2023-04-20 23:48:10.000000 cryptographyComplements-0.2.9/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:20:29.353103 cryptographyComplements-0.2.9/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-21 00:20:29.000000 cryptographyComplements-0.2.9/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 00:20:29.355322 cryptographyComplements-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-21 00:20:24.000000 cryptographyComplements-0.2.9/setup.py
```

### Comparing `cryptographyComplements-0.2.8/LICENSE` & `cryptographyComplements-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.8/PKG-INFO` & `cryptographyComplements-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.8/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.2.9/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.8/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.9/cryptographyComplements/mathFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,8 +312,15 @@
 
     if EuclideanAlgorithm(a, p*q) != 1:
         return False
 
     if pow(a, (p-1)*(q-1)//g, p*q) != 1:
         return False
 
-    return True
+    return True
+
+
+def PrimeNumberTheorem(number: int) -> float:
+    "Given a number, calculate using the Natural Logarithm how much primes are below that number. \n\nNote: Value is an estimate."
+    import math
+
+    return number / (math.log(number))
```

### Comparing `cryptographyComplements-0.2.8/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.9/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.8/cryptographyComplements/tools.py` & `cryptographyComplements-0.2.9/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.8/setup.py` & `cryptographyComplements-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.8',
+    version='0.2.9',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

