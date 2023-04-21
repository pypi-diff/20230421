# Comparing `tmp/prefect-docker-0.2.1.tar.gz` & `tmp/prefect-docker-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-gnqi19rs/prefect-docker-0.2.1.tar", last modified: Thu Apr  6 16:48:14 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-2imrtbfp/prefect-docker-0.2.2.tar", last modified: Fri Apr 21 00:04:48 2023, max compression
```

## Comparing `prefect-docker-0.2.1.tar` & `prefect-docker-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 16:48:14.000000 prefect-docker-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    39036 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-06 16:46:52.000000 prefect-docker-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41841 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/versioneer.py
```

### Comparing `prefect-docker-0.2.1/LICENSE` & `prefect-docker-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/PKG-INFO` & `prefect-docker-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.1
+Version: 0.2.2
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.1/README.md` & `prefect-docker-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/prefect_docker/containers.py` & `prefect-docker-0.2.2/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/prefect_docker/credentials.py` & `prefect-docker-0.2.2/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/prefect_docker/host.py` & `prefect-docker-0.2.2/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/prefect_docker/images.py` & `prefect-docker-0.2.2/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/prefect_docker/projects/steps.py` & `prefect-docker-0.2.2/prefect_docker/projects/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         ```yaml
         build:
             - prefect_docker.projects.steps.build_docker_image:
                 requires: prefect-docker
                 image_name: repo-name/image-name
                 tag: dev
                 dockerfile: auto
-                credentials: "{{ prefect.block.docker-registry-credentials.dev-registry }}"
+                credentials: "{{ prefect.blocks.docker-registry-credentials.dev-registry }}"
         ```
     """  # noqa
     auto_build = dockerfile == "auto"
     if auto_build:
         lines = []
         base_image = get_prefect_image_name()
         lines.append(f"FROM {base_image}")
```

### Comparing `prefect-docker-0.2.1/prefect_docker/worker.py` & `prefect-docker-0.2.2/prefect_docker/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,41 +28,31 @@
 import anyio.abc
 import docker
 import docker.errors
 import packaging.version
 import prefect
 from docker import DockerClient
 from docker.models.containers import Container
-from packaging import version
 from prefect.client.orchestration import ServerType, get_client
 from prefect.client.schemas import FlowRun
 from prefect.docker import (
     format_outlier_version_name,
     get_prefect_image_name,
     parse_image_tag,
 )
+from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import PREFECT_API_URL
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
+from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
 from pydantic import Field, validator
 from slugify import slugify
 from typing_extensions import Literal
 
-# TODO: Remove this after next prefect release
-if version.parse(prefect.__version__) <= version.parse("2.9.0"):
-    from prefect.experimental.workers.base import (
-        BaseJobConfiguration,
-        BaseWorker,
-        BaseWorkerResult,
-    )
-else:
-    from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
-
-
 CONTAINER_LABELS = {
     "io.prefect.version": prefect.__version__,
 }
 
 
 class ImagePullPolicy(enum.Enum):
     """Enum representing the image pull policy options for a Docker container."""
@@ -419,14 +409,63 @@
 
         exit_code = container.attrs["State"].get("ExitCode")
         return DockerWorkerResult(
             status_code=exit_code if exit_code is not None else -1,
             identifier=container_pid,
         )
 
+    async def kill_infrastructure(
+        self,
+        infrastructure_pid: str,
+        configuration: DockerWorkerJobConfiguration,
+        grace_seconds: int = 30,
+    ):
+        """
+        Stops a container for a cancelled flow run based on the provided infrastructure
+        PID.
+        """
+        docker_client = self._get_client()
+
+        base_url, container_id = self._parse_infrastructure_pid(infrastructure_pid)
+        if docker_client.api.base_url != base_url:
+            raise InfrastructureNotAvailable(
+                "".join(
+                    [
+                        (
+                            f"Unable to stop container {container_id!r}: the current"
+                            " Docker API "
+                        ),
+                        (
+                            f"URL {docker_client.api.base_url!r} does not match the"
+                            " expected "
+                        ),
+                        f"API base URL {base_url}.",
+                    ]
+                )
+            )
+        await run_sync_in_worker_thread(
+            self._stop_container, container_id, docker_client, grace_seconds
+        )
+
+    def _stop_container(
+        self,
+        container_id: str,
+        client: "DockerClient",
+        grace_seconds: int = 30,
+    ):
+        try:
+            container = client.containers.get(container_id=container_id)
+        except docker.errors.NotFound:
+            raise InfrastructureNotFound(
+                f"Unable to stop container {container_id!r}: The container was not"
+                " found."
+            )
+
+        container.stop(timeout=grace_seconds)
+
     def _get_client(self):
         """Returns a docker client."""
         try:
             with warnings.catch_warnings():
                 # Silence warnings due to use of deprecated methods within dockerpy
                 # See https://github.com/docker/docker-py/pull/2931
                 warnings.filterwarnings(
```

### Comparing `prefect-docker-0.2.1/prefect_docker.egg-info/PKG-INFO` & `prefect-docker-0.2.2/prefect_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.1
+Version: 0.2.2
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.1/prefect_docker.egg-info/SOURCES.txt` & `prefect-docker-0.2.2/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/setup.cfg` & `prefect-docker-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/setup.py` & `prefect-docker-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/tests/test_containers.py` & `prefect-docker-0.2.2/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/tests/test_host.py` & `prefect-docker-0.2.2/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/tests/test_images.py` & `prefect-docker-0.2.2/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.1/tests/test_worker.py` & `prefect-docker-0.2.2/tests/test_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import re
 import uuid
 from unittest.mock import MagicMock
 
 import anyio.abc
 import docker
+import docker.errors
 import docker.models.containers
 import pytest
 from docker import DockerClient
 from docker.models.containers import Container
 from prefect.client.schemas import FlowRun
 from prefect.docker import get_prefect_image_name
+from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
 )
 from prefect.testing.utilities import assert_does_not_warn
@@ -1011,7 +1014,76 @@
     assert "hello" in captured.out
 
 
 async def test_worker_errors_out_on_ephemeral_apis():
     with pytest.raises(RuntimeError, match="ephemeral"):
         async with DockerWorker(work_pool_name="test", test_mode=False) as worker:
             await worker.run()
+
+
+async def test_kill_infrastructure_calls_container_stop(
+    mock_docker_client, default_docker_worker_job_configuration
+):
+    async with DockerWorker(work_pool_name="test") as worker:
+        await worker.kill_infrastructure(
+            infrastructure_pid=f"{FAKE_BASE_URL}:{FAKE_CONTAINER_ID}",
+            configuration=default_docker_worker_job_configuration,
+            grace_seconds=0,
+        )
+    mock_docker_client.containers.get.return_value.stop.assert_called_once()
+
+
+async def test_kill_infrastructure_calls_container_stop_with_correct_grace_seconds(
+    mock_docker_client, default_docker_worker_job_configuration
+):
+    GRACE_SECONDS = 42
+    async with DockerWorker(work_pool_name="test") as worker:
+        await worker.kill_infrastructure(
+            infrastructure_pid=f"{FAKE_BASE_URL}:{FAKE_CONTAINER_ID}",
+            configuration=default_docker_worker_job_configuration,
+            grace_seconds=GRACE_SECONDS,
+        )
+
+    mock_docker_client.containers.get.return_value.stop.assert_called_with(
+        timeout=GRACE_SECONDS
+    )
+
+
+async def test_kill_infrastructure_raises_infra_not_available_with_bad_host_url(
+    mock_docker_client, default_docker_worker_job_configuration
+):
+    BAD_BASE_URL = "bad-base-url"
+    expected_string = "".join(
+        [
+            f"Unable to stop container {FAKE_CONTAINER_ID!r}: the current Docker API ",
+            f"URL {mock_docker_client.api.base_url!r} does not match the expected ",
+            f"API base URL {BAD_BASE_URL}.",
+        ]
+    )
+    with pytest.raises(InfrastructureNotAvailable, match=re.escape(expected_string)):
+        async with DockerWorker(work_pool_name="test") as worker:
+            await worker.kill_infrastructure(
+                infrastructure_pid=f"{BAD_BASE_URL}:{FAKE_CONTAINER_ID}",
+                configuration=default_docker_worker_job_configuration,
+                grace_seconds=0,
+            )
+
+
+async def test_kill_infrastructure_raises_infra_not_found_with_bad_container_id(
+    mock_docker_client, default_docker_worker_job_configuration
+):
+    mock_docker_client.containers.get.side_effect = [docker.errors.NotFound("msg")]
+
+    BAD_CONTAINER_ID = "bad-container-id"
+    with pytest.raises(
+        InfrastructureNotFound,
+        match=(
+            f"Unable to stop container {BAD_CONTAINER_ID!r}: The container was not"
+            " found."
+        ),
+    ):
+        async with DockerWorker(work_pool_name="test") as worker:
+            await worker.kill_infrastructure(
+                infrastructure_pid=f"{FAKE_BASE_URL}:{BAD_CONTAINER_ID}",
+                configuration=default_docker_worker_job_configuration,
+                grace_seconds=0,
+            )
```

### Comparing `prefect-docker-0.2.1/versioneer.py` & `prefect-docker-0.2.2/versioneer.py`

 * *Files identical despite different names*

