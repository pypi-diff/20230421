# Comparing `tmp/findlibs-0.0.2.tar.gz` & `tmp/findlibs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlibs-0.0.2.tar", last modified: Thu May 20 13:31:57 2021, max compression
+gzip compressed data, was "findlibs-0.0.3.tar", last modified: Fri Apr 21 08:32:11 2023, max compression
```

## Comparing `findlibs-0.0.2.tar` & `findlibs-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 13:31:57.613990 findlibs-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-05-20 13:31:50.000000 findlibs-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-05-20 13:31:57.613990 findlibs-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-05-20 13:31:50.000000 findlibs-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 13:31:57.613990 findlibs-0.0.2/findlibs/
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-05-20 13:31:50.000000 findlibs-0.0.2/findlibs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-20 13:31:57.613990 findlibs-0.0.2/findlibs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-05-20 13:31:57.000000 findlibs-0.0.2/findlibs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-05-20 13:31:57.000000 findlibs-0.0.2/findlibs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-20 13:31:57.000000 findlibs-0.0.2/findlibs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-05-20 13:31:57.000000 findlibs-0.0.2/findlibs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-20 13:31:57.000000 findlibs-0.0.2/findlibs.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-20 13:31:57.613990 findlibs-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-05-20 13:31:50.000000 findlibs-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 08:31:58.000000 findlibs-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 08:32:11.515379 findlibs-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-21 08:31:58.000000 findlibs-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/findlibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 08:31:58.000000 findlibs-0.0.3/findlibs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:32:11.515379 findlibs-0.0.3/findlibs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:32:11.000000 findlibs-0.0.3/findlibs.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:32:11.515379 findlibs-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-21 08:31:58.000000 findlibs-0.0.3/setup.py
```

### Comparing `findlibs-0.0.2/LICENSE` & `findlibs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `findlibs-0.0.2/PKG-INFO` & `findlibs-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: findlibs
-Version: 0.0.2
+Version: 0.0.3
 Summary: A packages to search for shared libraries on various platforms
 Home-page: https://github.com/ecmwf/findlibs
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
-Description: # findlibs
-        
-        A Python package that search for shared libraries on various platforms.
-        
-        
-        ```python
-        import findlibs
-        lib = findlibs.find("eccodes")
-        ```
-        
 Keywords: tool
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# findlibs
+
+A Python package that search for shared libraries on various platforms.
+
+```python
+import findlibs
+lib = findlibs.find("eccodes")
+
+# If package name differs from library name use:
+lib = findlibs.find(lib_name="odccore", pkg_name="odc")
+```
```

### Comparing `findlibs-0.0.2/findlibs.egg-info/PKG-INFO` & `findlibs-0.0.3/findlibs.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: findlibs
-Version: 0.0.2
+Version: 0.0.3
 Summary: A packages to search for shared libraries on various platforms
 Home-page: https://github.com/ecmwf/findlibs
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
-Description: # findlibs
-        
-        A Python package that search for shared libraries on various platforms.
-        
-        
-        ```python
-        import findlibs
-        lib = findlibs.find("eccodes")
-        ```
-        
 Keywords: tool
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# findlibs
+
+A Python package that search for shared libraries on various platforms.
+
+```python
+import findlibs
+lib = findlibs.find("eccodes")
+
+# If package name differs from library name use:
+lib = findlibs.find(lib_name="odccore", pkg_name="odc")
+```
```

### Comparing `findlibs-0.0.2/setup.py` & `findlibs-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 setuptools.setup(
     name="findlibs",
     version=version,
     description="A packages to search for shared libraries on various platforms",
     long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     author="European Centre for Medium-Range Weather Forecasts (ECMWF)",
     author_email="software.support@ecmwf.int",
     license="Apache License Version 2.0",
     url="https://github.com/ecmwf/findlibs",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[],
```

