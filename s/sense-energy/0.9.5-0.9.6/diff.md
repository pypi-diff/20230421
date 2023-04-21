# Comparing `tmp/sense_energy-0.9.5.tar.gz` & `tmp/sense_energy-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense_energy-0.9.5.tar", last modified: Mon Jan 17 20:35:43 2022, max compression
+gzip compressed data, was "sense_energy-0.9.6.tar", last modified: Wed Jan 19 02:33:15 2022, max compression
```

## Comparing `sense_energy-0.9.5.tar` & `sense_energy-0.9.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-17 20:35:43.337204 sense_energy-0.9.5/
--rw-rw-r--   0 home      (1000) home      (1000)     3796 2022-01-17 20:35:43.337204 sense_energy-0.9.5/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)     2659 2021-02-12 19:43:05.000000 sense_energy-0.9.5/README.md
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-17 20:35:43.333204 sense_energy-0.9.5/sense_energy/
--rw-rw-r--   0 home      (1000) home      (1000)      308 2022-01-17 20:35:35.000000 sense_energy-0.9.5/sense_energy/__init__.py
--rw-rw-r--   0 home      (1000) home      (1000)     5467 2022-01-17 20:35:35.000000 sense_energy-0.9.5/sense_energy/asyncsenseable.py
--rw-rw-r--   0 home      (1000) home      (1000)     2921 2021-02-12 19:43:05.000000 sense_energy-0.9.5/sense_energy/plug_instance.py
--rw-rw-r--   0 home      (1000) home      (1000)     5667 2022-01-17 20:35:35.000000 sense_energy-0.9.5/sense_energy/sense_api.py
--rw-rw-r--   0 home      (1000) home      (1000)      162 2021-02-12 19:43:05.000000 sense_energy-0.9.5/sense_energy/sense_exceptions.py
--rw-rw-r--   0 home      (1000) home      (1000)     3190 2021-11-09 00:25:11.000000 sense_energy-0.9.5/sense_energy/sense_link.py
--rw-rw-r--   0 home      (1000) home      (1000)     5392 2022-01-17 20:35:35.000000 sense_energy-0.9.5/sense_energy/senseable.py
--rw-rw-r--   0 home      (1000) home      (1000)     1344 2021-02-12 19:43:05.000000 sense_energy-0.9.5/sense_energy/tplink_encryption.py
-drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-17 20:35:43.337204 sense_energy-0.9.5/sense_energy.egg-info/
--rw-rw-r--   0 home      (1000) home      (1000)     3796 2022-01-17 20:35:43.000000 sense_energy-0.9.5/sense_energy.egg-info/PKG-INFO
--rw-rw-r--   0 home      (1000) home      (1000)      429 2022-01-17 20:35:43.000000 sense_energy-0.9.5/sense_energy.egg-info/SOURCES.txt
--rw-rw-r--   0 home      (1000) home      (1000)        1 2022-01-17 20:35:43.000000 sense_energy-0.9.5/sense_energy.egg-info/dependency_links.txt
--rw-rw-r--   0 home      (1000) home      (1000)       73 2022-01-17 20:35:43.000000 sense_energy-0.9.5/sense_energy.egg-info/requires.txt
--rw-rw-r--   0 home      (1000) home      (1000)       13 2022-01-17 20:35:43.000000 sense_energy-0.9.5/sense_energy.egg-info/top_level.txt
--rw-rw-r--   0 home      (1000) home      (1000)       38 2022-01-17 20:35:43.337204 sense_energy-0.9.5/setup.cfg
--rw-rw-r--   0 home      (1000) home      (1000)      881 2022-01-17 20:35:35.000000 sense_energy-0.9.5/setup.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-19 02:33:15.162496 sense_energy-0.9.6/
+-rw-rw-r--   0 home      (1000) home      (1000)     3796 2022-01-19 02:33:15.162496 sense_energy-0.9.6/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)     2659 2021-02-12 19:43:05.000000 sense_energy-0.9.6/README.md
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-19 02:33:15.162496 sense_energy-0.9.6/sense_energy/
+-rw-rw-r--   0 home      (1000) home      (1000)      308 2022-01-19 02:32:58.000000 sense_energy-0.9.6/sense_energy/__init__.py
+-rw-rw-r--   0 home      (1000) home      (1000)     5410 2022-01-19 02:32:58.000000 sense_energy-0.9.6/sense_energy/asyncsenseable.py
+-rw-rw-r--   0 home      (1000) home      (1000)     2921 2021-02-12 19:43:05.000000 sense_energy-0.9.6/sense_energy/plug_instance.py
+-rw-rw-r--   0 home      (1000) home      (1000)     5917 2022-01-19 02:32:58.000000 sense_energy-0.9.6/sense_energy/sense_api.py
+-rw-rw-r--   0 home      (1000) home      (1000)      162 2021-02-12 19:43:05.000000 sense_energy-0.9.6/sense_energy/sense_exceptions.py
+-rw-rw-r--   0 home      (1000) home      (1000)     3190 2021-11-09 00:25:11.000000 sense_energy-0.9.6/sense_energy/sense_link.py
+-rw-rw-r--   0 home      (1000) home      (1000)     5378 2022-01-19 02:32:58.000000 sense_energy-0.9.6/sense_energy/senseable.py
+-rw-rw-r--   0 home      (1000) home      (1000)     1344 2021-02-12 19:43:05.000000 sense_energy-0.9.6/sense_energy/tplink_encryption.py
+drwxrwxr-x   0 home      (1000) home      (1000)        0 2022-01-19 02:33:15.162496 sense_energy-0.9.6/sense_energy.egg-info/
+-rw-rw-r--   0 home      (1000) home      (1000)     3796 2022-01-19 02:33:15.000000 sense_energy-0.9.6/sense_energy.egg-info/PKG-INFO
+-rw-rw-r--   0 home      (1000) home      (1000)      429 2022-01-19 02:33:15.000000 sense_energy-0.9.6/sense_energy.egg-info/SOURCES.txt
+-rw-rw-r--   0 home      (1000) home      (1000)        1 2022-01-19 02:33:15.000000 sense_energy-0.9.6/sense_energy.egg-info/dependency_links.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       73 2022-01-19 02:33:15.000000 sense_energy-0.9.6/sense_energy.egg-info/requires.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       13 2022-01-19 02:33:15.000000 sense_energy-0.9.6/sense_energy.egg-info/top_level.txt
+-rw-rw-r--   0 home      (1000) home      (1000)       38 2022-01-19 02:33:15.162496 sense_energy-0.9.6/setup.cfg
+-rw-rw-r--   0 home      (1000) home      (1000)      881 2022-01-19 02:32:58.000000 sense_energy-0.9.6/setup.py
```

### Comparing `sense_energy-0.9.5/PKG-INFO` & `sense_energy-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sense_energy
-Version: 0.9.5
+Version: 0.9.6
 Summary: API for the Sense Energy Monitor
 Home-page: https://github.com/scottbonline/sense
 Author: scottbonline
 Author-email: scottbonline@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/scottbonline/sense/archive/0.9.5.tar.gz
+Download-URL: https://github.com/scottbonline/sense/archive/0.9.6.tar.gz
 Description: # sense_api
         ## Sense Energy Monitor API Interface
         The Sense API provides access to the unofficial API for the Sense Energy Monitor.  Through the API,
         one can retrieve both realtime and trend data including individual devices.
         
         Systematic access to the Sense monitor data. Exploratory work on pulling data from Sense
         to be used in other tools - HomeASsistant, Smartthings, ActiveTiles, etc.
```

### Comparing `sense_energy-0.9.5/README.md` & `sense_energy-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `sense_energy-0.9.5/sense_energy/asyncsenseable.py` & `sense_energy-0.9.6/sense_energy/asyncsenseable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 import json
 import ssl
 
 import aiohttp
 import websockets
-from datetime import datetime, timezone, timedelta
 
 from .sense_api import *
 from .sense_exceptions import *
 
 
 class ASyncSenseable(SenseableBase):
     def __init__(
@@ -113,21 +112,21 @@
             # timed out
             raise SenseAPITimeoutException("API call timed out") from ex
 
     async def get_trend_data(self, scale, dt=None):
         if scale.upper() not in valid_scales:
             raise Exception("%s not a valid scale" % scale)
         if not dt:
-            dt = datetime.now(timezone(timedelta(0))).astimezone()
+            dt = datetime.utcnow()
         json = self.api_call(
-            "app/history/trends?monitor_id=%s&scale=%s&start=%s"
-            % (self.sense_monitor_id, scale, dt.isoformat())
+            'app/history/trends?monitor_id=%s&scale=%s&start=%s'
+            % (self.sense_monitor_id, scale, dt.strftime('%Y-%m-%dT%H:%M:%S'))
         )
         self._trend_data[scale] = await json
-
+        
     async def update_trend_data(self, dt=None):
         for scale in valid_scales:
             await self.get_trend_data(scale, dt)
 
     async def get_monitor_data(self):        
         json = await self.api_call("app/monitors/%s/overview" % self.sense_monitor_id)
         if 'monitor_overview' in json and 'monitor' in json['monitor_overview']:
```

### Comparing `sense_energy-0.9.5/sense_energy/plug_instance.py` & `sense_energy-0.9.6/sense_energy/plug_instance.py`

 * *Files identical despite different names*

### Comparing `sense_energy-0.9.5/sense_energy/sense_api.py` & `sense_energy-0.9.6/sense_energy/sense_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import sys
 from time import time
+from datetime import datetime
 
 from .sense_exceptions import *
 
 API_URL = 'https://api.sense.com/apiservice/api/v1/'
 WS_URL = "wss://clientrt.sense.com/monitors/%s/realtimefeed?access_token=%s"
 API_TIMEOUT = 5
 WSS_TIMEOUT = 5
 RATE_LIMIT = 60
 
-# for the last hour, day, week, month, or year
-valid_scales = ['HOUR', 'DAY', 'WEEK', 'MONTH', 'YEAR']
+# for the last day, week, month, or year
+valid_scales = ['DAY', 'WEEK', 'MONTH', 'YEAR']
 
 
 class SenseableBase(object):
 
     def __init__(self, username=None, password=None,
                  api_timeout=API_TIMEOUT, wss_timeout=WSS_TIMEOUT):
 
@@ -188,15 +189,21 @@
         return [d['name'] for d in self._realtime.get('devices', {})]
         
     @property
     def time_zone(self):
         return self._monitor.get('time_zone', '')
         
     def trend_start(self, scale):
-        return self._trend_data[scale]['start']
+        if 'start' not in self._trend_data[scale]:
+            return None
+        try:
+            start_iso = self._trend_data[scale]['start'].replace('Z', '+00:00')
+            return datetime.strptime(start_iso, '%Y-%m-%dT%H:%M:%S.%f%z')
+        except:
+            return None
 
     def get_trend(self, scale, key):
         if isinstance(key, bool):
             key = 'production' if key is True else 'consumption'
         else:
             key = 'consumption' if key == 'usage' else key
         if key not in self._trend_data[scale]: return 0
```

### Comparing `sense_energy-0.9.5/sense_energy/sense_link.py` & `sense_energy-0.9.6/sense_energy/sense_link.py`

 * *Files identical despite different names*

### Comparing `sense_energy-0.9.5/sense_energy/senseable.py` & `sense_energy-0.9.6/sense_energy/senseable.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,18 @@
         finally:
             if ws: ws.close()    
     
     def get_trend_data(self, scale, dt=None):
         if scale.upper() not in valid_scales:
             raise Exception("%s not a valid scale" % scale)
         if not dt:
-            dt = datetime.now(timezone(timedelta(0))).astimezone()
+            dt = datetime.utcnow()
         self._trend_data[scale] = self.api_call(
-            'app/history/trends?monitor_id=%s&scale=%s&start=%s' %
-            (self.sense_monitor_id, scale, dt.isoformat()))
+            'app/history/trends?monitor_id=%s&scale=%s&start=%s'
+            % (self.sense_monitor_id, scale, dt.strftime('%Y-%m-%dT%H:%M:%S')))
 
     def update_trend_data(self, dt=None):
         for scale in valid_scales:
             self.get_trend_data(scale, dt)
 
     def api_call(self, url, payload={}):
         try:
```

### Comparing `sense_energy-0.9.5/sense_energy/tplink_encryption.py` & `sense_energy-0.9.6/sense_energy/tplink_encryption.py`

 * *Files identical despite different names*

### Comparing `sense_energy-0.9.5/sense_energy.egg-info/PKG-INFO` & `sense_energy-0.9.6/sense_energy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sense-energy
-Version: 0.9.5
+Version: 0.9.6
 Summary: API for the Sense Energy Monitor
 Home-page: https://github.com/scottbonline/sense
 Author: scottbonline
 Author-email: scottbonline@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/scottbonline/sense/archive/0.9.5.tar.gz
+Download-URL: https://github.com/scottbonline/sense/archive/0.9.6.tar.gz
 Description: # sense_api
         ## Sense Energy Monitor API Interface
         The Sense API provides access to the unofficial API for the Sense Energy Monitor.  Through the API,
         one can retrieve both realtime and trend data including individual devices.
         
         Systematic access to the Sense monitor data. Exploratory work on pulling data from Sense
         to be used in other tools - HomeASsistant, Smartthings, ActiveTiles, etc.
```

### Comparing `sense_energy-0.9.5/setup.py` & `sense_energy-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     packages = ['sense_energy'], 
     install_requires=[
         'requests',
         'websocket-client',
         'websockets;python_version>="3.5"',
         'aiohttp;python_version>="3.5"',
     ], 
-    version = '0.9.5',
+    version = '0.9.6',
     description = 'API for the Sense Energy Monitor',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'scottbonline',
     author_email = 'scottbonline@gmail.com',
     url = 'https://github.com/scottbonline/sense',
-    download_url = 'https://github.com/scottbonline/sense/archive/0.9.5.tar.gz',
+    download_url = 'https://github.com/scottbonline/sense/archive/0.9.6.tar.gz',
     keywords = ['sense', 'energy', 'api', 'pytest'], 
     classifiers = [
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
     ],
 )
```

