# Comparing `tmp/crowdcores-node-1.1.1.tar.gz` & `tmp/crowdcores-node-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdcores-node-1.1.1.tar", last modified: Thu Apr 20 00:04:13 2023, max compression
+gzip compressed data, was "crowdcores-node-1.1.2.tar", last modified: Fri Apr 21 15:39:47 2023, max compression
```

## Comparing `crowdcores-node-1.1.1.tar` & `crowdcores-node-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:04:13.388360 crowdcores-node-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-20 00:04:13.388360 crowdcores-node-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      345 2023-04-19 22:11:11.000000 crowdcores-node-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:04:13.388360 crowdcores-node-1.1.1/crowdcores_node/
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.1/crowdcores_node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4729 2023-04-19 23:48:27.000000 crowdcores-node-1.1.1/crowdcores_node/crowdcores_node.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-04-19 22:09:24.000000 crowdcores-node-1.1.1/crowdcores_node/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:04:13.388360 crowdcores-node-1.1.1/crowdcores_node.egg-info/
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 00:04:13.000000 crowdcores-node-1.1.1/crowdcores_node.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 00:04:13.388360 crowdcores-node-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      352 2023-04-20 00:03:55.000000 crowdcores-node-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:39:47.975465 crowdcores-node-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 01:07:39.000000 crowdcores-node-1.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-21 15:39:47.975465 crowdcores-node-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-19 22:11:11.000000 crowdcores-node-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:39:47.971465 crowdcores-node-1.1.2/crowdcores_node/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-18 22:47:07.000000 crowdcores-node-1.1.2/crowdcores_node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-04-20 23:09:10.000000 crowdcores-node-1.1.2/crowdcores_node/crowdcores_node.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-04-19 22:09:24.000000 crowdcores-node-1.1.2/crowdcores_node/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:39:47.975465 crowdcores-node-1.1.2/crowdcores_node.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-21 15:39:47.000000 crowdcores-node-1.1.2/crowdcores_node.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 15:39:47.975465 crowdcores-node-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      352 2023-04-21 15:39:22.000000 crowdcores-node-1.1.2/setup.py
```

### Comparing `crowdcores-node-1.1.1/LICENSE.txt` & `crowdcores-node-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crowdcores-node-1.1.1/crowdcores_node/crowdcores_node.py` & `crowdcores-node-1.1.2/crowdcores_node/crowdcores_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import websockets
 import time
 import json
 import torch
 from transformers import pipeline
 import sys
+import os
 
 #polyfills for earlier  versions of python
 try:
     asyncio.create_task
 except AttributeError:
     def asyncio_create_task(coro, *, loop=None):
         if loop is None:
@@ -29,15 +30,14 @@
             loop.close()
 else:
     asyncio_run = asyncio.run
 
 
 
 
-
 model_names=[];
 models_pipelines={};
 
 async def run_async(func, *args, **kwargs):
     loop = asyncio.get_event_loop()
     result = await loop.run_in_executor(None, func, *args, **kwargs)
     return result
@@ -76,15 +76,15 @@
             "exception_message":str(e)
         }
         return response
 
 
 async def process_pipeline_request(websocket,message):
     response = await run_async(do_process_pipeline_request,websocket,message)
-    data = {'command': 'completed_pipeline_request','pipeline_response':response}
+    data = {'command': 'completed_pipeline_request','pipeline_response':response,'pipeline_request':message}
     await websocket.send(json.dumps(data))
 
 
 async def init_load_models(websocket):
     await run_async(load_models,websocket)
     print("Models Download Complete")
     data = {'command': 'completed_models_download'}
@@ -123,14 +123,17 @@
         #print("sending");
         await asyncio.sleep(15)
         data = {'command': 'ping'}
         await websocket.send(json.dumps(data))
 
 async def start_node(websocket):
         data = {'command': 'node_started'}
+        API_KEY = os.getenv('CROWDCORES_API_KEY');
+        if API_KEY:
+            data['api_key']=API_KEY;
         await websocket.send(json.dumps(data))
 
 async def client():
     while True:
         try:
             async with websockets.connect("ws://ws.crowdcores.com") as websocket:
                 consumer_task=asyncio_create_task(receive_loop(websocket))
```

### Comparing `crowdcores-node-1.1.1/crowdcores_node/manager.py` & `crowdcores-node-1.1.2/crowdcores_node/manager.py`

 * *Files identical despite different names*

