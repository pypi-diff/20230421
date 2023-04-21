# Comparing `tmp/hti_index-0.1.0.tar.gz` & `tmp/hti_index-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hti_index-0.1.0.tar", last modified: Thu Apr 20 00:23:33 2023, max compression
+gzip compressed data, was "hti_index-0.1.1.tar", last modified: Fri Apr 21 06:06:55 2023, max compression
```

## Comparing `hti_index-0.1.0.tar` & `hti_index-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-20 00:23:33.840852 hti_index-0.1.0/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.0/LICENSE
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-20 00:23:33.840533 hti_index-0.1.0/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.0/README.md
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-20 00:23:33.839486 hti_index-0.1.0/hti_index/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       92 2023-04-19 23:42:14.000000 hti_index-0.1.0/hti_index/__init__.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3095 2023-04-20 00:12:09.000000 hti_index-0.1.0/hti_index/component.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     2696 2023-04-20 00:20:10.000000 hti_index-0.1.0/hti_index/composite.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3833 2023-04-20 00:22:25.000000 hti_index-0.1.0/hti_index/indexer.py
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-19 20:12:55.000000 hti_index-0.1.0/hti_index/utils.py
-drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-20 00:23:33.840301 hti_index-0.1.0/hti_index.egg-info/
--rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-20 00:23:33.000000 hti_index-0.1.0/hti_index.egg-info/PKG-INFO
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      298 2023-04-20 00:23:33.000000 hti_index-0.1.0/hti_index.egg-info/SOURCES.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-20 00:23:33.000000 hti_index-0.1.0/hti_index.egg-info/dependency_links.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-20 00:23:33.000000 hti_index-0.1.0/hti_index.egg-info/requires.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-20 00:23:33.000000 hti_index-0.1.0/hti_index.egg-info/top_level.txt
--rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-20 00:23:33.840915 hti_index-0.1.0/setup.cfg
--rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-20 00:21:30.000000 hti_index-0.1.0/setup.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.318132 hti_index-0.1.1/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        0 2023-04-19 14:21:14.000000 hti_index-0.1.1/LICENSE
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:06:55.317778 hti_index-0.1.1/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2884 2023-04-20 00:19:29.000000 hti_index-0.1.1/README.md
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.316453 hti_index-0.1.1/hti_index/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      148 2023-04-21 06:02:31.000000 hti_index-0.1.1/hti_index/__init__.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3095 2023-04-20 00:12:09.000000 hti_index-0.1.1/hti_index/component.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     2696 2023-04-20 00:20:10.000000 hti_index-0.1.1/hti_index/composite.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3977 2023-04-21 06:06:46.000000 hti_index-0.1.1/hti_index/flowfreq.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     5361 2023-04-21 05:32:49.000000 hti_index-0.1.1/hti_index/indexer.py
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     1808 2023-04-21 06:02:13.000000 hti_index-0.1.1/hti_index/utils.py
+drwxr-xr-x   0 mohameddiomande   (501) staff       (20)        0 2023-04-21 06:06:55.317467 hti_index-0.1.1/hti_index.egg-info/
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)     3357 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/PKG-INFO
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      320 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/SOURCES.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        1 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/dependency_links.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)        6 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/requires.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       10 2023-04-21 06:06:55.000000 hti_index-0.1.1/hti_index.egg-info/top_level.txt
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)       38 2023-04-21 06:06:55.318202 hti_index-0.1.1/setup.cfg
+-rw-r--r--   0 mohameddiomande   (501) staff       (20)      751 2023-04-21 06:06:01.000000 hti_index-0.1.1/setup.py
```

### Comparing `hti_index-0.1.0/PKG-INFO` & `hti_index-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti_index
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.0/README.md` & `hti_index-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.0/hti_index/component.py` & `hti_index-0.1.1/hti_index/component.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.0/hti_index/composite.py` & `hti_index-0.1.1/hti_index/composite.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.0/hti_index/indexer.py` & `hti_index-0.1.1/hti_index/indexer.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 class HTIIndex:
     def __init__(self, size: int):
         self.size = size
         self.lookup_table: Dict[str, NodeComposite] = {}
         self.hash_table = np.empty((size,), dtype=object)
         self.num_items = 0
+        self.root = None
 
+            
     def __len__(self):
         return self.num_items
 
     def insert(self, key: str, value: Any):
         node = NodeComposite(key=key, value=value)
         self.lookup_table[key] = node
         hash_value = self._hash_key(key)
@@ -100,10 +102,42 @@
         results = []
         for bucket in self.hash_table:
             if bucket is not None:
                 for node in bucket:
                     results.extend(self._get_range(node, start, end))
         return results
     
+
+    def _get_node_frequency(self, key: str) -> int:
+        return len(self.get_bucket(key))
+    
+    def _get_transition_frequency(self, prev_key: str, key: str) -> int:
+        return sum(1 for node in self.get_bucket(prev_key) if node.key == key)
+
+        
+    def _get_node_probability(self, key: str) -> float:
+        return self._get_node_frequency(key) / self.num_items
+            
+    def _get_transition_probability(self, prev_key: str, key: str) -> float:
+        return self._get_transition_frequency(prev_key, key) / self.num_items
+    
+    def _get_node_entropy(self, key: str) -> float:
+        prob = self._get_node_probability(key)
+        return -prob * np.log2(prob)
+    
+    def _get_transition_entropy(self, prev_key: str, key: str) -> float:
+        prob = self._get_transition_probability(prev_key, key)
+        return -prob * np.log2(prob)
+            
+    def _get_node_information(self, key: str) -> float:
+        return self._get_node_entropy(key) * self._get_node_frequency(key)
+    
+    def _get_transition_information(self, prev_key: str, key: str) -> float:
+        return self._get_transition_entropy(prev_key, key) * self._get_transition_frequency(prev_key, key)
     
+    def _get_node_information_gain(self, key: str) -> float:
+        return self._get_node_information(key) / self.num_items
     
+    def _get_transition_information_gain(self, prev_key: str, key: str) -> float:
+        return self._get_transition_information(prev_key, key) / self.num_items
     
+
```

### Comparing `hti_index-0.1.0/hti_index/utils.py` & `hti_index-0.1.1/hti_index/utils.py`

 * *Files identical despite different names*

### Comparing `hti_index-0.1.0/hti_index.egg-info/PKG-INFO` & `hti_index-0.1.1/hti_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hti-index
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for implementing a HasH Table Index
 Home-page: https://github.com/diomandeee/hti_index
 Author: Mohamed Diomande
 Author-email: gdiomande7907@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hti_index-0.1.0/setup.py` & `hti_index-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Description: Setup script for the qbf_index package
 from setuptools import setup, find_packages
 
 setup(
     name='hti_index',
-    version='0.1.0',
+    version='0.1.1',
     author='Mohamed Diomande',
     author_email='gdiomande7907@gmail.com',
     description='Python package for implementing a HasH Table Index', 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/diomandeee/hti_index',
     packages=find_packages(),
```

