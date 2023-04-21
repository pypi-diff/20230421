# Comparing `tmp/gefyra-1.0.4.tar.gz` & `tmp/gefyra-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.0.4.tar", max compression
+gzip compressed data, was "gefyra-1.0.5.tar", max compression
```

## Comparing `gefyra-1.0.4.tar` & `gefyra-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2151 2023-03-14 15:37:12.993181 gefyra-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/__init__.py
--rw-r--r--   0        0        0    13357 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/__main__.py
--rw-r--r--   0        0        0      169 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/list.py
--rw-r--r--   0        0        0     6218 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/up.py
--rw-r--r--   0        0        0     1078 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     5507 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8727 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     1608 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8959 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6416 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1037 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0      945 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/networking.py
--rw-r--r--   0        0        0     3918 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-03-14 15:37:12.993181 gefyra-1.0.4/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-03-14 15:37:12.993181 gefyra-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-04-21 14:57:48.029554 gefyra-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/__init__.py
+-rw-r--r--   0        0        0    13357 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/__main__.py
+-rw-r--r--   0        0        0      169 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/list.py
+-rw-r--r--   0        0        0     6218 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/up.py
+-rw-r--r--   0        0        0     1078 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     5507 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     1608 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8959 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1037 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0      945 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3918 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-04-21 14:57:48.029554 gefyra-1.0.5/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-04-21 14:57:48.033554 gefyra-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.5/PKG-INFO
```

### Comparing `gefyra-1.0.4/README.md` & `gefyra-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/__main__.py` & `gefyra-1.0.5/gefyra/__main__.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/bridge.py` & `gefyra-1.0.5/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/down.py` & `gefyra-1.0.5/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/list.py` & `gefyra-1.0.5/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/run.py` & `gefyra-1.0.5/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/status.py` & `gefyra-1.0.5/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/up.py` & `gefyra-1.0.5/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/api/utils.py` & `gefyra-1.0.5/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/cluster/manager.py` & `gefyra-1.0.5/gefyra/cluster/manager.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/cluster/resources.py` & `gefyra-1.0.5/gefyra/cluster/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,18 +203,22 @@
     pod: V1Pod,
     workload: Union[V1Deployment, V1StatefulSet],
     config: ClientConfiguration,
 ) -> bool:
     if workload.kind == "StatefulSet":
         return pod.metadata.owner_references[0].uid == workload.metadata.uid
     elif workload.kind == "Deployment":
-        replicaset_set = config.K8S_APP_API.read_namespaced_replica_set(
-            name=pod.metadata.owner_references[0].name,
-            namespace=pod.metadata.namespace,
-        )
+        try:
+            replicaset_set = config.K8S_APP_API.read_namespaced_replica_set(
+                name=pod.metadata.owner_references[0].name,
+                namespace=pod.metadata.namespace,
+            )
+        except ApiException as e:
+            if e.status == 404:
+                return False
         return replicaset_set.metadata.owner_references[0].uid == workload.metadata.uid
     raise RuntimeError(
         f"Unknown workload type for owner reference check: {workload.kind}/{workload.metadata.name}."
     )
 
 
 def get_pods_and_containers_for_workload(
@@ -253,15 +257,14 @@
         namespace=namespace, label_selector=label_selector
     )
     for pod in pods.items:
         if owner_reference_consistent(pod, workload, config):
             result[pod.metadata.name] = [
                 container.name for container in pod.spec.containers
             ]
-
     return result
 
 
 def get_pods_and_containers_for_pod_name(
     config: ClientConfiguration, name: str, namespace: str
 ) -> Dict[str, List[str]]:
     result = {}
```

### Comparing `gefyra-1.0.4/gefyra/cluster/utils.py` & `gefyra-1.0.5/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/configuration.py` & `gefyra-1.0.5/gefyra/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.0.4"
+__VERSION__ = "1.0.5"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
```

### Comparing `gefyra-1.0.4/gefyra/local/bridge.py` & `gefyra-1.0.5/gefyra/local/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,11 +194,16 @@
     exit_code, output = cargo.exec_run(
         f"bash patchContainerGateway.sh {container.name} {cargo_ip}"
     )
     if exit_code == 0:
         logger.debug(f"Gateway patch applied to '{container.name}'")
 
     else:
+        container = config.DOCKER.containers.get(container.id)
+        if container.status != "running":
+            raise RuntimeError(
+                f"Container {name} is not running. Check whether your command is valid for the chosen image."
+            )
         raise RuntimeError(
             f"Gateway patch could not be applied to '{container.name}': {output}"
         )
     return container
```

### Comparing `gefyra-1.0.4/gefyra/local/cargo.py` & `gefyra-1.0.5/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.0.5/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/check.py` & `gefyra-1.0.5/gefyra/local/check.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/minikube.py` & `gefyra-1.0.5/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/networking.py` & `gefyra-1.0.5/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/telemetry.py` & `gefyra-1.0.5/gefyra/local/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/gefyra/local/utils.py` & `gefyra-1.0.5/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.4/pyproject.toml` & `gefyra-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.0.4"
+version = "1.0.5"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.0.4/PKG-INFO` & `gefyra-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.0.4
+Version: 1.0.5
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

