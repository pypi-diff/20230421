# Comparing `tmp/cognite-seismic-sdk-0.3.8.tar.gz` & `tmp/cognite-seismic-sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite-seismic-sdk-0.3.8.tar", max compression
+gzip compressed data, was "cognite-seismic-sdk-0.3.9.tar", max compression
```

## Comparing `cognite-seismic-sdk-0.3.8.tar` & `cognite-seismic-sdk-0.3.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0        0 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/__init__.py
--rw-r--r--   0        0        0      714 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/__init__.py
--rw-r--r--   0        0        0        0 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/__init__.py
--rw-r--r--   0        0        0      678 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/api.py
--rw-r--r--   0        0        0    15012 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/file.py
--rw-r--r--   0        0        0     1006 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/grpc_helpers.py
--rw-r--r--   0        0        0     3330 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/job.py
--rw-r--r--   0        0        0     5286 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/partition.py
--rw-r--r--   0        0        0    13650 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/seismics.py
--rw-r--r--   0        0        0     8738 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/seismicstores.py
--rw-r--r--   0        0        0    21111 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/survey.py
--rw-r--r--   0        0        0    17414 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/traces.py
--rw-r--r--   0        0        0     3551 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api/utility.py
--rw-r--r--   0        0        0     9652 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_api_client.py
--rw-r--r--   0        0        0     4056 2022-09-05 10:10:22.290034 cognite-seismic-sdk-0.3.8/cognite/seismic/_token.py
--rw-r--r--   0        0        0      369 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/_version.py
--rw-r--r--   0        0        0      452 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/__init__.py
--rw-r--r--   0        0        0    41643 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/api_types.py
--rw-r--r--   0        0        0     4592 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/errors.py
--rw-r--r--   0        0        0    35819 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/extents.py
--rw-r--r--   0        0        0     2566 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/geometry.py
--rw-r--r--   0        0        0     5472 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/searchspec.py
--rw-r--r--   0        0        0    10169 2022-09-05 10:10:22.294034 cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/trace_data.py
--rw-r--r--   0        0        0        0 2022-09-05 10:12:47.849674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/__init__.py
--rw-r--r--   0        0        0     1616 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_job_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_job_pb2_grpc.py
--rw-r--r--   0        0        0    19902 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_messages_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_messages_pb2_grpc.py
--rw-r--r--   0        0        0     2481 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_pb2.py
--rw-r--r--   0        0        0    25665 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_pb2_grpc.py
--rw-r--r--   0        0        0     1409 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/persisted_trace_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/persisted_trace_pb2_grpc.py
--rw-r--r--   0        0        0    31651 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_messages_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_messages_pb2_grpc.py
--rw-r--r--   0        0        0     3911 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_pb2.py
--rw-r--r--   0        0        0    45897 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_pb2_grpc.py
--rw-r--r--   0        0        0    20971 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/types_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:47.833674 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/types_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-09-05 10:12:48.093673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/__init__.py
--rw-r--r--   0        0        0    32458 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_datatypes_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_datatypes_pb2_grpc.py
--rw-r--r--   0        0        0    40803 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_messages_pb2.py
--rw-r--r--   0        0        0      159 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_messages_pb2_grpc.py
--rw-r--r--   0        0        0     5137 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_pb2.py
--rw-r--r--   0        0        0    58386 2022-09-05 10:12:48.081673 cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_pb2_grpc.py
--rw-r--r--   0        0        0     2543 2022-09-05 10:10:22.298034 cognite-seismic-sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 cognite-seismic-sdk-0.3.8/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 cognite-seismic-sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/__init__.py
+-rw-r--r--   0        0        0      714 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/__init__.py
+-rw-r--r--   0        0        0      678 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/api.py
+-rw-r--r--   0        0        0    15012 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/file.py
+-rw-r--r--   0        0        0     1006 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/grpc_helpers.py
+-rw-r--r--   0        0        0     3604 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/job.py
+-rw-r--r--   0        0        0     5286 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/partition.py
+-rw-r--r--   0        0        0    13650 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/seismics.py
+-rw-r--r--   0        0        0     8738 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/seismicstores.py
+-rw-r--r--   0        0        0    21111 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/survey.py
+-rw-r--r--   0        0        0    17414 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/traces.py
+-rw-r--r--   0        0        0     3551 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api/utility.py
+-rw-r--r--   0        0        0     9652 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_api_client.py
+-rw-r--r--   0        0        0     4056 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_token.py
+-rw-r--r--   0        0        0      369 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/_version.py
+-rw-r--r--   0        0        0      452 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/__init__.py
+-rw-r--r--   0        0        0    41643 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/api_types.py
+-rw-r--r--   0        0        0     4592 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/errors.py
+-rw-r--r--   0        0        0    35819 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/extents.py
+-rw-r--r--   0        0        0     2566 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/geometry.py
+-rw-r--r--   0        0        0     5472 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/searchspec.py
+-rw-r--r--   0        0        0    10169 2022-09-08 15:54:20.593300 cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/trace_data.py
+-rw-r--r--   0        0        0        0 2022-09-08 15:57:09.537934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/__init__.py
+-rw-r--r--   0        0        0     1616 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_job_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_job_pb2_grpc.py
+-rw-r--r--   0        0        0    19902 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_messages_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_messages_pb2_grpc.py
+-rw-r--r--   0        0        0     2481 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_pb2.py
+-rw-r--r--   0        0        0    25665 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1409 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/persisted_trace_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/persisted_trace_pb2_grpc.py
+-rw-r--r--   0        0        0    31651 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_messages_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_messages_pb2_grpc.py
+-rw-r--r--   0        0        0     3911 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_pb2.py
+-rw-r--r--   0        0        0    45897 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20971 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/types_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.513934 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/types_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-09-08 15:57:09.861935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/__init__.py
+-rw-r--r--   0        0        0    32458 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_datatypes_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_datatypes_pb2_grpc.py
+-rw-r--r--   0        0        0    40803 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_messages_pb2.py
+-rw-r--r--   0        0        0      159 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_messages_pb2_grpc.py
+-rw-r--r--   0        0        0     5137 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_pb2.py
+-rw-r--r--   0        0        0    58386 2022-09-08 15:57:09.841935 cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2543 2022-09-08 15:54:20.601300 cognite-seismic-sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 cognite-seismic-sdk-0.3.9/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 cognite-seismic-sdk-0.3.9/PKG-INFO
```

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/__init__.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/api.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/api.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/file.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/file.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/grpc_helpers.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/grpc_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/job.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/job.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,24 +52,31 @@
         def proto_timestamp(datetime: datetime.datetime):
             timestamp = datetime.timestamp()
             seconds = int(timestamp)
             nanos = int(timestamp % 1 * 1e9)
             proto_timestamp = Timestamp(seconds=seconds, nanos=nanos)
             return proto_timestamp
 
+        if sum([job_id is not None, file_id is not None, file_uuid is not None]) > 1:
+            raise ValueError("Only one of job_id, file_id or file_uuid can be specified.")
+
         req = SearchJobStatusRequest(
-            job_id=job_id or "",
-            file_id=file_id or 0,
-            file_uuid=file_uuid or "",
             status=JobStatusProto.ValueType(status.value),
             target_storage_tier_name=StringValue(value=target_storage_tier_name)
             if target_storage_tier_name is not None
             else None,
             started_before=proto_timestamp(started_before) if started_before is not None else None,
             started_after=proto_timestamp(started_after) if started_after is not None else None,
             updated_before=proto_timestamp(updated_before) if updated_before is not None else None,
             updated_after=proto_timestamp(updated_after) if updated_after is not None else None,
         )
 
+        if job_id is not None:
+            req.job_id = job_id
+        if file_id is not None:
+            req.file_id = file_id
+        if file_uuid is not None:
+            req.file_uuid = file_uuid
+
         results = self.query.SearchJobStatus(req)
         for s in results:
             yield JobStatus._from_proto(s)
```

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/partition.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/partition.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/seismics.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/seismics.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/seismicstores.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/seismicstores.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/survey.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/survey.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/traces.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/traces.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api/utility.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api/utility.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_api_client.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/_token.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/_token.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/api_types.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/api_types.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/errors.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/errors.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/extents.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/extents.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/geometry.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/geometry.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/searchspec.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/searchspec.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/data_classes/trace_data.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/data_classes/trace_data.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_job_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_job_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_messages_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/ingest_service_pb2_grpc.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/ingest_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/persisted_trace_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/persisted_trace_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_messages_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/query_service_pb2_grpc.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/types_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/types_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_datatypes_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_datatypes_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_messages_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_pb2.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/cognite/seismic/protos/v1/seismic_service_pb2_grpc.py` & `cognite-seismic-sdk-0.3.9/cognite/seismic/protos/v1/seismic_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognite-seismic-sdk-0.3.8/pyproject.toml` & `cognite-seismic-sdk-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-seismic-sdk"
-version = "0.3.8"
+version = "0.3.9"
 description = ""
 authors = ["cognite <support@cognite.com>"]
 
 packages = [
     { include="cognite" },
 ]
 include = ["cognite/seismic/protos/**/*.py"]
```

### Comparing `cognite-seismic-sdk-0.3.8/setup.py` & `cognite-seismic-sdk-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata'],
  'tox_deps': ['msal>=1.15.0,<2.0.0', 'shapely>=1.7,<2.0']}
 
 setup_kwargs = {
     'name': 'cognite-seismic-sdk',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '',
     'long_description': 'None',
     'author': 'cognite',
     'author_email': 'support@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cognite-seismic-sdk-0.3.8/PKG-INFO` & `cognite-seismic-sdk-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-seismic-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

