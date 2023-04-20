# Comparing `tmp/nmodl_preprocessor-1.0.2.tar.gz` & `tmp/nmodl_preprocessor-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.2.tar", last modified: Wed Apr 19 23:45:51 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.3.tar", last modified: Thu Apr 20 00:16:27 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.2.tar` & `nmodl_preprocessor-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.2/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.2/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.2/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1089 2023-04-17 16:48:55.000000 nmodl_preprocessor-1.0.2/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)    14444 2023-04-19 23:31:48.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     3664 2023-04-19 22:43:58.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     2994 2023-04-19 23:30:29.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      480 2023-04-19 21:45:07.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      444 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-04-19 23:45:51.000000 nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/top_level.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      971 2023-04-19 23:36:20.000000 nmodl_preprocessor-1.0.2/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:45:51.358063 nmodl_preprocessor-1.0.2/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 00:16:27.435535 nmodl_preprocessor-1.0.3/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.3/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.3/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.3/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-20 00:16:27.435535 nmodl_preprocessor-1.0.3/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1089 2023-04-17 16:48:55.000000 nmodl_preprocessor-1.0.3/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 00:16:27.431535 nmodl_preprocessor-1.0.3/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)    14444 2023-04-19 23:31:48.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     3664 2023-04-19 22:43:58.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2994 2023-04-19 23:30:29.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      480 2023-04-19 21:45:07.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-04-20 00:16:27.431535 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1830 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      444 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-04-20 00:16:27.000000 nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/top_level.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-04-20 00:16:03.000000 nmodl_preprocessor-1.0.3/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-20 00:16:27.435535 nmodl_preprocessor-1.0.3/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.2/DETAILS.pdf` & `nmodl_preprocessor-1.0.3/DETAILS.pdf`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/LICENSE.txt` & `nmodl_preprocessor-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/PKG-INFO` & `nmodl_preprocessor-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
-Project-URL: homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
+Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
```

### Comparing `nmodl_preprocessor-1.0.2/README.md` & `nmodl_preprocessor-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/nmodl_preprocessor/__main__.py` & `nmodl_preprocessor-1.0.3/nmodl_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/nmodl_preprocessor/nmodl_to_python.py` & `nmodl_preprocessor-1.0.3/nmodl_preprocessor/nmodl_to_python.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/nmodl_preprocessor/rw_patterns.py` & `nmodl_preprocessor-1.0.3/nmodl_preprocessor/rw_patterns.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.2/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.3/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.2
+Version: 1.0.3
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
-Project-URL: homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
+Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
```

### Comparing `nmodl_preprocessor-1.0.2/pyproject.toml` & `nmodl_preprocessor-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["nmodl_preprocessor"]
+
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.2"
+version = "1.0.3"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
+license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
-license = {text = "MIT"}
+urls = {Homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"}
 keywords = ["nmodl", "neuron"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Development Status :: 5 - Production/Stable",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.7"
 dependencies = ["nmodl"]
-
-[project.urls]
-homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"
-
-[tool.setuptools]
-packages = ["nmodl_preprocessor"]
-
-[project.scripts]
-nmodl_preprocessor = "nmodl_preprocessor:__main__._placeholder"
+scripts = {nmodl_preprocessor = "nmodl_preprocessor:__main__._placeholder"}
```

