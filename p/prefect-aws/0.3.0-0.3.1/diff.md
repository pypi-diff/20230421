# Comparing `tmp/prefect-aws-0.3.0.tar.gz` & `tmp/prefect-aws-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-4uymi3en/prefect-aws-0.3.0.tar", last modified: Thu Apr  6 13:35:12 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-o3glckyr/prefect-aws-0.3.1.tar", last modified: Fri Apr 21 00:08:40 2023, max compression
```

## Comparing `prefect-aws-0.3.0.tar` & `prefect-aws-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    57054 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/ecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    32792 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 13:35:12.000000 prefect-aws-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    66908 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-06 13:33:33.000000 prefect-aws-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57767 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/ecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32782 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56563 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:08:40.000000 prefect-aws-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67274 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-04-21 00:06:59.000000 prefect-aws-0.3.1/versioneer.py
```

### Comparing `prefect-aws-0.3.0/LICENSE` & `prefect-aws-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/PKG-INFO` & `prefect-aws-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.0
+Version: 0.3.1
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.0 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.1 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.0/README.md` & `prefect-aws-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/prefect_aws/batch.py` & `prefect-aws-0.3.1/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/prefect_aws/client_parameters.py` & `prefect-aws-0.3.1/prefect_aws/client_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,16 +81,18 @@
         """
         verify = values.get("verify")
 
         # deprecate using verify in favor of verify_cert_path
         # so the UI looks nicer
         if verify is not None and not isinstance(verify, bool):
             warnings.warn(
-                "verify should be a boolean. "
-                "If you want to use a CA cert bundle, use verify_cert_path instead.",
+                (
+                    "verify should be a boolean. "
+                    "If you want to use a CA cert bundle, use verify_cert_path instead."
+                ),
                 DeprecationWarning,
             )
         return values
 
     @root_validator
     def verify_cert_path_and_verify(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """
```

### Comparing `prefect-aws-0.3.0/prefect_aws/client_waiter.py` & `prefect-aws-0.3.1/prefect_aws/client_waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,11 +66,11 @@
         waiter_model = WaiterModel(waiter_definition)
         waiter = create_waiter_with_client(waiter_name, waiter_model, boto_client)
     elif waiter_name in boto_client.waiter_names:
         waiter = boto_client.get_waiter(waiter_name)
     else:
         raise ValueError(
             f"The waiter name, {waiter_name}, is not a valid boto waiter; "
-            f"if using a custom waiter, you must provide a waiter definition"
+            "if using a custom waiter, you must provide a waiter definition"
         )
 
     await run_sync_in_worker_thread(waiter.wait, **waiter_kwargs)
```

### Comparing `prefect-aws-0.3.0/prefect_aws/credentials.py` & `prefect-aws-0.3.1/prefect_aws/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from prefect.blocks.abstract import CredentialsBlock
 from pydantic import Field, SecretStr
 
 from prefect_aws.client_parameters import AwsClientParameters
 
 
 class ClientType(Enum):
-
     S3 = "s3"
     ECS = "ecs"
     BATCH = "batch"
     SECRETS_MANAGER = "secretsmanager"
 
 
 class AwsCredentials(CredentialsBlock):
```

### Comparing `prefect-aws-0.3.0/prefect_aws/ecs.py` & `prefect-aws-0.3.1/prefect_aws/ecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.pydantic import JsonPatch
 from pydantic import Field, root_validator, validator
 from slugify import slugify
 from typing_extensions import Literal, Self
 
 from prefect_aws import AwsCredentials
+from prefect_aws.workers.ecs_worker import _TAG_REGEX
 
 # Internal type alias for ECS clients which are generated dynamically in botocore
 _ECSClient = Any
 
 
 if TYPE_CHECKING:
     from prefect.client.schemas import FlowRun
@@ -148,14 +149,15 @@
     "compatibilities",
     "taskDefinitionArn",
     "revision",
     "status",
     "requiresAttributes",
     "registeredAt",
     "registeredBy",
+    "deregisteredAt",
 ]
 
 
 def get_prefect_container(containers: List[dict]) -> Optional[dict]:
     """
     Extract the Prefect container from a list of containers or container definitions.
     If not found, `None` is returned.
@@ -386,23 +388,23 @@
             "console. Unless you have configured AWS CloudWatch logs manually on your "
             "task definition, this requires the same prerequisites outlined in "
             "`configure_cloudwatch_logs`."
         ),
     )
 
     # Task run settings
-    launch_type: Optional[
-        Literal["FARGATE", "EC2", "EXTERNAL", "FARGATE_SPOT"]
-    ] = Field(
-        default="FARGATE",
-        description=(
-            "The type of ECS task run infrastructure that should be used. Note that "
-            "'FARGATE_SPOT' is not a formal ECS launch type, but we will configure the "
-            "proper capacity provider stategy if set here."
-        ),
+    launch_type: Optional[Literal["FARGATE", "EC2", "EXTERNAL", "FARGATE_SPOT"]] = (
+        Field(
+            default="FARGATE",
+            description=(
+                "The type of ECS task run infrastructure that should be used. Note that"
+                " 'FARGATE_SPOT' is not a formal ECS launch type, but we will configure"
+                " the proper capacity provider stategy if set here."
+            ),
+        )
     )
     vpc_id: Optional[str] = Field(
         title="VPC ID",
         default=None,
         description=(
             "The AWS VPC to link the task run to. This is only applicable when using "
             "the 'awsvpc' network mode for your task. FARGATE tasks require this "
@@ -689,15 +691,17 @@
             ecs_client.stop_task(cluster=cluster, task=task)
         except Exception as exc:
             # Raise a special exception if the task does not exist
             if "ClusterNotFound" in str(exc):
                 raise InfrastructureNotFound(
                     f"Cannot stop ECS task: the cluster {cluster!r} could not be found."
                 ) from exc
-            if "not find task" in str(exc):
+            if "not find task" in str(exc) or "referenced task was not found" in str(
+                exc
+            ):
                 raise InfrastructureNotFound(
                     f"Cannot stop ECS task: the task {task!r} could not be found in "
                     f"cluster {cluster!r}."
                 ) from exc
             if "no registered tasks" in str(exc):
                 raise InfrastructureNotFound(
                     f"Cannot stop ECS task: the cluster {cluster!r} has no tasks."
@@ -1009,17 +1013,17 @@
         reaches a STOPPED status or the provided `until_status`.
 
         Emits a log each time the status changes.
         """
         last_status = status = current_status
         t0 = time.time()
         while status != until_status:
-            tasks = ecs_client.describe_tasks(tasks=[task_arn], cluster=cluster_arn)[
-                "tasks"
-            ]
+            tasks = ecs_client.describe_tasks(
+                tasks=[task_arn], cluster=cluster_arn, include=["TAGS"]
+            )["tasks"]
 
             if tasks:
                 task = tasks[0]
 
                 status = task["lastStatus"]
                 if status != last_status:
                     self.logger.info(f"{self._log_prefix}: Status is {status}.")
@@ -1037,15 +1041,15 @@
                 # watch timeout though.
                 self.logger.debug(f"{self._log_prefix}: Task not found.")
 
             elapsed_time = time.time() - t0
             if timeout is not None and elapsed_time > timeout:
                 raise RuntimeError(
                     f"Timed out after {elapsed_time}s while watching task for status "
-                    "{until_status or 'STOPPED'}"
+                    f"{until_status or 'STOPPED'}"
                 )
             time.sleep(self.task_watch_poll_interval)
 
     def _wait_for_task_start(
         self, task_arn: str, cluster_arn: str, ecs_client: _ECSClient, timeout: int
     ) -> dict:
         """
@@ -1401,15 +1405,16 @@
             help_message = (
                 "Pass an explicit `vpc_id` or configure a default VPC."
                 if not vpc_id
                 else "Check that the VPC exists in the current region."
             )
             raise ValueError(
                 f"Failed to find {vpc_message}. "
-                "Network configuration cannot be inferred. " + help_message
+                "Network configuration cannot be inferred. "
+                + help_message
             )
 
         vpc_id = vpcs[0]["VpcId"]
         subnets = ec2_client.describe_subnets(
             Filters=[{"Name": "vpc-id", "Values": [vpc_id]}]
         )["Subnets"]
         if not subnets:
@@ -1418,29 +1423,44 @@
                 "Network configuration cannot be inferred."
             )
 
         return {
             "awsvpcConfiguration": {
                 "subnets": [s["SubnetId"] for s in subnets],
                 "assignPublicIp": "ENABLED",
+                "securityGroups": [],
             }
         }
 
     def _prepare_task_run(
         self,
         network_config: Optional[dict],
         task_definition_arn: str,
     ) -> dict:
         """
         Prepare a task run request payload.
         """
         task_run = {
             "overrides": self._prepare_task_run_overrides(),
             "tags": [
-                {"key": key, "value": value} for key, value in self.labels.items()
+                {
+                    "key": slugify(
+                        key,
+                        regex_pattern=_TAG_REGEX,
+                        allow_unicode=True,
+                        lowercase=False,
+                    ),
+                    "value": slugify(
+                        value,
+                        regex_pattern=_TAG_REGEX,
+                        allow_unicode=True,
+                        lowercase=False,
+                    ),
+                }
+                for key, value in self.labels.items()
             ],
             "taskDefinition": task_definition_arn,
         }
 
         if self.cluster:
             task_run["cluster"] = self.cluster
```

### Comparing `prefect-aws-0.3.0/prefect_aws/projects/steps.py` & `prefect-aws-0.3.1/prefect_aws/projects/steps.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,29 +149,34 @@
         ```
     """
     if credentials is None:
         credentials = {}
     if client_parameters is None:
         client_parameters = {}
     advanced_config = client_parameters.pop("config", {})
-    bucket_resource = (
-        boto3.Session(**credentials)
-        .resource("s3", **client_parameters, config=Config(**advanced_config))
-        .Bucket(bucket)
-    )
+
+    session = boto3.Session(**credentials)
+    s3 = session.client("s3", **client_parameters, config=Config(**advanced_config))
 
     local_path = Path.cwd()
-    for obj in bucket_resource.objects.filter(Prefix=folder):
-        if obj.key[-1] == "/":
-            # object is a folder and will be created if it contains any objects
-            continue
-        target = PurePosixPath(
-            local_path / relative_path_to_current_platform(obj.key).relative_to(folder)
-        )
-        Path.mkdir(Path(target.parent), parents=True, exist_ok=True)
-        bucket_resource.download_file(obj.key, str(target))
+
+    paginator = s3.get_paginator("list_objects_v2")
+    for result in paginator.paginate(Bucket=bucket, Prefix=folder):
+        for obj in result.get("Contents", []):
+            remote_key = obj["Key"]
+
+            if remote_key[-1] == "/":
+                # object is a folder and will be created if it contains any objects
+                continue
+
+            target = PurePosixPath(
+                local_path
+                / relative_path_to_current_platform(remote_key).relative_to(folder)
+            )
+            Path.mkdir(Path(target.parent), parents=True, exist_ok=True)
+            s3.download_file(bucket, remote_key, str(target))
 
     return {
         "bucket": bucket,
         "folder": folder,
         "directory": str(local_path),
     }
```

### Comparing `prefect-aws-0.3.0/prefect_aws/s3.py` & `prefect-aws-0.3.1/prefect_aws/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
         return self.bucket_folder
 
     @basepath.setter
     def basepath(self, value: str) -> None:
         self.bucket_folder = value
 
     def _resolve_path(self, path: str) -> str:
-
         """
         A helper function used in write_path to join `self.basepath` and `path`.
 
         Args:
 
             path: Name of the key, e.g. "file1". Each object in your
                 bucket has a unique key (or key name).
@@ -299,15 +298,14 @@
         path = (
             (Path(self.bucket_folder) / path).as_posix() if self.bucket_folder else path
         )
 
         return path
 
     def _get_s3_client(self) -> boto3.client:
-
         """
         Authenticate MinIO credentials or AWS credentials and return an S3 client.
         This is a helper function called by read_path() or write_path().
         """
         return self.credentials.get_s3_client()
 
     def _get_bucket_resource(self) -> boto3.resource:
@@ -412,15 +410,14 @@
                 )
                 uploaded_file_count += 1
 
         return uploaded_file_count
 
     @sync_compatible
     async def read_path(self, path: str) -> bytes:
-
         """
         Read specified path from S3 and return contents. Provide the entire
         path to the key in S3.
 
         Args:
             path: Entire path to (and including) the key.
 
@@ -445,32 +442,29 @@
             ```
         """
         path = self._resolve_path(path)
 
         return await run_sync_in_worker_thread(self._read_sync, path)
 
     def _read_sync(self, key: str) -> bytes:
-
         """
         Called by read_path(). Creates an S3 client and retrieves the
         contents from  a specified path.
         """
 
         s3_client = self._get_s3_client()
 
         with io.BytesIO() as stream:
-
             s3_client.download_fileobj(Bucket=self.bucket_name, Key=key, Fileobj=stream)
             stream.seek(0)
             output = stream.read()
             return output
 
     @sync_compatible
     async def write_path(self, path: str, content: bytes) -> str:
-
         """
         Writes to an S3 bucket.
 
         Args:
 
             path: The key name. Each object in your bucket has a unique
                 key (or key name).
@@ -501,24 +495,22 @@
         path = self._resolve_path(path)
 
         await run_sync_in_worker_thread(self._write_sync, path, content)
 
         return path
 
     def _write_sync(self, key: str, data: bytes) -> None:
-
         """
         Called by write_path(). Creates an S3 client and uploads a file
         object.
         """
 
         s3_client = self._get_s3_client()
 
         with io.BytesIO(data) as stream:
-
             s3_client.upload_fileobj(Fileobj=stream, Bucket=self.bucket_name, Key=key)
 
     # NEW BLOCK INTERFACE METHODS BELOW
     @staticmethod
     def _list_objects_sync(page_iterator: PageIterator) -> List[Dict[str, Any]]:
         """
         Synchronous method to collect S3 objects into a list
@@ -711,15 +703,15 @@
             Bucket=self.bucket_name,
             Key=bucket_path,
             Fileobj=to_file_object,
             **download_kwargs,
         )
         self.logger.info(
             f"Downloaded object from bucket {self.bucket_name!r} path {bucket_path!r} "
-            f"to file object."
+            "to file object."
         )
         return to_file_object
 
     @sync_compatible
     async def download_folder_to_path(
         self,
         from_folder: str,
@@ -881,15 +873,15 @@
             client.upload_fileobj,
             Fileobj=from_file_object,
             Bucket=self.bucket_name,
             Key=bucket_path,
             **upload_kwargs,
         )
         self.logger.info(
-            f"Uploaded from file object to the bucket "
+            "Uploaded from file object to the bucket "
             f"{self.bucket_name!r} path {bucket_path!r}."
         )
         return bucket_path
 
     @sync_compatible
     async def upload_from_folder(
         self,
```

### Comparing `prefect-aws-0.3.0/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.1/prefect_aws/secrets_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,17 +328,17 @@
 
     """
     if not force_delete_without_recovery and not (7 <= recovery_window_in_days <= 30):
         raise ValueError("Recovery window must be between 7 and 30 days.")
 
     delete_secret_kwargs: Dict[str, Union[str, int, bool]] = dict(SecretId=secret_name)
     if force_delete_without_recovery:
-        delete_secret_kwargs[
-            "ForceDeleteWithoutRecovery"
-        ] = force_delete_without_recovery
+        delete_secret_kwargs["ForceDeleteWithoutRecovery"] = (
+            force_delete_without_recovery
+        )
     else:
         delete_secret_kwargs["RecoveryWindowInDays"] = recovery_window_in_days
 
     logger = get_run_logger()
     logger.info("Deleting secret %s", secret_name)
 
     client = aws_credentials.get_boto3_session().client("secretsmanager")
@@ -486,15 +486,15 @@
         """
         if force_delete_without_recovery and recovery_window_in_days:
             raise ValueError(
                 "Cannot specify recovery window and force delete without recovery."
             )
         elif not (7 <= recovery_window_in_days <= 30):
             raise ValueError(
-                f"Recovery window must be between 7 and 30 days, got "
+                "Recovery window must be between 7 and 30 days, got "
                 f"{recovery_window_in_days}."
             )
 
         client = self.aws_credentials.get_secrets_manager_client()
         response = await run_sync_in_worker_thread(
             client.delete_secret,
             SecretId=self.secret_name,
```

### Comparing `prefect-aws-0.3.0/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.1/prefect_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.0
+Version: 0.3.1
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.0 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.1 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.0/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.1/prefect_aws.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 prefect_aws.egg-info/SOURCES.txt
 prefect_aws.egg-info/dependency_links.txt
 prefect_aws.egg-info/entry_points.txt
 prefect_aws.egg-info/requires.txt
 prefect_aws.egg-info/top_level.txt
 prefect_aws/projects/__init__.py
 prefect_aws/projects/steps.py
+prefect_aws/workers/__init__.py
+prefect_aws/workers/ecs_worker.py
 tests/test_batch.py
 tests/test_block_standards.py
 tests/test_client_parameters.py
 tests/test_client_waiter.py
 tests/test_credentials.py
 tests/test_ecs.py
 tests/test_s3.py
```

### Comparing `prefect-aws-0.3.0/setup.cfg` & `prefect-aws-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/setup.py` & `prefect-aws-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/tests/test_batch.py` & `prefect-aws-0.3.1/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/tests/test_block_standards.py` & `prefect-aws-0.3.1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/tests/test_client_parameters.py` & `prefect-aws-0.3.1/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/tests/test_client_waiter.py` & `prefect-aws-0.3.1/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/tests/test_credentials.py` & `prefect-aws-0.3.1/tests/test_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,26 @@
 from botocore.client import BaseClient
 from moto import mock_s3
 
 from prefect_aws.credentials import AwsCredentials, ClientType, MinIOCredentials
 
 
 def test_aws_credentials_get_boto3_session():
-
     """
     Asserts that instantiated AwsCredentials block creates an
     authenticated boto3 session.
     """
 
     with mock_s3():
         aws_credentials_block = AwsCredentials()
         boto3_session = aws_credentials_block.get_boto3_session()
         assert isinstance(boto3_session, Session)
 
 
 def test_minio_credentials_get_boto3_session():
-
     """
     Asserts that instantiated MinIOCredentials block creates
     an authenticated boto3 session.
     """
 
     minio_credentials_block = MinIOCredentials(
         minio_root_user="root_user", minio_root_password="root_password"
```

### Comparing `prefect-aws-0.3.0/tests/test_ecs.py` & `prefect-aws-0.3.1/tests/test_ecs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from functools import partial
 from typing import Any, Awaitable, Callable, Dict, List, Optional
 from unittest.mock import MagicMock
 
 import anyio
 import pytest
 import yaml
+from botocore.exceptions import ClientError
 from moto import mock_ec2, mock_ecs, mock_logs
 from moto.ec2.utils import generate_instance_identity_document
 from prefect.docker import get_prefect_image_name
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.logging.configuration import setup_logging
 from prefect.server.schemas.core import Deployment, Flow, FlowRun
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from pydantic import ValidationError
 
 from prefect_aws.ecs import (
     ECS_DEFAULT_CPU,
     ECS_DEFAULT_MEMORY,
-    PREFECT_ECS_CONTAINER_NAME,
     ECSTask,
     get_container,
     get_prefect_container,
     parse_task_identifier,
 )
 
 setup_logging()
@@ -55,32 +55,35 @@
             for attr, attr_patches in patches.items():
                 original_method = getattr(backend, attr)
                 setattr(
                     backend, attr, partial(injected_call, original_method, attr_patches)
                 )
 
 
+def patch_run_task(mock, run_task, *args, **kwargs):
+    """
+    Track calls to `run_task` by calling a mock as well.
+    """
+    mock(*args, **kwargs)
+    return run_task(*args, **kwargs)
+
+
 def patch_describe_tasks_add_prefect_container(describe_tasks, *args, **kwargs):
     """
     Adds the minimal prefect container to moto's task description.
     """
     result = describe_tasks(*args, **kwargs)
     for task in result:
-        task.containers = [{"name": PREFECT_ECS_CONTAINER_NAME}]
+        if not task.containers:
+            task.containers = []
+        if not get_prefect_container(task.containers):
+            task.containers.append({"name": "prefect"})
     return result
 
 
-def patch_run_task(mock, run_task, *args, **kwargs):
-    """
-    Track calls to `run_task` by calling a mock as well.
-    """
-    mock(*args, **kwargs)
-    return run_task(*args, **kwargs)
-
-
 def patch_calculate_task_resource_requirements(
     _calculate_task_resource_requirements, task_definition
 ):
     """
     Adds support for non-EC2 execution modes to moto's calculation of task definition.
     """
     for container_definition in task_definition.container_definitions:
@@ -169,15 +172,17 @@
     return ecs_client.create_cluster(clusterName=cluster_name)["cluster"]["clusterArn"]
 
 
 def describe_task(ecs_client, task_arn, **kwargs) -> dict:
     """
     Describe a single ECS task
     """
-    return ecs_client.describe_tasks(tasks=[task_arn], **kwargs)["tasks"][0]
+    return ecs_client.describe_tasks(tasks=[task_arn], include=["TAGS"], **kwargs)[
+        "tasks"
+    ][0]
 
 
 async def stop_task(ecs_client, task_arn, **kwargs):
     """
     Stop an ECS task.
 
     Additional keyword arguments are passed to `ECSClient.stop_task`.
@@ -237,15 +242,15 @@
         with mock_ec2():
             with mock_logs():
                 session = aws_credentials.get_boto3_session()
 
                 inject_moto_patches(
                     ecs,
                     {
-                        # Add a container when describing any task
+                        # Ensure container is created in described tasks
                         "describe_tasks": [patch_describe_tasks_add_prefect_container],
                         # Fix moto internal resource requirement calculations
                         "_calculate_task_resource_requirements": [
                             patch_calculate_task_resource_requirements
                         ],
                         # Add log group creation
                         "run_task": [partial(create_log_stream, session)],
@@ -944,15 +949,19 @@
 
     await run_then_stop_task(task)
 
     network_configuration = mock_run_task.call_args[0][1].get("networkConfiguration")
 
     # Subnet ids are copied from the vpc
     assert network_configuration == {
-        "awsvpcConfiguration": {"subnets": [subnet.id], "assignPublicIp": "ENABLED"}
+        "awsvpcConfiguration": {
+            "subnets": [subnet.id],
+            "assignPublicIp": "ENABLED",
+            "securityGroups": [],
+        }
     }
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_network_config_from_default_vpc(aws_credentials):
     session = aws_credentials.get_boto3_session()
     ec2_client = session.client("ec2")
@@ -978,14 +987,15 @@
     network_configuration = mock_run_task.call_args[0][1].get("networkConfiguration")
 
     # Subnet ids are copied from the vpc
     assert network_configuration == {
         "awsvpcConfiguration": {
             "subnets": [subnet["SubnetId"] for subnet in default_subnets],
             "assignPublicIp": "ENABLED",
+            "securityGroups": [],
         }
     }
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 @pytest.mark.parametrize("explicit_network_mode", [True, False])
 async def test_network_config_is_empty_without_awsvpc_network_mode(
@@ -1062,15 +1072,18 @@
         )
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_log_options_requires_logging(aws_credentials):
     with pytest.raises(
         ValidationError,
-        match="`configure_cloudwatch_log` must be enabled to use `cloudwatch_logs_options`",  # noqa
+        match=(  # noqa
+            "`configure_cloudwatch_log` must be enabled to use"
+            " `cloudwatch_logs_options`"
+        ),
     ):
         ECSTask(
             aws_credentials=aws_credentials,
             command=["prefect", "version"],
             configure_cloudwatch_logs=False,
             cloudwatch_logs_options={"foo": " bar"},
         )
@@ -1237,15 +1250,16 @@
     with pytest.warns(
         UserWarning,
         match=(
             "Found network mode 'bridge' which is not compatible with launch type "
             f"{launch_type!r}"
         ),
     ):
-        await run_then_stop_task(task)
+        with pytest.raises(ClientError):
+            await run_then_stop_task(task)
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_deregister_task_definition(aws_credentials):
     task = ECSTask(
         aws_credentials=aws_credentials,
         auto_deregister_task_definition=True,
@@ -1254,17 +1268,16 @@
 
     session = aws_credentials.get_boto3_session()
     ecs_client = session.client("ecs")
 
     task_arn = await run_then_stop_task(task)
 
     task = describe_task(ecs_client, task_arn)
-    with pytest.raises(Exception, match="is not a task_definition"):
-        # Oh no it's gone
-        describe_task_definition(ecs_client, task)
+    task_definition = describe_task_definition(ecs_client, task)
+    assert task_definition["status"] == "INACTIVE"
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_latest_task_definition_used_if_equal(aws_credentials):
     task = ECSTask(aws_credentials=aws_credentials)
     print(task.preview())
 
@@ -1451,15 +1464,16 @@
         task["taskDefinitionArn"] != task_definition_arn
     ), "A new task definition should be registered"
 
     assert (
         "Settings require changes to the linked task definition. "
         "A new task definition will be registered. "
         "Enable DEBUG level logs to see the difference."
-    ) in caplog.text
+        in caplog.text
+    )
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_task_definition_arn_with_overrides_requiring_copy_shows_diff(
     aws_credentials, caplog
 ):
     """
@@ -1483,24 +1497,23 @@
     print(task.preview())
     with caplog.at_level(logging.DEBUG, logger=task.logger.name):
         await run_then_stop_task(task)
 
     assert (
         "Settings require changes to the linked task definition. "
         "A new task definition will be registered. "
-    ) in caplog.text
+        in caplog.text
+    )
 
-    assert ("Enable DEBUG level logs to see the difference.") not in caplog.text
+    assert "Enable DEBUG level logs to see the difference." not in caplog.text
 
-    expected_diff = textwrap.dedent(
-        """
+    expected_diff = textwrap.dedent("""
         -                            'image': 'prefecthq/prefect:2.1.0-python3.8',
         +                            'image': 'foobar',
-        """
-    )
+        """)
     assert expected_diff in caplog.text
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 @pytest.mark.parametrize(
     "overrides",
     [
@@ -1530,15 +1543,17 @@
     session = aws_credentials.get_boto3_session()
     ecs_client = session.client("ecs")
 
     if "cluster" in overrides:
         create_test_ecs_cluster(ecs_client, overrides["cluster"])
         add_ec2_instance_to_ecs_cluster(session, overrides["cluster"])
 
-    task_definition_arn = ecs_client.register_task_definition(**BASE_TASK_DEFINITION,)[
+    task_definition_arn = ecs_client.register_task_definition(
+        **BASE_TASK_DEFINITION,
+    )[
         "taskDefinition"
     ]["taskDefinitionArn"]
 
     # Set the default launch type for compatibility with the base task definition
     overrides.setdefault("launch_type", "EC2")
 
     task = ECSTask(
@@ -1573,16 +1588,15 @@
         launch_type="EC2",
         image=None,
     )
     print(task.preview())
     task_arn = await run_then_stop_task(task)
 
     task = describe_task(ecs_client, task_arn)
-    # The task definition can be retrieved still
-    assert describe_task_definition(ecs_client, task)
+    describe_task_definition(ecs_client, task)["status"] == "ACTIVE"
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_adding_security_groups_to_network_config(aws_credentials):
     session = aws_credentials.get_boto3_session()
     ec2_resource = session.resource("ec2")
     vpc = ec2_resource.create_vpc(CidrBlock="10.0.0.0/16")
@@ -1615,16 +1629,16 @@
 
     network_configuration = mock_run_task.call_args[0][1].get("networkConfiguration")
 
     # Subnet ids are copied from the vpc
     assert network_configuration == {
         "awsvpcConfiguration": {
             "subnets": [subnet.id],
-            "securityGroups": [security_group_id],
             "assignPublicIp": "ENABLED",
+            "securityGroups": [security_group_id],
         }
     }
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_disable_public_ip_in_network_config(aws_credentials):
     session = aws_credentials.get_boto3_session()
@@ -1656,14 +1670,15 @@
     network_configuration = mock_run_task.call_args[0][1].get("networkConfiguration")
 
     # Subnet ids are copied from the vpc
     assert network_configuration == {
         "awsvpcConfiguration": {
             "subnets": [subnet.id],
             "assignPublicIp": "DISABLED",
+            "securityGroups": [],
         }
     }
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_custom_subnets_in_the_network_configuration(aws_credentials):
     session = aws_credentials.get_boto3_session()
@@ -1699,14 +1714,15 @@
     network_configuration = mock_run_task.call_args[0][1].get("networkConfiguration")
 
     # Subnet ids are copied from the vpc
     assert network_configuration == {
         "awsvpcConfiguration": {
             "subnets": [subnet.id],
             "assignPublicIp": "DISABLED",
+            "securityGroups": [],
         }
     }
 
 
 @pytest.mark.usefixtures("ecs_mocks")
 async def test_task_customizations_as_string(aws_credentials):
     tc = (
```

### Comparing `prefect-aws-0.3.0/tests/test_s3.py` & `prefect-aws-0.3.1/tests/test_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,19 +275,17 @@
 
 
 BUCKET_NAME = "test_bucket"
 
 
 @pytest.fixture
 def s3():
-
     """Mock connection to AWS S3 with boto3 client."""
 
     with mock_s3():
-
         yield boto3.client(
             service_name="s3",
             region_name="us-east-1",
             aws_access_key_id="minioadmin",
             aws_secret_access_key="testing",
             aws_session_token="testing",
         )
@@ -307,15 +305,14 @@
 
     file.unlink()
     assert not file.exists()
 
 
 @pytest.fixture(params=["aws_credentials", "minio_credentials"])
 def s3_bucket(s3, request, aws_creds_block, minio_creds_block):
-
     key = request.param
 
     if key == "aws_credentials":
         fs = S3Bucket(bucket_name=BUCKET_NAME, credentials=aws_creds_block)
     elif key == "minio_credentials":
         fs = S3Bucket(bucket_name=BUCKET_NAME, credentials=minio_creds_block)
 
@@ -327,37 +324,34 @@
 @pytest.fixture
 def s3_bucket_with_file(s3_bucket):
     key = s3_bucket.write_path("test.txt", content=b"hello")
     return s3_bucket, key
 
 
 async def test_read_write_roundtrip(s3_bucket):
-
     """
     Create an S3 bucket, instantiate S3Bucket block, write to and read from
     bucket.
     """
 
     key = await s3_bucket.write_path("test.txt", content=b"hello")
     assert await s3_bucket.read_path(key) == b"hello"
 
 
 async def test_write_with_missing_directory_succeeds(s3_bucket):
-
     """
     Create an S3 bucket, instantiate S3Bucket block, write to path with
     missing directory.
     """
 
     key = await s3_bucket.write_path("folder/test.txt", content=b"hello")
     assert await s3_bucket.read_path(key) == b"hello"
 
 
 async def test_read_fails_does_not_exist(s3_bucket):
-
     """
     Create an S3 bucket, instantiate S3Bucket block, assert read from
     nonexistent path fails.
     """
 
     with pytest.raises(ClientError):
         await s3_bucket.read_path("test_bucket/foo/bar")
```

### Comparing `prefect-aws-0.3.0/tests/test_secrets_manager.py` & `prefect-aws-0.3.1/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.0/versioneer.py` & `prefect-aws-0.3.1/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,17 +417,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = r'''
+LONG_VERSION_PY["git"] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
```

