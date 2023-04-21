# Comparing `tmp/libservice-0.1.7.tar.gz` & `tmp/libservice-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libservice-0.1.7.tar", last modified: Thu Apr 20 18:08:31 2023, max compression
+gzip compressed data, was "libservice-0.1.8.tar", last modified: Fri Apr 21 09:48:35 2023, max compression
```

## Comparing `libservice-0.1.7.tar` & `libservice-0.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.665641 libservice-0.1.7/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.657641 libservice-0.1.7/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.657641 libservice-0.1.7/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.657641 libservice-0.1.7/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.7/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.7/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.7/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-20 18:08:31.665641 libservice-0.1.7/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     3543 2023-04-20 08:27:55.000000 libservice-0.1.7/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.661641 libservice-0.1.7/libservice/
--rw-rw-r--   0 joente    (1000) joente    (1000)      134 2023-02-20 10:29:20.000000 libservice-0.1.7/libservice/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      919 2023-04-20 18:05:54.000000 libservice-0.1.7/libservice/asset.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-02-17 14:23:33.000000 libservice-0.1.7/libservice/check.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      451 2023-02-17 12:38:35.000000 libservice-0.1.7/libservice/exceptions.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.661641 libservice-0.1.7/libservice/hub/
--rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.7/libservice/hub/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.7/libservice/hub/client.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.661641 libservice-0.1.7/libservice/hub/net/
--rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.7/libservice/hub/net/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.7/libservice/hub/net/package.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.7/libservice/hub/net/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.7/libservice/hub/protocol.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.7/libservice/logger.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     7459 2023-02-20 10:18:27.000000 libservice-0.1.7/libservice/serviceroom.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.7/libservice/severity.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.7/libservice/start.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.665641 libservice-0.1.7/libservice/ticonn/
--rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.7/libservice/ticonn/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.7/libservice/ticonn/ticonn.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-20 18:08:31.661641 libservice-0.1.7/libservice.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-20 18:08:30.000000 libservice-0.1.7/libservice.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-04-20 18:08:31.000000 libservice-0.1.7/libservice.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-04-20 18:08:30.000000 libservice-0.1.7/libservice.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-04-20 18:08:31.000000 libservice-0.1.7/libservice.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-04-20 18:08:31.000000 libservice-0.1.7/libservice.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-04-20 08:15:18.000000 libservice-0.1.7/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-04-20 18:08:31.665641 libservice-0.1.7/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.7/setup.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-04-20 18:06:52.000000 libservice-0.1.7/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.752358 libservice-0.1.8/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 libservice-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 libservice-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-30 08:37:20.000000 libservice-0.1.8/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 libservice-0.1.8/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 libservice-0.1.8/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 09:48:35.756358 libservice-0.1.8/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3543 2023-04-20 08:27:55.000000 libservice-0.1.8/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      134 2023-02-20 10:29:20.000000 libservice-0.1.8/libservice/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      919 2023-04-20 18:05:54.000000 libservice-0.1.8/libservice/asset.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1125 2023-02-17 14:23:33.000000 libservice-0.1.8/libservice/check.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      849 2023-04-21 09:47:05.000000 libservice-0.1.8/libservice/exceptions.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/hub/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       50 2022-11-25 07:18:03.000000 libservice-0.1.8/libservice/hub/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4459 2023-02-20 09:45:11.000000 libservice-0.1.8/libservice/hub/client.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/hub/net/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-10-18 13:35:23.000000 libservice-0.1.8/libservice/hub/net/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2205 2022-12-27 19:39:41.000000 libservice-0.1.8/libservice/hub/net/package.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3128 2022-10-18 13:35:23.000000 libservice-0.1.8/libservice/hub/net/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1214 2023-02-20 09:46:36.000000 libservice-0.1.8/libservice/hub/protocol.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1666 2023-02-17 16:03:47.000000 libservice-0.1.8/libservice/logger.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     7659 2023-04-21 09:44:25.000000 libservice-0.1.8/libservice/serviceroom.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       86 2023-02-17 12:31:27.000000 libservice-0.1.8/libservice/severity.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2666 2023-02-20 13:20:33.000000 libservice-0.1.8/libservice/start.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice/ticonn/
+-rw-rw-r--   0 joente    (1000) joente    (1000)       27 2022-10-21 06:25:36.000000 libservice-0.1.8/libservice/ticonn/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       55 2022-10-21 06:25:36.000000 libservice-0.1.8/libservice/ticonn/ticonn.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-04-21 09:48:35.756358 libservice-0.1.8/libservice.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     4440 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      745 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       46 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-04-21 09:48:35.000000 libservice-0.1.8/libservice.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       75 2023-04-20 08:15:18.000000 libservice-0.1.8/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-04-21 09:48:35.756358 libservice-0.1.8/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1555 2023-02-20 09:28:37.000000 libservice-0.1.8/setup.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-04-21 09:45:06.000000 libservice-0.1.8/version.py
```

### Comparing `libservice-0.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `libservice-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `libservice-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/.github/workflows/ci.yml` & `libservice-0.1.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/.gitignore` & `libservice-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/LICENSE` & `libservice-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/PKG-INFO` & `libservice-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.7
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.8
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `libservice-0.1.7/README.md` & `libservice-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/asset.py` & `libservice-0.1.8/libservice/asset.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/check.py` & `libservice-0.1.8/libservice/check.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/hub/client.py` & `libservice-0.1.8/libservice/hub/client.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/hub/net/package.py` & `libservice-0.1.8/libservice/hub/net/package.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/hub/net/protocol.py` & `libservice-0.1.8/libservice/hub/net/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/hub/protocol.py` & `libservice-0.1.8/libservice/hub/protocol.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/logger.py` & `libservice-0.1.8/libservice/logger.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice/serviceroom.py` & `libservice-0.1.8/libservice/serviceroom.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 import sys
 from collections import defaultdict
 from thingsdb.room import Room
 from thingsdb.room import event
 from typing import List, Dict, Tuple, Callable, Union, Optional
 from .hub import hub
-from .exceptions import CheckException
+from .exceptions import CheckException, NoCountException
 from .asset import Asset
 from .check import CheckBase, CheckBaseMulti
 
 
 HUB_REQ_SLEEP = .001
 SLEEP_TIME = int(os.getenv('SLEEP_TIME', 2))
 DRY_RUN = os.getenv('DRY_RUN', '0') != '0'
@@ -86,25 +86,26 @@
                     }
                     self._scheduled[key][check_id] = (check_key, config)
 
         for cid in children:
             await self._load(cid)
 
     async def _send_to_hub(self, asset: Asset, result: Optional[dict],
-                           error: Optional[dict], ts: float):
+                           error: Optional[dict], ts: float, no_count: bool):
         if error:
             logging.error(error)
+
         path = asset.asset_id, asset.check_id
         check_data = {
             'result': result,
             'error': error,
             'framework': {
                 'duration': time.time() - ts,
                 'timestamp': int(ts),
-                'no_count': self._no_count,
+                'no_count': no_count,
             }
         }
         try:
             if DRY_RUN:
                 output = json.dumps(check_data, indent=2)
                 print('-'*80, file=sys.stderr)
                 print(output)
@@ -126,28 +127,31 @@
             results = [(None, error)] * len(assets)
         except Exception as e:
             msg = str(e) or type(e).__name__
             error = CheckException(msg).to_dict()
             results = [(None, error)] * len(assets)
 
         for asset, (result, error) in zip(assets, results):
-            await self._send_to_hub(asset, result, error, ts)
+            await self._send_to_hub(asset, result, error, ts, self._no_count)
             await asyncio.sleep(HUB_REQ_SLEEP)
 
     async def _run(self, check: CheckBase, asset: Asset):
         ts = time.time()
+        no_count = self._no_count
         try:
             result, error = await check.run(ts, asset)
+        except NoCountException as e:
+            result, error, no_count = e.result, None, True  # Force True
         except CheckException as e:
             result, error = None, e.to_dict()
         except Exception as e:
             msg = str(e) or type(e).__name__
             result, error = None, CheckException(msg).to_dict()
 
-        await self._send_to_hub(asset, result, error, ts)
+        await self._send_to_hub(asset, result, error, ts, no_count)
 
     async def run_loop(self):
         while True:
             work = self._get_work()
             total = len(self._scheduled)
             log_msg = f'Work: {len(work)} item(s), total: {total}'
             if work:
```

### Comparing `libservice-0.1.7/libservice/start.py` & `libservice-0.1.8/libservice/start.py`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/libservice.egg-info/PKG-INFO` & `libservice-0.1.8/libservice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: libservice
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library for building InfraSonar services
 Home-page: https://github.com/infrasonar/python-libservice
-Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.7
+Download-URL: https://github.com/infrasonar/python-libservice/tarball/v0.1.8
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,service
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `libservice-0.1.7/libservice.egg-info/SOURCES.txt` & `libservice-0.1.8/libservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libservice-0.1.7/setup.py` & `libservice-0.1.8/setup.py`

 * *Files identical despite different names*

