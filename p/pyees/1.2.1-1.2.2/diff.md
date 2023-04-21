# Comparing `tmp/pyees-1.2.1.tar.gz` & `tmp/pyees-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.1.tar", last modified: Fri Apr 21 11:06:18 2023, max compression
+gzip compressed data, was "pyees-1.2.2.tar", last modified: Fri Apr 21 11:08:58 2023, max compression
```

## Comparing `pyees-1.2.1.tar` & `pyees-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:06:17.995746 pyees-1.2.1/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-04-21 11:06:18.011371 pyees-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:06:17.745735 pyees-1.2.1/pyees/
--rw-rw-rw-   0        0        0      463 2023-04-19 10:58:55.000000 pyees-1.2.1/pyees/__init__.py
--rw-rw-rw-   0        0        0    15015 2023-04-19 12:43:26.000000 pyees-1.2.1/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.1/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9051 2023-04-21 09:09:36.000000 pyees-1.2.1/pyees/prop.py
--rw-rw-rw-   0        0        0    14724 2023-04-19 09:10:47.000000 pyees-1.2.1/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.2.1/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.1/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3889 2023-04-19 12:43:28.000000 pyees-1.2.1/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-04-21 11:06:00.000000 pyees-1.2.1/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-19 12:41:29.000000 pyees-1.2.1/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15043 2023-04-19 08:45:19.000000 pyees-1.2.1/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.1/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.1/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81276 2023-04-19 12:40:55.000000 pyees-1.2.1/pyees/testVariable.py
--rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.1/pyees/unit.py
--rw-rw-rw-   0        0        0    34969 2023-04-19 12:41:14.000000 pyees-1.2.1/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:06:17.948869 pyees-1.2.1/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-04-21 11:06:16.000000 pyees-1.2.1/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-21 11:06:16.000000 pyees-1.2.1/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:06:16.000000 pyees-1.2.1/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-21 11:06:16.000000 pyees-1.2.1/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 11:06:16.000000 pyees-1.2.1/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 11:06:18.042624 pyees-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-04-21 11:06:11.000000 pyees-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:08:58.267170 pyees-1.2.2/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-04-21 11:08:58.282795 pyees-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 11:08:57.954655 pyees-1.2.2/pyees/
+-rw-rw-rw-   0        0        0      445 2023-04-21 11:08:47.000000 pyees-1.2.2/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15015 2023-04-19 12:43:26.000000 pyees-1.2.2/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.2/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9051 2023-04-21 09:09:36.000000 pyees-1.2.2/pyees/prop.py
+-rw-rw-rw-   0        0        0    14724 2023-04-19 09:10:47.000000 pyees-1.2.2/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.2.2/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.2/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3889 2023-04-19 12:43:28.000000 pyees-1.2.2/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-04-21 11:06:00.000000 pyees-1.2.2/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-19 12:41:29.000000 pyees-1.2.2/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15043 2023-04-19 08:45:19.000000 pyees-1.2.2/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.2/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8958 2023-04-15 19:26:44.000000 pyees-1.2.2/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81276 2023-04-19 12:40:55.000000 pyees-1.2.2/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    45294 2023-04-15 19:24:42.000000 pyees-1.2.2/pyees/unit.py
+-rw-rw-rw-   0        0        0    34969 2023-04-19 12:41:14.000000 pyees-1.2.2/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-21 11:08:58.157789 pyees-1.2.2/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 11:08:56.000000 pyees-1.2.2/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-21 11:08:58.298422 pyees-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-04-21 11:08:50.000000 pyees-1.2.2/setup.py
```

### Comparing `pyees-1.2.1/LICENSE.txt` & `pyees-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/PKG-INFO` & `pyees-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.1
+Version: 1.2.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.1/README.md` & `pyees-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/fit.py` & `pyees-1.2.2/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/profilePyees.py` & `pyees-1.2.2/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/prop.py` & `pyees-1.2.2/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/readData.py` & `pyees-1.2.2/pyees/readData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/solve.py` & `pyees-1.2.2/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/stackOverflowODR.py` & `pyees-1.2.2/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testFit.py` & `pyees-1.2.2/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testProp.py` & `pyees-1.2.2/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testPyees.py` & `pyees-1.2.2/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testReadData.py` & `pyees-1.2.2/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testSolve.py` & `pyees-1.2.2/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testUnit.py` & `pyees-1.2.2/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/testVariable.py` & `pyees-1.2.2/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/unit.py` & `pyees-1.2.2/pyees/unit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees/variable.py` & `pyees-1.2.2/pyees/variable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.1/pyees.egg-info/PKG-INFO` & `pyees-1.2.2/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.1
+Version: 1.2.2
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.1/setup.py` & `pyees-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.1',
+    version='1.2.2',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

