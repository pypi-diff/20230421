# Comparing `tmp/cdp-client-2.0.4.tar.gz` & `tmp/cdp-client-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdp-client-2.0.4.tar", last modified: Mon Feb 27 10:12:48 2023, max compression
+gzip compressed data, was "/home/armin/PythonCDPClient/dist/tmp9yQ2id/cdp-client-2.0.5.tar", last modified: Fri Apr 21 14:08:52 2023, max compression
```

## Comparing `cdp-client-2.0.4.tar` & `cdp-client-2.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-02-27 10:12:48.000000 cdp-client-2.0.4/
-drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/
--rw-rw-r--   0 armin     (1000) armin     (1000)        1 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/dependency_links.txt
--rw-rw-r--   0 armin     (1000) armin     (1000)      530 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/SOURCES.txt
--rw-rw-r--   0 armin     (1000) armin     (1000)       68 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/requires.txt
--rw-rw-r--   0 armin     (1000) armin     (1000)       11 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/top_level.txt
--rw-rw-r--   0 armin     (1000) armin     (1000)    17253 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client.egg-info/PKG-INFO
--rw-rw-r--   0 armin     (1000) armin     (1000)       39 2023-02-17 11:04:01.000000 cdp-client-2.0.4/MANIFEST.in
-drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client/
--rw-rw-r--   0 armin     (1000) armin     (1000)    58846 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/cdp_pb2.py
-drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-02-27 10:12:48.000000 cdp-client-2.0.4/cdp_client/tests/
--rw-rw-r--   0 armin     (1000) armin     (1000)     2267 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/tests/test_client.py
--rw-rw-r--   0 armin     (1000) armin     (1000)       64 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/tests/test_main.py
--rw-rw-r--   0 armin     (1000) armin     (1000)    10815 2023-02-27 09:08:29.000000 cdp-client-2.0.4/cdp_client/tests/test_node.py
--rw-rw-r--   0 armin     (1000) armin     (1000)     6946 2023-02-27 09:08:29.000000 cdp-client-2.0.4/cdp_client/tests/fake_data.py
--rw-rw-r--   0 armin     (1000) armin     (1000)     2838 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/tests/test_nodetree.py
--rw-rw-r--   0 armin     (1000) armin     (1000)    14833 2023-02-27 09:08:29.000000 cdp-client-2.0.4/cdp_client/tests/test_connection.py
--rw-rw-r--   0 armin     (1000) armin     (1000)        0 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/tests/__init__.py
--rw-rw-r--   0 armin     (1000) armin     (1000)     2962 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/tests/test_requests.py
--rw-rw-r--   0 armin     (1000) armin     (1000)    32947 2023-02-27 10:11:55.000000 cdp-client-2.0.4/cdp_client/cdp.py
--rw-rw-r--   0 armin     (1000) armin     (1000)        0 2023-02-17 11:04:01.000000 cdp-client-2.0.4/cdp_client/__init__.py
--rw-rw-r--   0 armin     (1000) armin     (1000)       38 2023-02-27 10:12:48.000000 cdp-client-2.0.4/setup.cfg
--rw-rw-r--   0 armin     (1000) armin     (1000)    12857 2023-02-27 09:08:29.000000 cdp-client-2.0.4/README.rst
--rw-rw-r--   0 armin     (1000) armin     (1000)     1082 2023-02-17 11:04:01.000000 cdp-client-2.0.4/LICENSE.txt
--rw-rw-r--   0 armin     (1000) armin     (1000)    17253 2023-02-27 10:12:48.000000 cdp-client-2.0.4/PKG-INFO
--rw-rw-r--   0 armin     (1000) armin     (1000)     1394 2023-02-27 10:12:12.000000 cdp-client-2.0.4/setup.py
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-04-21 14:08:52.000000 cdp-client-2.0.5/
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/
+-rw-rw-r--   0 armin     (1000) armin     (1000)        1 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)      530 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)       68 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/requires.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)       11 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/top_level.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)    17253 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client.egg-info/PKG-INFO
+-rw-rw-r--   0 armin     (1000) armin     (1000)       39 2023-02-17 11:04:01.000000 cdp-client-2.0.5/MANIFEST.in
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client/
+-rw-rw-r--   0 armin     (1000) armin     (1000)    58846 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/cdp_pb2.py
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-04-21 14:08:52.000000 cdp-client-2.0.5/cdp_client/tests/
+-rw-rw-r--   0 armin     (1000) armin     (1000)     2267 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/tests/test_client.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)       64 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/tests/test_main.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)    10815 2023-02-27 09:08:29.000000 cdp-client-2.0.5/cdp_client/tests/test_node.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)     6946 2023-02-27 09:08:29.000000 cdp-client-2.0.5/cdp_client/tests/fake_data.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)     2838 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/tests/test_nodetree.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)    14833 2023-02-27 09:08:29.000000 cdp-client-2.0.5/cdp_client/tests/test_connection.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)        0 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/tests/__init__.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)     2962 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/tests/test_requests.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)    33191 2023-04-21 14:04:16.000000 cdp-client-2.0.5/cdp_client/cdp.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)        0 2023-02-17 11:04:01.000000 cdp-client-2.0.5/cdp_client/__init__.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)       38 2023-04-21 14:08:52.000000 cdp-client-2.0.5/setup.cfg
+-rw-rw-r--   0 armin     (1000) armin     (1000)    12857 2023-02-27 09:08:29.000000 cdp-client-2.0.5/README.rst
+-rw-rw-r--   0 armin     (1000) armin     (1000)     1082 2023-02-17 11:04:01.000000 cdp-client-2.0.5/LICENSE.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)    17253 2023-04-21 14:08:52.000000 cdp-client-2.0.5/PKG-INFO
+-rw-rw-r--   0 armin     (1000) armin     (1000)     1394 2023-04-21 13:32:59.000000 cdp-client-2.0.5/setup.py
```

### Comparing `cdp-client-2.0.4/cdp_client.egg-info/SOURCES.txt` & `cdp-client-2.0.5/cdp_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client.egg-info/PKG-INFO` & `cdp-client-2.0.5/cdp_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdp-client
-Version: 2.0.4
+Version: 2.0.5
 Summary: Provides an API that allows to interact with CDP applications
 Home-page: https://github.com/CDPTechnologies/PythonCDPClient
 Author: CDP Technologies AS
 Author-email: info@cdptech.com
 License: MIT
 Description: CDP-Client
         ==========
```

### Comparing `cdp-client-2.0.4/cdp_client/cdp_pb2.py` & `cdp-client-2.0.5/cdp_client/cdp_pb2.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/test_client.py` & `cdp-client-2.0.5/cdp_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/test_node.py` & `cdp-client-2.0.5/cdp_client/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/fake_data.py` & `cdp-client-2.0.5/cdp_client/tests/fake_data.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/test_nodetree.py` & `cdp-client-2.0.5/cdp_client/tests/test_nodetree.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/test_connection.py` & `cdp-client-2.0.5/cdp_client/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/tests/test_requests.py` & `cdp-client-2.0.5/cdp_client/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/cdp_client/cdp.py` & `cdp-client-2.0.5/cdp_client/cdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,19 @@
             return Promise(lambda resolve, reject: resolve(node))
 
         return fetch_structure().then(update_structure).then(fetch_value)
 
     def _send_value_request(self):
         max_fs = max(self._value_subscriptions, key=lambda e: e[1])[1]
         max_sample_rate = max(self._value_subscriptions, key=lambda e: e[2])[2]
+        #by studio api protocol 0 is the highest sample rate (all samples), so override maxSampleRate if 0 is found
+        for s in self._value_subscriptions:
+            if s[2] == 0:
+                max_sample_rate = 0
+                break
         self._connection.send_value_request(self._id(), max_fs, max_sample_rate)
 
     def _update_structure(self, structure):
         self._structure = structure
         new_children = list(self._structure.node)
         lost_children = list(self._children)
         removed_children = []
```

### Comparing `cdp-client-2.0.4/README.rst` & `cdp-client-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/LICENSE.txt` & `cdp-client-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdp-client-2.0.4/PKG-INFO` & `cdp-client-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdp-client
-Version: 2.0.4
+Version: 2.0.5
 Summary: Provides an API that allows to interact with CDP applications
 Home-page: https://github.com/CDPTechnologies/PythonCDPClient
 Author: CDP Technologies AS
 Author-email: info@cdptech.com
 License: MIT
 Description: CDP-Client
         ==========
```

### Comparing `cdp-client-2.0.4/setup.py` & `cdp-client-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='cdp-client',
-    version='2.0.4',
+    version='2.0.5',
     packages=find_packages(),
     install_requires=[
         'promise==2.2.1',
         'websocket-client==0.56.0',
         'protobuf==3.7.1',
         'mock==3.0.5'],
     keywords=["cdp cdpstudio studio client cdp-client cdp_client"],
```

