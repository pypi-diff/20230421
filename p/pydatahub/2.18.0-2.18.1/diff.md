# Comparing `tmp/pydatahub-2.18.0.tar.gz` & `tmp/pydatahub-2.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatahub-2.18.0.tar", last modified: Mon Mar 13 07:07:22 2023, max compression
+gzip compressed data, was "pydatahub-2.18.1.tar", last modified: Fri Apr 21 01:59:59 2023, max compression
```

## Comparing `pydatahub-2.18.0.tar` & `pydatahub-2.18.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.298429 pydatahub-2.18.0/
--rw-r--r--   0 lewei      (502) staff       (20)    11357 2022-12-08 08:16:24.000000 pydatahub-2.18.0/LICENSE
--rw-r--r--   0 lewei      (502) staff       (20)       83 2022-12-08 08:16:24.000000 pydatahub-2.18.0/MANIFEST.in
--rw-r--r--   0 lewei      (502) staff       (20)     7750 2023-03-13 07:07:22.298094 pydatahub-2.18.0/PKG-INFO
--rw-r--r--   0 lewei      (502) staff       (20)     6921 2022-12-08 08:16:24.000000 pydatahub-2.18.0/README.md
--rw-r--r--   0 lewei      (502) staff       (20)     7432 2022-12-08 08:16:24.000000 pydatahub-2.18.0/README.rst
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.276521 pydatahub-2.18.0/datahub/
--rw-r--r--   0 lewei      (502) staff       (20)     1103 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/__init__.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.278478 pydatahub-2.18.0/datahub/auth/
--rw-r--r--   0 lewei      (502) staff       (20)      970 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/auth/__init__.py
--rw-r--r--   0 lewei      (502) staff       (20)     4386 2023-01-09 08:50:32.000000 pydatahub-2.18.0/datahub/auth/aliyun_account.py
--rw-r--r--   0 lewei      (502) staff       (20)     1696 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/auth/core.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.282698 pydatahub-2.18.0/datahub/batch/
--rw-r--r--   0 lewei      (502) staff       (20)        0 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/__init__.py
--rw-r--r--   0 lewei      (502) staff       (20)     2900 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/batch_binary_record.py
--rw-r--r--   0 lewei      (502) staff       (20)     2851 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/batch_header.py
--rw-r--r--   0 lewei      (502) staff       (20)     5574 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/batch_serializer.py
--rw-r--r--   0 lewei      (502) staff       (20)    10234 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/binary_record.py
--rw-r--r--   0 lewei      (502) staff       (20)     1810 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/record_header.py
--rw-r--r--   0 lewei      (502) staff       (20)     4087 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/schema_registry_client.py
--rw-r--r--   0 lewei      (502) staff       (20)     1812 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/batch/utils.py
--rw-r--r--   0 lewei      (502) staff       (20)    42000 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/core.py
--rw-r--r--   0 lewei      (502) staff       (20)     7128 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/exceptions.py
--rw-r--r--   0 lewei      (502) staff       (20)    40655 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/implement.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.291056 pydatahub-2.18.0/datahub/models/
--rw-r--r--   0 lewei      (502) staff       (20)     1538 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/models/__init__.py
--rw-r--r--   0 lewei      (502) staff       (20)     3758 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/models/compress.py
--rw-r--r--   0 lewei      (502) staff       (20)    32629 2023-02-22 03:41:01.000000 pydatahub-2.18.0/datahub/models/connector.py
--rw-r--r--   0 lewei      (502) staff       (20)     1127 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/models/cursor.py
--rw-r--r--   0 lewei      (502) staff       (20)    27449 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/models/params.py
--rw-r--r--   0 lewei      (502) staff       (20)    15159 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/models/record.py
--rw-r--r--   0 lewei      (502) staff       (20)    41384 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/models/results.py
--rw-r--r--   0 lewei      (502) staff       (20)     6809 2022-07-08 09:55:09.000000 pydatahub-2.18.0/datahub/models/schema.py
--rw-r--r--   0 lewei      (502) staff       (20)     7157 2022-07-08 09:55:09.000000 pydatahub-2.18.0/datahub/models/shard.py
--rw-r--r--   0 lewei      (502) staff       (20)     8320 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/models/subscription.py
--rw-r--r--   0 lewei      (502) staff       (20)    10122 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/models/types.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.292660 pydatahub-2.18.0/datahub/proto/
--rw-r--r--   0 lewei      (502) staff       (20)      873 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/proto/__init__.py
--rw-r--r--   0 lewei      (502) staff       (20)     2709 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/proto/datahub_record_proto_pb.py
--rw-r--r--   0 lewei      (502) staff       (20)    11775 2023-03-11 02:15:41.000000 pydatahub-2.18.0/datahub/rest.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.295538 pydatahub-2.18.0/datahub/utils/
--rw-r--r--   0 lewei      (502) staff       (20)      931 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/utils/__init__.py
--rw-r--r--   0 lewei      (502) staff       (20)     1870 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/utils/codec.py
--rw-r--r--   0 lewei      (502) staff       (20)     1823 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/utils/constants.py
--rw-r--r--   0 lewei      (502) staff       (20)     2118 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/utils/converters.py
--rw-r--r--   0 lewei      (502) staff       (20)     3787 2022-12-08 08:16:24.000000 pydatahub-2.18.0/datahub/utils/validator.py
--rw-r--r--   0 lewei      (502) staff       (20)      909 2023-03-13 07:06:40.000000 pydatahub-2.18.0/datahub/version.py
-drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-03-13 07:07:22.297568 pydatahub-2.18.0/pydatahub.egg-info/
--rw-r--r--   0 lewei      (502) staff       (20)     7750 2023-03-13 07:07:22.000000 pydatahub-2.18.0/pydatahub.egg-info/PKG-INFO
--rw-r--r--   0 lewei      (502) staff       (20)     1158 2023-03-13 07:07:22.000000 pydatahub-2.18.0/pydatahub.egg-info/SOURCES.txt
--rw-r--r--   0 lewei      (502) staff       (20)        1 2023-03-13 07:07:22.000000 pydatahub-2.18.0/pydatahub.egg-info/dependency_links.txt
--rw-r--r--   0 lewei      (502) staff       (20)      142 2023-03-13 07:07:22.000000 pydatahub-2.18.0/pydatahub.egg-info/requires.txt
--rw-r--r--   0 lewei      (502) staff       (20)        8 2023-03-13 07:07:22.000000 pydatahub-2.18.0/pydatahub.egg-info/top_level.txt
--rw-r--r--   0 lewei      (502) staff       (20)      139 2022-12-08 08:16:24.000000 pydatahub-2.18.0/requirements.txt
--rw-r--r--   0 lewei      (502) staff       (20)       38 2023-03-13 07:07:22.298550 pydatahub-2.18.0/setup.cfg
--rw-r--r--   0 lewei      (502) staff       (20)     2082 2022-12-08 08:16:24.000000 pydatahub-2.18.0/setup.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.253542 pydatahub-2.18.1/
+-rw-r--r--   0 lewei      (502) staff       (20)    11357 2022-12-08 08:16:24.000000 pydatahub-2.18.1/LICENSE
+-rw-r--r--   0 lewei      (502) staff       (20)       83 2022-12-08 08:16:24.000000 pydatahub-2.18.1/MANIFEST.in
+-rw-r--r--   0 lewei      (502) staff       (20)     7750 2023-04-21 01:59:59.252341 pydatahub-2.18.1/PKG-INFO
+-rw-r--r--   0 lewei      (502) staff       (20)     6921 2022-12-08 08:16:24.000000 pydatahub-2.18.1/README.md
+-rw-r--r--   0 lewei      (502) staff       (20)     7432 2022-12-08 08:16:24.000000 pydatahub-2.18.1/README.rst
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.135071 pydatahub-2.18.1/datahub/
+-rw-r--r--   0 lewei      (502) staff       (20)     1103 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/__init__.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.137790 pydatahub-2.18.1/datahub/auth/
+-rw-r--r--   0 lewei      (502) staff       (20)      970 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/auth/__init__.py
+-rw-r--r--   0 lewei      (502) staff       (20)     4386 2023-01-09 08:50:32.000000 pydatahub-2.18.1/datahub/auth/aliyun_account.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1696 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/auth/core.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.157642 pydatahub-2.18.1/datahub/batch/
+-rw-r--r--   0 lewei      (502) staff       (20)        0 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/__init__.py
+-rw-r--r--   0 lewei      (502) staff       (20)     2900 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/batch_binary_record.py
+-rw-r--r--   0 lewei      (502) staff       (20)     2851 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/batch_header.py
+-rw-r--r--   0 lewei      (502) staff       (20)     5574 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/batch_serializer.py
+-rw-r--r--   0 lewei      (502) staff       (20)    10234 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/binary_record.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1810 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/record_header.py
+-rw-r--r--   0 lewei      (502) staff       (20)     4087 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/schema_registry_client.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1812 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/batch/utils.py
+-rw-r--r--   0 lewei      (502) staff       (20)    42000 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/core.py
+-rw-r--r--   0 lewei      (502) staff       (20)     7128 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/exceptions.py
+-rw-r--r--   0 lewei      (502) staff       (20)    40655 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/implement.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.177278 pydatahub-2.18.1/datahub/models/
+-rw-r--r--   0 lewei      (502) staff       (20)     1538 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/models/__init__.py
+-rw-r--r--   0 lewei      (502) staff       (20)     3758 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/models/compress.py
+-rw-r--r--   0 lewei      (502) staff       (20)    32629 2023-02-22 03:41:01.000000 pydatahub-2.18.1/datahub/models/connector.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1127 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/models/cursor.py
+-rw-r--r--   0 lewei      (502) staff       (20)    27449 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/models/params.py
+-rw-r--r--   0 lewei      (502) staff       (20)    15159 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/models/record.py
+-rw-r--r--   0 lewei      (502) staff       (20)    41384 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/models/results.py
+-rw-r--r--   0 lewei      (502) staff       (20)     7338 2023-04-20 13:00:22.000000 pydatahub-2.18.1/datahub/models/schema.py
+-rw-r--r--   0 lewei      (502) staff       (20)     7157 2022-07-08 09:55:09.000000 pydatahub-2.18.1/datahub/models/shard.py
+-rw-r--r--   0 lewei      (502) staff       (20)     8320 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/models/subscription.py
+-rw-r--r--   0 lewei      (502) staff       (20)    10122 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/models/types.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.180289 pydatahub-2.18.1/datahub/proto/
+-rw-r--r--   0 lewei      (502) staff       (20)      873 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/proto/__init__.py
+-rw-r--r--   0 lewei      (502) staff       (20)     2709 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/proto/datahub_record_proto_pb.py
+-rw-r--r--   0 lewei      (502) staff       (20)    11775 2023-04-20 13:03:04.000000 pydatahub-2.18.1/datahub/rest.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.185833 pydatahub-2.18.1/datahub/utils/
+-rw-r--r--   0 lewei      (502) staff       (20)      931 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/utils/__init__.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1870 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/utils/codec.py
+-rw-r--r--   0 lewei      (502) staff       (20)     1823 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/utils/constants.py
+-rw-r--r--   0 lewei      (502) staff       (20)     2118 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/utils/converters.py
+-rw-r--r--   0 lewei      (502) staff       (20)     3787 2022-12-08 08:16:24.000000 pydatahub-2.18.1/datahub/utils/validator.py
+-rw-r--r--   0 lewei      (502) staff       (20)      909 2023-04-21 01:59:21.000000 pydatahub-2.18.1/datahub/version.py
+drwxr-xr-x   0 lewei      (502) staff       (20)        0 2023-04-21 01:59:59.225297 pydatahub-2.18.1/pydatahub.egg-info/
+-rw-r--r--   0 lewei      (502) staff       (20)     7750 2023-04-21 01:59:58.000000 pydatahub-2.18.1/pydatahub.egg-info/PKG-INFO
+-rw-r--r--   0 lewei      (502) staff       (20)     1158 2023-04-21 01:59:59.000000 pydatahub-2.18.1/pydatahub.egg-info/SOURCES.txt
+-rw-r--r--   0 lewei      (502) staff       (20)        1 2023-04-21 01:59:58.000000 pydatahub-2.18.1/pydatahub.egg-info/dependency_links.txt
+-rw-r--r--   0 lewei      (502) staff       (20)      142 2023-04-21 01:59:58.000000 pydatahub-2.18.1/pydatahub.egg-info/requires.txt
+-rw-r--r--   0 lewei      (502) staff       (20)        8 2023-04-21 01:59:58.000000 pydatahub-2.18.1/pydatahub.egg-info/top_level.txt
+-rw-r--r--   0 lewei      (502) staff       (20)      139 2022-12-08 08:16:24.000000 pydatahub-2.18.1/requirements.txt
+-rw-r--r--   0 lewei      (502) staff       (20)       38 2023-04-21 01:59:59.253994 pydatahub-2.18.1/setup.cfg
+-rw-r--r--   0 lewei      (502) staff       (20)     2082 2022-12-08 08:16:24.000000 pydatahub-2.18.1/setup.py
```

### Comparing `pydatahub-2.18.0/LICENSE` & `pydatahub-2.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/PKG-INFO` & `pydatahub-2.18.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatahub
-Version: 2.18.0
+Version: 2.18.1
 Summary: Datahub Python SDK
 Home-page: https://github.com/aliyun/aliyun-datahub-sdk-python
 Author: andy.xs
 Author-email: helloworld.xs@foxmail.com
 License: Apache License 2.0
 Keywords: pydatahub,python,aliyun,datahub,sdk
 Platform: UNKNOWN
```

### Comparing `pydatahub-2.18.0/README.md` & `pydatahub-2.18.1/README.md`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/README.rst` & `pydatahub-2.18.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/__init__.py` & `pydatahub-2.18.1/datahub/__init__.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/auth/__init__.py` & `pydatahub-2.18.1/datahub/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/auth/aliyun_account.py` & `pydatahub-2.18.1/datahub/auth/aliyun_account.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/auth/core.py` & `pydatahub-2.18.1/datahub/auth/core.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/batch_binary_record.py` & `pydatahub-2.18.1/datahub/batch/batch_binary_record.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/batch_header.py` & `pydatahub-2.18.1/datahub/batch/batch_header.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/batch_serializer.py` & `pydatahub-2.18.1/datahub/batch/batch_serializer.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/binary_record.py` & `pydatahub-2.18.1/datahub/batch/binary_record.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/record_header.py` & `pydatahub-2.18.1/datahub/batch/record_header.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/schema_registry_client.py` & `pydatahub-2.18.1/datahub/batch/schema_registry_client.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/batch/utils.py` & `pydatahub-2.18.1/datahub/batch/utils.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/core.py` & `pydatahub-2.18.1/datahub/core.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/exceptions.py` & `pydatahub-2.18.1/datahub/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/implement.py` & `pydatahub-2.18.1/datahub/implement.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/__init__.py` & `pydatahub-2.18.1/datahub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/compress.py` & `pydatahub-2.18.1/datahub/models/compress.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/connector.py` & `pydatahub-2.18.1/datahub/models/connector.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/cursor.py` & `pydatahub-2.18.1/datahub/models/cursor.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/params.py` & `pydatahub-2.18.1/datahub/models/params.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/record.py` & `pydatahub-2.18.1/datahub/models/record.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/results.py` & `pydatahub-2.18.1/datahub/models/results.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/schema.py` & `pydatahub-2.18.1/datahub/models/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,23 +51,26 @@
     """
     Field
 
     Members:
         name (:class:`str`): field name
 
         type (:class:`str`): field type
+
+        comment (:class:`str`): field comment
     """
 
-    __slots__ = ('_name', '_type', '_allow_null')
+    __slots__ = ('_name', '_type', '_comment', '_allow_null')
 
-    def __init__(self, name, field_type, allow_null=True):
+    def __init__(self, name, field_type, comment="", allow_null=True):
         if not check_type(field_type, FieldType):
             raise InvalidParameterException(ErrorMessage.INVALID_TYPE % ('field_type', FieldType.__name__))
         self._name = utils.to_str(name)
         self._type = field_type
+        self._comment = comment
         self._allow_null = allow_null
 
     @property
     def name(self):
         return self._name
 
     @name.setter
@@ -86,30 +89,40 @@
     def allow_null(self):
         return self._allow_null
 
     @allow_null.setter
     def allow_null(self, value):
         self._allow_null = value
 
+    @property
+    def comment(self):
+        return self._comment
+
+    @comment.setter
+    def comment(self, value):
+        self._comment = value
+
     def to_json(self):
         data = {
             "name": self._name,
-            "type": self._type.value
+            "type": self._type.value,
+            "comment": self._comment
         }
         if not self._allow_null:
             data["notnull"] = not self._allow_null
         return data
 
     @classmethod
     def from_json(cls, field_json):
         allow_null = not field_json['notnull'] if 'notnull' in field_json else True
-        return cls(field_json['name'], FieldType(field_json['type'].lower()), allow_null)
+        comment = field_json['comment'] if 'comment' in field_json else ""
+        return cls(field_json['name'], FieldType(field_json['type'].lower()), comment, allow_null)
 
     def __repr__(self):
-        return '<field {0}, type {1}, allow_null {2}>'.format(self._name, self._type.name.lower(), self._allow_null)
+        return '<field {0}, type {1}, comment {2}, allow_null {3}>'.format(self._name, self._type.name.lower(), self._comment, self._allow_null)
 
 
 class RecordSchema(object):
     """
     Record schema class, Tuple type Topic will use it.
 
     Members:
@@ -171,21 +184,22 @@
             'fields': [field.to_json() for field in self._field_list]
         }
 
     def to_json_string(self):
         return json.dumps(self.to_json())
 
     @classmethod
-    def from_lists(cls, names, types, allow_nulls=None):
-        if len(names) != len(types) or (allow_nulls and len(allow_nulls) != len(names)):
+    def from_lists(cls, names, types, comments=None, allow_nulls=None):
+        if len(names) != len(types) or (comments and len(comments) != len(names)) or (allow_nulls and len(allow_nulls) != len(names)):
             raise InvalidParameterException('Length of lists are not equal')
         field_list = []
         for index in range(0, len(names)):
             allow_null = allow_nulls[index] if allow_nulls else True
-            field_list.append(Field(names[index], types[index], allow_null))
+            comment = comments[index] if comments else ""
+            field_list.append(Field(names[index], types[index], comment, allow_null))
         return cls(field_list=field_list)
 
     @classmethod
     def from_json(cls, fields_json):
         field_list = []
         for field in fields_json['fields']:
             field_list.append(Field.from_json(field))
```

### Comparing `pydatahub-2.18.0/datahub/models/shard.py` & `pydatahub-2.18.1/datahub/models/shard.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/subscription.py` & `pydatahub-2.18.1/datahub/models/subscription.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/models/types.py` & `pydatahub-2.18.1/datahub/models/types.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/proto/__init__.py` & `pydatahub-2.18.1/datahub/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/proto/datahub_record_proto_pb.py` & `pydatahub-2.18.1/datahub/proto/datahub_record_proto_pb.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/rest.py` & `pydatahub-2.18.1/datahub/rest.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/utils/__init__.py` & `pydatahub-2.18.1/datahub/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/utils/codec.py` & `pydatahub-2.18.1/datahub/utils/codec.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/utils/constants.py` & `pydatahub-2.18.1/datahub/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/utils/converters.py` & `pydatahub-2.18.1/datahub/utils/converters.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/utils/validator.py` & `pydatahub-2.18.1/datahub/utils/validator.py`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/datahub/version.py` & `pydatahub-2.18.1/datahub/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """ version
 """
 
-__version__ = '2.18.0'
+__version__ = '2.18.1'
 __datahub_client_version__ = '1.1'
```

### Comparing `pydatahub-2.18.0/pydatahub.egg-info/PKG-INFO` & `pydatahub-2.18.1/pydatahub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatahub
-Version: 2.18.0
+Version: 2.18.1
 Summary: Datahub Python SDK
 Home-page: https://github.com/aliyun/aliyun-datahub-sdk-python
 Author: andy.xs
 Author-email: helloworld.xs@foxmail.com
 License: Apache License 2.0
 Keywords: pydatahub,python,aliyun,datahub,sdk
 Platform: UNKNOWN
```

### Comparing `pydatahub-2.18.0/pydatahub.egg-info/SOURCES.txt` & `pydatahub-2.18.1/pydatahub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydatahub-2.18.0/setup.py` & `pydatahub-2.18.1/setup.py`

 * *Files identical despite different names*

