# Comparing `tmp/xia_scw_instance-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 101435 bytes, number of entries: 7
--rw-r--r--  2.0 unx      107 b- defN 23-Apr-20 14:09 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   240640 b- defN 23-Apr-20 14:14 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      620 b- defN 23-Apr-20 14:14 xia_scw_instance-0.0.3.dist-info/RECORD
-7 files, 242307 bytes uncompressed, 100321 bytes compressed:  58.6%
+Zip file size: 106397 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      141 b- defN 23-Apr-20 15:51 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   252928 b- defN 23-Apr-20 15:57 xia_scw_instance/instance.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      620 b- defN 23-Apr-20 15:57 xia_scw_instance-0.0.4.dist-info/RECORD
+7 files, 254656 bytes uncompressed, 105283 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_scw_instance/__init__.py
 Comment: 
 
 Filename: xia_scw_instance/instance.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_instance-0.0.3.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.3.dist-info/METADATA
+Filename: xia_scw_instance-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.3.dist-info/WHEEL
+Filename: xia_scw_instance-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.3.dist-info/top_level.txt
+Filename: xia_scw_instance-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.3.dist-info/RECORD
+Filename: xia_scw_instance-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
-from xia_scw_instance.instance import ScwInstance
+from xia_scw_instance.instance import ScwInstance, ScwLanInstance
 
 
 __all__ = [
-    "ScwInstance"
+    "ScwInstance", "ScwLanInstance"
 ]
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_scw_instance-0.0.3.dist-info/METADATA` & `xia_scw_instance-0.0.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: xia-engine-terraform
+Requires-Dist: xia-scw-vpc
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-instance.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-scw-instance/
 
 ====================================
 X-I-A
```

## Comparing `xia_scw_instance-0.0.3.dist-info/RECORD` & `xia_scw_instance-0.0.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_scw_instance/__init__.py,sha256=QN2C2gAbLj2knZrfhMrkR86fc1pXYReHuNDX62_Eidk,107
-xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=Tse7s3ziMabnmt4cTe16UGSyANPHT_BWRdF-yZ-oqos,240640
-xia_scw_instance-0.0.3.dist-info/LICENSE.txt,sha256=shnIQsYEvU4d6D0nUxqrQjhHb0U9ulEMxyt2I58AdZ4,152
-xia_scw_instance-0.0.3.dist-info/METADATA,sha256=ioOFGr8kStGACF5MBPNmarTTX163ct235iGyKrdUBMU,672
-xia_scw_instance-0.0.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_instance-0.0.3.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
-xia_scw_instance-0.0.3.dist-info/RECORD,,
+xia_scw_instance/__init__.py,sha256=ZjkLmLNSeCvY-sm7ZybmxhTLwYUg1Hz2K_CkQa7D9uI,141
+xia_scw_instance/instance.cp39-win_amd64.pyd,sha256=KhB6bdgSC4l5kL9_7_3cTDdyLF407UqgGNazjuqZffw,252928
+xia_scw_instance-0.0.4.dist-info/LICENSE.txt,sha256=o9HFrLthNawEZL_aAWSGK75D0FuK5K4A867ZydnZBWU,152
+xia_scw_instance-0.0.4.dist-info/METADATA,sha256=z-8aqTjJ0Byl15guH59CZpAl6j1aFbRgChS2ay4WBlc,699
+xia_scw_instance-0.0.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_scw_instance-0.0.4.dist-info/top_level.txt,sha256=ffd5mxc0r47bbdzdm8uAtew5JL-56N5Dvcrqvp9tri0,17
+xia_scw_instance-0.0.4.dist-info/RECORD,,
```

