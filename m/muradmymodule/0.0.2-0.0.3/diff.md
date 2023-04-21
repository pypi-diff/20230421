# Comparing `tmp/muradmymodule-0.0.2.tar.gz` & `tmp/muradmymodule-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muradmymodule-0.0.2.tar", last modified: Fri Apr 21 04:17:35 2023, max compression
+gzip compressed data, was "muradmymodule-0.0.3.tar", last modified: Fri Apr 21 06:23:03 2023, max compression
```

## Comparing `muradmymodule-0.0.2.tar` & `muradmymodule-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:17:35.858226 muradmymodule-0.0.2/
--rw-rw-rw-   0        0        0      618 2023-04-21 04:17:35.856225 muradmymodule-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 04:17:35.838428 muradmymodule-0.0.2/muradmymodule/
--rw-rw-rw-   0        0        0       50 2023-04-21 03:12:32.000000 muradmymodule-0.0.2/muradmymodule/__init__.py
--rw-rw-rw-   0        0        0       32 2023-04-21 04:07:57.000000 muradmymodule-0.0.2/muradmymodule/add.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:17:35.855226 muradmymodule-0.0.2/muradmymodule/extras/
--rw-rw-rw-   0        0        0       56 2023-04-21 03:13:22.000000 muradmymodule-0.0.2/muradmymodule/extras/__init__.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:08:35.000000 muradmymodule-0.0.2/muradmymodule/extras/divide.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:08:47.000000 muradmymodule-0.0.2/muradmymodule/extras/multiply.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:08:18.000000 muradmymodule-0.0.2/muradmymodule/subtract.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:17:35.846792 muradmymodule-0.0.2/muradmymodule.egg-info/
--rw-rw-rw-   0        0        0      618 2023-04-21 04:17:35.000000 muradmymodule-0.0.2/muradmymodule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-21 04:17:35.000000 muradmymodule-0.0.2/muradmymodule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:17:35.000000 muradmymodule-0.0.2/muradmymodule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-21 04:17:35.000000 muradmymodule-0.0.2/muradmymodule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 04:17:35.858226 muradmymodule-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-21 04:17:29.000000 muradmymodule-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:23:03.572328 muradmymodule-0.0.3/
+-rw-rw-rw-   0        0        0      626 2023-04-21 06:23:03.570323 muradmymodule-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 06:23:03.552550 muradmymodule-0.0.3/extras/
+-rw-rw-rw-   0        0        0       56 2023-04-21 03:13:22.000000 muradmymodule-0.0.3/extras/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:08:35.000000 muradmymodule-0.0.3/extras/divide.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:08:47.000000 muradmymodule-0.0.3/extras/multiply.py
+drwxrwxrwx   0        0        0        0 2023-04-21 06:23:03.567173 muradmymodule-0.0.3/muradmymodule.egg-info/
+-rw-rw-rw-   0        0        0      626 2023-04-21 06:23:02.000000 muradmymodule-0.0.3/muradmymodule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-21 06:23:02.000000 muradmymodule-0.0.3/muradmymodule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 06:23:02.000000 muradmymodule-0.0.3/muradmymodule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 06:23:02.000000 muradmymodule-0.0.3/muradmymodule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 06:23:03.572823 muradmymodule-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-04-21 06:22:39.000000 muradmymodule-0.0.3/setup.py
```

### Comparing `muradmymodule-0.0.2/PKG-INFO` & `muradmymodule-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: muradmymodule
-Version: 0.0.2
+Version: 0.0.3
 Summary: muradMy first Python package
 Home-page: UNKNOWN
 Author: murad delalisa
 Author-email: <youremail@email.com>
 License: UNKNOWN
-Description: muradMy first Python package with a slightly longer description
+Description: muradMy first Python package with a slightly longer description v 0.0.3
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `muradmymodule-0.0.2/muradmymodule.egg-info/PKG-INFO` & `muradmymodule-0.0.3/muradmymodule.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: muradmymodule
-Version: 0.0.2
+Version: 0.0.3
 Summary: muradMy first Python package
 Home-page: UNKNOWN
 Author: murad delalisa
 Author-email: <youremail@email.com>
 License: UNKNOWN
-Description: muradMy first Python package with a slightly longer description
+Description: muradMy first Python package with a slightly longer description v 0.0.3
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `muradmymodule-0.0.2/setup.py` & `muradmymodule-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3'
 DESCRIPTION = 'muradMy first Python package'
-LONG_DESCRIPTION = 'muradMy first Python package with a slightly longer description'
+LONG_DESCRIPTION = 'muradMy first Python package with a slightly longer description v 0.0.3'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="muradmymodule", 
         version=VERSION,
         author="murad delalisa",
```

