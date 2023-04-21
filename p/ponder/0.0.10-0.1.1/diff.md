# Comparing `tmp/ponder-0.0.10-cp39-cp39-win_amd64.whl.zip` & `tmp/ponder-0.1.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1757789 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  4985856 b- defN 23-Apr-20 15:48 ponder.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    11254 b- defN 23-Apr-20 15:48 ponder-0.0.10.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      783 b- defN 23-Apr-20 15:48 ponder-0.0.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-20 15:48 ponder-0.0.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 23-Apr-20 15:48 ponder-0.0.10.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-20 15:48 ponder-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      569 b- defN 23-Apr-20 15:49 ponder-0.0.10.dist-info/RECORD
-7 files, 4998616 bytes uncompressed, 1756779 bytes compressed:  64.9%
+Zip file size: 1757792 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat  4985856 b- defN 23-Apr-21 02:00 ponder.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    11254 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      800 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      563 b- defN 23-Apr-21 02:00 ponder-0.1.1.dist-info/RECORD
+7 files, 4998627 bytes uncompressed, 1756794 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ponder.cp39-win_amd64.pyd
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/LICENSE.txt
+Filename: ponder-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/METADATA
+Filename: ponder-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/WHEEL
+Filename: ponder-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/entry_points.txt
+Filename: ponder-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/top_level.txt
+Filename: ponder-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ponder-0.0.10.dist-info/RECORD
+Filename: ponder-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ponder-0.0.10.dist-info/LICENSE.txt` & `ponder-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `ponder-0.0.10.dist-info/METADATA` & `ponder-0.1.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ponder
-Version: 0.0.10
+Version: 0.1.1
 Summary: Ponder - An extension to Modin that runs pandas and numpy in your database or data warehouse.
 Home-page: https://ponder.io
 Author: Ponder
-Author-email: contact@ponder.io
-License: UNKNOWN
+Author-email: support@ponder.io
+License: Other/Proprietary License
 Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: snowflake-connector-python[pandas]
 Requires-Dist: big
 Requires-Dist: boto3
 Requires-Dist: cloudpickle (==2.0.0)
```

