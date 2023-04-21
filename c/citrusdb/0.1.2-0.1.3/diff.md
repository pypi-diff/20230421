# Comparing `tmp/citrusdb-0.1.2.tar.gz` & `tmp/citrusdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.1.2.tar", last modified: Mon Apr 17 08:14:07 2023, max compression
+gzip compressed data, was "citrusdb-0.1.3.tar", last modified: Fri Apr 21 10:47:53 2023, max compression
```

## Comparing `citrusdb-0.1.2.tar` & `citrusdb-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.706528 citrusdb-0.1.2/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.1.2/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)      565 2023-04-17 08:14:07.706377 citrusdb-0.1.2/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)       56 2023-04-17 04:31:14.000000 citrusdb-0.1.2/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.704872 citrusdb-0.1.2/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)       80 2023-04-15 19:56:16.000000 citrusdb-0.1.2/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.705771 citrusdb-0.1.2/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:33:43.000000 citrusdb-0.1.2/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2299 2023-04-17 06:29:42.000000 citrusdb-0.1.2/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.704190 citrusdb-0.1.2/citrusdb/db/
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.705989 citrusdb-0.1.2/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:03:22.000000 citrusdb-0.1.2/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1406 2023-04-17 07:26:20.000000 citrusdb-0.1.2/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.706222 citrusdb-0.1.2/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-17 05:54:34.000000 citrusdb-0.1.2/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      383 2023-04-17 06:23:53.000000 citrusdb-0.1.2/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-17 08:14:07.705545 citrusdb-0.1.2/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)      565 2023-04-17 08:14:07.000000 citrusdb-0.1.2/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      387 2023-04-17 08:14:07.000000 citrusdb-0.1.2/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-04-17 08:14:07.000000 citrusdb-0.1.2/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-04-17 08:14:07.000000 citrusdb-0.1.2/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-04-17 08:14:07.000000 citrusdb-0.1.2/citrusdb.egg-info/top_level.txt
--rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-04-17 08:13:45.000000 citrusdb-0.1.2/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-04-17 08:14:07.706590 citrusdb-0.1.2/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-04-17 08:14:00.000000 citrusdb-0.1.2/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150783 citrusdb-0.1.3/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.1.3/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-04-21 10:47:53.150654 citrusdb-0.1.3/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      181 2023-04-21 09:07:38.000000 citrusdb-0.1.3/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.148960 citrusdb-0.1.3/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)       81 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.149997 citrusdb-0.1.3/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:33:43.000000 citrusdb-0.1.3/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4442 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.148285 citrusdb-0.1.3/citrusdb/db/
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150261 citrusdb-0.1.3/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-15 19:03:22.000000 citrusdb-0.1.3/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1415 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.150496 citrusdb-0.1.3/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-04-17 05:54:34.000000 citrusdb-0.1.3/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      355 2023-04-21 10:45:02.000000 citrusdb-0.1.3/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-04-21 10:47:53.149735 citrusdb-0.1.3/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)      690 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      387 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       40 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        9 2023-04-21 10:47:53.000000 citrusdb-0.1.3/citrusdb.egg-info/top_level.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)      598 2023-04-21 10:47:18.000000 citrusdb-0.1.3/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-04-21 10:47:53.150817 citrusdb-0.1.3/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      771 2023-04-21 10:47:30.000000 citrusdb-0.1.3/setup.py
```

### Comparing `citrusdb-0.1.2/LICENSE` & `citrusdb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.1.2/citrusdb/db/index/hnswlib.py` & `citrusdb-0.1.3/citrusdb/db/index/hnswlib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 import hnswlib
 
+
 class HnswIndex:
     _id: str
     _index: hnswlib.Index
 
-    def __init__(self, id, space = "cosine", dim = 1536):
+    def __init__(self, id, space="cosine", dim=1536):
         self._id = id
-        self._index = hnswlib.Index(
-                space = space,
-                dim = dim)
+        self._index = hnswlib.Index(space=space, dim=dim)
 
     def init_index(
-            self,
-            max_elements = 1000,
-            M = 16,
-            ef_construction = 200,
-            allow_replace_deleted = False):
-        self._index.init_index(
-                max_elements,
-                M,
-                ef_construction,
-                allow_replace_deleted)
-
-    def add_items(
-            self,
-            data,
-            ids,
-            replace_deleted = False):
+        self, max_elements=1000, M=16, ef_construction=200, allow_replace_deleted=False
+    ):
+        self._index.init_index(max_elements, M, ef_construction, allow_replace_deleted)
+
+    def add_items(self, data, ids, replace_deleted=False):
         max_elements = self._index.max_elements
         curr_elements = self._index.element_count
 
-        # Increase index size 
+        # Increase index size
         if curr_elements + len(data) > max_elements:
             new_size = max(curr_elements + len(data), 2 * max_elements)
             self._index.resize_index(new_size)
 
         self._index.add_items(data, ids, replace_deleted)
 
-    def knn_query(self, query_embedding, k = 1):
+    def knn_query(self, query_embedding, k=1):
         labels, distances = self._index.knn_query(query_embedding, k)
         return labels[0], distances
 
     def get_dimension(self):
         return self._index.dim
 
+    def load_index(self, path: str, allow_replace_deleted=False):
+        self._index.load_index(path, allow_replace_deleted=allow_replace_deleted)
+
+    def save_index(self, path: str):
+        self._index.save_index(path)
+
     def get_status(self):
         print("Max elements", self._index.max_elements)
         print("Current elements", self._index.element_count)
-
```

### Comparing `citrusdb-0.1.2/pyproject.toml` & `citrusdb-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.1.2"
+version = "0.1.3"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "citrus."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.1.2/setup.py` & `citrusdb-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.1.2",
+    version="0.1.3",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=find_packages(exclude=["demo"]),
```

