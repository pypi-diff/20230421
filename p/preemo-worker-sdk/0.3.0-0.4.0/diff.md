# Comparing `tmp/preemo_worker_sdk-0.3.0.tar.gz` & `tmp/preemo_worker_sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preemo_worker_sdk-0.3.0.tar", max compression
+gzip compressed data, was "preemo_worker_sdk-0.4.0.tar", max compression
```

## Comparing `preemo_worker_sdk-0.3.0.tar` & `preemo_worker_sdk-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
--rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.3.0/README.md
--rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.3.0/preemo/__init__.py
--rw-r--r--   0        0        0      306 2023-04-06 00:44:52.196888 preemo_worker_sdk-0.3.0/preemo/gen/__init__.py
--rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197079 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/__init__.py
--rw-r--r--   0        0        0     4345 2023-04-06 00:44:52.045784 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.py
--rw-r--r--   0        0        0     7822 2023-04-07 21:20:34.286564 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     2733 2023-04-06 00:44:52.045917 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.py
--rw-r--r--   0        0        0     5420 2023-04-06 00:44:52.209089 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
--rw-r--r--   0        0        0     2642 2023-04-06 00:44:52.046026 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.py
--rw-r--r--   0        0        0     4134 2023-04-06 00:44:52.213421 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi
--rw-r--r--   0        0        0     2837 2023-04-06 00:44:52.046135 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
--rw-r--r--   0        0        0     5105 2023-04-06 00:44:52.217891 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
--rw-r--r--   0        0        0     4212 2023-04-06 00:44:52.046231 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.py
--rw-r--r--   0        0        0     7654 2023-04-06 00:44:52.222757 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi
--rw-r--r--   0        0        0     2792 2023-04-06 00:44:52.046329 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.py
--rw-r--r--   0        0        0     5685 2023-04-06 00:44:52.228008 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
--rw-r--r--   0        0        0     1382 2023-04-06 00:44:52.046428 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.py
--rw-r--r--   0        0        0     1811 2023-04-06 00:44:52.232051 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.pyi
--rw-r--r--   0        0        0     1665 2023-04-06 00:44:52.046532 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.py
--rw-r--r--   0        0        0     3019 2023-04-06 00:44:52.236010 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.pyi
--rw-r--r--   0        0        0     1128 2023-04-06 00:44:52.046634 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.py
--rw-r--r--   0        0        0     1515 2023-04-06 00:44:52.239908 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.pyi
--rw-r--r--   0        0        0     1403 2023-04-06 00:44:52.046746 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.py
--rw-r--r--   0        0        0     1721 2023-04-06 00:44:52.243919 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.pyi
--rw-r--r--   0        0        0     1222 2023-04-06 00:44:52.046859 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.py
--rw-r--r--   0        0        0     1539 2023-04-06 00:44:52.248123 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
--rw-r--r--   0        0        0     1085 2023-04-06 00:44:52.046972 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.py
--rw-r--r--   0        0        0      786 2023-04-06 00:44:52.252283 preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197557 preemo_worker_sdk-0.3.0/preemo/gen/models/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-06 00:44:52.047113 preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.py
--rw-r--r--   0        0        0     1624 2023-04-06 00:44:52.256316 preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.pyi
--rw-r--r--   0        0        0     1174 2023-04-06 00:44:52.047229 preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.py
--rw-r--r--   0        0        0     1396 2023-04-06 00:44:52.260232 preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.pyi
--rw-r--r--   0        0        0      306 2023-04-06 00:44:52.197729 preemo_worker_sdk-0.3.0/preemo/gen/services/__init__.py
--rw-r--r--   0        0        0     4369 2023-04-06 00:44:52.189708 preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.py
--rw-r--r--   0        0        0     1302 2023-04-06 00:44:52.264181 preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.pyi
--rw-r--r--   0        0        0    19585 2023-04-06 00:44:52.189860 preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.py
--rw-r--r--   0        0        0     5787 2023-04-06 00:44:52.268251 preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.3.0/preemo/py.typed
--rw-r--r--   0        0        0     3310 2023-04-07 21:20:34.286985 preemo_worker_sdk-0.3.0/preemo/worker/__init__.py
--rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.3.0/preemo/worker/__init__.pyi
--rw-r--r--   0        0        0    12028 2023-04-07 21:20:34.287528 preemo_worker_sdk-0.3.0/preemo/worker/_artifact_manager.py
--rw-r--r--   0        0        0      759 2023-04-07 21:20:34.287821 preemo_worker_sdk-0.3.0/preemo/worker/_env.py
--rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.3.0/preemo/worker/_function_registry.py
--rw-r--r--   0        0        0     9948 2023-04-07 16:55:48.486452 preemo_worker_sdk-0.3.0/preemo/worker/_messaging_client.py
--rw-r--r--   0        0        0     2538 2023-04-07 21:20:34.288187 preemo_worker_sdk-0.3.0/preemo/worker/_sdk_server.py
--rw-r--r--   0        0        0     3229 2023-04-07 21:20:34.288581 preemo_worker_sdk-0.3.0/preemo/worker/_sdk_service.py
--rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.3.0/preemo/worker/_types.py
--rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.3.0/preemo/worker/_validation.py
--rw-r--r--   0        0        0     6887 2023-04-07 21:20:34.288862 preemo_worker_sdk-0.3.0/preemo/worker/_worker_client.py
--rw-r--r--   0        0        0     1698 2023-04-07 21:20:52.735653 preemo_worker_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3476 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-03-02 18:51:16.179376 preemo_worker_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2713 2023-04-07 21:20:34.285759 preemo_worker_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0       98 2023-03-02 18:51:16.180791 preemo_worker_sdk-0.4.0/preemo/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242370 preemo_worker_sdk-0.4.0/preemo/gen/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.242697 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/__init__.py
+-rw-r--r--   0        0        0     4333 2023-04-21 16:59:41.866999 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py
+-rw-r--r--   0        0        0     7285 2023-04-21 16:59:41.867117 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi
+-rw-r--r--   0        0        0     3035 2023-04-21 16:59:41.867661 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_create_artifact_pb2.py
+-rw-r--r--   0        0        0     6629 2023-04-21 16:59:41.867943 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi
+-rw-r--r--   0        0        0     2642 2023-04-20 22:13:04.136336 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_execute_function_pb2.py
+-rw-r--r--   0        0        0     4134 2023-04-20 22:13:04.257705 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi
+-rw-r--r--   0        0        0     2837 2023-04-20 22:13:04.136444 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py
+-rw-r--r--   0        0        0     5106 2023-04-21 16:59:41.868456 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4502 2023-04-21 16:59:41.868856 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.py
+-rw-r--r--   0        0        0     7767 2023-04-21 16:59:41.869023 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi
+-rw-r--r--   0        0        0     2792 2023-04-20 22:13:04.136642 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_pb2.py
+-rw-r--r--   0        0        0     5686 2023-04-21 16:59:41.869205 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi
+-rw-r--r--   0        0        0     4409 2023-04-21 16:59:41.869446 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.py
+-rw-r--r--   0        0        0     7699 2023-04-21 16:59:41.869645 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_upload_url_pb2.pyi
+-rw-r--r--   0        0        0     1382 2023-04-20 22:13:04.136842 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/check_function_pb2.py
+-rw-r--r--   0        0        0     1811 2023-04-20 22:13:04.280322 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/check_function_pb2.pyi
+-rw-r--r--   0        0        0     1665 2023-04-20 22:13:04.136937 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/execute_function_pb2.py
+-rw-r--r--   0        0        0     3019 2023-04-20 22:13:04.284329 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/execute_function_pb2.pyi
+-rw-r--r--   0        0        0     1128 2023-04-20 22:13:04.137055 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/header_pb2.py
+-rw-r--r--   0        0        0     1515 2023-04-20 22:13:04.288198 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/header_pb2.pyi
+-rw-r--r--   0        0        0     1403 2023-04-20 22:13:04.137163 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/register_function_pb2.py
+-rw-r--r--   0        0        0     1721 2023-04-20 22:13:04.292227 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/register_function_pb2.pyi
+-rw-r--r--   0        0        0     1222 2023-04-20 22:13:04.137267 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/sdk_server_ready_pb2.py
+-rw-r--r--   0        0        0     1539 2023-04-20 22:13:04.296209 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi
+-rw-r--r--   0        0        0     1085 2023-04-20 22:13:04.137366 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/terminate_pb2.py
+-rw-r--r--   0        0        0      786 2023-04-20 22:13:04.300561 preemo_worker_sdk-0.4.0/preemo/gen/endpoints/terminate_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243206 preemo_worker_sdk-0.4.0/preemo/gen/models/__init__.py
+-rw-r--r--   0        0        0     1104 2023-04-21 16:59:41.869910 preemo_worker_sdk-0.4.0/preemo/gen/models/artifact_type_pb2.py
+-rw-r--r--   0        0        0     1129 2023-04-21 16:59:41.870254 preemo_worker_sdk-0.4.0/preemo/gen/models/artifact_type_pb2.pyi
+-rw-r--r--   0        0        0     1135 2023-04-20 22:13:04.137575 preemo_worker_sdk-0.4.0/preemo/gen/models/registered_function_pb2.py
+-rw-r--r--   0        0        0     1624 2023-04-20 22:13:04.311020 preemo_worker_sdk-0.4.0/preemo/gen/models/registered_function_pb2.pyi
+-rw-r--r--   0        0        0     1174 2023-04-20 22:13:04.137675 preemo_worker_sdk-0.4.0/preemo/gen/models/value_pb2.py
+-rw-r--r--   0        0        0     1396 2023-04-20 22:13:04.318152 preemo_worker_sdk-0.4.0/preemo/gen/models/value_pb2.pyi
+-rw-r--r--   0        0        0      306 2023-04-20 22:13:04.243405 preemo_worker_sdk-0.4.0/preemo/gen/services/__init__.py
+-rw-r--r--   0        0        0     4369 2023-04-20 22:13:04.235240 preemo_worker_sdk-0.4.0/preemo/gen/services/sdk_pb2_grpc.py
+-rw-r--r--   0        0        0     1302 2023-04-20 22:13:04.322250 preemo_worker_sdk-0.4.0/preemo/gen/services/sdk_pb2_grpc.pyi
+-rw-r--r--   0        0        0    21861 2023-04-21 16:59:41.870861 preemo_worker_sdk-0.4.0/preemo/gen/services/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     6536 2023-04-21 16:59:41.871238 preemo_worker_sdk-0.4.0/preemo/gen/services/worker_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-03-02 18:51:16.182528 preemo_worker_sdk-0.4.0/preemo/py.typed
+-rw-r--r--   0        0        0     2559 2023-04-20 22:59:58.827517 preemo_worker_sdk-0.4.0/preemo/worker/__init__.py
+-rw-r--r--   0        0        0      576 2023-04-07 21:20:34.287302 preemo_worker_sdk-0.4.0/preemo/worker/__init__.pyi
+-rw-r--r--   0        0        0    13221 2023-04-21 16:59:41.871754 preemo_worker_sdk-0.4.0/preemo/worker/_artifact_manager.py
+-rw-r--r--   0        0        0     1748 2023-04-20 22:59:58.827942 preemo_worker_sdk-0.4.0/preemo/worker/_env_manager.py
+-rw-r--r--   0        0        0     1876 2023-04-05 17:22:19.458494 preemo_worker_sdk-0.4.0/preemo/worker/_function_registry.py
+-rw-r--r--   0        0        0    11315 2023-04-21 16:59:41.872373 preemo_worker_sdk-0.4.0/preemo/worker/_messaging_client.py
+-rw-r--r--   0        0        0     2538 2023-04-10 22:31:00.968657 preemo_worker_sdk-0.4.0/preemo/worker/_sdk_server.py
+-rw-r--r--   0        0        0     3581 2023-04-21 16:59:41.872685 preemo_worker_sdk-0.4.0/preemo/worker/_sdk_service.py
+-rw-r--r--   0        0        0     1222 2023-03-22 21:19:28.059400 preemo_worker_sdk-0.4.0/preemo/worker/_types.py
+-rw-r--r--   0        0        0      527 2023-03-21 22:01:19.925183 preemo_worker_sdk-0.4.0/preemo/worker/_validation.py
+-rw-r--r--   0        0        0     7044 2023-04-21 16:59:41.872944 preemo_worker_sdk-0.4.0/preemo/worker/_worker_client.py
+-rw-r--r--   0        0        0     1698 2023-04-21 17:00:05.070273 preemo_worker_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3476 1970-01-01 00:00:00.000000 preemo_worker_sdk-0.4.0/PKG-INFO
```

### Comparing `preemo_worker_sdk-0.3.0/LICENSE` & `preemo_worker_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/README.md` & `preemo_worker_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: endpoints/batch_create_artifact_part.proto
+# source: endpoints/batch_allocate_artifact_part.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*endpoints/batch_create_artifact_part.proto\x12\tendpoints\"\"\n CreateArtifactPartConfigMetadata\"\xe7\x01\n\x18\x43reateArtifactPartConfig\x12`\n\x18metadatas_by_part_number\x18\x01 \x03(\x0b\x32>.endpoints.CreateArtifactPartConfig.MetadatasByPartNumberEntry\x1ai\n\x1aMetadatasByPartNumberEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.endpoints.CreateArtifactPartConfigMetadata:\x02\x38\x01\"\xe5\x01\n\x1e\x42\x61tchCreateArtifactPartRequest\x12\x62\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32\x42.endpoints.BatchCreateArtifactPartRequest.ConfigsByArtifactIdEntry\x1a_\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.endpoints.CreateArtifactPartConfig:\x02\x38\x01\"X\n CreateArtifactPartResultMetadata\x12\x1e\n\x11upload_signed_url\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x14\n\x12_upload_signed_url\"\xe7\x01\n\x18\x43reateArtifactPartResult\x12`\n\x18metadatas_by_part_number\x18\x01 \x03(\x0b\x32>.endpoints.CreateArtifactPartResult.MetadatasByPartNumberEntry\x1ai\n\x1aMetadatasByPartNumberEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.endpoints.CreateArtifactPartResultMetadata:\x02\x38\x01\"\xe7\x01\n\x1f\x42\x61tchCreateArtifactPartResponse\x12\x63\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32\x43.endpoints.BatchCreateArtifactPartResponse.ResultsByArtifactIdEntry\x1a_\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32#.endpoints.CreateArtifactPartResult:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,endpoints/batch_allocate_artifact_part.proto\x12\tendpoints\"$\n\"AllocateArtifactPartConfigMetadata\"\xed\x01\n\x1a\x41llocateArtifactPartConfig\x12\x62\n\x18metadatas_by_part_number\x18\x01 \x03(\x0b\x32@.endpoints.AllocateArtifactPartConfig.MetadatasByPartNumberEntry\x1ak\n\x1aMetadatasByPartNumberEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.endpoints.AllocateArtifactPartConfigMetadata:\x02\x38\x01\"\xeb\x01\n BatchAllocateArtifactPartRequest\x12\x64\n\x16\x63onfigs_by_artifact_id\x18\x01 \x03(\x0b\x32\x44.endpoints.BatchAllocateArtifactPartRequest.ConfigsByArtifactIdEntry\x1a\x61\n\x18\x43onfigsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.endpoints.AllocateArtifactPartConfig:\x02\x38\x01\"$\n\"AllocateArtifactPartResultMetadata\"\xed\x01\n\x1a\x41llocateArtifactPartResult\x12\x62\n\x18metadatas_by_part_number\x18\x01 \x03(\x0b\x32@.endpoints.AllocateArtifactPartResult.MetadatasByPartNumberEntry\x1ak\n\x1aMetadatasByPartNumberEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12<\n\x05value\x18\x02 \x01(\x0b\x32-.endpoints.AllocateArtifactPartResultMetadata:\x02\x38\x01\"\xed\x01\n!BatchAllocateArtifactPartResponse\x12\x65\n\x16results_by_artifact_id\x18\x01 \x03(\x0b\x32\x45.endpoints.BatchAllocateArtifactPartResponse.ResultsByArtifactIdEntry\x1a\x61\n\x18ResultsByArtifactIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.endpoints.AllocateArtifactPartResult:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_create_artifact_part_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_allocate_artifact_part_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _CREATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._options = None
-  _CREATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_options = b'8\001'
-  _BATCHCREATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._options = None
-  _BATCHCREATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_options = b'8\001'
-  _CREATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._options = None
-  _CREATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_options = b'8\001'
-  _BATCHCREATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._options = None
-  _BATCHCREATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_options = b'8\001'
-  _CREATEARTIFACTPARTCONFIGMETADATA._serialized_start=57
-  _CREATEARTIFACTPARTCONFIGMETADATA._serialized_end=91
-  _CREATEARTIFACTPARTCONFIG._serialized_start=94
-  _CREATEARTIFACTPARTCONFIG._serialized_end=325
-  _CREATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_start=220
-  _CREATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_end=325
-  _BATCHCREATEARTIFACTPARTREQUEST._serialized_start=328
-  _BATCHCREATEARTIFACTPARTREQUEST._serialized_end=557
-  _BATCHCREATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_start=462
-  _BATCHCREATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_end=557
-  _CREATEARTIFACTPARTRESULTMETADATA._serialized_start=559
-  _CREATEARTIFACTPARTRESULTMETADATA._serialized_end=647
-  _CREATEARTIFACTPARTRESULT._serialized_start=650
-  _CREATEARTIFACTPARTRESULT._serialized_end=881
-  _CREATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_start=776
-  _CREATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_end=881
-  _BATCHCREATEARTIFACTPARTRESPONSE._serialized_start=884
-  _BATCHCREATEARTIFACTPARTRESPONSE._serialized_end=1115
-  _BATCHCREATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=1020
-  _BATCHCREATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=1115
+  _ALLOCATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._options = None
+  _ALLOCATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_options = b'8\001'
+  _BATCHALLOCATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._options = None
+  _BATCHALLOCATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_options = b'8\001'
+  _ALLOCATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._options = None
+  _ALLOCATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_options = b'8\001'
+  _BATCHALLOCATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._options = None
+  _BATCHALLOCATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_options = b'8\001'
+  _ALLOCATEARTIFACTPARTCONFIGMETADATA._serialized_start=59
+  _ALLOCATEARTIFACTPARTCONFIGMETADATA._serialized_end=95
+  _ALLOCATEARTIFACTPARTCONFIG._serialized_start=98
+  _ALLOCATEARTIFACTPARTCONFIG._serialized_end=335
+  _ALLOCATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_start=228
+  _ALLOCATEARTIFACTPARTCONFIG_METADATASBYPARTNUMBERENTRY._serialized_end=335
+  _BATCHALLOCATEARTIFACTPARTREQUEST._serialized_start=338
+  _BATCHALLOCATEARTIFACTPARTREQUEST._serialized_end=573
+  _BATCHALLOCATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_start=476
+  _BATCHALLOCATEARTIFACTPARTREQUEST_CONFIGSBYARTIFACTIDENTRY._serialized_end=573
+  _ALLOCATEARTIFACTPARTRESULTMETADATA._serialized_start=575
+  _ALLOCATEARTIFACTPARTRESULTMETADATA._serialized_end=611
+  _ALLOCATEARTIFACTPARTRESULT._serialized_start=614
+  _ALLOCATEARTIFACTPARTRESULT._serialized_end=851
+  _ALLOCATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_start=744
+  _ALLOCATEARTIFACTPARTRESULT_METADATASBYPARTNUMBERENTRY._serialized_end=851
+  _BATCHALLOCATEARTIFACTPARTRESPONSE._serialized_start=854
+  _BATCHALLOCATEARTIFACTPARTRESPONSE._serialized_end=1091
+  _BATCHALLOCATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_start=994
+  _BATCHALLOCATEARTIFACTPARTRESPONSE_RESULTSBYARTIFACTIDENTRY._serialized_end=1091
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_allocate_artifact_part_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -13,171 +13,166 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class CreateArtifactPartConfigMetadata(google.protobuf.message.Message):
-    """This config is included for potential future use."""
+class AllocateArtifactPartConfigMetadata(google.protobuf.message.Message):
+    """This message is included for potential future use."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___CreateArtifactPartConfigMetadata = CreateArtifactPartConfigMetadata
+global___AllocateArtifactPartConfigMetadata = AllocateArtifactPartConfigMetadata
 
 @typing_extensions.final
-class CreateArtifactPartConfig(google.protobuf.message.Message):
+class AllocateArtifactPartConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class MetadatasByPartNumberEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
-        def value(self) -> global___CreateArtifactPartConfigMetadata: ...
+        def value(self) -> global___AllocateArtifactPartConfigMetadata: ...
         def __init__(
             self,
             *,
             key: builtins.int = ...,
-            value: global___CreateArtifactPartConfigMetadata | None = ...,
+            value: global___AllocateArtifactPartConfigMetadata | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     METADATAS_BY_PART_NUMBER_FIELD_NUMBER: builtins.int
     @property
-    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactPartConfigMetadata]:
-        """For an artifact, part numbers must be sequential positive integers starting with 0."""
+    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___AllocateArtifactPartConfigMetadata]:
+        """For an artifact, part numbers must be sequential integers starting with 0."""
     def __init__(
         self,
         *,
-        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___CreateArtifactPartConfigMetadata] | None = ...,
+        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___AllocateArtifactPartConfigMetadata] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas_by_part_number", b"metadatas_by_part_number"]) -> None: ...
 
-global___CreateArtifactPartConfig = CreateArtifactPartConfig
+global___AllocateArtifactPartConfig = AllocateArtifactPartConfig
 
 @typing_extensions.final
-class BatchCreateArtifactPartRequest(google.protobuf.message.Message):
+class BatchAllocateArtifactPartRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___CreateArtifactPartConfig: ...
+        def value(self) -> global___AllocateArtifactPartConfig: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___CreateArtifactPartConfig | None = ...,
+            value: global___AllocateArtifactPartConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___CreateArtifactPartConfig]: ...
+    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___AllocateArtifactPartConfig]: ...
     def __init__(
         self,
         *,
-        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___CreateArtifactPartConfig] | None = ...,
+        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___AllocateArtifactPartConfig] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
 
-global___BatchCreateArtifactPartRequest = BatchCreateArtifactPartRequest
+global___BatchAllocateArtifactPartRequest = BatchAllocateArtifactPartRequest
 
 @typing_extensions.final
-class CreateArtifactPartResultMetadata(google.protobuf.message.Message):
+class AllocateArtifactPartResultMetadata(google.protobuf.message.Message):
+    """This message is included for potential future use."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    UPLOAD_SIGNED_URL_FIELD_NUMBER: builtins.int
-    upload_signed_url: builtins.str
     def __init__(
         self,
-        *,
-        upload_signed_url: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_upload_signed_url", b"_upload_signed_url", "upload_signed_url", b"upload_signed_url"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_upload_signed_url", b"_upload_signed_url", "upload_signed_url", b"upload_signed_url"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_upload_signed_url", b"_upload_signed_url"]) -> typing_extensions.Literal["upload_signed_url"] | None: ...
 
-global___CreateArtifactPartResultMetadata = CreateArtifactPartResultMetadata
+global___AllocateArtifactPartResultMetadata = AllocateArtifactPartResultMetadata
 
 @typing_extensions.final
-class CreateArtifactPartResult(google.protobuf.message.Message):
+class AllocateArtifactPartResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class MetadatasByPartNumberEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
-        def value(self) -> global___CreateArtifactPartResultMetadata: ...
+        def value(self) -> global___AllocateArtifactPartResultMetadata: ...
         def __init__(
             self,
             *,
             key: builtins.int = ...,
-            value: global___CreateArtifactPartResultMetadata | None = ...,
+            value: global___AllocateArtifactPartResultMetadata | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     METADATAS_BY_PART_NUMBER_FIELD_NUMBER: builtins.int
     @property
-    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactPartResultMetadata]: ...
+    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___AllocateArtifactPartResultMetadata]: ...
     def __init__(
         self,
         *,
-        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___CreateArtifactPartResultMetadata] | None = ...,
+        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___AllocateArtifactPartResultMetadata] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas_by_part_number", b"metadatas_by_part_number"]) -> None: ...
 
-global___CreateArtifactPartResult = CreateArtifactPartResult
+global___AllocateArtifactPartResult = AllocateArtifactPartResult
 
 @typing_extensions.final
-class BatchCreateArtifactPartResponse(google.protobuf.message.Message):
+class BatchAllocateArtifactPartResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ResultsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___CreateArtifactPartResult: ...
+        def value(self) -> global___AllocateArtifactPartResult: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___CreateArtifactPartResult | None = ...,
+            value: global___AllocateArtifactPartResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___CreateArtifactPartResult]: ...
+    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___AllocateArtifactPartResult]: ...
     def __init__(
         self,
         *,
-        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___CreateArtifactPartResult] | None = ...,
+        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___AllocateArtifactPartResult] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
 
-global___BatchCreateArtifactPartResponse = BatchCreateArtifactPartResponse
+global___BatchAllocateArtifactPartResponse = BatchAllocateArtifactPartResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_create_artifact_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,34 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from models import artifact_type_pb2 as models_dot_artifact__type__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%endpoints/batch_create_artifact.proto\x12\tendpoints\"\x16\n\x14\x43reateArtifactConfig\"\xc9\x01\n\x1a\x42\x61tchCreateArtifactRequest\x12S\n\x10\x63onfigs_by_index\x18\x01 \x03(\x0b\x32\x39.endpoints.BatchCreateArtifactRequest.ConfigsByIndexEntry\x1aV\n\x13\x43onfigsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactConfig:\x02\x38\x01\"z\n\x14\x43reateArtifactResult\x12\x18\n\x0b\x61rtifact_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12 \n\x13part_size_threshold\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x0e\n\x0c_artifact_idB\x16\n\x14_part_size_threshold\"\xcb\x01\n\x1b\x42\x61tchCreateArtifactResponse\x12T\n\x10results_by_index\x18\x01 \x03(\x0b\x32:.endpoints.BatchCreateArtifactResponse.ResultsByIndexEntry\x1aV\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactResult:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%endpoints/batch_create_artifact.proto\x12\tendpoints\x1a\x1amodels/artifact_type.proto\"\x82\x01\n\x14\x43reateArtifactConfig\x12\x30\n\rartifact_type\x18\x01 \x01(\x0e\x32\x14.models.ArtifactTypeH\x00\x88\x01\x01\x12\x17\n\npart_count\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x10\n\x0e_artifact_typeB\r\n\x0b_part_count\"\xc9\x01\n\x1a\x42\x61tchCreateArtifactRequest\x12S\n\x10\x63onfigs_by_index\x18\x01 \x03(\x0b\x32\x39.endpoints.BatchCreateArtifactRequest.ConfigsByIndexEntry\x1aV\n\x13\x43onfigsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactConfig:\x02\x38\x01\"z\n\x14\x43reateArtifactResult\x12\x18\n\x0b\x61rtifact_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x12 \n\x13part_size_threshold\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x0e\n\x0c_artifact_idB\x16\n\x14_part_size_threshold\"\xcb\x01\n\x1b\x42\x61tchCreateArtifactResponse\x12T\n\x10results_by_index\x18\x01 \x03(\x0b\x32:.endpoints.BatchCreateArtifactResponse.ResultsByIndexEntry\x1aV\n\x13ResultsByIndexEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.endpoints.CreateArtifactResult:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.batch_create_artifact_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._options = None
   _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_options = b'8\001'
   _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._options = None
   _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_options = b'8\001'
-  _CREATEARTIFACTCONFIG._serialized_start=52
-  _CREATEARTIFACTCONFIG._serialized_end=74
-  _BATCHCREATEARTIFACTREQUEST._serialized_start=77
-  _BATCHCREATEARTIFACTREQUEST._serialized_end=278
-  _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_start=192
-  _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_end=278
-  _CREATEARTIFACTRESULT._serialized_start=280
-  _CREATEARTIFACTRESULT._serialized_end=402
-  _BATCHCREATEARTIFACTRESPONSE._serialized_start=405
-  _BATCHCREATEARTIFACTRESPONSE._serialized_end=608
-  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_start=522
-  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_end=608
+  _CREATEARTIFACTCONFIG._serialized_start=81
+  _CREATEARTIFACTCONFIG._serialized_end=211
+  _BATCHCREATEARTIFACTREQUEST._serialized_start=214
+  _BATCHCREATEARTIFACTREQUEST._serialized_end=415
+  _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_start=329
+  _BATCHCREATEARTIFACTREQUEST_CONFIGSBYINDEXENTRY._serialized_end=415
+  _CREATEARTIFACTRESULT._serialized_start=417
+  _CREATEARTIFACTRESULT._serialized_end=539
+  _BATCHCREATEARTIFACTRESPONSE._serialized_start=542
+  _BATCHCREATEARTIFACTRESPONSE._serialized_end=745
+  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_start=659
+  _BATCHCREATEARTIFACTRESPONSE_RESULTSBYINDEXENTRY._serialized_end=745
 # @@protoc_insertion_point(module_scope)
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -14,117 +14,110 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class CreateArtifactConfig(google.protobuf.message.Message):
-    """This config is included for potential future use.
-    In the future it may include part count, expiration, or other metadata.
-    """
-
+class FinalizeArtifactConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    TOTAL_SIZE_FIELD_NUMBER: builtins.int
+    PART_COUNT_FIELD_NUMBER: builtins.int
+    total_size: builtins.int
+    """Required field representing the size in bytes of the combined artifact parts."""
+    part_count: builtins.int
+    """Required field indicating the number of parts that were written to."""
     def __init__(
         self,
+        *,
+        total_size: builtins.int | None = ...,
+        part_count: builtins.int | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_size", b"_total_size"]) -> typing_extensions.Literal["total_size"] | None: ...
 
-global___CreateArtifactConfig = CreateArtifactConfig
+global___FinalizeArtifactConfig = FinalizeArtifactConfig
 
 @typing_extensions.final
-class BatchCreateArtifactRequest(google.protobuf.message.Message):
+class BatchFinalizeArtifactRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class ConfigsByIndexEntry(google.protobuf.message.Message):
+    class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.int
+        key: builtins.str
         @property
-        def value(self) -> global___CreateArtifactConfig: ...
+        def value(self) -> global___FinalizeArtifactConfig: ...
         def __init__(
             self,
             *,
-            key: builtins.int = ...,
-            value: global___CreateArtifactConfig | None = ...,
+            key: builtins.str = ...,
+            value: global___FinalizeArtifactConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    CONFIGS_BY_INDEX_FIELD_NUMBER: builtins.int
+    CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_index(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactConfig]:
-        """This field is a map instead of an array to avoid depending on the
-        response array being in the same order as the request array.
-        """
+    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactConfig]: ...
     def __init__(
         self,
         *,
-        configs_by_index: collections.abc.Mapping[builtins.int, global___CreateArtifactConfig] | None = ...,
+        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactConfig] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configs_by_index", b"configs_by_index"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
 
-global___BatchCreateArtifactRequest = BatchCreateArtifactRequest
+global___BatchFinalizeArtifactRequest = BatchFinalizeArtifactRequest
 
 @typing_extensions.final
-class CreateArtifactResult(google.protobuf.message.Message):
+class FinalizeArtifactResult(google.protobuf.message.Message):
+    """This message is included for potential future use."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ARTIFACT_ID_FIELD_NUMBER: builtins.int
-    PART_SIZE_THRESHOLD_FIELD_NUMBER: builtins.int
-    artifact_id: builtins.str
-    """Required field representing the unique identifier for a file stored in the cloud."""
-    part_size_threshold: builtins.int
-    """Required field indicating the precise number of bytes a part should
-    reach before creating the next part.
-    """
     def __init__(
         self,
-        *,
-        artifact_id: builtins.str | None = ...,
-        part_size_threshold: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_artifact_id", b"_artifact_id"]) -> typing_extensions.Literal["artifact_id"] | None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_size_threshold", b"_part_size_threshold"]) -> typing_extensions.Literal["part_size_threshold"] | None: ...
 
-global___CreateArtifactResult = CreateArtifactResult
+global___FinalizeArtifactResult = FinalizeArtifactResult
 
 @typing_extensions.final
-class BatchCreateArtifactResponse(google.protobuf.message.Message):
+class BatchFinalizeArtifactResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class ResultsByIndexEntry(google.protobuf.message.Message):
+    class ResultsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.int
+        key: builtins.str
         @property
-        def value(self) -> global___CreateArtifactResult: ...
+        def value(self) -> global___FinalizeArtifactResult: ...
         def __init__(
             self,
             *,
-            key: builtins.int = ...,
-            value: global___CreateArtifactResult | None = ...,
+            key: builtins.str = ...,
+            value: global___FinalizeArtifactResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    RESULTS_BY_INDEX_FIELD_NUMBER: builtins.int
+    RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def results_by_index(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactResult]: ...
+    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactResult]: ...
     def __init__(
         self,
         *,
-        results_by_index: collections.abc.Mapping[builtins.int, global___CreateArtifactResult] | None = ...,
+        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactResult] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["results_by_index", b"results_by_index"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
 
-global___BatchCreateArtifactResponse = BatchCreateArtifactResponse
+global___BatchFinalizeArtifactResponse = BatchFinalizeArtifactResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_finalize_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,110 +14,118 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class FinalizeArtifactConfig(google.protobuf.message.Message):
+class GetArtifactConfig(google.protobuf.message.Message):
+    """This message is included for potential future use."""
+
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TOTAL_SIZE_FIELD_NUMBER: builtins.int
-    PART_COUNT_FIELD_NUMBER: builtins.int
-    total_size: builtins.int
-    """Required field representing the size in bytes of the combined artifact parts."""
-    part_count: builtins.int
-    """Required field indicating the number of parts that were written to."""
     def __init__(
         self,
-        *,
-        total_size: builtins.int | None = ...,
-        part_count: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_total_size", b"_total_size", "part_count", b"part_count", "total_size", b"total_size"]) -> None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_size", b"_total_size"]) -> typing_extensions.Literal["total_size"] | None: ...
 
-global___FinalizeArtifactConfig = FinalizeArtifactConfig
+global___GetArtifactConfig = GetArtifactConfig
 
 @typing_extensions.final
-class BatchFinalizeArtifactRequest(google.protobuf.message.Message):
+class BatchGetArtifactRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___FinalizeArtifactConfig: ...
+        def value(self) -> global___GetArtifactConfig: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___FinalizeArtifactConfig | None = ...,
+            value: global___GetArtifactConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactConfig]: ...
+    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactConfig]: ...
     def __init__(
         self,
         *,
-        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactConfig] | None = ...,
+        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactConfig] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
 
-global___BatchFinalizeArtifactRequest = BatchFinalizeArtifactRequest
+global___BatchGetArtifactRequest = BatchGetArtifactRequest
 
 @typing_extensions.final
-class FinalizeArtifactResult(google.protobuf.message.Message):
-    """This result is included for potential future use."""
-
+class GetArtifactResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    PART_COUNT_FIELD_NUMBER: builtins.int
+    PART_SIZE_THRESHOLD_FIELD_NUMBER: builtins.int
+    TOTAL_SIZE_FIELD_NUMBER: builtins.int
+    part_count: builtins.int
+    """Required field indicating the number of parts uploaded by the artifact."""
+    part_size_threshold: builtins.int
+    """Required field indicating the precise number of bytes each part contains,
+    other than the final part, which can contain fewer bytes.
+    """
+    total_size: builtins.int
+    """Required field indicating the size in bytes of the combined parts."""
     def __init__(
         self,
+        *,
+        part_count: builtins.int | None = ...,
+        part_size_threshold: builtins.int | None = ...,
+        total_size: builtins.int | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_part_size_threshold", b"_part_size_threshold", "_total_size", b"_total_size", "part_count", b"part_count", "part_size_threshold", b"part_size_threshold", "total_size", b"total_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_part_size_threshold", b"_part_size_threshold", "_total_size", b"_total_size", "part_count", b"part_count", "part_size_threshold", b"part_size_threshold", "total_size", b"total_size"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_size_threshold", b"_part_size_threshold"]) -> typing_extensions.Literal["part_size_threshold"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_size", b"_total_size"]) -> typing_extensions.Literal["total_size"] | None: ...
 
-global___FinalizeArtifactResult = FinalizeArtifactResult
+global___GetArtifactResult = GetArtifactResult
 
 @typing_extensions.final
-class BatchFinalizeArtifactResponse(google.protobuf.message.Message):
+class BatchGetArtifactResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ResultsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___FinalizeArtifactResult: ...
+        def value(self) -> global___GetArtifactResult: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___FinalizeArtifactResult | None = ...,
+            value: global___GetArtifactResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FinalizeArtifactResult]: ...
+    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactResult]: ...
     def __init__(
         self,
         *,
-        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___FinalizeArtifactResult] | None = ...,
+        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactResult] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
 
-global___BatchFinalizeArtifactResponse = BatchFinalizeArtifactResponse
+global___BatchGetArtifactResponse = BatchGetArtifactResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_part_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_download_url_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -13,170 +13,170 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class GetArtifactPartConfigMetadata(google.protobuf.message.Message):
-    """This config is included for potential future use."""
+class GetArtifactDownloadUrlConfigMetadata(google.protobuf.message.Message):
+    """This message is included for potential future use."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___GetArtifactPartConfigMetadata = GetArtifactPartConfigMetadata
+global___GetArtifactDownloadUrlConfigMetadata = GetArtifactDownloadUrlConfigMetadata
 
 @typing_extensions.final
-class GetArtifactPartConfig(google.protobuf.message.Message):
+class GetArtifactDownloadUrlConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class MetadatasByPartNumberEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
-        def value(self) -> global___GetArtifactPartConfigMetadata: ...
+        def value(self) -> global___GetArtifactDownloadUrlConfigMetadata: ...
         def __init__(
             self,
             *,
             key: builtins.int = ...,
-            value: global___GetArtifactPartConfigMetadata | None = ...,
+            value: global___GetArtifactDownloadUrlConfigMetadata | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     METADATAS_BY_PART_NUMBER_FIELD_NUMBER: builtins.int
     @property
-    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GetArtifactPartConfigMetadata]: ...
+    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GetArtifactDownloadUrlConfigMetadata]: ...
     def __init__(
         self,
         *,
-        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___GetArtifactPartConfigMetadata] | None = ...,
+        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___GetArtifactDownloadUrlConfigMetadata] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas_by_part_number", b"metadatas_by_part_number"]) -> None: ...
 
-global___GetArtifactPartConfig = GetArtifactPartConfig
+global___GetArtifactDownloadUrlConfig = GetArtifactDownloadUrlConfig
 
 @typing_extensions.final
-class BatchGetArtifactPartRequest(google.protobuf.message.Message):
+class BatchGetArtifactDownloadUrlRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___GetArtifactPartConfig: ...
+        def value(self) -> global___GetArtifactDownloadUrlConfig: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___GetArtifactPartConfig | None = ...,
+            value: global___GetArtifactDownloadUrlConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactPartConfig]: ...
+    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactDownloadUrlConfig]: ...
     def __init__(
         self,
         *,
-        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactPartConfig] | None = ...,
+        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactDownloadUrlConfig] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
 
-global___BatchGetArtifactPartRequest = BatchGetArtifactPartRequest
+global___BatchGetArtifactDownloadUrlRequest = BatchGetArtifactDownloadUrlRequest
 
 @typing_extensions.final
-class GetArtifactPartResultMetadata(google.protobuf.message.Message):
+class GetArtifactDownloadUrlResultMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DOWNLOAD_SIGNED_URL_FIELD_NUMBER: builtins.int
-    download_signed_url: builtins.str
+    SIGNED_URL_FIELD_NUMBER: builtins.int
+    signed_url: builtins.str
     def __init__(
         self,
         *,
-        download_signed_url: builtins.str | None = ...,
+        signed_url: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_download_signed_url", b"_download_signed_url", "download_signed_url", b"download_signed_url"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_download_signed_url", b"_download_signed_url", "download_signed_url", b"download_signed_url"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_download_signed_url", b"_download_signed_url"]) -> typing_extensions.Literal["download_signed_url"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_signed_url", b"_signed_url", "signed_url", b"signed_url"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_signed_url", b"_signed_url", "signed_url", b"signed_url"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_signed_url", b"_signed_url"]) -> typing_extensions.Literal["signed_url"] | None: ...
 
-global___GetArtifactPartResultMetadata = GetArtifactPartResultMetadata
+global___GetArtifactDownloadUrlResultMetadata = GetArtifactDownloadUrlResultMetadata
 
 @typing_extensions.final
-class GetArtifactPartResult(google.protobuf.message.Message):
+class GetArtifactDownloadUrlResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class MetadatasByPartNumberEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
-        def value(self) -> global___GetArtifactPartResultMetadata: ...
+        def value(self) -> global___GetArtifactDownloadUrlResultMetadata: ...
         def __init__(
             self,
             *,
             key: builtins.int = ...,
-            value: global___GetArtifactPartResultMetadata | None = ...,
+            value: global___GetArtifactDownloadUrlResultMetadata | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     METADATAS_BY_PART_NUMBER_FIELD_NUMBER: builtins.int
     @property
-    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GetArtifactPartResultMetadata]: ...
+    def metadatas_by_part_number(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___GetArtifactDownloadUrlResultMetadata]: ...
     def __init__(
         self,
         *,
-        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___GetArtifactPartResultMetadata] | None = ...,
+        metadatas_by_part_number: collections.abc.Mapping[builtins.int, global___GetArtifactDownloadUrlResultMetadata] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas_by_part_number", b"metadatas_by_part_number"]) -> None: ...
 
-global___GetArtifactPartResult = GetArtifactPartResult
+global___GetArtifactDownloadUrlResult = GetArtifactDownloadUrlResult
 
 @typing_extensions.final
-class BatchGetArtifactPartResponse(google.protobuf.message.Message):
+class BatchGetArtifactDownloadUrlResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ResultsByArtifactIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
-        def value(self) -> global___GetArtifactPartResult: ...
+        def value(self) -> global___GetArtifactDownloadUrlResult: ...
         def __init__(
             self,
             *,
             key: builtins.str = ...,
-            value: global___GetArtifactPartResult | None = ...,
+            value: global___GetArtifactDownloadUrlResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
     @property
-    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactPartResult]: ...
+    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactDownloadUrlResult]: ...
     def __init__(
         self,
         *,
-        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactPartResult] | None = ...,
+        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactDownloadUrlResult] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
 
-global___BatchGetArtifactPartResponse = BatchGetArtifactPartResponse
+global___BatchGetArtifactDownloadUrlResponse = BatchGetArtifactDownloadUrlResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_get_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/batch_get_artifact_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/batch_create_artifact_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -3,129 +3,140 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
+import preemo.gen.models.artifact_type_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class GetArtifactConfig(google.protobuf.message.Message):
-    """This config is included for potential future use."""
-
+class CreateArtifactConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    ARTIFACT_TYPE_FIELD_NUMBER: builtins.int
+    PART_COUNT_FIELD_NUMBER: builtins.int
+    artifact_type: preemo.gen.models.artifact_type_pb2.ArtifactType.ValueType
+    """Required field representing the type of content the artifact will contain."""
+    part_count: builtins.int
+    """Optional field representing the initial number of parts to allocate for this artifact."""
     def __init__(
         self,
+        *,
+        artifact_type: preemo.gen.models.artifact_type_pb2.ArtifactType.ValueType | None = ...,
+        part_count: builtins.int | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_artifact_type", b"_artifact_type", "_part_count", b"_part_count", "artifact_type", b"artifact_type", "part_count", b"part_count"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_artifact_type", b"_artifact_type", "_part_count", b"_part_count", "artifact_type", b"artifact_type", "part_count", b"part_count"]) -> None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_artifact_type", b"_artifact_type"]) -> typing_extensions.Literal["artifact_type"] | None: ...
+    @typing.overload
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
 
-global___GetArtifactConfig = GetArtifactConfig
+global___CreateArtifactConfig = CreateArtifactConfig
 
 @typing_extensions.final
-class BatchGetArtifactRequest(google.protobuf.message.Message):
+class BatchCreateArtifactRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class ConfigsByArtifactIdEntry(google.protobuf.message.Message):
+    class ConfigsByIndexEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
+        key: builtins.int
         @property
-        def value(self) -> global___GetArtifactConfig: ...
+        def value(self) -> global___CreateArtifactConfig: ...
         def __init__(
             self,
             *,
-            key: builtins.str = ...,
-            value: global___GetArtifactConfig | None = ...,
+            key: builtins.int = ...,
+            value: global___CreateArtifactConfig | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    CONFIGS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
+    CONFIGS_BY_INDEX_FIELD_NUMBER: builtins.int
     @property
-    def configs_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactConfig]: ...
+    def configs_by_index(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactConfig]:
+        """This field is a map instead of an array to avoid depending on the
+        response array being in the same order as the request array.
+        """
     def __init__(
         self,
         *,
-        configs_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactConfig] | None = ...,
+        configs_by_index: collections.abc.Mapping[builtins.int, global___CreateArtifactConfig] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["configs_by_artifact_id", b"configs_by_artifact_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["configs_by_index", b"configs_by_index"]) -> None: ...
 
-global___BatchGetArtifactRequest = BatchGetArtifactRequest
+global___BatchCreateArtifactRequest = BatchCreateArtifactRequest
 
 @typing_extensions.final
-class GetArtifactResult(google.protobuf.message.Message):
+class CreateArtifactResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PART_COUNT_FIELD_NUMBER: builtins.int
+    ARTIFACT_ID_FIELD_NUMBER: builtins.int
     PART_SIZE_THRESHOLD_FIELD_NUMBER: builtins.int
-    TOTAL_SIZE_FIELD_NUMBER: builtins.int
-    part_count: builtins.int
-    """Required field indicating the number of parts uploaded by the artifact."""
+    artifact_id: builtins.str
+    """Required field representing the unique identifier for a file stored in the cloud."""
     part_size_threshold: builtins.int
-    """Required field indicating the precise number of bytes each part contains,
-    other than the final part, which can contain fewer bytes.
+    """Required field indicating the precise number of bytes a part should
+    reach before creating the next part.
     """
-    total_size: builtins.int
-    """Required field indicating the size in bytes of the combined parts."""
     def __init__(
         self,
         *,
-        part_count: builtins.int | None = ...,
+        artifact_id: builtins.str | None = ...,
         part_size_threshold: builtins.int | None = ...,
-        total_size: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_part_size_threshold", b"_part_size_threshold", "_total_size", b"_total_size", "part_count", b"part_count", "part_size_threshold", b"part_size_threshold", "total_size", b"total_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_part_count", b"_part_count", "_part_size_threshold", b"_part_size_threshold", "_total_size", b"_total_size", "part_count", b"part_count", "part_size_threshold", b"part_size_threshold", "total_size", b"total_size"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_artifact_id", b"_artifact_id", "_part_size_threshold", b"_part_size_threshold", "artifact_id", b"artifact_id", "part_size_threshold", b"part_size_threshold"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_count", b"_part_count"]) -> typing_extensions.Literal["part_count"] | None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["_artifact_id", b"_artifact_id"]) -> typing_extensions.Literal["artifact_id"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_part_size_threshold", b"_part_size_threshold"]) -> typing_extensions.Literal["part_size_threshold"] | None: ...
-    @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["_total_size", b"_total_size"]) -> typing_extensions.Literal["total_size"] | None: ...
 
-global___GetArtifactResult = GetArtifactResult
+global___CreateArtifactResult = CreateArtifactResult
 
 @typing_extensions.final
-class BatchGetArtifactResponse(google.protobuf.message.Message):
+class BatchCreateArtifactResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class ResultsByArtifactIdEntry(google.protobuf.message.Message):
+    class ResultsByIndexEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
+        key: builtins.int
         @property
-        def value(self) -> global___GetArtifactResult: ...
+        def value(self) -> global___CreateArtifactResult: ...
         def __init__(
             self,
             *,
-            key: builtins.str = ...,
-            value: global___GetArtifactResult | None = ...,
+            key: builtins.int = ...,
+            value: global___CreateArtifactResult | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    RESULTS_BY_ARTIFACT_ID_FIELD_NUMBER: builtins.int
+    RESULTS_BY_INDEX_FIELD_NUMBER: builtins.int
     @property
-    def results_by_artifact_id(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GetArtifactResult]: ...
+    def results_by_index(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___CreateArtifactResult]: ...
     def __init__(
         self,
         *,
-        results_by_artifact_id: collections.abc.Mapping[builtins.str, global___GetArtifactResult] | None = ...,
+        results_by_index: collections.abc.Mapping[builtins.int, global___CreateArtifactResult] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["results_by_artifact_id", b"results_by_artifact_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["results_by_index", b"results_by_index"]) -> None: ...
 
-global___BatchGetArtifactResponse = BatchGetArtifactResponse
+global___BatchCreateArtifactResponse = BatchCreateArtifactResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/check_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/check_function_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/check_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/execute_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/execute_function_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/execute_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/header_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/header_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/header_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/register_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/register_function_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/register_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/sdk_server_ready_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n endpoints/sdk_server_ready.proto\x12\tendpoints\"I\n\x15SDKServerReadyRequest\x12\x1c\n\x0fsdk_server_port\x18\x01 \x01(\rH\x00\x88\x01\x01\x42\x12\n\x10_sdk_server_port\"\x18\n\x16SDKServerReadyResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n endpoints/sdk_server_ready.proto\x12\tendpoints\"I\n\x15SdkServerReadyRequest\x12\x1c\n\x0fsdk_server_port\x18\x01 \x01(\rH\x00\x88\x01\x01\x42\x12\n\x10_sdk_server_port\"\x18\n\x16SdkServerReadyResponseb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'endpoints.sdk_server_ready_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _SDKSERVERREADYREQUEST._serialized_start=47
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/sdk_server_ready_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class SDKServerReadyRequest(google.protobuf.message.Message):
+class SdkServerReadyRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SDK_SERVER_PORT_FIELD_NUMBER: builtins.int
     sdk_server_port: builtins.int
     """Required field for the port on which the SDK server is listening."""
     def __init__(
         self,
         *,
         sdk_server_port: builtins.int | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_sdk_server_port", b"_sdk_server_port", "sdk_server_port", b"sdk_server_port"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_sdk_server_port", b"_sdk_server_port", "sdk_server_port", b"sdk_server_port"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_sdk_server_port", b"_sdk_server_port"]) -> typing_extensions.Literal["sdk_server_port"] | None: ...
 
-global___SDKServerReadyRequest = SDKServerReadyRequest
+global___SdkServerReadyRequest = SdkServerReadyRequest
 
 @typing_extensions.final
-class SDKServerReadyResponse(google.protobuf.message.Message):
+class SdkServerReadyResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___SDKServerReadyResponse = SDKServerReadyResponse
+global___SdkServerReadyResponse = SdkServerReadyResponse
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/terminate_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/endpoints/terminate_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/endpoints/terminate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/models/registered_function_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/models/registered_function_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/models/registered_function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.py` & `preemo_worker_sdk-0.4.0/preemo/gen/models/value_pb2.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/models/value_pb2.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/models/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.py` & `preemo_worker_sdk-0.4.0/preemo/gen/services/sdk_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from endpoints import execute_function_pb2 as endpoints_dot_execute__function__pb2
 from endpoints import terminate_pb2 as endpoints_dot_terminate__pb2
 
 
-class SDKServiceStub(object):
+class SdkServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ExecuteFunction = channel.unary_unary(
-                '/services.SDKService/ExecuteFunction',
+                '/services.SdkService/ExecuteFunction',
                 request_serializer=endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.FromString,
                 )
         self.Terminate = channel.unary_unary(
-                '/services.SDKService/Terminate',
+                '/services.SdkService/Terminate',
                 request_serializer=endpoints_dot_terminate__pb2.TerminateRequest.SerializeToString,
                 response_deserializer=endpoints_dot_terminate__pb2.TerminateResponse.FromString,
                 )
 
 
-class SDKServiceServicer(object):
+class SdkServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ExecuteFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
@@ -39,48 +39,48 @@
     def Terminate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_SDKServiceServicer_to_server(servicer, server):
+def add_SdkServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ExecuteFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.ExecuteFunction,
                     request_deserializer=endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.FromString,
                     response_serializer=endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.SerializeToString,
             ),
             'Terminate': grpc.unary_unary_rpc_method_handler(
                     servicer.Terminate,
                     request_deserializer=endpoints_dot_terminate__pb2.TerminateRequest.FromString,
                     response_serializer=endpoints_dot_terminate__pb2.TerminateResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'services.SDKService', rpc_method_handlers)
+            'services.SdkService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class SDKService(object):
+class SdkService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def ExecuteFunction(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.SDKService/ExecuteFunction',
+        return grpc.experimental.unary_unary(request, target, '/services.SdkService/ExecuteFunction',
             endpoints_dot_execute__function__pb2.ExecuteFunctionRequest.SerializeToString,
             endpoints_dot_execute__function__pb2.ExecuteFunctionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Terminate(request,
@@ -89,12 +89,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.SDKService/Terminate',
+        return grpc.experimental.unary_unary(request, target, '/services.SdkService/Terminate',
             endpoints_dot_terminate__pb2.TerminateRequest.SerializeToString,
             endpoints_dot_terminate__pb2.TerminateResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/services/sdk_pb2_grpc.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/services/sdk_pb2_grpc.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 isort:skip_file
 """
 import abc
 import preemo.gen.endpoints.execute_function_pb2
 import preemo.gen.endpoints.terminate_pb2
 import grpc
 
-class SDKServiceStub:
+class SdkServiceStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
     ExecuteFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionRequest,
         preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionResponse,
     ]
     Terminate: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.terminate_pb2.TerminateRequest,
         preemo.gen.endpoints.terminate_pb2.TerminateResponse,
     ]
 
-class SDKServiceServicer(metaclass=abc.ABCMeta):
+class SdkServiceServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def ExecuteFunction(
         self,
         request: preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.execute_function_pb2.ExecuteFunctionResponse: ...
     @abc.abstractmethod
     def Terminate(
         self,
         request: preemo.gen.endpoints.terminate_pb2.TerminateRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.terminate_pb2.TerminateResponse: ...
 
-def add_SDKServiceServicer_to_server(servicer: SDKServiceServicer, server: grpc.Server) -> None: ...
+def add_SdkServiceServicer_to_server(servicer: SdkServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.py` & `preemo_worker_sdk-0.4.0/preemo/gen/services/worker_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from endpoints import batch_create_artifact_part_pb2 as endpoints_dot_batch__create__artifact__part__pb2
+from endpoints import batch_allocate_artifact_part_pb2 as endpoints_dot_batch__allocate__artifact__part__pb2
 from endpoints import batch_create_artifact_pb2 as endpoints_dot_batch__create__artifact__pb2
 from endpoints import batch_execute_function_pb2 as endpoints_dot_batch__execute__function__pb2
 from endpoints import batch_finalize_artifact_pb2 as endpoints_dot_batch__finalize__artifact__pb2
-from endpoints import batch_get_artifact_part_pb2 as endpoints_dot_batch__get__artifact__part__pb2
+from endpoints import batch_get_artifact_download_url_pb2 as endpoints_dot_batch__get__artifact__download__url__pb2
 from endpoints import batch_get_artifact_pb2 as endpoints_dot_batch__get__artifact__pb2
+from endpoints import batch_get_artifact_upload_url_pb2 as endpoints_dot_batch__get__artifact__upload__url__pb2
 from endpoints import check_function_pb2 as endpoints_dot_check__function__pb2
 from endpoints import header_pb2 as endpoints_dot_header__pb2
 from endpoints import register_function_pb2 as endpoints_dot_register__function__pb2
 from endpoints import sdk_server_ready_pb2 as endpoints_dot_sdk__server__ready__pb2
 
 
 class WorkerServiceStub(object):
@@ -19,44 +20,49 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.BatchAllocateArtifactPart = channel.unary_unary(
+                '/services.WorkerService/BatchAllocateArtifactPart',
+                request_serializer=endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartRequest.SerializeToString,
+                response_deserializer=endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartResponse.FromString,
+                )
         self.BatchCreateArtifact = channel.unary_unary(
                 '/services.WorkerService/BatchCreateArtifact',
                 request_serializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.FromString,
                 )
-        self.BatchCreateArtifactPart = channel.unary_unary(
-                '/services.WorkerService/BatchCreateArtifactPart',
-                request_serializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.SerializeToString,
-                response_deserializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.FromString,
-                )
         self.BatchExecuteFunction = channel.unary_unary(
                 '/services.WorkerService/BatchExecuteFunction',
                 request_serializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionResponse.FromString,
                 )
         self.BatchFinalizeArtifact = channel.unary_unary(
                 '/services.WorkerService/BatchFinalizeArtifact',
                 request_serializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactResponse.FromString,
                 )
+        self.BatchGetArtifactDownloadUrl = channel.unary_unary(
+                '/services.WorkerService/BatchGetArtifactDownloadUrl',
+                request_serializer=endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlRequest.SerializeToString,
+                response_deserializer=endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlResponse.FromString,
+                )
+        self.BatchGetArtifactUploadUrl = channel.unary_unary(
+                '/services.WorkerService/BatchGetArtifactUploadUrl',
+                request_serializer=endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlRequest.SerializeToString,
+                response_deserializer=endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlResponse.FromString,
+                )
         self.BatchGetArtifact = channel.unary_unary(
                 '/services.WorkerService/BatchGetArtifact',
                 request_serializer=endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactRequest.SerializeToString,
                 response_deserializer=endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactResponse.FromString,
                 )
-        self.BatchGetArtifactPart = channel.unary_unary(
-                '/services.WorkerService/BatchGetArtifactPart',
-                request_serializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartRequest.SerializeToString,
-                response_deserializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartResponse.FromString,
-                )
         self.CheckFunction = channel.unary_unary(
                 '/services.WorkerService/CheckFunction',
                 request_serializer=endpoints_dot_check__function__pb2.CheckFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_check__function__pb2.CheckFunctionResponse.FromString,
                 )
         self.Initiate = channel.unary_unary(
                 '/services.WorkerService/Initiate',
@@ -64,31 +70,31 @@
                 response_deserializer=endpoints_dot_header__pb2.HeaderResponse.FromString,
                 )
         self.RegisterFunction = channel.unary_unary(
                 '/services.WorkerService/RegisterFunction',
                 request_serializer=endpoints_dot_register__function__pb2.RegisterFunctionRequest.SerializeToString,
                 response_deserializer=endpoints_dot_register__function__pb2.RegisterFunctionResponse.FromString,
                 )
-        self.SDKServerReady = channel.unary_unary(
-                '/services.WorkerService/SDKServerReady',
-                request_serializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.SerializeToString,
-                response_deserializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.FromString,
+        self.SdkServerReady = channel.unary_unary(
+                '/services.WorkerService/SdkServerReady',
+                request_serializer=endpoints_dot_sdk__server__ready__pb2.SdkServerReadyRequest.SerializeToString,
+                response_deserializer=endpoints_dot_sdk__server__ready__pb2.SdkServerReadyResponse.FromString,
                 )
 
 
 class WorkerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def BatchCreateArtifact(self, request, context):
+    def BatchAllocateArtifactPart(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def BatchCreateArtifactPart(self, request, context):
+    def BatchCreateArtifact(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def BatchExecuteFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -98,21 +104,27 @@
 
     def BatchFinalizeArtifact(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def BatchGetArtifact(self, request, context):
+    def BatchGetArtifactDownloadUrl(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def BatchGetArtifactUploadUrl(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def BatchGetArtifactPart(self, request, context):
+    def BatchGetArtifact(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CheckFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -128,53 +140,58 @@
 
     def RegisterFunction(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def SDKServerReady(self, request, context):
+    def SdkServerReady(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_WorkerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'BatchAllocateArtifactPart': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchAllocateArtifactPart,
+                    request_deserializer=endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartRequest.FromString,
+                    response_serializer=endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartResponse.SerializeToString,
+            ),
             'BatchCreateArtifact': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchCreateArtifact,
                     request_deserializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactRequest.FromString,
                     response_serializer=endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.SerializeToString,
             ),
-            'BatchCreateArtifactPart': grpc.unary_unary_rpc_method_handler(
-                    servicer.BatchCreateArtifactPart,
-                    request_deserializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.FromString,
-                    response_serializer=endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.SerializeToString,
-            ),
             'BatchExecuteFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchExecuteFunction,
                     request_deserializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionRequest.FromString,
                     response_serializer=endpoints_dot_batch__execute__function__pb2.BatchExecuteFunctionResponse.SerializeToString,
             ),
             'BatchFinalizeArtifact': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchFinalizeArtifact,
                     request_deserializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactRequest.FromString,
                     response_serializer=endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactResponse.SerializeToString,
             ),
+            'BatchGetArtifactDownloadUrl': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchGetArtifactDownloadUrl,
+                    request_deserializer=endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlRequest.FromString,
+                    response_serializer=endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlResponse.SerializeToString,
+            ),
+            'BatchGetArtifactUploadUrl': grpc.unary_unary_rpc_method_handler(
+                    servicer.BatchGetArtifactUploadUrl,
+                    request_deserializer=endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlRequest.FromString,
+                    response_serializer=endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlResponse.SerializeToString,
+            ),
             'BatchGetArtifact': grpc.unary_unary_rpc_method_handler(
                     servicer.BatchGetArtifact,
                     request_deserializer=endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactRequest.FromString,
                     response_serializer=endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactResponse.SerializeToString,
             ),
-            'BatchGetArtifactPart': grpc.unary_unary_rpc_method_handler(
-                    servicer.BatchGetArtifactPart,
-                    request_deserializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartRequest.FromString,
-                    response_serializer=endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartResponse.SerializeToString,
-            ),
             'CheckFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.CheckFunction,
                     request_deserializer=endpoints_dot_check__function__pb2.CheckFunctionRequest.FromString,
                     response_serializer=endpoints_dot_check__function__pb2.CheckFunctionResponse.SerializeToString,
             ),
             'Initiate': grpc.unary_unary_rpc_method_handler(
                     servicer.Initiate,
@@ -182,60 +199,60 @@
                     response_serializer=endpoints_dot_header__pb2.HeaderResponse.SerializeToString,
             ),
             'RegisterFunction': grpc.unary_unary_rpc_method_handler(
                     servicer.RegisterFunction,
                     request_deserializer=endpoints_dot_register__function__pb2.RegisterFunctionRequest.FromString,
                     response_serializer=endpoints_dot_register__function__pb2.RegisterFunctionResponse.SerializeToString,
             ),
-            'SDKServerReady': grpc.unary_unary_rpc_method_handler(
-                    servicer.SDKServerReady,
-                    request_deserializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.FromString,
-                    response_serializer=endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.SerializeToString,
+            'SdkServerReady': grpc.unary_unary_rpc_method_handler(
+                    servicer.SdkServerReady,
+                    request_deserializer=endpoints_dot_sdk__server__ready__pb2.SdkServerReadyRequest.FromString,
+                    response_serializer=endpoints_dot_sdk__server__ready__pb2.SdkServerReadyResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'services.WorkerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class WorkerService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def BatchCreateArtifact(request,
+    def BatchAllocateArtifactPart(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchCreateArtifact',
-            endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactRequest.SerializeToString,
-            endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchAllocateArtifactPart',
+            endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartRequest.SerializeToString,
+            endpoints_dot_batch__allocate__artifact__part__pb2.BatchAllocateArtifactPartResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def BatchCreateArtifactPart(request,
+    def BatchCreateArtifact(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchCreateArtifactPart',
-            endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartRequest.SerializeToString,
-            endpoints_dot_batch__create__artifact__part__pb2.BatchCreateArtifactPartResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchCreateArtifact',
+            endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactRequest.SerializeToString,
+            endpoints_dot_batch__create__artifact__pb2.BatchCreateArtifactResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def BatchExecuteFunction(request,
             target,
             options=(),
@@ -266,44 +283,61 @@
         return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchFinalizeArtifact',
             endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactRequest.SerializeToString,
             endpoints_dot_batch__finalize__artifact__pb2.BatchFinalizeArtifactResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def BatchGetArtifact(request,
+    def BatchGetArtifactDownloadUrl(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchGetArtifact',
-            endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactRequest.SerializeToString,
-            endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchGetArtifactDownloadUrl',
+            endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlRequest.SerializeToString,
+            endpoints_dot_batch__get__artifact__download__url__pb2.BatchGetArtifactDownloadUrlResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def BatchGetArtifactUploadUrl(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchGetArtifactUploadUrl',
+            endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlRequest.SerializeToString,
+            endpoints_dot_batch__get__artifact__upload__url__pb2.BatchGetArtifactUploadUrlResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def BatchGetArtifactPart(request,
+    def BatchGetArtifact(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchGetArtifactPart',
-            endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartRequest.SerializeToString,
-            endpoints_dot_batch__get__artifact__part__pb2.BatchGetArtifactPartResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/BatchGetArtifact',
+            endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactRequest.SerializeToString,
+            endpoints_dot_batch__get__artifact__pb2.BatchGetArtifactResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CheckFunction(request,
             target,
             options=(),
@@ -351,22 +385,22 @@
         return grpc.experimental.unary_unary(request, target, '/services.WorkerService/RegisterFunction',
             endpoints_dot_register__function__pb2.RegisterFunctionRequest.SerializeToString,
             endpoints_dot_register__function__pb2.RegisterFunctionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def SDKServerReady(request,
+    def SdkServerReady(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/SDKServerReady',
-            endpoints_dot_sdk__server__ready__pb2.SDKServerReadyRequest.SerializeToString,
-            endpoints_dot_sdk__server__ready__pb2.SDKServerReadyResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/services.WorkerService/SdkServerReady',
+            endpoints_dot_sdk__server__ready__pb2.SdkServerReadyRequest.SerializeToString,
+            endpoints_dot_sdk__server__ready__pb2.SdkServerReadyResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/gen/services/worker_pb2_grpc.pyi` & `preemo_worker_sdk-0.4.0/preemo/gen/services/worker_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,115 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
-import preemo.gen.endpoints.batch_create_artifact_part_pb2
+import preemo.gen.endpoints.batch_allocate_artifact_part_pb2
 import preemo.gen.endpoints.batch_create_artifact_pb2
 import preemo.gen.endpoints.batch_execute_function_pb2
 import preemo.gen.endpoints.batch_finalize_artifact_pb2
-import preemo.gen.endpoints.batch_get_artifact_part_pb2
+import preemo.gen.endpoints.batch_get_artifact_download_url_pb2
 import preemo.gen.endpoints.batch_get_artifact_pb2
+import preemo.gen.endpoints.batch_get_artifact_upload_url_pb2
 import preemo.gen.endpoints.check_function_pb2
 import preemo.gen.endpoints.header_pb2
 import preemo.gen.endpoints.register_function_pb2
 import preemo.gen.endpoints.sdk_server_ready_pb2
 import grpc
 
 class WorkerServiceStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
+    BatchAllocateArtifactPart: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.batch_allocate_artifact_part_pb2.BatchAllocateArtifactPartRequest,
+        preemo.gen.endpoints.batch_allocate_artifact_part_pb2.BatchAllocateArtifactPartResponse,
+    ]
     BatchCreateArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactRequest,
         preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactResponse,
     ]
-    BatchCreateArtifactPart: grpc.UnaryUnaryMultiCallable[
-        preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartRequest,
-        preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartResponse,
-    ]
     BatchExecuteFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionRequest,
         preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionResponse,
     ]
     BatchFinalizeArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactRequest,
         preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactResponse,
     ]
+    BatchGetArtifactDownloadUrl: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.batch_get_artifact_download_url_pb2.BatchGetArtifactDownloadUrlRequest,
+        preemo.gen.endpoints.batch_get_artifact_download_url_pb2.BatchGetArtifactDownloadUrlResponse,
+    ]
+    BatchGetArtifactUploadUrl: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.batch_get_artifact_upload_url_pb2.BatchGetArtifactUploadUrlRequest,
+        preemo.gen.endpoints.batch_get_artifact_upload_url_pb2.BatchGetArtifactUploadUrlResponse,
+    ]
     BatchGetArtifact: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactRequest,
         preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactResponse,
     ]
-    BatchGetArtifactPart: grpc.UnaryUnaryMultiCallable[
-        preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartRequest,
-        preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartResponse,
-    ]
     CheckFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.check_function_pb2.CheckFunctionRequest,
         preemo.gen.endpoints.check_function_pb2.CheckFunctionResponse,
     ]
     Initiate: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.header_pb2.HeaderRequest,
         preemo.gen.endpoints.header_pb2.HeaderResponse,
     ]
     RegisterFunction: grpc.UnaryUnaryMultiCallable[
         preemo.gen.endpoints.register_function_pb2.RegisterFunctionRequest,
         preemo.gen.endpoints.register_function_pb2.RegisterFunctionResponse,
     ]
-    SDKServerReady: grpc.UnaryUnaryMultiCallable[
-        preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyRequest,
-        preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyResponse,
+    SdkServerReady: grpc.UnaryUnaryMultiCallable[
+        preemo.gen.endpoints.sdk_server_ready_pb2.SdkServerReadyRequest,
+        preemo.gen.endpoints.sdk_server_ready_pb2.SdkServerReadyResponse,
     ]
 
 class WorkerServiceServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def BatchCreateArtifact(
+    def BatchAllocateArtifactPart(
         self,
-        request: preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactRequest,
+        request: preemo.gen.endpoints.batch_allocate_artifact_part_pb2.BatchAllocateArtifactPartRequest,
         context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactResponse: ...
+    ) -> preemo.gen.endpoints.batch_allocate_artifact_part_pb2.BatchAllocateArtifactPartResponse: ...
     @abc.abstractmethod
-    def BatchCreateArtifactPart(
+    def BatchCreateArtifact(
         self,
-        request: preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartRequest,
+        request: preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactRequest,
         context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.batch_create_artifact_part_pb2.BatchCreateArtifactPartResponse: ...
+    ) -> preemo.gen.endpoints.batch_create_artifact_pb2.BatchCreateArtifactResponse: ...
     @abc.abstractmethod
     def BatchExecuteFunction(
         self,
         request: preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.batch_execute_function_pb2.BatchExecuteFunctionResponse: ...
     @abc.abstractmethod
     def BatchFinalizeArtifact(
         self,
         request: preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.batch_finalize_artifact_pb2.BatchFinalizeArtifactResponse: ...
     @abc.abstractmethod
-    def BatchGetArtifact(
+    def BatchGetArtifactDownloadUrl(
         self,
-        request: preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactRequest,
+        request: preemo.gen.endpoints.batch_get_artifact_download_url_pb2.BatchGetArtifactDownloadUrlRequest,
         context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactResponse: ...
+    ) -> preemo.gen.endpoints.batch_get_artifact_download_url_pb2.BatchGetArtifactDownloadUrlResponse: ...
     @abc.abstractmethod
-    def BatchGetArtifactPart(
+    def BatchGetArtifactUploadUrl(
         self,
-        request: preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartRequest,
+        request: preemo.gen.endpoints.batch_get_artifact_upload_url_pb2.BatchGetArtifactUploadUrlRequest,
         context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.batch_get_artifact_part_pb2.BatchGetArtifactPartResponse: ...
+    ) -> preemo.gen.endpoints.batch_get_artifact_upload_url_pb2.BatchGetArtifactUploadUrlResponse: ...
+    @abc.abstractmethod
+    def BatchGetArtifact(
+        self,
+        request: preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactRequest,
+        context: grpc.ServicerContext,
+    ) -> preemo.gen.endpoints.batch_get_artifact_pb2.BatchGetArtifactResponse: ...
     @abc.abstractmethod
     def CheckFunction(
         self,
         request: preemo.gen.endpoints.check_function_pb2.CheckFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.check_function_pb2.CheckFunctionResponse: ...
     @abc.abstractmethod
@@ -110,14 +121,14 @@
     @abc.abstractmethod
     def RegisterFunction(
         self,
         request: preemo.gen.endpoints.register_function_pb2.RegisterFunctionRequest,
         context: grpc.ServicerContext,
     ) -> preemo.gen.endpoints.register_function_pb2.RegisterFunctionResponse: ...
     @abc.abstractmethod
-    def SDKServerReady(
+    def SdkServerReady(
         self,
-        request: preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyRequest,
+        request: preemo.gen.endpoints.sdk_server_ready_pb2.SdkServerReadyRequest,
         context: grpc.ServicerContext,
-    ) -> preemo.gen.endpoints.sdk_server_ready_pb2.SDKServerReadyResponse: ...
+    ) -> preemo.gen.endpoints.sdk_server_ready_pb2.SdkServerReadyResponse: ...
 
 def add_WorkerServiceServicer_to_server(servicer: WorkerServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/__init__.py` & `preemo_worker_sdk-0.4.0/preemo/worker/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,62 @@
-import threading
-from typing import Optional
+from threading import Thread as _Thread
+from typing import Optional as _Optional
 
 from preemo.gen.endpoints.sdk_server_ready_pb2 import (
-    SDKServerReadyRequest as _SDKServerReadyRequest,
+    SdkServerReadyRequest as _SdkServerReadyRequest,
 )
 from preemo.worker._artifact_manager import ArtifactManager as _ArtifactManager
 from preemo.worker._artifact_manager import IArtifactManager as _IArtifactManager
-from preemo.worker._env import get_optional_int_env as _get_optional_int_env
-from preemo.worker._env import get_optional_string_env as _get_optional_string_env
+from preemo.worker._env_manager import EnvManager as _EnvManager
 from preemo.worker._function_registry import FunctionRegistry as _FunctionRegistry
 from preemo.worker._messaging_client import IMessagingClient as _IMessagingClient
 from preemo.worker._messaging_client import (
     LocalMessagingClient as _LocalMessagingClient,
 )
 from preemo.worker._messaging_client import MessagingClient as _MessagingClient
-from preemo.worker._sdk_server import SDKServer as _SDKServer
+from preemo.worker._sdk_server import SdkServer as _SdkServer
 from preemo.worker._worker_client import WorkerClient as _WorkerClient
 
 
-def _construct_artifact_manager(
-    messaging_client: _IMessagingClient,
-) -> _IArtifactManager:
-    max_download_threads = _get_optional_int_env("PREEMO_MAX_DOWNLOAD_THREADS")
-    if max_download_threads is None:
-        max_download_threads = 5
-
-    max_upload_threads = _get_optional_int_env("PREEMO_MAX_UPLOAD_THREADS")
-    if max_upload_threads is None:
-        max_upload_threads = 5
-
-    return _ArtifactManager(
-        max_download_threads=max_download_threads,
-        max_upload_threads=max_upload_threads,
-        messaging_client=messaging_client,
-    )
-
-
 def _construct_messaging_client() -> _IMessagingClient:
-    worker_server_url = _get_optional_string_env("PREEMO_WORKER_SERVER_URL")
-
-    if worker_server_url is None:
+    if _EnvManager.worker_server_url is None:
         return _LocalMessagingClient()
 
-    return _MessagingClient(worker_server_url=worker_server_url)
+    return _MessagingClient(worker_server_url=_EnvManager.worker_server_url)
 
 
 def _start_sdk_server(
     *, artifact_manager: _IArtifactManager, function_registry: _FunctionRegistry
-) -> Optional[_SDKServer]:
-    sdk_server_host = _get_optional_string_env("PREEMO_SDK_SERVER_HOST")
-    if sdk_server_host is None:
+) -> _Optional[_SdkServer]:
+    if _EnvManager.sdk_server_host is None:
         return None
 
-    server = _SDKServer(
+    server = _SdkServer(
         artifact_manager=artifact_manager,
         function_registry=function_registry,
-        sdk_server_host=sdk_server_host,
+        sdk_server_host=_EnvManager.sdk_server_host,
     )
     # This thread will keep the process running until the server is closed
-    threading.Thread(target=lambda: server.wait_until_close()).start()
+    _Thread(target=lambda: server.wait_until_close()).start()
 
     return server
 
 
 def _construct_worker_client() -> _WorkerClient:
     messaging_client = _construct_messaging_client()
-    artifact_manager = _construct_artifact_manager(messaging_client=messaging_client)
+    artifact_manager = _ArtifactManager(messaging_client=messaging_client)
 
     function_registry = _FunctionRegistry()
     sdk_server = _start_sdk_server(
         artifact_manager=artifact_manager, function_registry=function_registry
     )
 
     if sdk_server is not None:
         messaging_client.sdk_server_ready(
-            _SDKServerReadyRequest(sdk_server_port=sdk_server.get_port())
+            _SdkServerReadyRequest(sdk_server_port=sdk_server.get_port())
         )
 
     return _WorkerClient(
         artifact_manager=artifact_manager,
         function_registry=function_registry,
         messaging_client=messaging_client,
     )
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/__init__.pyi` & `preemo_worker_sdk-0.4.0/preemo/worker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_artifact_manager.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_artifact_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,181 +1,227 @@
 import concurrent.futures
+import enum
 import math
 from typing import Dict, List, Protocol, runtime_checkable
 
 import requests
 from pydantic import StrictInt
 
-from preemo.gen.endpoints.batch_create_artifact_part_pb2 import (
-    BatchCreateArtifactPartRequest,
-    CreateArtifactPartConfig,
-    CreateArtifactPartConfigMetadata,
+from preemo.gen.endpoints.batch_allocate_artifact_part_pb2 import (
+    AllocateArtifactPartConfig,
+    AllocateArtifactPartConfigMetadata,
+    BatchAllocateArtifactPartRequest,
 )
 from preemo.gen.endpoints.batch_create_artifact_pb2 import (
     BatchCreateArtifactRequest,
     CreateArtifactConfig,
 )
 from preemo.gen.endpoints.batch_finalize_artifact_pb2 import (
     BatchFinalizeArtifactRequest,
     FinalizeArtifactConfig,
 )
-from preemo.gen.endpoints.batch_get_artifact_part_pb2 import (
-    BatchGetArtifactPartRequest,
-    GetArtifactPartConfig,
-    GetArtifactPartConfigMetadata,
+from preemo.gen.endpoints.batch_get_artifact_download_url_pb2 import (
+    BatchGetArtifactDownloadUrlRequest,
+    GetArtifactDownloadUrlConfig,
+    GetArtifactDownloadUrlConfigMetadata,
 )
 from preemo.gen.endpoints.batch_get_artifact_pb2 import (
     BatchGetArtifactRequest,
     GetArtifactConfig,
 )
+from preemo.gen.endpoints.batch_get_artifact_upload_url_pb2 import (
+    BatchGetArtifactUploadUrlRequest,
+    GetArtifactUploadUrlConfig,
+    GetArtifactUploadUrlConfigMetadata,
+)
+from preemo.gen.models.artifact_type_pb2 import (
+    ARTIFACT_TYPE_PARAMS,
+    ARTIFACT_TYPE_RESULT,
+)
+from preemo.worker._env_manager import EnvManager
 from preemo.worker._messaging_client import IMessagingClient
 from preemo.worker._types import ImmutableModel, StringValue
-from preemo.worker._validation import ensure_keys_match
 
 
 class ArtifactId(StringValue):
     pass
 
 
 class Artifact(ImmutableModel):
     id: ArtifactId
     part_size_threshold: StrictInt
 
 
+class ArtifactType(enum.Enum):
+    PARAMS = "params"
+    RESULT = "result"
+
+
 @runtime_checkable
 class IArtifactManager(Protocol):
-    def create_artifact(self, content: bytes) -> ArtifactId:
+    def create_artifact(self, *, content: bytes, type_: ArtifactType) -> ArtifactId:
         pass
 
-    def create_artifacts(self, contents: List[bytes]) -> List[ArtifactId]:
+    def create_artifacts(
+        self, *, contents: List[bytes], type_: ArtifactType
+    ) -> List[ArtifactId]:
         pass
 
-    def get_artifact(self, artifact_id: ArtifactId) -> bytes:
+    def get_artifact(self, *, artifact_id: ArtifactId) -> bytes:
         pass
 
-    def get_artifacts(self, artifact_ids: List[ArtifactId]) -> List[bytes]:
+    def get_artifacts(self, *, artifact_ids: List[ArtifactId]) -> List[bytes]:
         pass
 
 
 class ArtifactManager:
     @staticmethod
     def _calculate_part_count(*, content_length: int, part_size_threshold: int) -> int:
         return max(1, math.ceil(content_length / part_size_threshold))
 
-    @staticmethod
-    def _upload_content(*, content: memoryview, url: str) -> None:
-        response = requests.put(
-            url=url, data=content, headers={"Content-Encoding": "gzip"}
-        )
-
-        # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
-        if not response.ok:
-            raise Exception(f"unexpected response while uploading: {response}")
-
-    @staticmethod
-    def _download_content(*, url: str) -> bytes:
-        response = requests.get(url=url, headers={"Accept-Encoding": "gzip"})
-
-        # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
-        if not response.ok:
-            raise Exception(f"unexpected response while downloading: {response}")
-
-        return response.content
-
     def __init__(
         self,
         *,
-        max_download_threads: int,
-        max_upload_threads: int,
         messaging_client: IMessagingClient,
     ) -> None:
-        if max_download_threads <= 0:
-            raise ValueError("max_download_threads must be positive")
+        self._messaging_client = messaging_client
+
+    def _write_content(self, *, content: memoryview, url: str) -> None:
+        if EnvManager.is_development:
+            # treat url as file path
+            with open(url, "wb") as fout:
+                fout.write(content)
+        else:
+            # TODO(adrian@preemo.io, 04/11/2023): might be post
+            response = requests.put(
+                url=url, data=content, headers={"Content-Encoding": "gzip"}
+            )
 
-        if max_upload_threads <= 0:
-            raise ValueError("max_upload_threads must be positive")
+            # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
+            if not response.ok:
+                raise Exception(f"unexpected response while uploading: {response}")
+
+    def _read_content(self, *, url: str) -> bytes:
+        if EnvManager.is_development:
+            # treat url as file path
+            with open(url, "rb") as fin:
+                return fin.read()
+        else:
+            response = requests.get(url=url, headers={"Accept-Encoding": "gzip"})
+
+            # TODO(adrian@preemo.io, 04/15/2023): should retry if it fails
+            if not response.ok:
+                raise Exception(f"unexpected response while downloading: {response}")
 
-        self._max_download_threads = max_download_threads
-        self._max_upload_threads = max_upload_threads
-        self._messaging_client = messaging_client
+            return response.content
 
-    def _create_artifacts(self, *, count: int) -> List[Artifact]:
-        configs_by_index = {i: CreateArtifactConfig() for i in range(count)}
+    def _create_artifacts(
+        self,
+        *,
+        count: int,
+        type_: ArtifactType,
+    ) -> List[Artifact]:
+        if type_ == ArtifactType.PARAMS:
+            artifact_type = ARTIFACT_TYPE_PARAMS
+        elif type_ == ArtifactType.RESULT:
+            artifact_type = ARTIFACT_TYPE_RESULT
+        else:
+            raise AssertionError(f"Expected code to be unreachable, but got: {type_}")
+
+        configs_by_index = {
+            i: CreateArtifactConfig(artifact_type=artifact_type) for i in range(count)
+        }
         response = self._messaging_client.batch_create_artifact(
             BatchCreateArtifactRequest(configs_by_index=configs_by_index)
         )
 
         return [
             Artifact(
                 id=ArtifactId(value=result.artifact_id),
                 part_size_threshold=result.part_size_threshold,
             )
             for _, result in sorted(
                 response.results_by_index.items(), key=lambda x: x[0]
             )
         ]
 
-    def create_artifact(self, content: bytes) -> ArtifactId:
-        artifact_ids = self.create_artifacts([content])
+    def create_artifact(self, *, content: bytes, type_: ArtifactType) -> ArtifactId:
+        artifact_ids = self.create_artifacts(contents=[content], type_=type_)
         if len(artifact_ids) != 1:
             raise Exception("expected exactly one artifact to be created")
 
         return artifact_ids[0]
 
-    def create_artifacts(self, contents: List[bytes]) -> List[ArtifactId]:
-        artifacts = self._create_artifacts(count=len(contents))
+    def create_artifacts(
+        self, *, contents: List[bytes], type_: ArtifactType
+    ) -> List[ArtifactId]:
+        artifacts = self._create_artifacts(count=len(contents), type_=type_)
         if len(artifacts) != len(contents):
             raise Exception("expected artifacts and contents lengths to be equal")
         artifacts_and_contents = zip(artifacts, contents)
 
-        configs_by_artifact_id_value: Dict[str, CreateArtifactPartConfig] = {}
+        allocate_configs_by_artifact_id_value: Dict[
+            str, AllocateArtifactPartConfig
+        ] = {}
+        upload_configs_by_artifact_id_value: Dict[str, GetArtifactUploadUrlConfig] = {}
         for artifact, content in artifacts_and_contents:
             part_count = ArtifactManager._calculate_part_count(
                 content_length=len(content),
                 part_size_threshold=artifact.part_size_threshold,
             )
 
-            configs_by_artifact_id_value[artifact.id.value] = CreateArtifactPartConfig(
+            allocate_configs_by_artifact_id_value[
+                artifact.id.value
+            ] = AllocateArtifactPartConfig(
                 metadatas_by_part_number={
-                    part_number: CreateArtifactPartConfigMetadata()
+                    part_number: AllocateArtifactPartConfigMetadata()
                     for part_number in range(part_count)
                 }
             )
 
-        response = self._messaging_client.batch_create_artifact_part(
-            BatchCreateArtifactPartRequest(
-                configs_by_artifact_id=configs_by_artifact_id_value
+            upload_configs_by_artifact_id_value[
+                artifact.id.value
+            ] = GetArtifactUploadUrlConfig(
+                metadatas_by_part_number={
+                    part_number: GetArtifactUploadUrlConfigMetadata()
+                    for part_number in range(part_count)
+                }
+            )
+
+        self._messaging_client.batch_allocate_artifact_part(
+            BatchAllocateArtifactPartRequest(
+                configs_by_artifact_id=allocate_configs_by_artifact_id_value
+            )
+        )
+
+        get_url_response = self._messaging_client.batch_get_artifact_upload_url(
+            BatchGetArtifactUploadUrlRequest(
+                configs_by_artifact_id=upload_configs_by_artifact_id_value
             )
         )
 
         with concurrent.futures.ThreadPoolExecutor(
-            max_workers=self._max_upload_threads
+            max_workers=EnvManager.max_upload_threads
         ) as executor:
             futures = []
             for artifact, content in artifacts_and_contents:
                 content_view = memoryview(content)
-
-                config = configs_by_artifact_id_value[artifact.id.value]
-                result = response.results_by_artifact_id[artifact.id.value]
-                ensure_keys_match(
-                    expected=config.metadatas_by_part_number,
-                    actual=result.metadatas_by_part_number,
-                )
+                result = get_url_response.results_by_artifact_id[artifact.id.value]
 
                 for part_number, metadata in result.metadatas_by_part_number.items():
                     start_index = part_number * artifact.part_size_threshold
                     part_content = content_view[
                         start_index : start_index + artifact.part_size_threshold
                     ]
 
                     futures.append(
                         executor.submit(
-                            ArtifactManager._upload_content,
+                            self._write_content,
                             content=part_content,
-                            url=metadata.upload_signed_url,
+                            url=metadata.signed_url,
                         )
                     )
 
             # TODO(adrian@preemo.io, 04/15/2023): add exception handling
             done, not_done = concurrent.futures.wait(
                 futures, return_when=concurrent.futures.ALL_COMPLETED
             )
@@ -199,70 +245,64 @@
                     for artifact, content in artifacts_and_contents
                 }
             )
         )
 
         return [artifact.id for artifact in artifacts]
 
-    def get_artifact(self, artifact_id: ArtifactId) -> bytes:
-        contents = self.get_artifacts([artifact_id])
+    def get_artifact(self, *, artifact_id: ArtifactId) -> bytes:
+        contents = self.get_artifacts(artifact_ids=[artifact_id])
         if len(contents) != 1:
             raise Exception("expected exactly one artifact to be retrieved")
 
         return contents[0]
 
-    def get_artifacts(self, artifact_ids: List[ArtifactId]) -> List[bytes]:
+    def get_artifacts(self, *, artifact_ids: List[ArtifactId]) -> List[bytes]:
         get_artifact_response = self._messaging_client.batch_get_artifact(
             BatchGetArtifactRequest(
                 configs_by_artifact_id={
                     artifact_id.value: GetArtifactConfig()
                     for artifact_id in artifact_ids
                 }
             )
         )
 
         configs_by_artifact_id_value = {
-            artifact_id_value: GetArtifactPartConfig(
+            artifact_id_value: GetArtifactDownloadUrlConfig(
                 metadatas_by_part_number={
-                    part_number: GetArtifactPartConfigMetadata()
+                    part_number: GetArtifactDownloadUrlConfigMetadata()
                     for part_number in range(result.part_count)
                 }
             )
             for artifact_id_value, result in get_artifact_response.results_by_artifact_id.items()
         }
-        get_artifact_part_response = self._messaging_client.batch_get_artifact_part(
-            BatchGetArtifactPartRequest(
+        get_url_response = self._messaging_client.batch_get_artifact_download_url(
+            BatchGetArtifactDownloadUrlRequest(
                 configs_by_artifact_id=configs_by_artifact_id_value
             )
         )
 
         with concurrent.futures.ThreadPoolExecutor(
-            max_workers=self._max_download_threads
+            max_workers=EnvManager.max_download_threads
         ) as executor:
             futures_by_artifact_id_and_part_number: Dict[
                 ArtifactId, Dict[int, concurrent.futures.Future]
             ] = {}
             for (
                 artifact_id_value,
                 artifact_part_result,
-            ) in get_artifact_part_response.results_by_artifact_id.items():
-                config = configs_by_artifact_id_value[artifact_id_value]
-                ensure_keys_match(
-                    expected=config.metadatas_by_part_number,
-                    actual=artifact_part_result.metadatas_by_part_number,
-                )
-
+            ) in get_url_response.results_by_artifact_id.items():
                 futures_by_part_number: Dict[int, concurrent.futures.Future] = {}
                 for (
                     part_number,
                     metadata,
                 ) in artifact_part_result.metadatas_by_part_number.items():
                     futures_by_part_number[part_number] = executor.submit(
-                        ArtifactManager._download_content,
-                        url=metadata.download_signed_url,
+                        self._read_content,
+                        url=metadata.signed_url,
                     )
 
                 futures_by_artifact_id_and_part_number[
                     ArtifactId(value=artifact_id_value)
                 ] = futures_by_part_number
 
             futures = [
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_function_registry.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_function_registry.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_messaging_client.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_messaging_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 from typing import Protocol, runtime_checkable
 
 import grpc
 
 from preemo import __version__
-from preemo.gen.endpoints.batch_create_artifact_part_pb2 import (
-    BatchCreateArtifactPartRequest,
-    BatchCreateArtifactPartResponse,
+from preemo.gen.endpoints.batch_allocate_artifact_part_pb2 import (
+    BatchAllocateArtifactPartRequest,
+    BatchAllocateArtifactPartResponse,
 )
 from preemo.gen.endpoints.batch_create_artifact_pb2 import (
     BatchCreateArtifactRequest,
     BatchCreateArtifactResponse,
 )
 from preemo.gen.endpoints.batch_execute_function_pb2 import (
     BatchExecuteFunctionRequest,
     BatchExecuteFunctionResponse,
 )
 from preemo.gen.endpoints.batch_finalize_artifact_pb2 import (
     BatchFinalizeArtifactRequest,
     BatchFinalizeArtifactResponse,
 )
-from preemo.gen.endpoints.batch_get_artifact_part_pb2 import (
-    BatchGetArtifactPartRequest,
-    BatchGetArtifactPartResponse,
+from preemo.gen.endpoints.batch_get_artifact_download_url_pb2 import (
+    BatchGetArtifactDownloadUrlRequest,
+    BatchGetArtifactDownloadUrlResponse,
 )
 from preemo.gen.endpoints.batch_get_artifact_pb2 import (
     BatchGetArtifactRequest,
     BatchGetArtifactResponse,
 )
+from preemo.gen.endpoints.batch_get_artifact_upload_url_pb2 import (
+    BatchGetArtifactUploadUrlRequest,
+    BatchGetArtifactUploadUrlResponse,
+)
 from preemo.gen.endpoints.check_function_pb2 import (
     CheckFunctionRequest,
     CheckFunctionResponse,
 )
 from preemo.gen.endpoints.header_pb2 import HeaderRequest, HeaderResponse
 from preemo.gen.endpoints.register_function_pb2 import (
     RegisterFunctionRequest,
     RegisterFunctionResponse,
 )
 from preemo.gen.endpoints.sdk_server_ready_pb2 import (
-    SDKServerReadyRequest,
-    SDKServerReadyResponse,
+    SdkServerReadyRequest,
+    SdkServerReadyResponse,
 )
 from preemo.gen.services.worker_pb2_grpc import WorkerServiceStub
 from preemo.worker._validation import ensure_keys_match
 
 
 @runtime_checkable
 class IMessagingClient(Protocol):
+    def batch_allocate_artifact_part(
+        self, request: BatchAllocateArtifactPartRequest
+    ) -> BatchAllocateArtifactPartResponse:
+        pass
+
     def batch_create_artifact(
         self, request: BatchCreateArtifactRequest
     ) -> BatchCreateArtifactResponse:
         pass
 
-    def batch_create_artifact_part(
-        self, request: BatchCreateArtifactPartRequest
-    ) -> BatchCreateArtifactPartResponse:
-        pass
-
     def batch_execute_function(
         self, request: BatchExecuteFunctionRequest
     ) -> BatchExecuteFunctionResponse:
         pass
 
     def batch_finalize_artifact(
         self, request: BatchFinalizeArtifactRequest
@@ -67,44 +71,67 @@
         pass
 
     def batch_get_artifact(
         self, request: BatchGetArtifactRequest
     ) -> BatchGetArtifactResponse:
         pass
 
-    def batch_get_artifact_part(
-        self, request: BatchGetArtifactPartRequest
-    ) -> BatchGetArtifactPartResponse:
+    def batch_get_artifact_download_url(
+        self, request: BatchGetArtifactDownloadUrlRequest
+    ) -> BatchGetArtifactDownloadUrlResponse:
+        pass
+
+    def batch_get_artifact_upload_url(
+        self, request: BatchGetArtifactUploadUrlRequest
+    ) -> BatchGetArtifactUploadUrlResponse:
         pass
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         pass
 
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         pass
 
     def sdk_server_ready(
-        self, request: SDKServerReadyRequest
-    ) -> SDKServerReadyResponse:
+        self, request: SdkServerReadyRequest
+    ) -> SdkServerReadyResponse:
         pass
 
 
 class MessagingClient:
     def __init__(self, *, worker_server_url: str) -> None:
         # TODO(adrian@preemo.io, 03/25/2023): investigate whether it makes sense to use secure_channel instead
         self._channel = grpc.insecure_channel(target=worker_server_url)
         self._worker_service = WorkerServiceStub(self._channel)
 
         self._initiate(HeaderRequest(version=__version__))
 
     def _initiate(self, request: HeaderRequest) -> HeaderResponse:
         return self._worker_service.Initiate(request)
 
+    def batch_allocate_artifact_part(
+        self, request: BatchAllocateArtifactPartRequest
+    ) -> BatchAllocateArtifactPartResponse:
+        response = self._worker_service.BatchAllocateArtifactPart(request)
+        ensure_keys_match(
+            expected=request.configs_by_artifact_id,
+            actual=response.results_by_artifact_id,
+        )
+
+        for artifact_id, result in response.results_by_artifact_id.items():
+            config = request.configs_by_artifact_id[artifact_id]
+            ensure_keys_match(
+                expected=config.metadatas_by_part_number,
+                actual=result.metadatas_by_part_number,
+            )
+
+        return response
+
     def batch_create_artifact(
         self, request: BatchCreateArtifactRequest
     ) -> BatchCreateArtifactResponse:
         response = self._worker_service.BatchCreateArtifact(request)
         ensure_keys_match(
             expected=request.configs_by_index, actual=response.results_by_index
         )
@@ -116,38 +143,14 @@
             if not result.HasField("part_size_threshold"):
                 raise Exception(
                     "expected CreateArtifactResult to have part_size_threshold"
                 )
 
         return response
 
-    def batch_create_artifact_part(
-        self, request: BatchCreateArtifactPartRequest
-    ) -> BatchCreateArtifactPartResponse:
-        response = self._worker_service.BatchCreateArtifactPart(request)
-        ensure_keys_match(
-            expected=request.configs_by_artifact_id,
-            actual=response.results_by_artifact_id,
-        )
-
-        for artifact_id, result in response.results_by_artifact_id.items():
-            config = request.configs_by_artifact_id[artifact_id]
-            ensure_keys_match(
-                expected=config.metadatas_by_part_number,
-                actual=result.metadatas_by_part_number,
-            )
-
-            for metadata in result.metadatas_by_part_number.values():
-                if not metadata.HasField("upload_signed_url"):
-                    raise Exception(
-                        "expected CreateArtifactPartResultMetadata to have upload_signed_url"
-                    )
-
-        return response
-
     def batch_execute_function(
         self, request: BatchExecuteFunctionRequest
     ) -> BatchExecuteFunctionResponse:
         response = self._worker_service.BatchExecuteFunction(request)
         ensure_keys_match(
             expected=request.parameters_by_index,
             actual=response.results_by_index,
@@ -185,66 +188,90 @@
                 )
 
             if not result.HasField("total_size"):
                 raise Exception("expected GetArtifactResult to have total_size")
 
         return response
 
-    def batch_get_artifact_part(
-        self, request: BatchGetArtifactPartRequest
-    ) -> BatchGetArtifactPartResponse:
-        response = self._worker_service.BatchGetArtifactPart(request)
+    def batch_get_artifact_download_url(
+        self, request: BatchGetArtifactDownloadUrlRequest
+    ) -> BatchGetArtifactDownloadUrlResponse:
+        response = self._worker_service.BatchGetArtifactDownloadUrl(request)
         ensure_keys_match(
             expected=request.configs_by_artifact_id,
             actual=response.results_by_artifact_id,
         )
 
         for artifact_id, result in response.results_by_artifact_id.items():
             config = request.configs_by_artifact_id[artifact_id]
             ensure_keys_match(
                 expected=config.metadatas_by_part_number,
                 actual=result.metadatas_by_part_number,
             )
 
             for metadata in result.metadatas_by_part_number.values():
-                if not metadata.HasField("download_signed_url"):
+                if not metadata.HasField("signed_url"):
                     raise Exception(
-                        "expected GetArtifactPartResultMetadata to have download_signed_url"
+                        "expected GetArtifactDownloadUrlResultMetadata to have signed_url"
+                    )
+
+        return response
+
+    def batch_get_artifact_upload_url(
+        self, request: BatchGetArtifactUploadUrlRequest
+    ) -> BatchGetArtifactUploadUrlResponse:
+        response = self._worker_service.BatchGetArtifactUploadUrl(request)
+        ensure_keys_match(
+            expected=request.configs_by_artifact_id,
+            actual=response.results_by_artifact_id,
+        )
+
+        for artifact_id, result in response.results_by_artifact_id.items():
+            config = request.configs_by_artifact_id[artifact_id]
+            ensure_keys_match(
+                expected=config.metadatas_by_part_number,
+                actual=result.metadatas_by_part_number,
+            )
+
+            for metadata in result.metadatas_by_part_number.values():
+                if not metadata.HasField("signed_url"):
+                    raise Exception(
+                        "expected GetArtifactUploadUrlResultMetadata to have signed_url"
                     )
 
         return response
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         return self._worker_service.CheckFunction(request)
 
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         return self._worker_service.RegisterFunction(request)
 
     def sdk_server_ready(
-        self, request: SDKServerReadyRequest
-    ) -> SDKServerReadyResponse:
-        return self._worker_service.SDKServerReady(request)
+        self, request: SdkServerReadyRequest
+    ) -> SdkServerReadyResponse:
+        return self._worker_service.SdkServerReady(request)
 
 
 # This class is intended to be used for tests and local development
 class LocalMessagingClient:
+    def batch_allocate_artifact_part(
+        self, request: BatchAllocateArtifactPartRequest
+    ) -> BatchAllocateArtifactPartResponse:
+        print(f"sending batch allocate artifact part request: {request}")
+        return BatchAllocateArtifactPartResponse()
+
     def batch_create_artifact(
         self, request: BatchCreateArtifactRequest
     ) -> BatchCreateArtifactResponse:
         print(f"sending batch create artifact request: {request}")
         return BatchCreateArtifactResponse()
 
-    def batch_create_artifact_part(
-        self, request: BatchCreateArtifactPartRequest
-    ) -> BatchCreateArtifactPartResponse:
-        print(f"sending batch create artifact part request: {request}")
-        return BatchCreateArtifactPartResponse()
-
     def batch_execute_function(
         self, request: BatchExecuteFunctionRequest
     ) -> BatchExecuteFunctionResponse:
         print(f"sending batch execute function request: {request}")
         return BatchExecuteFunctionResponse()
 
     def batch_finalize_artifact(
@@ -255,28 +282,34 @@
 
     def batch_get_artifact(
         self, request: BatchGetArtifactRequest
     ) -> BatchGetArtifactResponse:
         print(f"sending batch get artifact request: {request}")
         return BatchGetArtifactResponse()
 
-    def batch_get_artifact_part(
-        self, request: BatchGetArtifactPartRequest
-    ) -> BatchGetArtifactPartResponse:
-        print(f"sending batch get artifact part request: {request}")
-        return BatchGetArtifactPartResponse()
+    def batch_get_artifact_download_url(
+        self, request: BatchGetArtifactDownloadUrlRequest
+    ) -> BatchGetArtifactDownloadUrlResponse:
+        print(f"sending batch get artifact download url request: {request}")
+        return BatchGetArtifactDownloadUrlResponse()
+
+    def batch_get_artifact_upload_url(
+        self, request: BatchGetArtifactUploadUrlRequest
+    ) -> BatchGetArtifactUploadUrlResponse:
+        print(f"sending batch get artifact upload url request: {request}")
+        return BatchGetArtifactUploadUrlResponse()
 
     def check_function(self, request: CheckFunctionRequest) -> CheckFunctionResponse:
         print(f"sending check function request: {request}")
         return CheckFunctionResponse()
 
     def register_function(
         self, request: RegisterFunctionRequest
     ) -> RegisterFunctionResponse:
         print(f"sending register function request: {request}")
         return RegisterFunctionResponse()
 
     def sdk_server_ready(
-        self, request: SDKServerReadyRequest
-    ) -> SDKServerReadyResponse:
+        self, request: SdkServerReadyRequest
+    ) -> SdkServerReadyResponse:
         print(f"sending sdk server ready request: {request}")
-        return SDKServerReadyResponse()
+        return SdkServerReadyResponse()
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_sdk_server.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_sdk_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import concurrent.futures
 import random
 
 import grpc
 
-from preemo.gen.services.sdk_pb2_grpc import add_SDKServiceServicer_to_server
+from preemo.gen.services.sdk_pb2_grpc import add_SdkServiceServicer_to_server
 from preemo.worker._artifact_manager import IArtifactManager
 from preemo.worker._function_registry import FunctionRegistry
-from preemo.worker._sdk_service import SDKService
+from preemo.worker._sdk_service import SdkService
 
 
-class SDKServer:
+class SdkServer:
     @staticmethod
     def _generate_random_port() -> int:
         return random.randrange(60_000, 61_000)
 
     @staticmethod
     def _bind_server_to_random_port(*, server: grpc.Server, host: str) -> int:
         attempt_count = 0
         while True:
-            port = SDKServer._generate_random_port()
+            port = SdkServer._generate_random_port()
             try:
                 # TODO(adrian@preemo.io, 03/27/2023): investigate whether it makes sense to use add_secure_port instead
                 server.add_insecure_port(f"{host}:{port}")
             except RuntimeError as e:
                 if len(e.args) < 1:
                     raise e
 
@@ -50,23 +50,23 @@
             # This option prevents multiple servers from reusing the same port (see https://groups.google.com/g/grpc-io/c/RB69llv2tC4/m/7E__iL3LAwAJ)
             options=(("grpc.so_reuseport", 0),),
         )
 
         def close() -> None:
             server.stop(grace=10)  # seconds
 
-        add_SDKServiceServicer_to_server(
-            SDKService(
+        add_SdkServiceServicer_to_server(
+            SdkService(
                 artifact_manager=artifact_manager,
                 function_registry=function_registry,
                 terminate_server=close,
             ),
             server,
         )
-        port = SDKServer._bind_server_to_random_port(
+        port = SdkServer._bind_server_to_random_port(
             server=server, host=sdk_server_host
         )
 
         server.start()
         print(f"sdk server has started on port {port}")
 
         self._server = server
```

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_types.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_types.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_validation.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_validation.py`

 * *Files identical despite different names*

### Comparing `preemo_worker_sdk-0.3.0/preemo/worker/_worker_client.py` & `preemo_worker_sdk-0.4.0/preemo/worker/_worker_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from google.protobuf.struct_pb2 import NULL_VALUE
 
 from preemo.gen.endpoints.batch_execute_function_pb2 import BatchExecuteFunctionRequest
 from preemo.gen.endpoints.check_function_pb2 import CheckFunctionRequest
 from preemo.gen.endpoints.register_function_pb2 import RegisterFunctionRequest
 from preemo.gen.models.registered_function_pb2 import RegisteredFunction
 from preemo.gen.models.value_pb2 import Value
-from preemo.worker._artifact_manager import ArtifactId, IArtifactManager
+from preemo.worker._artifact_manager import ArtifactId, ArtifactType, IArtifactManager
 from preemo.worker._function_registry import FunctionRegistry
 from preemo.worker._messaging_client import IMessagingClient
 from preemo.worker._types import assert_never
 
 
 class Result:
     # TODO(adrian@preemo.io, 04/20/2023): need to sort out how this class
@@ -20,15 +20,15 @@
     def __init__(
         self, *, artifact_id: ArtifactId, artifact_manager: IArtifactManager
     ) -> None:
         self._artifact_id = artifact_id
         self._artifact_manager = artifact_manager
 
     def get(self) -> bytes:
-        return self._artifact_manager.get_artifact(self._artifact_id)
+        return self._artifact_manager.get_artifact(artifact_id=self._artifact_id)
 
 
 class Function:
     def __init__(
         self,
         *,
         artifact_manager: IArtifactManager,
@@ -53,15 +53,17 @@
             )
         )
 
     def __call__(self, params: Optional[bytes] = None) -> Optional[Result]:
         if params is None:
             function_parameter = Value(null_value=NULL_VALUE)
         else:
-            artifact_id = self._artifact_manager.create_artifact(params)
+            artifact_id = self._artifact_manager.create_artifact(
+                content=params, type_=ArtifactType.PARAMS
+            )
             function_parameter = Value(artifact_id=artifact_id.value)
 
         response = self._messaging_client.batch_execute_function(
             BatchExecuteFunctionRequest(
                 function_to_execute=RegisteredFunction(
                     name=self.name, namespace=self.namespace
                 ),
@@ -129,15 +131,17 @@
         else:
             if count is not None:
                 raise ValueError("params and count must not both be specified")
 
             if len(params) == 0:
                 return []
 
-            artifact_ids = self._artifact_manager.create_artifacts(params)
+            artifact_ids = self._artifact_manager.create_artifacts(
+                contents=params, type_=ArtifactType.PARAMS
+            )
             function_parameters_by_index = {
                 i: Value(artifact_id=artifact_id.value)
                 for i, artifact_id in enumerate(artifact_ids)
             }
 
         response = self._messaging_client.batch_execute_function(
             BatchExecuteFunctionRequest(
```

### Comparing `preemo_worker_sdk-0.3.0/pyproject.toml` & `preemo_worker_sdk-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preemo_worker_sdk"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 license = "MIT"
 authors = [
   "Forrest Moret <forrest@preemo.io>",
   "Adrian Miguel <adrian@preemo.io>",
 ]
 readme = "README.md"
```

### Comparing `preemo_worker_sdk-0.3.0/PKG-INFO` & `preemo_worker_sdk-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preemo-worker-sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Home-page: https://www.preemo.io/
 License: MIT
 Author: Forrest Moret
 Author-email: forrest@preemo.io
 Requires-Python: >=3.8.13,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

