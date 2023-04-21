# Comparing `tmp/prefect-kubernetes-0.2.4.tar.gz` & `tmp/prefect-kubernetes-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-35dpud7r/prefect-kubernetes-0.2.4.tar", last modified: Thu Apr  6 21:56:24 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-r8p0z9xb/prefect-kubernetes-0.2.5.tar", last modified: Fri Apr 21 00:03:22 2023, max compression
```

## Comparing `prefect-kubernetes-0.2.4.tar` & `prefect-kubernetes-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    29178 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:56:24.000000 prefect-kubernetes-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    71880 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-06 21:55:00.000000 prefect-kubernetes-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77561 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/versioneer.py
```

### Comparing `prefect-kubernetes-0.2.4/LICENSE` & `prefect-kubernetes-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/PKG-INFO` & `prefect-kubernetes-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-kubernetes
```

### Comparing `prefect-kubernetes-0.2.4/README.md` & `prefect-kubernetes-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/credentials.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/custom_objects.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/deployments.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/exceptions.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/flows.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/jobs.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/pods.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/services.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/utilities.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes/worker.py` & `prefect-kubernetes-0.2.5/prefect_kubernetes/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,43 +91,32 @@
 import math
 import os
 import time
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Tuple
 
 import anyio.abc
-import prefect
-from packaging import version
 from prefect.blocks.kubernetes import KubernetesClusterConfig
 from prefect.docker import get_prefect_image_name
+from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.importtools import lazy_import
 from prefect.utilities.pydantic import JsonPatch
 from prefect.utilities.templating import find_placeholders
+from prefect.workers.base import (
+    BaseJobConfiguration,
+    BaseVariables,
+    BaseWorker,
+    BaseWorkerResult,
+)
 from pydantic import Field, validator
 from typing_extensions import Literal
 
-# TODO: Remove this after next prefect release
-if version.parse(prefect.__version__) <= version.parse("2.9.0"):
-    from prefect.experimental.workers.base import (
-        BaseJobConfiguration,
-        BaseVariables,
-        BaseWorker,
-        BaseWorkerResult,
-    )
-else:
-    from prefect.workers.base import (
-        BaseJobConfiguration,
-        BaseWorker,
-        BaseWorkerResult,
-        BaseVariables,
-    )
-
 from prefect_kubernetes.utilities import (
     _slugify_label_key,
     _slugify_label_value,
     _slugify_name,
 )
 
 if TYPE_CHECKING:
@@ -503,14 +492,74 @@
 
             # Monitor the job until completion
             status_code = await run_sync_in_worker_thread(
                 self._watch_job, job.metadata.name, configuration, client
             )
             return KubernetesWorkerResult(identifier=pid, status_code=status_code)
 
+    async def kill_infrastructure(
+        self,
+        infrastructure_pid: str,
+        configuration: KubernetesWorkerJobConfiguration,
+        grace_seconds: int = 30,
+    ):
+        """
+        Stops a job for a cancelled flow run based on the provided infrastructure PID
+        and run configuration.
+        """
+        await run_sync_in_worker_thread(
+            self._stop_job, infrastructure_pid, configuration, grace_seconds
+        )
+
+    def _stop_job(
+        self,
+        infrastructure_pid: str,
+        configuration: KubernetesWorkerJobConfiguration,
+        grace_seconds: int = 30,
+    ):
+        client = self._get_configured_kubernetes_client(configuration)
+        job_cluster_uid, job_namespace, job_name = self._parse_infrastructure_pid(
+            infrastructure_pid
+        )
+
+        if job_namespace != configuration.namespace:
+            raise InfrastructureNotAvailable(
+                f"Unable to kill job {job_name!r}: The job is running in namespace "
+                f"{job_namespace!r} but this worker expected jobs to be running in "
+                f"namespace {configuration.namespace!r} based on the work pool and "
+                "deployment configuration."
+            )
+
+        current_cluster_uid = self._get_cluster_uid(client)
+        if job_cluster_uid != current_cluster_uid:
+            raise InfrastructureNotAvailable(
+                f"Unable to kill job {job_name!r}: The job is running on another "
+                "cluster than the one specified by the infrastructure PID."
+            )
+
+        with self._get_batch_client(client) as batch_client:
+            try:
+                batch_client.delete_namespaced_job(
+                    name=job_name,
+                    namespace=job_namespace,
+                    grace_period_seconds=grace_seconds,
+                    # Foreground propagation deletes dependent objects before deleting
+                    # owner objects. This ensures that the pods are cleaned up before
+                    # the job is marked as deleted.
+                    # See: https://kubernetes.io/docs/concepts/architecture/garbage-collection/#foreground-deletion # noqa
+                    propagation_policy="Foreground",
+                )
+            except kubernetes.client.exceptions.ApiException as exc:
+                if exc.status == 404:
+                    raise InfrastructureNotFound(
+                        f"Unable to kill job {job_name!r}: The job was not found."
+                    ) from exc
+                else:
+                    raise
+
     def _get_configured_kubernetes_client(
         self, configuration: KubernetesWorkerJobConfiguration
     ) -> "ApiClient":
         """
         Returns a configured Kubernetes client.
         """
```

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/PKG-INFO` & `prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # prefect-kubernetes
```

### Comparing `prefect-kubernetes-0.2.4/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/setup.cfg` & `prefect-kubernetes-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/setup.py` & `prefect-kubernetes-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,10 +38,11 @@
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

### Comparing `prefect-kubernetes-0.2.4/tests/test_block_standards.py` & `prefect-kubernetes-0.2.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_credentials.py` & `prefect-kubernetes-0.2.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_custom_objects.py` & `prefect-kubernetes-0.2.5/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_deployments.py` & `prefect-kubernetes-0.2.5/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_flows.py` & `prefect-kubernetes-0.2.5/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_jobs.py` & `prefect-kubernetes-0.2.5/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_pods.py` & `prefect-kubernetes-0.2.5/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_services.py` & `prefect-kubernetes-0.2.5/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_utilities.py` & `prefect-kubernetes-0.2.5/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.4/tests/test_worker.py` & `prefect-kubernetes-0.2.5/tests/test_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pendulum
 import prefect
 import pytest
 from kubernetes.client.exceptions import ApiException
 from kubernetes.config import ConfigException
 from prefect.client.schemas import FlowRun
 from prefect.docker import get_prefect_image_name
+from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
@@ -1838,7 +1839,148 @@
                     func=mock_batch_client.list_namespaced_job,
                     field_selector=mock.ANY,
                     namespace=mock.ANY,
                     timeout_seconds=pytest.approx(10, abs=1),
                 ),
             ]
         )
+
+    class TestKillInfrastructure:
+        async def test_kill_infrastructure_calls_delete_namespaced_job(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                await k8s_worker.kill_infrastructure(
+                    infrastructure_pid=f"{MOCK_CLUSTER_UID}:default:mock-k8s-v1-job",
+                    grace_seconds=0,
+                    configuration=default_configuration,
+                )
+
+            assert len(mock_batch_client.mock_calls) == 1
+            mock_batch_client.delete_namespaced_job.assert_called_once_with(
+                name="mock-k8s-v1-job",
+                namespace="default",
+                grace_period_seconds=0,
+                propagation_policy="Foreground",
+            )
+
+        async def test_kill_infrastructure_uses_correct_grace_seconds(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            GRACE_SECONDS = 42
+            async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                await k8s_worker.kill_infrastructure(
+                    infrastructure_pid=f"{MOCK_CLUSTER_UID}:default:mock-k8s-v1-job",
+                    grace_seconds=GRACE_SECONDS,
+                    configuration=default_configuration,
+                )
+
+            assert len(mock_batch_client.mock_calls) == 1
+            mock_batch_client.delete_namespaced_job.assert_called_once_with(
+                name="mock-k8s-v1-job",
+                namespace="default",
+                grace_period_seconds=GRACE_SECONDS,
+                propagation_policy="Foreground",
+            )
+
+        async def test_kill_infrastructure_raises_infra_not_available_on_mismatched_cluster_namespace(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            BAD_NAMESPACE = "dog"
+            with pytest.raises(
+                InfrastructureNotAvailable,
+                match=(
+                    "Unable to kill job 'mock-k8s-v1-job': The job is running in "
+                    f"namespace {BAD_NAMESPACE!r} but this worker expected jobs "
+                    "to be running in namespace 'default' based on the work pool and "
+                    "deployment configuration."
+                ),
+            ):
+                async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                    await k8s_worker.kill_infrastructure(
+                        infrastructure_pid=f"{MOCK_CLUSTER_UID}:{BAD_NAMESPACE}:mock-k8s-v1-job",
+                        grace_seconds=0,
+                        configuration=default_configuration,
+                    )
+
+        async def test_kill_infrastructure_raises_infra_not_available_on_mismatched_cluster_uid(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            BAD_CLUSTER = "4321"
+
+            with pytest.raises(
+                InfrastructureNotAvailable,
+                match=(
+                    "Unable to kill job 'mock-k8s-v1-job': The job is running on another "
+                    "cluster."
+                ),
+            ):
+                async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                    await k8s_worker.kill_infrastructure(
+                        infrastructure_pid=f"{BAD_CLUSTER}:default:mock-k8s-v1-job",
+                        grace_seconds=0,
+                        configuration=default_configuration,
+                    )
+
+        async def test_kill_infrastructure_raises_infrastructure_not_found_on_404(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            mock_batch_client.delete_namespaced_job.side_effect = [
+                ApiException(status=404)
+            ]
+
+            with pytest.raises(
+                InfrastructureNotFound,
+                match="Unable to kill job 'mock-k8s-v1-job': The job was not found.",
+            ):
+                async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                    await k8s_worker.kill_infrastructure(
+                        infrastructure_pid=f"{MOCK_CLUSTER_UID}:default:mock-k8s-v1-job",
+                        grace_seconds=0,
+                        configuration=default_configuration,
+                    )
+
+        async def test_kill_infrastructure_passes_other_k8s_api_errors_through(
+            self,
+            default_configuration,
+            mock_batch_client,
+            mock_core_client,
+            mock_watch,
+            monkeypatch,
+        ):
+            mock_batch_client.delete_namespaced_job.side_effect = [
+                ApiException(status=400)
+            ]
+            with pytest.raises(
+                ApiException,
+            ):
+                async with KubernetesWorker(work_pool_name="test") as k8s_worker:
+                    await k8s_worker.kill_infrastructure(
+                        infrastructure_pid=f"{MOCK_CLUSTER_UID}:default:dog",
+                        grace_seconds=0,
+                        configuration=default_configuration,
+                    )
```

### Comparing `prefect-kubernetes-0.2.4/versioneer.py` & `prefect-kubernetes-0.2.5/versioneer.py`

 * *Files identical despite different names*

