# Comparing `tmp/twitter-api-client-0.6.7.tar.gz` & `tmp/twitter-api-client-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.7.tar", last modified: Wed Apr 19 23:58:34 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.8.tar", last modified: Fri Apr 21 03:30:21 2023, max compression
```

## Comparing `twitter-api-client-0.6.7.tar` & `twitter-api-client-0.6.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.6.7/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     8154 2023-04-19 23:58:30.000000 twitter-api-client-0.6.7/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.7/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22355 2023-04-19 20:10:25.000000 twitter-api-client-0.6.7/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.6.7/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5527 2023-04-19 22:52:46.000000 twitter-api-client-0.6.7/twitter/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/twitter/noauth/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.7/twitter/noauth/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.6.7/twitter/noauth/operation.py
--rw-r--r--   0 x         (1000) x         (1000)     7404 2023-04-19 19:28:54.000000 twitter-api-client-0.6.7/twitter/noauth/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.6.7/twitter/noauth/util.py
--rw-r--r--   0 x         (1000) x         (1000)    10521 2023-04-19 23:25:47.000000 twitter-api-client-0.6.7/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     4902 2023-04-19 22:46:55.000000 twitter-api-client-0.6.7/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     3269 2023-04-19 22:46:55.000000 twitter-api-client-0.6.7/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 23:58:34.256752 twitter-api-client-0.6.7/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-19 23:58:34.000000 twitter-api-client-0.6.7/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      459 2023-04-19 23:58:34.000000 twitter-api-client-0.6.7/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-19 23:58:34.000000 twitter-api-client-0.6.7/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-19 23:58:34.000000 twitter-api-client-0.6.7/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-19 23:58:34.000000 twitter-api-client-0.6.7/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 03:30:21.247119 twitter-api-client-0.6.8/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.6.8/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-21 03:30:21.247119 twitter-api-client-0.6.8/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-21 03:30:21.247119 twitter-api-client-0.6.8/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8154 2023-04-21 03:30:15.000000 twitter-api-client-0.6.8/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 03:30:21.243786 twitter-api-client-0.6.8/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.8/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    21981 2023-04-21 03:28:04.000000 twitter-api-client-0.6.8/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.6.8/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5527 2023-04-19 22:52:46.000000 twitter-api-client-0.6.8/twitter/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 03:30:21.243786 twitter-api-client-0.6.8/twitter/noauth/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.8/twitter/noauth/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.6.8/twitter/noauth/operation.py
+-rw-r--r--   0 x         (1000) x         (1000)     7404 2023-04-19 19:28:54.000000 twitter-api-client-0.6.8/twitter/noauth/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.6.8/twitter/noauth/util.py
+-rw-r--r--   0 x         (1000) x         (1000)    10880 2023-04-21 03:28:04.000000 twitter-api-client-0.6.8/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4902 2023-04-19 22:46:55.000000 twitter-api-client-0.6.8/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3781 2023-04-21 03:29:56.000000 twitter-api-client-0.6.8/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-21 03:30:21.247119 twitter-api-client-0.6.8/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-21 03:30:21.000000 twitter-api-client-0.6.8/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      459 2023-04-21 03:30:21.000000 twitter-api-client-0.6.8/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-21 03:30:21.000000 twitter-api-client-0.6.8/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-21 03:30:21.000000 twitter-api-client-0.6.8/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-21 03:30:21.000000 twitter-api-client-0.6.8/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.7/LICENSE` & `twitter-api-client-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/PKG-INFO` & `twitter-api-client-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.7
+Version: 0.6.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.6.7/setup.py` & `twitter-api-client-0.6.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.6.7",
+    version="0.6.8",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
```

### Comparing `twitter-api-client-0.6.7/twitter/account.py` & `twitter-api-client-0.6.8/twitter/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import asyncio
 import hashlib
 import logging.config
 import math
 import mimetypes
-import platform
 import random
 import time
 from copy import deepcopy
 from datetime import datetime
 from pathlib import Path
 from urllib.parse import urlencode
 from uuid import uuid1, getnode
@@ -16,29 +14,14 @@
 from requests import Response
 from tqdm import tqdm
 
 from .constants import *
 from .login import login
 from .util import find_key, get_headers, fmt_status, get_cursor, save_data
 
-try:
-    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
-        import nest_asyncio
-
-        nest_asyncio.apply()
-except:
-    ...
-
-if platform.system() != 'Windows':
-    import uvloop
-
-    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-else:
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
 
 class GraphQL:
     def __init__(self, operation: tuple, variables: dict, features: dict = Operation.default_features):
         self.operation = operation
```

### Comparing `twitter-api-client-0.6.7/twitter/constants.py` & `twitter-api-client-0.6.8/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/login.py` & `twitter-api-client-0.6.8/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/noauth/operation.py` & `twitter-api-client-0.6.8/twitter/noauth/operation.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/noauth/scraper.py` & `twitter-api-client-0.6.8/twitter/noauth/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/noauth/util.py` & `twitter-api-client-0.6.8/twitter/noauth/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/scraper.py` & `twitter-api-client-0.6.8/twitter/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import logging.config
 import math
+import platform
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from urllib.parse import urlsplit
 
 import orjson
 from aiohttp import ClientSession, TCPConnector, ClientResponse
@@ -14,14 +15,29 @@
 from .constants import *
 from .login import login
 from .util import find_key, save_data, get_cursor, get_headers, set_qs, fmt_status
 
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
+try:
+    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
+        import nest_asyncio
+
+        nest_asyncio.apply()
+except:
+    ...
+
+if platform.system() != 'Windows':
+    import uvloop
+
+    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+else:
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+
 
 class Scraper:
     def __init__(self, email: str, username: str, password: str, *, save=True, debug=False):
         self.session = login(email, username, password)
         self.api = 'https://twitter.com/i/api/graphql'
         self.save = save
         self.debug = debug
```

### Comparing `twitter-api-client-0.6.7/twitter/search.py` & `twitter-api-client-0.6.8/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.7/twitter/util.py` & `twitter-api-client-0.6.8/twitter/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,14 +51,26 @@
     elif 300 <= status < 400:
         color = MAGENTA
     elif 400 <= status < 600:
         color = RED
     return f'[{color}{status}{RESET}]'
 
 
+def save_data(data: list, op: str, key: str | int):
+    try:
+        path = Path(f'data/raw/{key}')
+        path.mkdir(parents=True, exist_ok=True)
+        (path / f'{time.time_ns()}_{op}.json').write_text(
+            orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
+            encoding='utf-8'
+        )
+    except Exception as e:
+        print(f'failed to save data: {e}')
+
+
 def find_key(obj: any, key: str) -> list:
     """
     Find all values of a given key within a nested dict or list of dicts
 
     @param obj: dictionary or list of dictionaries
     @param key: key to search for
     @return: list of values
@@ -80,17 +92,24 @@
             for k in obj:
                 L.extend(helper(obj[k], key, []))
         return L
 
     return helper(obj, key, [])
 
 
-def save_data(data: list, op: str, key: str | int):
-    try:
-        path = Path(f'data/raw/{key}')
-        path.mkdir(parents=True, exist_ok=True)
-        (path / f'{time.time_ns()}_{op}.json').write_text(
-            orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
-            encoding='utf-8'
-        )
-    except Exception as e:
-        print(f'failed to save data: {e}')
+def keys(d: dict, paths=False) -> list:
+    """
+    Get all unique keys from nested dicts
+    """
+    def get(d, curr_key=[]):
+        for k, v in d.items():
+            if isinstance(v, dict):
+                yield from get(v, curr_key + [k])
+            elif isinstance(v, list):
+                for i in v:
+                    yield from get(i, curr_key + [k])
+            else:
+                yield curr_key + [k]
+
+    if paths:
+        return list(get(d))
+    return list({y for x in get(d) for y in x})
```

### Comparing `twitter-api-client-0.6.7/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.8/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.7
+Version: 0.6.8
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
```

