# Comparing `tmp/binn-0.0.1.tar.gz` & `tmp/binn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binn-0.0.1.tar", last modified: Fri Apr 21 09:03:14 2023, max compression
+gzip compressed data, was "binn-0.0.2.tar", last modified: Fri Apr 21 09:25:23 2023, max compression
```

## Comparing `binn-0.0.1.tar` & `binn-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:03:14.284349 binn-0.0.1/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1086 2023-01-24 09:18:18.000000 binn-0.0.1/LICENSE
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     6273 2023-04-21 09:03:14.280349 binn-0.0.1/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     5488 2023-04-21 08:16:21.000000 binn-0.0.1/README.md
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:03:14.280349 binn-0.0.1/binn/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      196 2023-04-21 08:16:21.000000 binn-0.0.1/binn/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    13183 2023-04-21 08:16:21.000000 binn-0.0.1/binn/binn.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     7455 2023-04-21 08:16:21.000000 binn-0.0.1/binn/explainer.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      641 2023-04-21 08:16:21.000000 binn-0.0.1/binn/logger.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    22646 2023-04-21 08:16:21.000000 binn-0.0.1/binn/network.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    14431 2023-04-21 08:16:21.000000 binn-0.0.1/binn/plot.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     4892 2023-04-21 08:16:21.000000 binn-0.0.1/binn/sklearn.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:03:14.280349 binn-0.0.1/binn.egg-info/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     6273 2023-04-21 09:03:14.000000 binn-0.0.1/binn.egg-info/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      288 2023-04-21 09:03:14.000000 binn-0.0.1/binn.egg-info/SOURCES.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2023-04-21 09:03:14.000000 binn-0.0.1/binn.egg-info/dependency_links.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       51 2023-04-21 09:03:14.000000 binn-0.0.1/binn.egg-info/requires.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        5 2023-04-21 09:03:14.000000 binn-0.0.1/binn.egg-info/top_level.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      772 2023-04-21 08:59:19.000000 binn-0.0.1/pyproject.toml
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2023-04-21 09:03:14.284349 binn-0.0.1/setup.cfg
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      452 2023-04-21 08:59:49.000000 binn-0.0.1/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:25:23.861841 binn-0.0.2/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1086 2023-01-24 09:18:18.000000 binn-0.0.2/LICENSE
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     6295 2023-04-21 09:25:23.861841 binn-0.0.2/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     5510 2023-04-21 09:21:30.000000 binn-0.0.2/README.md
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:25:23.861841 binn-0.0.2/binn/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      196 2023-04-21 08:16:21.000000 binn-0.0.2/binn/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    13183 2023-04-21 08:16:21.000000 binn-0.0.2/binn/binn.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     7455 2023-04-21 08:16:21.000000 binn-0.0.2/binn/explainer.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      641 2023-04-21 08:16:21.000000 binn-0.0.2/binn/logger.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    22646 2023-04-21 08:16:21.000000 binn-0.0.2/binn/network.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    14431 2023-04-21 08:16:21.000000 binn-0.0.2/binn/plot.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     4892 2023-04-21 08:16:21.000000 binn-0.0.2/binn/sklearn.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-04-21 09:25:23.861841 binn-0.0.2/binn.egg-info/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     6295 2023-04-21 09:25:23.000000 binn-0.0.2/binn.egg-info/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      288 2023-04-21 09:25:23.000000 binn-0.0.2/binn.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2023-04-21 09:25:23.000000 binn-0.0.2/binn.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       69 2023-04-21 09:25:23.000000 binn-0.0.2/binn.egg-info/requires.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        5 2023-04-21 09:25:23.000000 binn-0.0.2/binn.egg-info/top_level.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      772 2023-04-21 09:25:15.000000 binn-0.0.2/pyproject.toml
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2023-04-21 09:25:23.861841 binn-0.0.2/setup.cfg
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      483 2023-04-21 09:24:46.000000 binn-0.0.2/setup.py
```

### Comparing `binn-0.0.1/LICENSE` & `binn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/PKG-INFO` & `binn-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to generate and interpret biologically informed neural networks.
 Home-page: https://github.com/InfectionMedicineProteomics/BINN
 Author: Erik Hartman
 Author-email: Erik Hartman <erik.hartman@hotmail.com>, Aaron Scott <aaron.scott@med.lu.se>
 License: MIT
 Project-URL: Homepage, https://infectionmedicineproteomics.github.io/BINN/
 Project-URL: Bug Tracker, https://github.com/InfectionMedicineProteomics/BINN/issues
@@ -137,15 +137,15 @@
 Plotting a subgraph starting from a node generates the plot:
 ![Pathway sankey!](/img/sankey.png "Pathway sankey")
 A compelte sankey may look like this:
 ![Complete sankey!](/img/test.png "Complete sankey")
 
 ## Installation
 
-The package can be installed with git.
+The package can be installed and built from source with git.
 
 ```
 git clone git@github.com:InfectionMedicineProteomics/BINN.git
 pip install -e BINN/
 ```
 
 ## Testing
```

### Comparing `binn-0.0.1/README.md` & `binn-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 Plotting a subgraph starting from a node generates the plot:
 ![Pathway sankey!](/img/sankey.png "Pathway sankey")
 A compelte sankey may look like this:
 ![Complete sankey!](/img/test.png "Complete sankey")
 
 ## Installation
 
-The package can be installed with git.
+The package can be installed and built from source with git.
 
 ```
 git clone git@github.com:InfectionMedicineProteomics/BINN.git
 pip install -e BINN/
 ```
 
 ## Testing
```

### Comparing `binn-0.0.1/binn/binn.py` & `binn-0.0.2/binn/binn.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn/explainer.py` & `binn-0.0.2/binn/explainer.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn/logger.py` & `binn-0.0.2/binn/logger.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn/network.py` & `binn-0.0.2/binn/network.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn/plot.py` & `binn-0.0.2/binn/plot.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn/sklearn.py` & `binn-0.0.2/binn/sklearn.py`

 * *Files identical despite different names*

### Comparing `binn-0.0.1/binn.egg-info/PKG-INFO` & `binn-0.0.2/binn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to generate and interpret biologically informed neural networks.
 Home-page: https://github.com/InfectionMedicineProteomics/BINN
 Author: Erik Hartman
 Author-email: Erik Hartman <erik.hartman@hotmail.com>, Aaron Scott <aaron.scott@med.lu.se>
 License: MIT
 Project-URL: Homepage, https://infectionmedicineproteomics.github.io/BINN/
 Project-URL: Bug Tracker, https://github.com/InfectionMedicineProteomics/BINN/issues
@@ -137,15 +137,15 @@
 Plotting a subgraph starting from a node generates the plot:
 ![Pathway sankey!](/img/sankey.png "Pathway sankey")
 A compelte sankey may look like this:
 ![Complete sankey!](/img/test.png "Complete sankey")
 
 ## Installation
 
-The package can be installed with git.
+The package can be installed and built from source with git.
 
 ```
 git clone git@github.com:InfectionMedicineProteomics/BINN.git
 pip install -e BINN/
 ```
 
 ## Testing
```

### Comparing `binn-0.0.1/pyproject.toml` & `binn-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "binn"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Erik Hartman", email="erik.hartman@hotmail.com" },
   { name="Aaron Scott", email="aaron.scott@med.lu.se" }
 ]
 description = "A package to generate and interpret biologically informed neural networks."
 readme = "README.md"
 requires-python = ">=3.7"
```

