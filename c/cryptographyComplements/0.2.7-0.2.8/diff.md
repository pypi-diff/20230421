# Comparing `tmp/cryptographyComplements-0.2.7.tar.gz` & `tmp/cryptographyComplements-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.7.tar", last modified: Sun Apr 16 13:33:31 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.8.tar", last modified: Thu Apr 20 23:51:16 2023, max compression
```

## Comparing `cryptographyComplements-0.2.7.tar` & `cryptographyComplements-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.305603 cryptographyComplements-0.2.7/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-16 13:33:31.305101 cryptographyComplements-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.7/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.302051 cryptographyComplements-0.2.7/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.7/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.7/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.7/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2575 2023-04-10 21:54:35.000000 cryptographyComplements-0.2.7/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     3166 2023-04-16 13:32:27.000000 cryptographyComplements-0.2.7/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.304060 cryptographyComplements-0.2.7/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-16 13:33:31.000000 cryptographyComplements-0.2.7/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 13:33:31.306785 cryptographyComplements-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-16 13:33:11.000000 cryptographyComplements-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.808192 cryptographyComplements-0.2.8/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-20 23:51:16.807218 cryptographyComplements-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.8/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.804448 cryptographyComplements-0.2.8/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.8/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.8/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.8/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     3307 2023-04-20 23:46:09.000000 cryptographyComplements-0.2.8/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3292 2023-04-20 23:48:10.000000 cryptographyComplements-0.2.8/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:51:16.806217 cryptographyComplements-0.2.8/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-20 23:51:16.000000 cryptographyComplements-0.2.8/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 23:51:16.808192 cryptographyComplements-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-20 23:51:11.000000 cryptographyComplements-0.2.8/setup.py
```

### Comparing `cryptographyComplements-0.2.7/LICENSE` & `cryptographyComplements-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.7/PKG-INFO` & `cryptographyComplements-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.7/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.2.8/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.7/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.8/cryptographyComplements/mathFunctions.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.7/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.8/cryptographyComplements/primalityTests.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,8 +63,43 @@
 
     if EuclideanAlgorithm(p, a) != 1:
         return False
     
     if FermatLittleTheorem(a, p) == 1:
         return True
     
-    return False
+    return False
+
+import random
+
+def MillerRabinPrimalityTest(n: int, k: int) -> bool:
+    "Given a number: n, to check and k: the number of test to execute, see if the number is prime or not. This primality test is probabilistic."
+
+    if Numbers.isEven(n):
+        return False
+    
+
+    q = (n - 1) // 2
+    p = 1
+    while q % 2 == 0:
+        q //= 2
+        p += 1
+
+
+    for i in range(k):
+        a = random.randint(2, n - 2)
+
+        # x = (a**q) % n
+        x = pow(a, q, n)
+
+        for j in range(p):
+            y = (x**2) % n
+
+            if y == 1 and x != 1 and x != (n-1):
+                return False
+        
+            x = y
+
+        if y != 1:
+            return False
+        
+    return True
```

### Comparing `cryptographyComplements-0.2.7/cryptographyComplements/tools.py` & `cryptographyComplements-0.2.8/cryptographyComplements/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,46 +40,48 @@
                 continue
             else:
                 return False
             
         return True
 
     def listMultiplication(arg: list):
-        "From a given list or tuple in input, calculate the multiplication of the numbers inside it"
+        "From a given list or tuple in input, calculate the multiplication of the numbers inside it. \n\nNote: Non-numerical values will be skipped."
 
-        if isinstance(arg, int):
+        if isinstance(arg, int) or isinstance(arg, float):
             return arg
 
         result = 1
 
         for i in arg:
 
-            if not isinstance(i, int) and not isinstance(i, float):
-                return None
-
-            result *= int(i)
+            try:
+                result *= int(i)
+            
+            except ValueError:
+                continue
 
         return result
 
     def listSum(arg: list):
-        "From a given list or tuple in input, calculate the addition of the numbers inside it"
+        "From a given list or tuple in input, calculate the addition of the numbers inside it. \n\nNote: Non-numerical values will be skipped."
 
         
-        if isinstance(arg, int):
+        if isinstance(arg, int) or isinstance(arg, float):
             return arg
         
 
         result = 0
 
         for i in arg:
 
-            if not isinstance(i, int) and not isinstance(i, float):
-                return None
+            try:
+                result += int(i)
 
-            result += int(i)
+            except ValueError:
+                continue
 
         return result
     
 
 class stopwatch:
     "Create as many stopwatch as you need."
     def start():
```

### Comparing `cryptographyComplements-0.2.7/setup.py` & `cryptographyComplements-0.2.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.7',
+    version='0.2.8',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

