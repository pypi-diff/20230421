# Comparing `tmp/pymathematics-2023.4.20.1.tar.gz` & `tmp/pymathematics-2023.4.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.20.1.tar", last modified: Thu Apr 20 13:27:44 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.21.tar", last modified: Fri Apr 21 17:57:20 2023, max compression
```

## Comparing `pymathematics-2023.4.20.1.tar` & `pymathematics-2023.4.21.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.284042 pymathematics-2023.4.20.1/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.20.1/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-20 13:27:44.275037 pymathematics-2023.4.20.1/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      120 2023-04-20 13:23:25.000000 pymathematics-2023.4.20.1/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.045541 pymathematics-2023.4.20.1/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    15044 2023-04-20 13:23:01.000000 pymathematics-2023.4.20.1/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      113 2023-04-20 13:23:07.000000 pymathematics-2023.4.20.1/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-20 13:27:44.225534 pymathematics-2023.4.20.1/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-20 13:27:43.000000 pymathematics-2023.4.20.1/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-20 13:27:44.287043 pymathematics-2023.4.20.1/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      691 2023-04-20 13:23:20.000000 pymathematics-2023.4.20.1/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-21 17:57:20.174223 pymathematics-2023.4.21/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.21/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-21 17:57:20.157222 pymathematics-2023.4.21/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      123 2023-04-21 17:53:24.000000 pymathematics-2023.4.21/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-21 17:57:19.619222 pymathematics-2023.4.21/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    15520 2023-04-21 17:53:02.000000 pymathematics-2023.4.21/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-21 15:12:13.000000 pymathematics-2023.4.21/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-21 17:57:20.089228 pymathematics-2023.4.21/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-21 17:57:18.000000 pymathematics-2023.4.21/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-21 17:57:19.000000 pymathematics-2023.4.21/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-21 17:57:18.000000 pymathematics-2023.4.21/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-21 17:57:19.000000 pymathematics-2023.4.21/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-21 17:57:20.176223 pymathematics-2023.4.21/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-21 17:56:59.000000 pymathematics-2023.4.21/setup.py
```

### Comparing `pymathematics-2023.4.20.1/LICENSE` & `pymathematics-2023.4.21/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.20.1/pymathematics/__init__.py` & `pymathematics-2023.4.21/pymathematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         `projection of vector1 to vector2`
         """
         return vector.dot_product(vector1,vector2)/vector.magnitude(vector2)
 
     def angle_of_projection(vector1:list,vector2:list) -> float:
         return f"arccos({vector.dot_product(vector1,vector2)}/{(vector.magnitude(vector1)*vector.magnitude(vector2))})"
-    
+
 class matrix:
     def determinant(matrix_):
         if len(matrix_) == 1:
             return matrix_[0][0]
         elif len(matrix_) == 2:
             return matrix_[0][0]*matrix_[1][1]-matrix_[0][1]*matrix_[1][0]
         det = 0
@@ -280,14 +280,25 @@
         d = len(array)-1
     elif kind == "population":
         d = len(array)
     else:
         raise ValueError(f"invalid input {kind}! input should be whether 'population' or 'sample'")
     return summation((x - mean(array))**2 for x in array)/d
 
+def skewness(array:list) -> float:
+    if len(array) == 0:
+        raise ValueError("length of an array shouldn't be 0")
+    return summation((x - mean(array))**3 for x in array)/(len(array)*standard_deviation(array,"population")**3)
+
+def kurtosis(array:list) -> float:
+    if len(array) == 0:
+        raise ValueError("length of an array shouldn't be 0")
+    moment = summation((x - mean(array))**4 for x in array)/len(array)
+    return (moment/variance(array)**2)-3
+
 def mode(array:list) -> int|float:
     freq = {}
     for each in array:
         if each in freq:
             freq[each] += 1
         else:
             freq[each] = 1
```

### Comparing `pymathematics-2023.4.20.1/setup.py` & `pymathematics-2023.4.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.20.1",
+    version = "2023.4.21",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

