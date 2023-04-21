# Comparing `tmp/xia_scw_instance-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 106397 bytes, number of entries: 7
--rw-r--r--  2.0 unx      141 b- defN 23-Apr-20 15:51 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   252928 b- defN 23-Apr-20 15:57 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      620 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/RECORD
-7 files, 254656 bytes uncompressed, 105283 bytes compressed:  58.7%
+Zip file size: 103389 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      107 b- defN 23-Apr-21 11:31 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   241152 b- defN 23-Apr-21 13:47 xia_scw_instance/instance.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/backend.tf
+-rw-rw-rw-  2.0 unx      125 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/main.tf
+-rw-rw-rw-  2.0 unx      393 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/output.tf
+-rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
+-rw-rw-rw-  2.0 unx      954 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/variables.tf
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1143 b- defN 23-Apr-21 13:47 xia_scw_instance-0.0.5.dist-info/RECORD
+12 files, 245253 bytes uncompressed, 101407 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
 Filename: xia_scw_instance/__init__.py
 Comment: 
 
 Filename: xia_scw_instance/instance.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_instance-0.0.4.dist-info/LICENSE.txt
+Filename: xia_scw_instance/templates/ScwInstance/backend.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.4.dist-info/METADATA
+Filename: xia_scw_instance/templates/ScwInstance/main.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.4.dist-info/WHEEL
+Filename: xia_scw_instance/templates/ScwInstance/output.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.4.dist-info/top_level.txt
+Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.4.dist-info/RECORD
+Filename: xia_scw_instance/templates/ScwInstance/variables.tf
+Comment: 
+
+Filename: xia_scw_instance-0.0.5.dist-info/LICENSE.txt
+Comment: 
+
+Filename: xia_scw_instance-0.0.5.dist-info/METADATA
+Comment: 
+
+Filename: xia_scw_instance-0.0.5.dist-info/WHEEL
+Comment: 
+
+Filename: xia_scw_instance-0.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: xia_scw_instance-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
-from xia_scw_instance.instance import ScwInstance, ScwLanInstance
+from xia_scw_instance.instance import ScwInstance
 
 
 __all__ = [
-    "ScwInstance", "ScwLanInstance"
+    "ScwInstance"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_scw_instance-0.0.4.dist-info/METADATA` & `xia_scw_instance-0.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

