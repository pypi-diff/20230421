# Comparing `tmp/data-diode-0.0.1.tar.gz` & `tmp/data-diode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-diode-0.0.1.tar", last modified: Fri Apr 21 14:34:25 2023, max compression
+gzip compressed data, was "data-diode-0.0.2.tar", last modified: Fri Apr 21 14:59:12 2023, max compression
```

## Comparing `data-diode-0.0.1.tar` & `data-diode-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:25.309183 data-diode-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 14:34:25.309183 data-diode-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-21 14:34:07.000000 data-diode-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:25.309183 data-diode-0.0.1/data_diode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:34:16.000000 data-diode-0.0.1/data_diode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 14:34:25.000000 data-diode-0.0.1/data_diode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:25.309183 data-diode-0.0.1/diode/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 14:34:07.000000 data-diode-0.0.1/diode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-21 14:34:07.000000 data-diode-0.0.1/diode/core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-21 14:34:07.000000 data-diode-0.0.1/diode/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:34:07.000000 data-diode-0.0.1/diode/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (123)     7937 2023-04-21 14:34:07.000000 data-diode-0.0.1/diode/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 14:34:07.000000 data-diode-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-21 14:34:25.309183 data-diode-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:34:07.000000 data-diode-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:59:12.153430 data-diode-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-21 14:59:12.153430 data-diode-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-21 14:58:55.000000 data-diode-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:59:12.149430 data-diode-0.0.2/data_diode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:59:04.000000 data-diode-0.0.2/data_diode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-21 14:59:12.000000 data-diode-0.0.2/data_diode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:59:12.149430 data-diode-0.0.2/diode/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 14:58:55.000000 data-diode-0.0.2/diode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-21 14:58:55.000000 data-diode-0.0.2/diode/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-21 14:58:55.000000 data-diode-0.0.2/diode/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:58:55.000000 data-diode-0.0.2/diode/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7937 2023-04-21 14:58:55.000000 data-diode-0.0.2/diode/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 14:58:55.000000 data-diode-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 14:59:12.153430 data-diode-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:58:55.000000 data-diode-0.0.2/setup.py
```

### Comparing `data-diode-0.0.1/PKG-INFO` & `data-diode-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data-diode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Send and receive data over serial diode
 Home-page: https://github.com/fionn/diode
 Author: Fionn Fitzmaurice
 Project-URL: Source Code, https://github.com/fionn/diode
 Project-URL: Changelog, https://github.com/fionn/diode/tags
 Project-URL: Documentation, https://github.com/fionn/diode/blob/master/README.md
 Project-URL: Bug Tracker, https://github.com/fionn/diode/issues
-Project-URL: PyPI, https://pypi.org/project/diode/
+Project-URL: PyPI, https://pypi.org/project/data-diode/
 Project-URL: Download, https://github.com/fionn/diode/archive/refs/heads/master.zip
 Keywords: diode,data diode
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Typing :: Typed
@@ -61,14 +61,16 @@
 
 ## Installation
 
 Install in developer mode with `make install_dev && source venv/bin/activate`.
 
 Install as user with `make install`.
 
+Install [from PyPI](https://pypi.org/project/data-diode/) with `pip install data-diode`.
+
 Install Bash completion with `source bash_completion/diode`.
 
 ## Testing
 
 Run `make test`.
 
 For ad-hoc testing, `socat -d -d pty,raw,echo=0 pty,raw,echo=0` can be useful to connect two virtual serial devices.
```

### Comparing `data-diode-0.0.1/README.md` & `data-diode-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 ## Installation
 
 Install in developer mode with `make install_dev && source venv/bin/activate`.
 
 Install as user with `make install`.
 
+Install [from PyPI](https://pypi.org/project/data-diode/) with `pip install data-diode`.
+
 Install Bash completion with `source bash_completion/diode`.
 
 ## Testing
 
 Run `make test`.
 
 For ad-hoc testing, `socat -d -d pty,raw,echo=0 pty,raw,echo=0` can be useful to connect two virtual serial devices.
```

### Comparing `data-diode-0.0.1/data_diode.egg-info/PKG-INFO` & `data-diode-0.0.2/data_diode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data-diode
-Version: 0.0.1
+Version: 0.0.2
 Summary: Send and receive data over serial diode
 Home-page: https://github.com/fionn/diode
 Author: Fionn Fitzmaurice
 Project-URL: Source Code, https://github.com/fionn/diode
 Project-URL: Changelog, https://github.com/fionn/diode/tags
 Project-URL: Documentation, https://github.com/fionn/diode/blob/master/README.md
 Project-URL: Bug Tracker, https://github.com/fionn/diode/issues
-Project-URL: PyPI, https://pypi.org/project/diode/
+Project-URL: PyPI, https://pypi.org/project/data-diode/
 Project-URL: Download, https://github.com/fionn/diode/archive/refs/heads/master.zip
 Keywords: diode,data diode
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Typing :: Typed
@@ -61,14 +61,16 @@
 
 ## Installation
 
 Install in developer mode with `make install_dev && source venv/bin/activate`.
 
 Install as user with `make install`.
 
+Install [from PyPI](https://pypi.org/project/data-diode/) with `pip install data-diode`.
+
 Install Bash completion with `source bash_completion/diode`.
 
 ## Testing
 
 Run `make test`.
 
 For ad-hoc testing, `socat -d -d pty,raw,echo=0 pty,raw,echo=0` can be useful to connect two virtual serial devices.
```

### Comparing `data-diode-0.0.1/diode/core.py` & `data-diode-0.0.2/diode/core.py`

 * *Files identical despite different names*

### Comparing `data-diode-0.0.1/diode/main.py` & `data-diode-0.0.2/diode/main.py`

 * *Files identical despite different names*

### Comparing `data-diode-0.0.1/diode/test.py` & `data-diode-0.0.2/diode/test.py`

 * *Files identical despite different names*

### Comparing `data-diode-0.0.1/setup.cfg` & `data-diode-0.0.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	Topic :: Security
 	Typing :: Typed
 project_urls = 
 	Source Code = https://github.com/fionn/diode
 	Changelog = https://github.com/fionn/diode/tags
 	Documentation = https://github.com/fionn/diode/blob/master/README.md
 	Bug Tracker = https://github.com/fionn/diode/issues
-	PyPI = https://pypi.org/project/diode/
+	PyPI = https://pypi.org/project/data-diode/
 	Download = https://github.com/fionn/diode/archive/refs/heads/master.zip
 
 [options]
 zip_safe = false
 pymodules = diode
 include_package_data = true
 packages = find:
```

