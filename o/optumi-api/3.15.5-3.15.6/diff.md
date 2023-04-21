# Comparing `tmp/optumi-api-3.15.5.tar.gz` & `tmp/optumi-api-3.15.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.15.5.tar", last modified: Wed Apr 12 20:24:32 2023, max compression
+gzip compressed data, was "optumi-api-3.15.6.tar", last modified: Thu Apr 20 17:47:32 2023, max compression
```

## Comparing `optumi-api-3.15.5.tar` & `optumi-api-3.15.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/
--rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-04-03 21:07:54.000000 optumi-api-3.15.5/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-04-03 21:07:54.000000 optumi-api-3.15.5/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-12 20:24:32.108225 optumi-api-3.15.5/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-03 21:07:54.000000 optumi-api-3.15.5/README.md
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-12 20:24:31.000000 optumi-api-3.15.5/core_version.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/optumi_api/
--rw-rw-r--   0 denis     (1001) denis     (1001)     2883 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/CloudFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3677 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5148 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/CloudStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3977 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Colab.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5352 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Container.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4402 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6563 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Executable.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1006 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/HoldoverTime.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/LocalFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2401 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/LocalStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1515 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Log.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6290 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/LoginServer.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6763 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Machine.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1956 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Machines.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Notebook.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6568 2023-04-12 20:23:17.000000 optumi-api-3.15.5/optumi_api/NotebookConfig.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2472 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Notifications.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      818 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Packages.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1620 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Program.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Provider.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1359 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Providers.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3281 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Resource.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Script.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4135 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Server.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1968 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Summary.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    19449 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/Workload.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3107 2023-04-07 01:15:24.000000 optumi-api-3.15.5/optumi_api/Workloads.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-04-07 16:00:16.000000 optumi-api-3.15.5/optumi_api/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    11309 2023-04-04 21:44:37.000000 optumi-api-3.15.5/optumi_api/api.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-04-04 21:44:37.000000 optumi-api-3.15.5/optumi_api/cli.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1786 2023-04-03 21:07:54.000000 optumi-api-3.15.5/optumi_api/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:32.108225 optumi-api-3.15.5/optumi_api.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/entry_points.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       41 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-04-12 20:24:32.000000 optumi-api-3.15.5/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-12 20:24:32.108225 optumi-api-3.15.5/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     2612 2023-04-04 21:44:37.000000 optumi-api-3.15.5/setup.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/
+-rw-rw-r--   0 jj        (1001) jj        (1001)      281 2023-04-17 18:17:12.000000 optumi-api-3.15.6/LICENSE
+-rw-rw-r--   0 jj        (1001) jj        (1001)       58 2023-04-17 18:17:12.000000 optumi-api-3.15.6/MANIFEST.in
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-04-20 17:47:32.071957 optumi-api-3.15.6/PKG-INFO
+-rw-rw-r--   0 jj        (1001) jj        (1001)      422 2023-04-17 18:17:12.000000 optumi-api-3.15.6/README.md
+-rw-rw-r--   0 jj        (1001) jj        (1001)      322 2023-04-20 17:47:31.000000 optumi-api-3.15.6/core_version.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/optumi_api/
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2883 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudFile.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3677 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5148 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/CloudStorage.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3977 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Colab.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5352 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Container.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4402 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4179 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6563 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Executable.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1006 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3070 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LocalFile.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2401 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LocalStorage.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1515 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Log.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6290 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/LoginServer.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6763 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Machine.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1956 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Machines.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      723 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Notebook.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     6568 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     2472 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Notifications.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      818 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Packages.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1620 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Program.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     5284 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Provider.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1359 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Providers.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3281 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Resource.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      696 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Script.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     4135 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Server.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1968 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Summary.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)    20470 2023-04-19 20:20:54.000000 optumi-api-3.15.6/optumi_api/Workload.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     3107 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/Workloads.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      838 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/__init__.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)      323 2023-04-20 14:07:13.000000 optumi-api-3.15.6/optumi_api/_version.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)    11309 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/api.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1418 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/cli.py
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1786 2023-04-17 18:17:12.000000 optumi-api-3.15.6/optumi_api/utils.py
+drwxrwxr-x   0 jj        (1001) jj        (1001)        0 2023-04-20 17:47:32.071957 optumi-api-3.15.6/optumi_api.egg-info/
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1560 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jj        (1001) jj        (1001)     1086 2023-04-20 17:47:32.000000 optumi-api-3.15.6/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       47 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)        1 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jj        (1001) jj        (1001)       41 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       11 2023-04-20 17:47:31.000000 optumi-api-3.15.6/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 jj        (1001) jj        (1001)       38 2023-04-20 17:47:32.071957 optumi-api-3.15.6/setup.cfg
+-rwxrwxr-x   0 jj        (1001) jj        (1001)     2612 2023-04-17 18:17:12.000000 optumi-api-3.15.6/setup.py
```

### Comparing `optumi-api-3.15.5/PKG-INFO` & `optumi-api-3.15.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.5
+Version: 3.15.6
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.5/optumi_api/CloudFile.py` & `optumi-api-3.15.6/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/CloudFileVersion.py` & `optumi-api-3.15.6/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/CloudStorage.py` & `optumi-api-3.15.6/optumi_api/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Colab.py` & `optumi-api-3.15.6/optumi_api/Colab.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Container.py` & `optumi-api-3.15.6/optumi_api/Container.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/ContainerRegistry.py` & `optumi-api-3.15.6/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/EnvironmentVariables.py` & `optumi-api-3.15.6/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Executable.py` & `optumi-api-3.15.6/optumi_api/Executable.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/HoldoverTime.py` & `optumi-api-3.15.6/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/LocalFile.py` & `optumi-api-3.15.6/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/LocalStorage.py` & `optumi-api-3.15.6/optumi_api/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Log.py` & `optumi-api-3.15.6/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/LoginServer.py` & `optumi-api-3.15.6/optumi_api/LoginServer.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Machine.py` & `optumi-api-3.15.6/optumi_api/Machine.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Machines.py` & `optumi-api-3.15.6/optumi_api/Machines.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Notebook.py` & `optumi-api-3.15.6/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/NotebookConfig.py` & `optumi-api-3.15.6/optumi_api/NotebookConfig.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Notifications.py` & `optumi-api-3.15.6/optumi_api/Notifications.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Packages.py` & `optumi-api-3.15.6/optumi_api/Packages.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Program.py` & `optumi-api-3.15.6/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Provider.py` & `optumi-api-3.15.6/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Providers.py` & `optumi-api-3.15.6/optumi_api/Providers.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Resource.py` & `optumi-api-3.15.6/optumi_api/Resource.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Script.py` & `optumi-api-3.15.6/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Server.py` & `optumi-api-3.15.6/optumi_api/Server.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Summary.py` & `optumi-api-3.15.6/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/Workload.py` & `optumi-api-3.15.6/optumi_api/Workload.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,20 +181,44 @@
 
         return w
 
     def _refresh(self):
         now = time.time()
         if now - self._last_refresh > 5:
             self._last_refresh = now
-            user_information = json.loads(optumi.core.get_workloads().text)
-            # Add apps from user information if they don't already exist
-            if "jobs" in user_information:
-                for workload in user_information["jobs"]:
-                    if workload["uuid"] == self._workload_uuid:
-                        self._handle_workload_update(workload)
+            if self.__get_status() != "completed":
+                workloads = json.loads(optumi.core.get_workloads().text)
+                if not self._workload_uuid in [workload["uuid"] for workload in workloads["jobs"]]:
+                    return
+
+                updates = json.loads(
+                    optumi.pull_workload_status_updates(
+                        [self._workload_uuid],
+                        [len(self._initializing_lines)],
+                        [len(self._preparing_lines)],
+                        [len(self._running_lines)],
+                    ).text
+                )[self._workload_uuid]
+
+                self._handle_workload_update(updates)
+
+                if self._module_uuid:
+                    updates = json.loads(
+                        optumi.pull_module_status_updates(
+                            [self._workload_uuid],
+                            [self._module_uuid],
+                            [len(self._update_lines)],
+                            [len(self._output)],
+                            [len(self._monitoring)],
+                            [self._last_patches],
+                            True,
+                        ).content
+                    )[self._module_uuid]
+
+                    self._handle_module_update(updates)
 
     # def __print_status(self):
     #     collapsed = collapseUpdates(
     #         self._initializing_lines + self._preparing_lines + self._running_lines
     #     ).split("\n")
     #     line = collapsed[-1] if collapsed[-1] != "" else collapsed[-2]
     #     print("\b" * self._last_line_length, end="")
@@ -293,21 +317,25 @@
         if optumi.utils.is_dynamic() and Workloads.current()._workload_uuid == self._workload_uuid:
             print("Stopping current workload")
             # This is for sessions
             code = os.system("jupyter lab stop 54321")
             if code > 15:  # 15 is SIGTERM
                 # This is for jobs
                 exit(0)
+            print("...completed")
         else:
-            print("Stopping workload " + self.name + "...")
             if self.status != "completed":
+                print("Stopping workload " + self.name + "...")
                 optumi.core.stop_notebook(self._workload_uuid)
                 if wait and self.status == "running":
                     self.wait(progress="silent")
-            print("...completed")
+                print("...completed")
+            else:
+                print("Workload not running")
+
 
     def remove(self, wait: bool = True):
         """Remove the current workload."""
         if self.status != "completed":
             self.stop(wait)
         print("Removing workload " + self.name + "...")
         optumi.core.teardown_notebook(self._workload_uuid)
```

### Comparing `optumi-api-3.15.5/optumi_api/Workloads.py` & `optumi-api-3.15.6/optumi_api/Workloads.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/__init__.py` & `optumi-api-3.15.6/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/api.py` & `optumi-api-3.15.6/optumi_api/api.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/cli.py` & `optumi-api-3.15.6/optumi_api/cli.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api/utils.py` & `optumi-api-3.15.6/optumi_api/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.15.6/optumi_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.15.5
+Version: 3.15.6
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.15.5/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.15.6/optumi_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optumi-api-3.15.5/setup.py` & `optumi-api-3.15.6/setup.py`

 * *Files identical despite different names*

