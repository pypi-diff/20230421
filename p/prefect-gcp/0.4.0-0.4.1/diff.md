# Comparing `tmp/prefect-gcp-0.4.0.tar.gz` & `tmp/prefect-gcp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-4xgiama3/prefect-gcp-0.4.0.tar", last modified: Thu Apr  6 10:40:55 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-pvh27_8d/prefect-gcp-0.4.1.tar", last modified: Fri Apr 21 00:07:50 2023, max compression
```

## Comparing `prefect-gcp-0.4.0.tar` & `prefect-gcp-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27556 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45746 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/prefect_gcp/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:40:55.000000 prefect-gcp-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    29062 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-06 10:39:09.000000 prefect-gcp-0.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33862 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27602 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45746 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30893 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/prefect_gcp/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:07:50.000000 prefect-gcp-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:05:39.000000 prefect-gcp-0.4.1/versioneer.py
```

### Comparing `prefect-gcp-0.4.0/LICENSE` & `prefect-gcp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/PKG-INFO` & `prefect-gcp-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.0
+Version: 0.4.1
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.0 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.1 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.0/README.md` & `prefect-gcp-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/aiplatform.py` & `prefect-gcp-0.4.1/prefect_gcp/aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/bigquery.py` & `prefect-gcp-0.4.1/prefect_gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/cloud_run.py` & `prefect-gcp-0.4.1/prefect_gcp/cloud_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,23 +563,23 @@
 
         return CloudRunJobResult(identifier=self.job_name, status_code=status_code)
 
     def _jobs_body(self) -> dict:
         """Create properly formatted body used for a Job CREATE request.
         See: https://cloud.google.com/run/docs/reference/rest/v1/namespaces.jobs
         """
-        jobs_metadata = {
-            "name": self.job_name,
-            "annotations": {
-                # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
-                "run.googleapis.com/launch-stage": "BETA",
-            },
+        jobs_metadata = {"name": self.job_name}
+
+        annotations = {
+            # See: https://cloud.google.com/run/docs/troubleshooting#launch-stage-validation  # noqa
+            "run.googleapis.com/launch-stage": "BETA",
         }
+        # add vpc connector if specified
         if self.vpc_connector_name:
-            jobs_metadata["annotations"][
+            annotations[
                 "run.googleapis.com/vpc-access-connector"
             ] = self.vpc_connector_name
 
         # env and command here
         containers = [self._add_container_settings({"image": self.image})]
 
         # apply this timeout to each task
@@ -587,14 +587,15 @@
 
         body = {
             "apiVersion": "run.googleapis.com/v1",
             "kind": "Job",
             "metadata": jobs_metadata,
             "spec": {  # JobSpec
                 "template": {  # ExecutionTemplateSpec
+                    "metadata": {"annotations": annotations},
                     "spec": {  # ExecutionSpec
                         "template": {  # TaskTemplateSpec
                             "spec": {
                                 "containers": containers,
                                 "timeoutSeconds": timeout_seconds,
                             }  # TaskSpec
                         }
```

### Comparing `prefect-gcp-0.4.0/prefect_gcp/cloud_storage.py` & `prefect-gcp-0.4.1/prefect_gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/credentials.py` & `prefect-gcp-0.4.1/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/projects/steps.py` & `prefect-gcp-0.4.1/prefect_gcp/projects/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp/secret_manager.py` & `prefect-gcp-0.4.1/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/prefect_gcp.egg-info/PKG-INFO` & `prefect-gcp-0.4.1/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.0
+Version: 0.4.1
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.0 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.1 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.0/prefect_gcp.egg-info/SOURCES.txt` & `prefect-gcp-0.4.1/prefect_gcp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 prefect_gcp/_version.py
 prefect_gcp/aiplatform.py
 prefect_gcp/bigquery.py
 prefect_gcp/cloud_run.py
 prefect_gcp/cloud_storage.py
 prefect_gcp/credentials.py
 prefect_gcp/secret_manager.py
+prefect_gcp/worker.py
 prefect_gcp.egg-info/PKG-INFO
 prefect_gcp.egg-info/SOURCES.txt
 prefect_gcp.egg-info/dependency_links.txt
 prefect_gcp.egg-info/entry_points.txt
 prefect_gcp.egg-info/requires.txt
 prefect_gcp.egg-info/top_level.txt
 prefect_gcp/projects/__init__.py
 prefect_gcp/projects/steps.py
 tests/test_aiplatform.py
 tests/test_bigquery.py
 tests/test_block_standards.py
 tests/test_cloud_run.py
 tests/test_cloud_storage.py
 tests/test_credentials.py
-tests/test_secret_manager.py
+tests/test_secret_manager.py
+tests/test_worker.py
```

### Comparing `prefect-gcp-0.4.0/prefect_gcp.egg-info/requires.txt` & `prefect-gcp-0.4.1/prefect_gcp.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-prefect>=2.7.2
+prefect>=2.10.5
 google-api-python-client>=2.20.0
 google-cloud-storage>=2.0.0
 
 [aiplatform]
 google-cloud-aiplatform
 
 [all_extras]
```

### Comparing `prefect-gcp-0.4.0/setup.cfg` & `prefect-gcp-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/setup.py` & `prefect-gcp-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_aiplatform.py` & `prefect-gcp-0.4.1/tests/test_aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_bigquery.py` & `prefect-gcp-0.4.1/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_block_standards.py` & `prefect-gcp-0.4.1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_cloud_run.py` & `prefect-gcp-0.4.1/tests/test_cloud_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,17 @@
             "timeoutSeconds"
         ] == str(timeout)
 
     def test_vpc_connector_name_added_correctly(self, cloud_run_job):
         cloud_run_job.vpc_connector_name = "vpc_name"
         result = cloud_run_job._jobs_body()
         assert (
-            result["metadata"]["annotations"]["run.googleapis.com/vpc-access-connector"]
+            result["spec"]["template"]["metadata"]["annotations"][
+                "run.googleapis.com/vpc-access-connector"
+            ]
             == "vpc_name"
         )
 
     def test_memory_validation_succeeds(self, gcp_credentials):
         """Make sure that memory validation doesn't fail when valid params provided."""
         CloudRunJob(
             image="gcr.io//not-a/real-image",
@@ -761,15 +763,14 @@
             raise Exception("This is an intentional exception")
 
         monkeypatch.setattr("prefect_gcp.cloud_run.Execution.get", raise_exception)
 
         with pytest.raises(Exception):
             cloud_run_job.run()
         calls = list_mock_calls(mock_client, 2)
-        # breakpoint()
         for call, expected_call in zip(calls, expected_calls):
             assert call.startswith(expected_call)
 
     async def test_kill(self, mock_client, cloud_run_job):
         mock_client.jobs().get().execute.return_value = self.job_ready
         mock_client.jobs().run().execute.return_value = self.job_ready
         mock_client.executions().get().execute.return_value = self.execution_not_found
```

### Comparing `prefect-gcp-0.4.0/tests/test_cloud_storage.py` & `prefect-gcp-0.4.1/tests/test_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_credentials.py` & `prefect-gcp-0.4.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/tests/test_secret_manager.py` & `prefect-gcp-0.4.1/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.0/versioneer.py` & `prefect-gcp-0.4.1/versioneer.py`

 * *Files identical despite different names*

