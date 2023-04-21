# Comparing `tmp/secapi-tl-1.1.5.tar.gz` & `tmp/secapi-tl-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secapi-tl-1.1.5.tar", last modified: Sat Apr 15 21:10:55 2023, max compression
+gzip compressed data, was "secapi-tl-1.1.6.tar", last modified: Fri Apr 21 14:39:16 2023, max compression
```

## Comparing `secapi-tl-1.1.5.tar` & `secapi-tl-1.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 21:10:55.430242 secapi-tl-1.1.5/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.5/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-15 21:10:55.426242 secapi-tl-1.1.5/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.5/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-15 21:10:13.000000 secapi-tl-1.1.5/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-15 21:10:55.430242 secapi-tl-1.1.5/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 21:10:55.426242 secapi-tl-1.1.5/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 21:10:55.426242 secapi-tl-1.1.5/src/secapi_tl/
--rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.5/src/secapi_tl/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.5/src/secapi_tl/filing.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-15 16:38:29.000000 secapi-tl-1.1.5/src/secapi_tl/filing_query.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.5/src/secapi_tl/key_mapper.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1385 2023-04-15 10:41:21.000000 secapi-tl-1.1.5/src/secapi_tl/request.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-15 21:10:55.426242 secapi-tl-1.1.5/src/secapi_tl.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-15 21:10:55.000000 secapi-tl-1.1.5/src/secapi_tl.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-15 21:10:55.000000 secapi-tl-1.1.5/src/secapi_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-15 21:10:55.000000 secapi-tl-1.1.5/src/secapi_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-15 21:10:55.000000 secapi-tl-1.1.5/src/secapi_tl.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-15 21:10:55.000000 secapi-tl-1.1.5/src/secapi_tl.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1063 2022-10-14 12:06:38.000000 secapi-tl-1.1.6/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3698 2023-04-09 10:03:28.000000 secapi-tl-1.1.6/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      391 2023-04-21 14:37:12.000000 secapi-tl-1.1.6/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/secapi_tl/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      299 2023-04-08 12:35:48.000000 secapi-tl-1.1.6/src/secapi_tl/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6136 2023-04-15 21:09:49.000000 secapi-tl-1.1.6/src/secapi_tl/filing.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4053 2023-04-15 16:38:29.000000 secapi-tl-1.1.6/src/secapi_tl/filing_query.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      989 2022-10-14 21:27:13.000000 secapi-tl-1.1.6/src/secapi_tl/key_mapper.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1377 2023-04-21 14:28:20.000000 secapi-tl-1.1.6/src/secapi_tl/request.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 14:39:16.898633 secapi-tl-1.1.6/src/secapi_tl.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5137 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      349 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       42 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       10 2023-04-21 14:39:16.000000 secapi-tl-1.1.6/src/secapi_tl.egg-info/top_level.txt
```

### Comparing `secapi-tl-1.1.5/LICENSE` & `secapi-tl-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.5/PKG-INFO` & `secapi-tl-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.5
+Version: 1.1.6
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `secapi-tl-1.1.5/README.md` & `secapi-tl-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.5/src/secapi_tl/filing.py` & `secapi-tl-1.1.6/src/secapi_tl/filing.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.5/src/secapi_tl/filing_query.py` & `secapi-tl-1.1.6/src/secapi_tl/filing_query.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.5/src/secapi_tl/key_mapper.py` & `secapi-tl-1.1.6/src/secapi_tl/key_mapper.py`

 * *Files identical despite different names*

### Comparing `secapi-tl-1.1.5/src/secapi_tl/request.py` & `secapi-tl-1.1.6/src/secapi_tl/request.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 an implementation as a normal function caused some issues
 by exceeding the request limits when used with threading.
 These issues disappeared with the implementation as a static method.
 """
 import time
 import math
 import requests
+from requests_random_user_agent import USER_AGENTS
+from random import choice
 from ratelimit import limits, sleep_and_retry
 
 SEC_REQUEST_COUNT = 1
 SEC_PERIOD = 0.1
-SEC_HEADER = {'User-Agent': "myUserAgent"}
 
 
 class Request:
 
     @staticmethod
     @sleep_and_retry
     @limits(calls=SEC_REQUEST_COUNT, period=SEC_PERIOD)
-    def sec_request(url: str, header: dict = None, retries: int=5):
-        if header is None:
-            header = SEC_HEADER
+    def sec_request(url: str, retries: int=5):
+        header = {"User-Agent": choice(USER_AGENTS)}
         response = requests.get(url=url, headers=header)
         if response.status_code != 200 and retries > 0:
             time.sleep(20 * (1 / math.exp(retries-1)))
-            response = Request.sec_request(url=url, header=header, retries=retries-1)
+            response = Request.sec_request(url=url, retries=retries-1)
 
         # raise Connection error on deepest function call if there was no successful response for all tries
         if response.status_code != 200 and retries == 0:
             raise ConnectionError(f"invalid response statuscode: {response.status_code}")
         return response
```

### Comparing `secapi-tl-1.1.5/src/secapi_tl.egg-info/PKG-INFO` & `secapi-tl-1.1.6/src/secapi_tl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secapi-tl
-Version: 1.1.5
+Version: 1.1.6
 License: MIT License
         
         Copyright (c) 2022 tlie03
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

