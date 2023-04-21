# Comparing `tmp/prefect-azure-0.2.5.tar.gz` & `tmp/prefect-azure-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-uvqrpkjx/prefect-azure-0.2.5.tar", last modified: Wed Mar 29 17:21:56 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-00ntg7f3/prefect-azure-0.2.6.tar", last modified: Fri Apr 21 00:06:36 2023, max compression
```

## Comparing `prefect-azure-0.2.5.tar` & `prefect-azure-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/prefect_azure/ml_datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:21:56.000000 prefect-azure-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-03-29 17:19:55.000000 prefect-azure-0.2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32501 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20976 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/ml_datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:36.000000 prefect-azure-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31854 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37149 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:04:40.000000 prefect-azure-0.2.6/versioneer.py
```

### Comparing `prefect-azure-0.2.5/LICENSE` & `prefect-azure-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/PKG-INFO` & `prefect-azure-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect tasks and subflows for interacting with Azure
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -173,14 +173,31 @@
 prefect deployment build a_flow_module.py:log_hello_flow --name aci-dev -ib container-instance-job/aci-dev
 ```
 
 Visit [Prefect Deployments](https://docs.prefect.io/tutorials/deployments/) for more information about deployments.
 
 For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
 
+## Azure Container Instance Worker
+The Azure Container Instance worker is an excellent way to run 
+[Prefect projects](https://docs.prefect.io/latest/concepts/projects/) on Azure. 
+
+To get started, create an Azure Container Instances typed work pool:
+```
+prefect work-pool create -t azure-container-instance my-aci-work-pool
+```
+
+Then, run a worker that pulls jobs from the work pool:
+```
+prefect worker start -n my-aci-worker -p my-aci-work-pool
+```
+
+The worker should automatically read the work pool's type and start an 
+Azure Container Instance worker.
+
 ## Resources
 
 If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.
 
 If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)
 
 Feel free to star or watch [`prefect-azure`](https://github.com/PrefectHQ/prefect-azure) for updates too!
```

### Comparing `prefect-azure-0.2.5/README.md` & `prefect-azure-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -145,14 +145,31 @@
 prefect deployment build a_flow_module.py:log_hello_flow --name aci-dev -ib container-instance-job/aci-dev
 ```
 
 Visit [Prefect Deployments](https://docs.prefect.io/tutorials/deployments/) for more information about deployments.
 
 For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
 
+## Azure Container Instance Worker
+The Azure Container Instance worker is an excellent way to run 
+[Prefect projects](https://docs.prefect.io/latest/concepts/projects/) on Azure. 
+
+To get started, create an Azure Container Instances typed work pool:
+```
+prefect work-pool create -t azure-container-instance my-aci-work-pool
+```
+
+Then, run a worker that pulls jobs from the work pool:
+```
+prefect worker start -n my-aci-worker -p my-aci-work-pool
+```
+
+The worker should automatically read the work pool's type and start an 
+Azure Container Instance worker.
+
 ## Resources
 
 If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.
 
 If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)
 
 Feel free to star or watch [`prefect-azure`](https://github.com/PrefectHQ/prefect-azure) for updates too!
```

### Comparing `prefect-azure-0.2.5/prefect_azure/blob_storage.py` & `prefect-azure-0.2.6/prefect_azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/prefect_azure/container_instance.py` & `prefect-azure-0.2.6/prefect_azure/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/prefect_azure/cosmos_db.py` & `prefect-azure-0.2.6/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/prefect_azure/credentials.py` & `prefect-azure-0.2.6/prefect_azure/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/prefect_azure/ml_datastore.py` & `prefect-azure-0.2.6/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/prefect_azure.egg-info/PKG-INFO` & `prefect-azure-0.2.6/prefect_azure.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect tasks and subflows for interacting with Azure
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -173,14 +173,31 @@
 prefect deployment build a_flow_module.py:log_hello_flow --name aci-dev -ib container-instance-job/aci-dev
 ```
 
 Visit [Prefect Deployments](https://docs.prefect.io/tutorials/deployments/) for more information about deployments.
 
 For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
 
+## Azure Container Instance Worker
+The Azure Container Instance worker is an excellent way to run 
+[Prefect projects](https://docs.prefect.io/latest/concepts/projects/) on Azure. 
+
+To get started, create an Azure Container Instances typed work pool:
+```
+prefect work-pool create -t azure-container-instance my-aci-work-pool
+```
+
+Then, run a worker that pulls jobs from the work pool:
+```
+prefect worker start -n my-aci-worker -p my-aci-work-pool
+```
+
+The worker should automatically read the work pool's type and start an 
+Azure Container Instance worker.
+
 ## Resources
 
 If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.
 
 If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)
 
 Feel free to star or watch [`prefect-azure`](https://github.com/PrefectHQ/prefect-azure) for updates too!
```

### Comparing `prefect-azure-0.2.5/prefect_azure.egg-info/SOURCES.txt` & `prefect-azure-0.2.6/prefect_azure.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 prefect_azure/ml_datastore.py
 prefect_azure.egg-info/PKG-INFO
 prefect_azure.egg-info/SOURCES.txt
 prefect_azure.egg-info/dependency_links.txt
 prefect_azure.egg-info/entry_points.txt
 prefect_azure.egg-info/requires.txt
 prefect_azure.egg-info/top_level.txt
+prefect_azure/workers/__init__.py
+prefect_azure/workers/container_instance.py
 tests/test_aci_infrastructure.py
+tests/test_aci_worker.py
 tests/test_blob_storage.py
 tests/test_block_standards.py
 tests/test_cosmos_db.py
 tests/test_credentials.py
 tests/test_ml_datastore.py
```

### Comparing `prefect-azure-0.2.5/setup.cfg` & `prefect-azure-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/setup.py` & `prefect-azure-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_aci_infrastructure.py` & `prefect-azure-0.2.6/tests/test_aci_infrastructure.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_blob_storage.py` & `prefect-azure-0.2.6/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_block_standards.py` & `prefect-azure-0.2.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_cosmos_db.py` & `prefect-azure-0.2.6/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_credentials.py` & `prefect-azure-0.2.6/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/tests/test_ml_datastore.py` & `prefect-azure-0.2.6/tests/test_ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.5/versioneer.py` & `prefect-azure-0.2.6/versioneer.py`

 * *Files identical despite different names*

