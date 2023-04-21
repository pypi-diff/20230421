# Comparing `tmp/dcicutils-7.2.0.1b2.tar.gz` & `tmp/dcicutils-7.2.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.2.0.1b2.tar", max compression
+gzip compressed data, was "dcicutils-7.2.0.1b3.tar", max compression
```

## Comparing `dcicutils-7.2.0.1b2.tar` & `dcicutils-7.2.0.1b3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1166 2023-04-18 15:27:06.157824 dcicutils-7.2.0.1b2/README.rst
--rw-r--r--   0        0        0        0 2023-04-18 15:27:06.157824 dcicutils-7.2.0.1b2/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/base.py
--rwxr-xr-x   0        0        0    52659 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    13639 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/command_utils.py
--rw-r--r--   0        0        0     1649 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46730 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9257 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/exceptions.py
--rw-r--r--   0        0        0    37025 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    11502 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27302 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/log_utils.py
--rw-r--r--   0        0        0    87196 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    20232 2023-04-18 15:27:06.161824 dcicutils-7.2.0.1b2/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   120743 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28713 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    19745 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0    10025 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     1769 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3680 2023-04-18 15:27:06.165824 dcicutils-7.2.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1166 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/README.rst
+-rw-r--r--   0        0        0        0 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/base.py
+-rwxr-xr-x   0        0        0    52659 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    13639 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     1649 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-04-21 20:39:11.078494 dcicutils-7.2.0.1b3/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46730 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9257 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    37025 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    11502 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27302 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    87196 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    20232 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   120743 2023-04-21 20:39:11.082494 dcicutils-7.2.0.1b3/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28713 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    19745 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0    10074 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     1769 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3680 2023-04-21 20:39:11.086494 dcicutils-7.2.0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 dcicutils-7.2.0.1b3/PKG-INFO
```

### Comparing `dcicutils-7.2.0.1b2/README.rst` & `dcicutils-7.2.0.1b3/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/base.py` & `dcicutils-7.2.0.1b3/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/beanstalk_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/cloudformation_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/codebuild_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/command_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/common.py` & `dcicutils-7.2.0.1b3/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/creds_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/data_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/deployment_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/diff_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/docker_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ecr_scripts.py` & `dcicutils-7.2.0.1b3/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ecr_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ecs_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/env_base.py` & `dcicutils-7.2.0.1b3/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/env_manager.py` & `dcicutils-7.2.0.1b3/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/env_scripts.py` & `dcicutils-7.2.0.1b3/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/env_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/env_utils_legacy.py` & `dcicutils-7.2.0.1b3/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/es_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/exceptions.py` & `dcicutils-7.2.0.1b3/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ff_mocks.py` & `dcicutils-7.2.0.1b3/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ff_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/jh_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/kibana/dashboards.json` & `dcicutils-7.2.0.1b3/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/kibana/readme.md` & `dcicutils-7.2.0.1b3/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/lang_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/log_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/misc_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/obfuscation_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/opensearch_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/qa_checkers.py` & `dcicutils-7.2.0.1b3/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/qa_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/redis_tools.py` & `dcicutils-7.2.0.1b3/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/redis_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/s3_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/secrets_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/snapshot_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/ssl_certificate_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     hostname = _normalize_hostname(hostname)
     try:
         certificate_pem = _get_ssl_certificate_pem(hostname, raise_exception=False)
         certificate_info = _get_ssl_certificate_info_from_pem(
             certificate_pem,
             raise_exception=raise_exception,
-            test_mode_certificate_expiration_warning_days=test_mode_certificate_expiration_warning_days
+            expires_soon_days=test_mode_certificate_expiration_warning_days
         )
         certificate_okay, certificate_exception = _is_ssl_certificate_okay(hostname, raise_exception=raise_exception)
         # The hostname from _get_ssl_certificate_info_from_pem is not necessarily exactly correct;
         # for example, for cgap-wolf.hms.harvard.edu it is imperva.com.
         certificate_info["hostname"] = hostname
         certificate_info["valid"] = certificate_info["valid"] and certificate_okay
         if certificate_exception:
@@ -68,24 +68,22 @@
         if raise_exception:
             raise e
         return None
 
 
 def _get_ssl_certificate_info_from_pem(pem_string: str,
                                        raise_exception: bool = False,
-                                       test_mode_certificate_expiration_warning_days: int = 0) -> Optional[dict]:
+                                       expires_soon_days: int = 0) -> Optional[dict]:
     """
     Returns a dictionary containing various data points for the given SSL certificate string
     string in PEM format. If an error is encountered in parsing this given string then returns
     None by default, or raises and exception of the given raise_exception argument is True.
     """
     now = datetime.now()
-    if test_mode_certificate_expiration_warning_days > 0:
-        expires_soon_days = test_mode_certificate_expiration_warning_days
-    else:
+    if expires_soon_days <= 0:
         expires_soon_days = _SSL_CERTIFICATE_EXPIRES_SOON_WARNING_DAYS
 
     def get_hostnames(certificate: OpenSSL.crypto.X509) -> list:
         """
         Returns the list of hostnames associated with the given SSL certificate. There can indeed
         be more than one hostname associated with a certificate, and we cannot determine the one
         primary one associated with it, so the caller (get_ssl_certificate_info) of this (outer)
@@ -147,16 +145,18 @@
         serial_number = str(certificate.get_serial_number())
         public_key_pem = certificate.get_pubkey().to_cryptography_key().public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo
         ).decode("UTF-8")
 
         return {
-            "common_name": common_name,
+            "name": None,  # Filled in by caller (get_ssl_certificate_info)
+            "hostname": None,  # Filled in by caller (get_ssl_certificate_info)
             "hostnames": hostnames,
+            "common_name": common_name,
             "owner": owner,
             "owner_entity": owner_entity,
             "owner_country": owner_country,
             "owner_state": owner_state,
             "owner_city": owner_city,
             "issuer": issuer,
             "issuer_entity": issuer_entity,
@@ -168,15 +168,16 @@
             "pem": pem_string,
             "serial_number": serial_number,
             "public_key_pem": public_key_pem,
             "valid": valid,
             "inactive": inactive,
             "expired": expired,
             "expires_soon": expires_soon,
-            "exception": None
+            "exception": None,
+            "timestamp": now.strftime("%Y-%m-%d %H:%M:%S")
         }
 
     except Exception as e:
         if raise_exception:
             raise e
         return None
```

### Comparing `dcicutils-7.2.0.1b2/dcicutils/trace_utils.py` & `dcicutils-7.2.0.1b3/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.2.0.1b2/pyproject.toml` & `dcicutils-7.2.0.1b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.2.0.1b2"
+version = "7.2.0.1b3"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.2.0.1b2/PKG-INFO` & `dcicutils-7.2.0.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.2.0.1b2
+Version: 7.2.0.1b3
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

