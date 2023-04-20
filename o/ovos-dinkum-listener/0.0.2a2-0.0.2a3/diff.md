# Comparing `tmp/ovos_dinkum_listener-0.0.2a2-py3-none-any.whl.zip` & `tmp/ovos_dinkum_listener-0.0.2a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,16 @@
-Zip file size: 1616 bytes, number of entries: 5
--rw-r--r--  2.0 unx      555 b- defN 23-Apr-10 17:46 ovos_dinkum_listener-0.0.2a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 17:46 ovos_dinkum_listener-0.0.2a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-Apr-10 17:46 ovos_dinkum_listener-0.0.2a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-10 17:46 ovos_dinkum_listener-0.0.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      466 b- defN 23-Apr-10 17:46 ovos_dinkum_listener-0.0.2a2.dist-info/RECORD
-5 files, 1191 bytes uncompressed, 728 bytes compressed:  38.9%
+Zip file size: 21465 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      578 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/__init__.py
+-rw-r--r--  2.0 unx    26500 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/__main__.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/plugins.py
+-rw-r--r--  2.0 unx     4540 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/transformers.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/version.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/voice_loop/__init__.py
+-rw-r--r--  2.0 unx     8686 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/voice_loop/hotwords.py
+-rw-r--r--  2.0 unx     4630 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/voice_loop/microphone.py
+-rw-r--r--  2.0 unx    17212 b- defN 23-Apr-20 22:42 ovos_dinkum_listener/voice_loop/voice_loop.py
+-rw-r--r--  2.0 unx      555 b- defN 23-Apr-20 22:42 ovos_dinkum_listener-0.0.2a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 22:42 ovos_dinkum_listener-0.0.2a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Apr-20 22:42 ovos_dinkum_listener-0.0.2a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-20 22:42 ovos_dinkum_listener-0.0.2a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Apr-20 22:42 ovos_dinkum_listener-0.0.2a3.dist-info/RECORD
+14 files, 68910 bytes uncompressed, 19217 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,16 +1,43 @@
-Filename: ovos_dinkum_listener-0.0.2a2.dist-info/METADATA
+Filename: ovos_dinkum_listener/__init__.py
 Comment: 
 
-Filename: ovos_dinkum_listener-0.0.2a2.dist-info/WHEEL
+Filename: ovos_dinkum_listener/__main__.py
 Comment: 
 
-Filename: ovos_dinkum_listener-0.0.2a2.dist-info/entry_points.txt
+Filename: ovos_dinkum_listener/plugins.py
 Comment: 
 
-Filename: ovos_dinkum_listener-0.0.2a2.dist-info/top_level.txt
+Filename: ovos_dinkum_listener/transformers.py
 Comment: 
 
-Filename: ovos_dinkum_listener-0.0.2a2.dist-info/RECORD
+Filename: ovos_dinkum_listener/version.py
+Comment: 
+
+Filename: ovos_dinkum_listener/voice_loop/__init__.py
+Comment: 
+
+Filename: ovos_dinkum_listener/voice_loop/hotwords.py
+Comment: 
+
+Filename: ovos_dinkum_listener/voice_loop/microphone.py
+Comment: 
+
+Filename: ovos_dinkum_listener/voice_loop/voice_loop.py
+Comment: 
+
+Filename: ovos_dinkum_listener-0.0.2a3.dist-info/METADATA
+Comment: 
+
+Filename: ovos_dinkum_listener-0.0.2a3.dist-info/WHEEL
+Comment: 
+
+Filename: ovos_dinkum_listener-0.0.2a3.dist-info/entry_points.txt
+Comment: 
+
+Filename: ovos_dinkum_listener-0.0.2a3.dist-info/top_level.txt
+Comment: 
+
+Filename: ovos_dinkum_listener-0.0.2a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ovos_dinkum_listener-0.0.2a2.dist-info/METADATA` & `ovos_dinkum_listener-0.0.2a3.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-dinkum-listener
-Version: 0.0.2a2
+Version: 0.0.2a3
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-dinkum-listener
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

