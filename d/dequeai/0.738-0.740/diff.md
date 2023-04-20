# Comparing `tmp/dequeai-0.738.tar.gz` & `tmp/dequeai-0.740.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.738.tar", last modified: Thu Apr 20 21:06:29 2023, max compression
+gzip compressed data, was "dequeai-0.740.tar", last modified: Thu Apr 20 21:08:13 2023, max compression
```

## Comparing `dequeai-0.738.tar` & `dequeai-0.740.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:06:29.761506 dequeai-0.738/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:06:29.761506 dequeai-0.738/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:06:29.761506 dequeai-0.738/dequeai/
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.738/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.738/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.738/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.738/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.738/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    24552 2023-04-20 21:06:04.000000 dequeai-0.738/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.738/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.738/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.738/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.738/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:06:29.761506 dequeai-0.738/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:06:29.000000 dequeai-0.738/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 21:06:29.000000 dequeai-0.738/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:06:29.000000 dequeai-0.738/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 21:06:29.000000 dequeai-0.738/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 21:06:29.000000 dequeai-0.738/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:06:29.761506 dequeai-0.738/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 21:06:15.000000 dequeai-0.738/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:08:13.594052 dequeai-0.740/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:08:13.594052 dequeai-0.740/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:08:13.594052 dequeai-0.740/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-20 21:04:18.000000 dequeai-0.740/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.740/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.740/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.740/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-04-20 20:33:33.000000 dequeai-0.740/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    24551 2023-04-20 21:07:51.000000 dequeai-0.740/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.740/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.740/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.740/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.740/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 21:08:13.594052 dequeai-0.740/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-20 21:08:13.000000 dequeai-0.740/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-20 21:08:13.000000 dequeai-0.740/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 21:08:13.000000 dequeai-0.740/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-20 21:08:13.000000 dequeai-0.740/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-20 21:08:13.000000 dequeai-0.740/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 21:08:13.594052 dequeai-0.740/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-20 21:07:59.000000 dequeai-0.740/setup.py
```

### Comparing `dequeai-0.738/dequeai/datatypes.py` & `dequeai-0.740/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.738/dequeai/dequeai.py` & `dequeai-0.740/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.738/dequeai/dequeai_run.py` & `dequeai-0.740/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/best/read/", json=req_data)
         data_list = resp.json()
         print(data_list)
         # Extract header names
         first_run_data_keys = list(data_list['run'][0]['best_experiment_data']['data'].keys())
         headers = ['Run ID', 'Best Metric Key', 'Best Metric'] + [f'{key}.{sub_key}' for key in first_run_data_keys for
                                                                   sub_key in
-                                                                  data_list['runs'][0]['best_experiment_data']['data'][
+                                                                  data_list['run'][0]['best_experiment_data']['data'][
                                                                       key]]
 
         # Extract rows
         rows = []
         for run in data_list['run']:
             best_metric = self._get_nested_value(run['best_experiment_data']['data'], metric_key)
             row = [run['run_id'], metric_key, best_metric]
```

### Comparing `dequeai-0.738/dequeai/parsing_service.py` & `dequeai-0.740/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.738/dequeai/rest_connect.py` & `dequeai-0.740/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.738/dequeai/util.py` & `dequeai-0.740/dequeai/util.py`

 * *Files identical despite different names*

