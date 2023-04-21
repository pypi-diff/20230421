# Comparing `tmp/distributed-transcoder-common-0.2.8.tar.gz` & `tmp/distributed_transcoder_common-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distributed-transcoder-common-0.2.8.tar", max compression
+gzip compressed data, was "distributed_transcoder_common-0.2.9.tar", max compression
```

## Comparing `distributed-transcoder-common-0.2.8.tar` & `distributed_transcoder_common-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       86 2023-04-04 05:32:08.748355 distributed-transcoder-common-0.2.8/distributed_transcoder_common/__init__.py
--rw-r--r--   0        0        0      561 2023-04-17 00:20:24.807686 distributed-transcoder-common-0.2.8/distributed_transcoder_common/message_types.py
--rw-r--r--   0        0        0     1939 2023-04-16 22:17:26.016806 distributed-transcoder-common-0.2.8/distributed_transcoder_common/models.py
--rw-r--r--   0        0        0      390 2023-04-17 00:20:34.627575 distributed-transcoder-common-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      695 2023-04-17 00:20:37.053000 distributed-transcoder-common-0.2.8/setup.py
--rw-r--r--   0        0        0      422 2023-04-17 00:20:37.053211 distributed-transcoder-common-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-04-18 05:37:08.403132 distributed_transcoder_common-0.2.9/distributed_transcoder_common/__init__.py
+-rw-r--r--   0        0        0      561 2023-04-18 05:37:08.403216 distributed_transcoder_common-0.2.9/distributed_transcoder_common/message_types.py
+-rw-r--r--   0        0        0     2059 2023-04-19 04:08:53.134420 distributed_transcoder_common-0.2.9/distributed_transcoder_common/models.py
+-rw-r--r--   0        0        0      390 2023-04-19 04:09:14.994076 distributed_transcoder_common-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 distributed_transcoder_common-0.2.9/PKG-INFO
```

### Comparing `distributed-transcoder-common-0.2.8/distributed_transcoder_common/message_types.py` & `distributed_transcoder_common-0.2.9/distributed_transcoder_common/message_types.py`

 * *Files identical despite different names*

### Comparing `distributed-transcoder-common-0.2.8/distributed_transcoder_common/models.py` & `distributed_transcoder_common-0.2.9/distributed_transcoder_common/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         "models.Preset", null=True
     )
     state = fields.CharField(max_length=20, default=STATE_QUEUED)
     error = fields.TextField(null=True)
     error_type = fields.CharField(max_length=50, null=True)
     created_at = fields.DatetimeField(auto_now_add=True)
     updated_at = fields.DatetimeField(auto_now=True)
+    transcode_started_at = fields.DatetimeField(null=True)
+    transcode_completed_at = fields.DatetimeField(null=True)
 
     class Meta:
         ordering = ["-created_at"]
 
 
 Tortoise.init_models(["distributed_transcoder_common.models"], "models")
 PresetOut = pydantic_model_creator(Preset, name="PresetOut")
```

