# Comparing `tmp/pychi-0.0.8.tar.gz` & `tmp/pychi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychi-0.0.8.tar", last modified: Wed Apr 12 07:37:05 2023, max compression
+gzip compressed data, was "pychi-0.0.9.tar", last modified: Wed Apr 12 09:28:27 2023, max compression
```

## Comparing `pychi-0.0.8.tar` & `pychi-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 07:36:42.000000 pychi-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-12 07:37:05.390815 pychi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-12 07:36:42.000000 pychi-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 07:36:56.000000 pychi-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:37:05.390815 pychi-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.386815 pychi-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/src/pychi/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/light.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-04-12 07:36:42.000000 pychi-0.0.8/src/pychi/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:37:05.390815 pychi-0.0.8/src/pychi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 07:37:05.000000 pychi-0.0.8/src/pychi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:28:27.491090 pychi-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 09:28:11.000000 pychi-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-04-12 09:28:27.491090 pychi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-12 09:28:11.000000 pychi-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 09:28:20.000000 pychi-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:28:27.491090 pychi-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:28:27.487090 pychi-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:28:27.491090 pychi-0.0.9/src/pychi/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 09:28:11.000000 pychi-0.0.9/src/pychi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-12 09:28:11.000000 pychi-0.0.9/src/pychi/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-12 09:28:11.000000 pychi-0.0.9/src/pychi/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-04-12 09:28:11.000000 pychi-0.0.9/src/pychi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-04-12 09:28:11.000000 pychi-0.0.9/src/pychi/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:28:27.491090 pychi-0.0.9/src/pychi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-04-12 09:28:27.000000 pychi-0.0.9/src/pychi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 09:28:27.000000 pychi-0.0.9/src/pychi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:28:27.000000 pychi-0.0.9/src/pychi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 09:28:27.000000 pychi-0.0.9/src/pychi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 09:28:27.000000 pychi-0.0.9/src/pychi.egg-info/top_level.txt
```

### Comparing `pychi-0.0.8/LICENSE` & `pychi-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pychi-0.0.8/PKG-INFO` & `pychi-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simulation package for the propagation of optical pulses in nonlinear media
 Author-email: Ultrafast Microphotonics Group - DESY <pychi@desy.de>
 Project-URL: Homepage, https://github.com/pychi-code/pychi
 Project-URL: Documentation, https://pychi.readthedocs.io/en/latest/index.html
 Project-URL: PyPI, https://pypi.org/project/pychi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,19 +33,30 @@
 ## Installation
 
 First, make sure pip is up-to-date using
 ```
 pip install --upgrade pip
 ```
 
-Then install the package using
+On Windows, install the package using
 ```
 pip install pychi
 ```
 
+On Mac, one might have to first run
+```
+pip install pyfftw
+```
+
+before using
+```
+pip install pychi
+```
+
+
 ## Documentation
 
 The documentation is available and best viewed under
 https://pychi.readthedocs.io/en/latest/
 This documentation has been automatically generated using SPHINX, and is still a work in progress. Do not hesitate to contact us for any needed clarifications and examples.
 
 ## Example
```

### Comparing `pychi-0.0.8/README.md` & `pychi-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,30 @@
 ## Installation
 
 First, make sure pip is up-to-date using
 ```
 pip install --upgrade pip
 ```
 
-Then install the package using
+On Windows, install the package using
 ```
 pip install pychi
 ```
 
+On Mac, one might have to first run
+```
+pip install pyfftw
+```
+
+before using
+```
+pip install pychi
+```
+
+
 ## Documentation
 
 The documentation is available and best viewed under
 https://pychi.readthedocs.io/en/latest/
 This documentation has been automatically generated using SPHINX, and is still a work in progress. Do not hesitate to contact us for any needed clarifications and examples.
 
 ## Example
```

### Comparing `pychi-0.0.8/pyproject.toml` & `pychi-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-dir]
 "" = "src"
 
 [project]
 name = "pychi"
-version = "0.0.8"
+version = "0.0.9"
 description = "Simulation package for the propagation of optical pulses in nonlinear media"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent"
 ]
 dependencies = [
-  "matplotlib==3.1.3",
+  "matplotlib>=3.1.3",
   "numpy==1.21.6",
   "scipy==1.4.1",
   "numba==0.56.0",
-  "pyFFTW==0.12.0"
+  "pyFFTW>=0.12.0"
 ]
 
   [[project.authors]]
   name = "Ultrafast Microphotonics Group - DESY"
   email = "pychi@desy.de"
 
   [project.urls]
```

### Comparing `pychi-0.0.8/src/pychi/light.py` & `pychi-0.0.9/src/pychi/light.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.8/src/pychi/materials.py` & `pychi-0.0.9/src/pychi/materials.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.8/src/pychi/models.py` & `pychi-0.0.9/src/pychi/models.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.8/src/pychi/solvers.py` & `pychi-0.0.9/src/pychi/solvers.py`

 * *Files identical despite different names*

### Comparing `pychi-0.0.8/src/pychi.egg-info/PKG-INFO` & `pychi-0.0.9/src/pychi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simulation package for the propagation of optical pulses in nonlinear media
 Author-email: Ultrafast Microphotonics Group - DESY <pychi@desy.de>
 Project-URL: Homepage, https://github.com/pychi-code/pychi
 Project-URL: Documentation, https://pychi.readthedocs.io/en/latest/index.html
 Project-URL: PyPI, https://pypi.org/project/pychi/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,19 +33,30 @@
 ## Installation
 
 First, make sure pip is up-to-date using
 ```
 pip install --upgrade pip
 ```
 
-Then install the package using
+On Windows, install the package using
 ```
 pip install pychi
 ```
 
+On Mac, one might have to first run
+```
+pip install pyfftw
+```
+
+before using
+```
+pip install pychi
+```
+
+
 ## Documentation
 
 The documentation is available and best viewed under
 https://pychi.readthedocs.io/en/latest/
 This documentation has been automatically generated using SPHINX, and is still a work in progress. Do not hesitate to contact us for any needed clarifications and examples.
 
 ## Example
```

