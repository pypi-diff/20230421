# Comparing `tmp/AStared-0.1.0.tar.gz` & `tmp/AStared-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AStared-0.1.0.tar", last modified: Fri Apr 21 02:41:49 2023, max compression
+gzip compressed data, was "AStared-0.1.1.tar", last modified: Fri Apr 21 02:48:44 2023, max compression
```

## Comparing `AStared-0.1.0.tar` & `AStared-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:41:49.321976 AStared-0.1.0/
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:41:49.321976 AStared-0.1.0/AStared/
--rw-rw-r--   0 steven    (1000) steven    (1000)     4960 2023-04-21 02:36:30.000000 AStared-0.1.0/AStared/AStared.py
--rw-rw-r--   0 steven    (1000) steven    (1000)        0 2023-04-17 01:47:02.000000 AStared-0.1.0/AStared/__init__.py
-drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:41:49.321976 AStared-0.1.0/AStared.egg-info/
--rw-rw-r--   0 steven    (1000) steven    (1000)     2162 2023-04-21 02:41:49.000000 AStared-0.1.0/AStared.egg-info/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)      195 2023-04-21 02:41:49.000000 AStared-0.1.0/AStared.egg-info/SOURCES.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-04-21 02:41:49.000000 AStared-0.1.0/AStared.egg-info/dependency_links.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)        8 2023-04-21 02:41:49.000000 AStared-0.1.0/AStared.egg-info/top_level.txt
--rw-rw-r--   0 steven    (1000) steven    (1000)     1069 2023-04-17 01:45:07.000000 AStared-0.1.0/LICENSE
--rw-rw-r--   0 steven    (1000) steven    (1000)     2162 2023-04-21 02:41:49.321976 AStared-0.1.0/PKG-INFO
--rw-rw-r--   0 steven    (1000) steven    (1000)       35 2023-04-17 01:45:07.000000 AStared-0.1.0/README.md
--rw-rw-r--   0 steven    (1000) steven    (1000)     1034 2023-04-20 23:16:32.000000 AStared-0.1.0/pyproject.toml
--rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-04-21 02:41:49.321976 AStared-0.1.0/setup.cfg
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:48:44.475538 AStared-0.1.1/
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:48:44.471539 AStared-0.1.1/AStared/
+-rw-rw-r--   0 steven    (1000) steven    (1000)     4960 2023-04-21 02:36:30.000000 AStared-0.1.1/AStared/AStared.py
+-rw-rw-r--   0 steven    (1000) steven    (1000)        0 2023-04-17 01:47:02.000000 AStared-0.1.1/AStared/__init__.py
+drwxrwxr-x   0 steven    (1000) steven    (1000)        0 2023-04-21 02:48:44.471539 AStared-0.1.1/AStared.egg-info/
+-rw-rw-r--   0 steven    (1000) steven    (1000)     2724 2023-04-21 02:48:44.000000 AStared-0.1.1/AStared.egg-info/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)      195 2023-04-21 02:48:44.000000 AStared-0.1.1/AStared.egg-info/SOURCES.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        1 2023-04-21 02:48:44.000000 AStared-0.1.1/AStared.egg-info/dependency_links.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)        8 2023-04-21 02:48:44.000000 AStared-0.1.1/AStared.egg-info/top_level.txt
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1069 2023-04-17 01:45:07.000000 AStared-0.1.1/LICENSE
+-rw-rw-r--   0 steven    (1000) steven    (1000)     2724 2023-04-21 02:48:44.475538 AStared-0.1.1/PKG-INFO
+-rw-rw-r--   0 steven    (1000) steven    (1000)      596 2023-04-21 02:47:46.000000 AStared-0.1.1/README.md
+-rw-rw-r--   0 steven    (1000) steven    (1000)     1034 2023-04-21 02:43:30.000000 AStared-0.1.1/pyproject.toml
+-rw-rw-r--   0 steven    (1000) steven    (1000)       38 2023-04-21 02:48:44.475538 AStared-0.1.1/setup.cfg
```

### Comparing `AStared-0.1.0/AStared/AStared.py` & `AStared-0.1.1/AStared/AStared.py`

 * *Files identical despite different names*

### Comparing `AStared-0.1.0/AStared.egg-info/PKG-INFO` & `AStared-0.1.1/AStared.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AStared
-Version: 0.1.0
+Version: 0.1.1
 Summary: AStar python implementatino
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
         
@@ -38,8 +38,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AStared
-A* python implementation
+This package provide the A* algorithm for any type of coordinates.
+You can find more information [here](https://en.wikipedia.org/wiki/A*_search_algorithm).
+
+## Installation
+```python3.11 -m pip install AStared```
+
+## Usage
+You can find examples [here](https://github.com/ThunderTecke/AStared/tree/main/examples).
+
+In global lines, you must define 2 functions to interact with your coordinates. And then pass it to the function `AStar`
+
+These function are :
+- Heuristic estimation to the end node
+- Neighbours giver, that return all valid neightbours that can be reached with only 1 step
```

### Comparing `AStared-0.1.0/LICENSE` & `AStared-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AStared-0.1.0/PKG-INFO` & `AStared-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AStared
-Version: 0.1.0
+Version: 0.1.1
 Summary: AStar python implementatino
 Author-email: ThunderTecke <thunder.tecke@gmail.com>
 Maintainer-email: ThunderTecke <thunder.tecke@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 ThunderTecke
         
@@ -38,8 +38,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AStared
-A* python implementation
+This package provide the A* algorithm for any type of coordinates.
+You can find more information [here](https://en.wikipedia.org/wiki/A*_search_algorithm).
+
+## Installation
+```python3.11 -m pip install AStared```
+
+## Usage
+You can find examples [here](https://github.com/ThunderTecke/AStared/tree/main/examples).
+
+In global lines, you must define 2 functions to interact with your coordinates. And then pass it to the function `AStar`
+
+These function are :
+- Heuristic estimation to the end node
+- Neighbours giver, that return all valid neightbours that can be reached with only 1 step
```

### Comparing `AStared-0.1.0/pyproject.toml` & `AStared-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["AStared"]
 
 [project]
 name = "AStared"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 maintainers = [{name = "ThunderTecke", email = "thunder.tecke@gmail.com"}]
 keywords = ["Python", "AStar", "Algorithm", "Pathfinding"]
 description = "AStar python implementatino"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
```

