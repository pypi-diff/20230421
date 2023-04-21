# Comparing `tmp/cy2py-1.1.5.tar.gz` & `tmp/cy2py-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cy2py-1.1.5.tar", last modified: Wed Nov 23 08:47:44 2022, max compression
+gzip compressed data, was "cy2py-1.1.6.tar", last modified: Fri Apr 21 13:54:43 2023, max compression
```

## Comparing `cy2py-1.1.5.tar` & `cy2py-1.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2022-11-23 08:47:44.478178 cy2py-1.1.5/
--rw-r--r--   0 andreasanturbano   (502) staff       (20)      557 2022-10-17 10:50:54.000000 cy2py-1.1.5/LICENSE
--rw-r--r--   0 andreasanturbano   (502) staff       (20)        0 2022-10-17 10:50:54.000000 cy2py-1.1.5/MANIFEST.in
--rw-r--r--   0 andreasanturbano   (502) staff       (20)     2955 2022-11-23 08:47:44.477979 cy2py-1.1.5/PKG-INFO
--rw-r--r--   0 andreasanturbano   (502) staff       (20)     2558 2022-10-17 10:50:54.000000 cy2py-1.1.5/README.md
--rw-r--r--   0 andreasanturbano   (502) staff       (20)       38 2022-11-23 08:47:44.478221 cy2py-1.1.5/setup.cfg
--rw-r--r--   0 andreasanturbano   (502) staff       (20)      873 2022-11-23 08:47:43.000000 cy2py-1.1.5/setup.py
-drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2022-11-23 08:47:44.475638 cy2py-1.1.5/src/
-drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2022-11-23 08:47:44.476936 cy2py-1.1.5/src/cy2py/
--rw-r--r--   0 andreasanturbano   (502) staff       (20)       19 2022-10-17 10:50:54.000000 cy2py-1.1.5/src/cy2py/__init__.py
--rw-r--r--   0 andreasanturbano   (502) staff       (20)      722 2022-10-17 10:50:54.000000 cy2py-1.1.5/src/cy2py/annotation_utils.py
--rwxrwxrwx   0 andreasanturbano   (502) staff       (20)     7781 2022-11-09 14:21:15.000000 cy2py-1.1.5/src/cy2py/cy2.py
--rw-r--r--   0 andreasanturbano   (502) staff       (20)     4846 2022-11-23 08:47:09.000000 cy2py-1.1.5/src/cy2py/utils.py
-drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2022-11-23 08:47:44.477433 cy2py-1.1.5/src/cy2py.egg-info/
--rw-r--r--   0 andreasanturbano   (502) staff       (20)     2955 2022-11-23 08:47:44.000000 cy2py-1.1.5/src/cy2py.egg-info/PKG-INFO
--rw-r--r--   0 andreasanturbano   (502) staff       (20)      343 2022-11-23 08:47:44.000000 cy2py-1.1.5/src/cy2py.egg-info/SOURCES.txt
--rw-r--r--   0 andreasanturbano   (502) staff       (20)        1 2022-11-23 08:47:44.000000 cy2py-1.1.5/src/cy2py.egg-info/dependency_links.txt
--rw-r--r--   0 andreasanturbano   (502) staff       (20)       79 2022-11-23 08:47:44.000000 cy2py-1.1.5/src/cy2py.egg-info/requires.txt
--rw-r--r--   0 andreasanturbano   (502) staff       (20)       12 2022-11-23 08:47:44.000000 cy2py-1.1.5/src/cy2py.egg-info/top_level.txt
-drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2022-11-23 08:47:44.477610 cy2py-1.1.5/src/tests/
--rw-r--r--   0 andreasanturbano   (502) staff       (20)        0 2022-10-17 10:50:43.000000 cy2py-1.1.5/src/tests/__init__.py
--rwxrwxrwx   0 andreasanturbano   (502) staff       (20)     3437 2022-09-12 16:45:49.000000 cy2py-1.1.5/src/tests/cypher_magic_test.py
+drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2023-04-21 13:54:43.113169 cy2py-1.1.6/
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)      557 2022-10-17 10:50:54.000000 cy2py-1.1.6/LICENSE
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)        0 2022-10-17 10:50:54.000000 cy2py-1.1.6/MANIFEST.in
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)     2955 2023-04-21 13:54:43.113041 cy2py-1.1.6/PKG-INFO
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)     2558 2022-10-17 10:50:54.000000 cy2py-1.1.6/README.md
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)       38 2023-04-21 13:54:43.113205 cy2py-1.1.6/setup.cfg
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)      873 2023-04-21 13:53:27.000000 cy2py-1.1.6/setup.py
+drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2023-04-21 13:54:43.110646 cy2py-1.1.6/src/
+drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2023-04-21 13:54:43.111963 cy2py-1.1.6/src/cy2py/
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)       19 2022-10-17 10:50:54.000000 cy2py-1.1.6/src/cy2py/__init__.py
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)      722 2022-10-17 10:50:54.000000 cy2py-1.1.6/src/cy2py/annotation_utils.py
+-rwxrwxrwx   0 andreasanturbano   (502) staff       (20)     7781 2022-11-09 14:21:15.000000 cy2py-1.1.6/src/cy2py/cy2.py
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)     5112 2023-04-21 13:53:07.000000 cy2py-1.1.6/src/cy2py/utils.py
+drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2023-04-21 13:54:43.112627 cy2py-1.1.6/src/cy2py.egg-info/
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)     2955 2023-04-21 13:54:43.000000 cy2py-1.1.6/src/cy2py.egg-info/PKG-INFO
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)      343 2023-04-21 13:54:43.000000 cy2py-1.1.6/src/cy2py.egg-info/SOURCES.txt
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)        1 2023-04-21 13:54:43.000000 cy2py-1.1.6/src/cy2py.egg-info/dependency_links.txt
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)       79 2023-04-21 13:54:43.000000 cy2py-1.1.6/src/cy2py.egg-info/requires.txt
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)       12 2023-04-21 13:54:43.000000 cy2py-1.1.6/src/cy2py.egg-info/top_level.txt
+drwxr-xr-x   0 andreasanturbano   (502) staff       (20)        0 2023-04-21 13:54:43.112816 cy2py-1.1.6/src/tests/
+-rw-r--r--   0 andreasanturbano   (502) staff       (20)        0 2022-10-17 10:50:43.000000 cy2py-1.1.6/src/tests/__init__.py
+-rwxr-xr-x   0 andreasanturbano   (502) staff       (20)     3769 2023-04-21 13:53:07.000000 cy2py-1.1.6/src/tests/cypher_magic_test.py
```

### Comparing `cy2py-1.1.5/LICENSE` & `cy2py-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cy2py-1.1.5/PKG-INFO` & `cy2py-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cy2py
-Version: 1.1.5
+Version: 1.1.6
 Home-page: https://github.com/conker84/cy2py
 Author: Andrea Santurbano
 Author-email: santand@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cy2py-1.1.5/README.md` & `cy2py-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cy2py-1.1.5/setup.py` & `cy2py-1.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "ipython-genutils>=0.1.0",
     "ipycytoscape>=1.3.3",
     "networkx"
 ]
 
 setup(
     name="cy2py",
-    version="1.1.5",
+    version="1.1.6",
     author="Andrea Santurbano",
     author_email="santand@gmail.com",
     description="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/conker84/cy2py",
     packages=find_packages("src"),
```

### Comparing `cy2py-1.1.5/src/cy2py/annotation_utils.py` & `cy2py-1.1.6/src/cy2py/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `cy2py-1.1.5/src/cy2py/cy2.py` & `cy2py-1.1.6/src/cy2py/cy2.py`

 * *Files identical despite different names*

### Comparing `cy2py-1.1.5/src/cy2py/utils.py` & `cy2py-1.1.6/src/cy2py/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import networkx as nx
 import ipycytoscape
 from IPython.core.display import display
+import json
 
 node_centered = {
     'selector': 'node',
     'style': {
         'font-size': '10',
         'label': 'data(label)',
         'height': '60',
@@ -54,14 +55,18 @@
         if label in captions:
             props['__labels'] = label
             if type(captions[label]) == list:
                 label = ' '.join(map(lambda l: props[l], captions[label]))
             else:
                 label = props[captions[label]]
 
+        # taken from https://stackoverflow.com/questions/11875770/how-to-overcome-datetime-datetime-not-json-serializable/36142844#36142844
+        json_str = json.dumps(props, indent=4, sort_keys=True, default=str)
+        props = json.loads(json_str)
+
         networkx_graph.add_node(node.id, label=label, color=color, properties=props, title=label, tooltip=str(props))
 
     def add_edge(edge):
         props = dict(edge.items())
         weight = props.get('weight', 1)
         networkx_graph.add_edge(edge.start_node.id, edge.end_node.id, weight=weight, label=edge.type, tooltip=str(props))
```

### Comparing `cy2py-1.1.5/src/cy2py.egg-info/PKG-INFO` & `cy2py-1.1.6/src/cy2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cy2py
-Version: 1.1.5
+Version: 1.1.6
 Home-page: https://github.com/conker84/cy2py
 Author: Andrea Santurbano
 Author-email: santand@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cy2py-1.1.5/src/tests/cypher_magic_test.py` & `cy2py-1.1.6/src/tests/cypher_magic_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,7 +101,18 @@
         assert res.success
         # do the second call by leveraging the cache
         res = self._ip.run_cell(raw_cell='''
             %%cypher
             SHOW DATABASES
         ''')
         assert res.success
+
+    def test_cell_magic_date(self):
+        self._ip.run_cell(raw_cell=f'''
+            neo4j_url = '{self.neo4j_url}'
+        ''')
+        res = self._ip.run_cell(raw_cell='''
+            %%cypher -u $neo4j_url
+            CREATE (n:Company {date: date('1970-01-01')})
+            RETURN n
+        ''')
+        assert res.success
```

