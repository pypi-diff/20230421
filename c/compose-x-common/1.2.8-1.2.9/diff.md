# Comparing `tmp/compose_x_common-1.2.8.tar.gz` & `tmp/compose_x_common-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose_x_common-1.2.8.tar", max compression
+gzip compressed data, was "compose_x_common-1.2.9.tar", max compression
```

## Comparing `compose_x_common-1.2.8.tar` & `compose_x_common-1.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    16725 2022-03-11 22:14:27.945418 compose_x_common-1.2.8/LICENSE
--rw-r--r--   0        0        0      262 2022-03-11 22:14:27.945418 compose_x_common-1.2.8/MANIFEST.in
--rw-r--r--   0        0        0      534 2022-03-11 22:14:27.945418 compose_x_common-1.2.8/README.rst
--rw-r--r--   0        0        0     2217 2023-02-21 10:07:13.908586 compose_x_common-1.2.8/pyproject.toml
--rw-r--r--   0        0        0      228 2023-02-21 10:07:13.909587 compose_x_common-1.2.8/src/compose_x_common/__init__.py
--rw-r--r--   0        0        0     3685 2022-11-21 14:56:47.102458 compose_x_common-1.2.8/src/compose_x_common/aws/__init__.py
--rw-r--r--   0        0        0     1863 2022-07-22 00:03:55.519715 compose_x_common-1.2.8/src/compose_x_common/aws/acm.py
--rw-r--r--   0        0        0     1557 2022-11-04 11:54:19.281200 compose_x_common-1.2.8/src/compose_x_common/aws/application_autoscaling.py
--rw-r--r--   0        0        0     4019 2022-11-21 14:57:22.051009 compose_x_common-1.2.8/src/compose_x_common/aws/arns.py
--rw-r--r--   0        0        0     1072 2022-06-15 07:27:09.923214 compose_x_common-1.2.8/src/compose_x_common/aws/cloudmap.py
--rw-r--r--   0        0        0      263 2022-06-15 07:27:09.923214 compose_x_common-1.2.8/src/compose_x_common/aws/codeguru_profiler.py
--rw-r--r--   0        0        0     2003 2022-09-12 06:21:59.941157 compose_x_common-1.2.8/src/compose_x_common/aws/cognito_userpool.py
--rw-r--r--   0        0        0      238 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/dynamodb.py
--rw-r--r--   0        0        0      471 2022-06-03 07:28:12.393610 compose_x_common-1.2.8/src/compose_x_common/aws/ecr/__init__.py
--rw-r--r--   0        0        0     4696 2022-11-09 15:53:55.621388 compose_x_common-1.2.8/src/compose_x_common/aws/ecr/images.py
--rw-r--r--   0        0        0     2168 2022-06-01 06:41:50.109299 compose_x_common-1.2.8/src/compose_x_common/aws/ecr/repositories.py
--rw-r--r--   0        0        0     6765 2022-10-04 13:02:05.943482 compose_x_common-1.2.8/src/compose_x_common/aws/ecs/__init__.py
--rw-r--r--   0        0        0     2280 2022-10-04 12:43:58.829061 compose_x_common-1.2.8/src/compose_x_common/aws/ecs/instances.py
--rw-r--r--   0        0        0     1613 2022-10-04 13:51:31.931108 compose_x_common-1.2.8/src/compose_x_common/aws/ecs/services.py
--rw-r--r--   0        0        0     1979 2022-08-30 21:05:57.065859 compose_x_common-1.2.8/src/compose_x_common/aws/ecs/tasks.py
--rw-r--r--   0        0        0      250 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/elasticache.py
--rw-r--r--   0        0        0      338 2022-11-21 14:54:54.576907 compose_x_common-1.2.8/src/compose_x_common/aws/glue/__init__.py
--rw-r--r--   0        0        0      317 2022-06-15 07:19:06.702901 compose_x_common-1.2.8/src/compose_x_common/aws/iam.py
--rw-r--r--   0        0        0      108 2022-11-04 12:27:16.152748 compose_x_common-1.2.8/src/compose_x_common/aws/kafka.py
--rw-r--r--   0        0        0      407 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/kinesis.py
--rw-r--r--   0        0        0     2934 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/kms.py
--rw-r--r--   0        0        0     3208 2022-11-08 11:00:03.696044 compose_x_common-1.2.8/src/compose_x_common/aws/msk.py
--rw-r--r--   0        0        0      410 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/neptune.py
--rw-r--r--   0        0        0      238 2022-06-15 07:27:09.924214 compose_x_common-1.2.8/src/compose_x_common/aws/opensearch.py
--rw-r--r--   0        0        0      556 2022-06-15 07:27:09.925214 compose_x_common-1.2.8/src/compose_x_common/aws/rds.py
--rw-r--r--   0        0        0     2427 2022-06-15 06:41:04.223263 compose_x_common-1.2.8/src/compose_x_common/aws/resourcegroupstaggingapi.py
--rw-r--r--   0        0        0     2145 2022-09-11 21:03:29.755298 compose_x_common-1.2.8/src/compose_x_common/aws/route53.py
--rw-r--r--   0        0        0      178 2022-09-12 06:44:47.805556 compose_x_common-1.2.8/src/compose_x_common/aws/s3.py
--rw-r--r--   0        0        0      882 2022-09-12 06:34:33.272917 compose_x_common-1.2.8/src/compose_x_common/aws/secrets_manager.py
--rw-r--r--   0        0        0     1601 2022-09-12 06:44:49.117539 compose_x_common-1.2.8/src/compose_x_common/aws/sns.py
--rw-r--r--   0        0        0      231 2022-06-15 07:27:09.925214 compose_x_common-1.2.8/src/compose_x_common/aws/sqs.py
--rw-r--r--   0        0        0      245 2022-06-15 07:27:09.925214 compose_x_common-1.2.8/src/compose_x_common/aws/ssm_parameter.py
--rw-r--r--   0        0        0     4548 2022-06-15 07:27:09.926214 compose_x_common-1.2.8/src/compose_x_common/aws/vpc.py
--rw-r--r--   0        0        0     4926 2023-01-18 11:55:19.555157 compose_x_common-1.2.8/src/compose_x_common/compose_x_common.py
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 compose_x_common-1.2.8/setup.py
--rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 compose_x_common-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-03-11 22:14:27.945418 compose_x_common-1.2.9/LICENSE
+-rw-r--r--   0        0        0      262 2022-03-11 22:14:27.945418 compose_x_common-1.2.9/MANIFEST.in
+-rw-r--r--   0        0        0      739 2023-03-19 15:02:14.794099 compose_x_common-1.2.9/README.rst
+-rw-r--r--   0        0        0     2219 2023-03-19 14:59:49.713373 compose_x_common-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-03-19 14:59:49.713373 compose_x_common-1.2.9/src/compose_x_common/__init__.py
+-rw-r--r--   0        0        0     3574 2023-03-19 14:59:49.702373 compose_x_common-1.2.9/src/compose_x_common/aws/__init__.py
+-rw-r--r--   0        0        0     1863 2022-07-22 00:03:55.519715 compose_x_common-1.2.9/src/compose_x_common/aws/acm.py
+-rw-r--r--   0        0        0     1557 2022-11-04 11:54:19.281200 compose_x_common-1.2.9/src/compose_x_common/aws/application_autoscaling.py
+-rw-r--r--   0        0        0     4019 2022-11-21 14:57:22.051009 compose_x_common-1.2.9/src/compose_x_common/aws/arns.py
+-rw-r--r--   0        0        0     1072 2022-06-15 07:27:09.923214 compose_x_common-1.2.9/src/compose_x_common/aws/cloudmap.py
+-rw-r--r--   0        0        0      263 2022-06-15 07:27:09.923214 compose_x_common-1.2.9/src/compose_x_common/aws/codeguru_profiler.py
+-rw-r--r--   0        0        0     2003 2022-09-12 06:21:59.941157 compose_x_common-1.2.9/src/compose_x_common/aws/cognito_userpool.py
+-rw-r--r--   0        0        0      238 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/dynamodb.py
+-rw-r--r--   0        0        0      471 2022-06-03 07:28:12.393610 compose_x_common-1.2.9/src/compose_x_common/aws/ecr/__init__.py
+-rw-r--r--   0        0        0     4696 2022-11-09 15:53:55.621388 compose_x_common-1.2.9/src/compose_x_common/aws/ecr/images.py
+-rw-r--r--   0        0        0     2168 2022-06-01 06:41:50.109299 compose_x_common-1.2.9/src/compose_x_common/aws/ecr/repositories.py
+-rw-r--r--   0        0        0     6765 2022-10-04 13:02:05.943482 compose_x_common-1.2.9/src/compose_x_common/aws/ecs/__init__.py
+-rw-r--r--   0        0        0     2280 2022-10-04 12:43:58.829061 compose_x_common-1.2.9/src/compose_x_common/aws/ecs/instances.py
+-rw-r--r--   0        0        0     1613 2022-10-04 13:51:31.931108 compose_x_common-1.2.9/src/compose_x_common/aws/ecs/services.py
+-rw-r--r--   0        0        0     1979 2022-08-30 21:05:57.065859 compose_x_common-1.2.9/src/compose_x_common/aws/ecs/tasks.py
+-rw-r--r--   0        0        0      250 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/elasticache.py
+-rw-r--r--   0        0        0      338 2022-11-21 14:54:54.576907 compose_x_common-1.2.9/src/compose_x_common/aws/glue/__init__.py
+-rw-r--r--   0        0        0      317 2022-06-15 07:19:06.702901 compose_x_common-1.2.9/src/compose_x_common/aws/iam.py
+-rw-r--r--   0        0        0      108 2022-11-04 12:27:16.152748 compose_x_common-1.2.9/src/compose_x_common/aws/kafka.py
+-rw-r--r--   0        0        0      407 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/kinesis.py
+-rw-r--r--   0        0        0     2934 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/kms.py
+-rw-r--r--   0        0        0     3208 2022-11-08 11:00:03.696044 compose_x_common-1.2.9/src/compose_x_common/aws/msk.py
+-rw-r--r--   0        0        0      410 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/neptune.py
+-rw-r--r--   0        0        0      238 2022-06-15 07:27:09.924214 compose_x_common-1.2.9/src/compose_x_common/aws/opensearch.py
+-rw-r--r--   0        0        0      556 2022-06-15 07:27:09.925214 compose_x_common-1.2.9/src/compose_x_common/aws/rds.py
+-rw-r--r--   0        0        0     2427 2022-06-15 06:41:04.223263 compose_x_common-1.2.9/src/compose_x_common/aws/resourcegroupstaggingapi.py
+-rw-r--r--   0        0        0     2145 2022-09-11 21:03:29.755298 compose_x_common-1.2.9/src/compose_x_common/aws/route53.py
+-rw-r--r--   0        0        0      178 2022-09-12 06:44:47.805556 compose_x_common-1.2.9/src/compose_x_common/aws/s3.py
+-rw-r--r--   0        0        0      882 2022-09-12 06:34:33.272917 compose_x_common-1.2.9/src/compose_x_common/aws/secrets_manager.py
+-rw-r--r--   0        0        0     1601 2022-09-12 06:44:49.117539 compose_x_common-1.2.9/src/compose_x_common/aws/sns.py
+-rw-r--r--   0        0        0      231 2022-06-15 07:27:09.925214 compose_x_common-1.2.9/src/compose_x_common/aws/sqs.py
+-rw-r--r--   0        0        0      245 2022-06-15 07:27:09.925214 compose_x_common-1.2.9/src/compose_x_common/aws/ssm_parameter.py
+-rw-r--r--   0        0        0     4548 2022-06-15 07:27:09.926214 compose_x_common-1.2.9/src/compose_x_common/aws/vpc.py
+-rw-r--r--   0        0        0     4926 2023-01-18 11:55:19.555157 compose_x_common-1.2.9/src/compose_x_common/compose_x_common.py
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 compose_x_common-1.2.9/setup.py
+-rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 compose_x_common-1.2.9/PKG-INFO
```

### Comparing `compose_x_common-1.2.8/LICENSE` & `compose_x_common-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/pyproject.toml` & `compose_x_common-1.2.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 [build-system]
 requires = ["poetry-core>=1.2.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "compose_x_common"
-version = "1.2.8"
+version = "1.2.9"
 description = "Common Library for Compose-X Projects"
 authors = ["John Preston <john@compose-x.io>"]
 maintainers = ["John Preston <john@compose-x.io>"]
 repository = "https://github.com/compose-x/compose-x-common-libs/"
 keywords = ["compose-x", "docker", "compose"]
 license = "MPL-2.0"
 include = [
     "LICENSE",
     "MANIFEST.in"
 ]
-classifiers=[
+classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 boto3 = "^1.22"
 flatdict = "^4.0.1"
 python-dateutil = "^2.8.2"
 
 
 [tool.poetry.dev-dependencies]
 placebo = ">=0.9.0,<1.0"
 pytest = "^7.2"
 Sphinx = "^5.0"
 sphinx-material = "^0.0.35"
-isort = "^5.10.1"
-black = "^22.3.0"
-pre-commit = "^2.19.0"
+isort = "^5.12"
+black = "^23.1"
+pre-commit = "^3.1"
 flake8-docstrings = "^1.6.0"
 coverage = "^7.0"
-tbump = "^6.8.0"
+tbump = "^6.9.0"
 pyupgrade = "^3.3"
 sphinx-rtd-theme = "^1.0.0"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/compose-x-common/"
 
 [tool.tbump.version]
-current = "1.2.8"
+current = "1.2.9"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -95,10 +95,10 @@
 branch = true
 source = ["src"]
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.flake8]
-exclude =[ ".git","__pycache__","docs/source/conf.py","old","build","dist","feature"]
+exclude = [".git", "__pycache__", "docs/source/conf.py", "old", "build", "dist", "feature"]
 max-line-length = 88
 max-complexity = 10
```

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/__init__.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,40 +48,41 @@
         )
     if as_str:
         return arn
     return match
 
 
 def get_assume_role_session(
-    session: Session, arn: str, session_name: str = None, region: str = None, **kwargs
-) -> Session:
+    session: Session,
+    arn: str,
+    session_name: str = None,
+    region: str = None,
+    include_full_return: bool = False,
+    **kwargs,
+) -> Union[Session, (Session, dict)]:
     """
-    Function to override ComposeXSettings session to specific session for Lookup
-
-    :param boto3.session.Session session: The original session fetching the credentials for X-Role
-    :param str arn: the IAM Role ARN to assume role with
-    :param str session_name: Override name of the session
-    :param region: AWS Region for API Calls
-    :return: boto3 session from lookup settings
-    :rtype: boto3.session.Session
+    Function to get a boto3.session.Session() based on assume another IAM role. Can return just the session
+    or the session and the full credentials return
     """
     args = deepcopy(kwargs)
-    if not session_name or "RoleSessionName" not in kwargs.keys():
+    if not session_name or "RoleSessionName" not in kwargs:
         args["RoleSessionName"] = "stsAssumeRole"
     args["RoleArn"] = arn
     args["DurationSeconds"] = set_else_none("DurationSeconds", kwargs, alt_value=900)
     validate_iam_role_arn(arn)
     creds = session.client("sts").assume_role(**args)
-
-    return Session(
+    session = Session(
         region_name=region,
         aws_access_key_id=creds["Credentials"]["AccessKeyId"],
         aws_session_token=creds["Credentials"]["SessionToken"],
         aws_secret_access_key=creds["Credentials"]["SecretAccessKey"],
     )
+    if include_full_return:
+        return session, creds
+    return session
 
 
 def get_resource_from_ccapi(
     type_name: str, identifier: Union[str, dict], session: Session = None, **kwargs
 ) -> dict:
     """
     Wrapper around cloudcontrol.get_resource
```

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/acm.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/acm.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/application_autoscaling.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/application_autoscaling.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/arns.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/arns.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/cloudmap.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/cloudmap.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/cognito_userpool.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/cognito_userpool.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecr/images.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecr/images.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecr/repositories.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecr/repositories.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecs/__init__.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecs/instances.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecs/instances.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecs/services.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecs/services.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/ecs/tasks.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/ecs/tasks.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/kms.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/kms.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/msk.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/msk.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/rds.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/rds.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/resourcegroupstaggingapi.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/route53.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/route53.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/secrets_manager.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/sns.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/sns.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/aws/vpc.py` & `compose_x_common-1.2.9/src/compose_x_common/aws/vpc.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/src/compose_x_common/compose_x_common.py` & `compose_x_common-1.2.9/src/compose_x_common/compose_x_common.py`

 * *Files identical despite different names*

### Comparing `compose_x_common-1.2.8/setup.py` & `compose_x_common-1.2.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.22,<2.0', 'flatdict>=4.0.1,<5.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'compose-x-common',
-    'version': '1.2.8',
+    'version': '1.2.9',
     'description': 'Common Library for Compose-X Projects',
-    'long_description': '=====================\nCompose-X -- Common\n=====================\n\n\n.. image:: https://img.shields.io/pypi/v/compose_x_common.svg\n        :target: https://pypi.python.org/pypi/compose_x_common\n\n.. image:: https://readthedocs.org/projects/compose-x-commons-lib/badge/?version=latest\n        :target: https://compose-x-commons-lib.readthedocs.io/en/latest/?version=latest\n        :alt: Documentation Status\n\n\n\n\nStandalone library of reusable functions"\n\n\n* Free software: MPL-2.0\n* Documentation: https://compose-x-common.readthedocs.io.\n',
+    'long_description': '=====================\nCompose-X -- Common\n=====================\n\n\n.. image:: https://img.shields.io/pypi/v/compose_x_common.svg\n    :target: https://pypi.python.org/pypi/compose_x_common\n\n\n--------------------------------------------------------------------------------------\nStandalone library of reusable functions to ease repetitive tasks & AWS functions\n--------------------------------------------------------------------------------------\n\nUsed in a majority of the `Compose-X`_ projects\n\nFeatures\n==========\n\n* Different helpers `compose_x_commom.compose_x_common`\n* Python ARN Regular expressions for different resources `compose_x_commom.aws.arns`\n* AWS Helpers `compose_x_commom.aws`\n\n.. _Compose-X: https://github.com/compose-x\n',
     'author': 'John Preston',
     'author_email': 'john@compose-x.io',
     'maintainer': 'John Preston',
     'maintainer_email': 'john@compose-x.io',
     'url': 'https://github.com/compose-x/compose-x-common-libs/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `compose_x_common-1.2.8/PKG-INFO` & `compose_x_common-1.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 Metadata-Version: 2.1
 Name: compose-x-common
-Version: 1.2.8
+Version: 1.2.9
 Summary: Common Library for Compose-X Projects
 Home-page: https://github.com/compose-x/compose-x-common-libs/
 License: MPL-2.0
 Keywords: compose-x,docker,compose
 Author: John Preston
 Author-email: john@compose-x.io
 Maintainer: John Preston
 Maintainer-email: john@compose-x.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.22,<2.0)
 Requires-Dist: flatdict (>=4.0.1,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/compose-x/compose-x-common-libs/
 Description-Content-Type: text/x-rst
 
 =====================
 Compose-X -- Common
 =====================
 
 
 .. image:: https://img.shields.io/pypi/v/compose_x_common.svg
-        :target: https://pypi.python.org/pypi/compose_x_common
-
-.. image:: https://readthedocs.org/projects/compose-x-commons-lib/badge/?version=latest
-        :target: https://compose-x-commons-lib.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
+    :target: https://pypi.python.org/pypi/compose_x_common
 
 
+--------------------------------------------------------------------------------------
+Standalone library of reusable functions to ease repetitive tasks & AWS functions
+--------------------------------------------------------------------------------------
 
+Used in a majority of the `Compose-X`_ projects
 
-Standalone library of reusable functions"
+Features
+==========
 
+* Different helpers `compose_x_commom.compose_x_common`
+* Python ARN Regular expressions for different resources `compose_x_commom.aws.arns`
+* AWS Helpers `compose_x_commom.aws`
 
-* Free software: MPL-2.0
-* Documentation: https://compose-x-common.readthedocs.io.
+.. _Compose-X: https://github.com/compose-x
```

