# Comparing `tmp/vidis_algorithms_api-0.4.1.tar.gz` & `tmp/vidis_algorithms_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidis_algorithms_api-0.4.1.tar", last modified: Fri Apr 21 10:47:22 2023, max compression
+gzip compressed data, was "vidis_algorithms_api-0.4.2.tar", last modified: Fri Apr 21 11:16:15 2023, max compression
```

## Comparing `vidis_algorithms_api-0.4.1.tar` & `vidis_algorithms_api-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.923940 vidis_algorithms_api-0.4.1/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 10:47:22.923940 vidis_algorithms_api-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.919940 vidis_algorithms_api-0.4.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.919940 vidis_algorithms_api-0.4.1/examples/dummy_example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.4.1/examples/dummy_example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.1/examples/dummy_example/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.919940 vidis_algorithms_api-0.4.1/examples/neural_network/
--rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.1/examples/neural_network/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.919940 vidis_algorithms_api-0.4.1/examples/neural_network/model/
--rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.1/examples/neural_network/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-21 10:47:04.000000 vidis_algorithms_api-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 10:47:22.923940 vidis_algorithms_api-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-21 10:47:04.000000 vidis_algorithms_api-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.919940 vidis_algorithms_api-0.4.1/vidis_algorithms_api/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-04-21 10:47:04.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api/Lifecycle.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api/Task.py
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.923940 vidis_algorithms_api-0.4.1/vidis_algorithms_api/core/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api/core/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 10:47:22.923940 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 10:47:22.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      571 2023-04-21 10:47:22.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 10:47:22.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 10:47:22.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-21 10:47:22.000000 vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/examples/dummy_example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.4.2/examples/dummy_example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.2/examples/dummy_example/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/examples/neural_network/
+-rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.2/examples/neural_network/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/examples/neural_network/model/
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.2/examples/neural_network/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-21 11:15:56.000000 vidis_algorithms_api-0.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-21 11:15:56.000000 vidis_algorithms_api-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/vidis_algorithms_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2023-04-21 11:15:56.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api/Lifecycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-04-21 10:13:42.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/vidis_algorithms_api/core/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api/core/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:16:15.799934 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-21 11:16:15.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      571 2023-04-21 11:16:15.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 11:16:15.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-21 11:16:15.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-21 11:16:15.000000 vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/top_level.txt
```

### Comparing `vidis_algorithms_api-0.4.1/README.md` & `vidis_algorithms_api-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.1/examples/dummy_example/algorithm.py` & `vidis_algorithms_api-0.4.2/examples/dummy_example/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.1/examples/neural_network/algorithm.py` & `vidis_algorithms_api-0.4.2/examples/neural_network/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.1/examples/neural_network/model/model.py` & `vidis_algorithms_api-0.4.2/examples/neural_network/model/model.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.1/setup.py` & `vidis_algorithms_api-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 
 def setup_package():
-    __version__ = '0.4.1'
+    __version__ = '0.4.2'
     url = 'https://github.com/Banayaki'
 
     setup(name='vidis_algorithms_api',
           description=description,
           version=__version__,
           url=url,
           license='MIT',
```

### Comparing `vidis_algorithms_api-0.4.1/vidis_algorithms_api/Lifecycle.py` & `vidis_algorithms_api-0.4.2/vidis_algorithms_api/Lifecycle.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class CeleryTaskLifecycle(celery.Task):
     def __init__(self):
         super(CeleryTaskLifecycle, self).__init__()
         self.layer = None
         
     def _call_remote(self, name_method: str, body: dict):
         with ClusterRpcProxy(settings.CELERY_BROKER) as rpc_client:
-            response = getattr(rpc_client.internal_hyperspecter_service, name_method)(
+            response = getattr(rpc_client.internal_layers_service, name_method)(
                 body
             )
             return response
         
     def before_start(self, task_id, args, kwargs):
         name, hsi_id, _ = args
         self.layer = self._call_remote("save_or_update", {
```

### Comparing `vidis_algorithms_api-0.4.1/vidis_algorithms_api/Task.py` & `vidis_algorithms_api-0.4.2/vidis_algorithms_api/Task.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.4.1/vidis_algorithms_api.egg-info/SOURCES.txt` & `vidis_algorithms_api-0.4.2/vidis_algorithms_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

