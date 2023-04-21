# Comparing `tmp/xia_scw_vpc-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.0.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 102132 bytes, number of entries: 7
--rw-r--r--  2.0 unx       87 b- defN 23-Apr-19 10:51 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   242688 b- defN 23-Apr-19 10:54 xia_scw_vpc/vpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-19 10:54 xia_scw_vpc-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-19 10:54 xia_scw_vpc-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-19 10:54 xia_scw_vpc-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-19 10:54 xia_scw_vpc-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      579 b- defN 23-Apr-19 10:54 xia_scw_vpc-0.0.2.dist-info/RECORD
-7 files, 244269 bytes uncompressed, 101098 bytes compressed:  58.6%
+Zip file size: 106931 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-21 05:41 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   251904 b- defN 23-Apr-21 06:01 xia_scw_vpc/vpc.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 06:01 xia_scw_vpc-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      652 b- defN 23-Apr-21 06:01 xia_scw_vpc-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 06:01 xia_scw_vpc-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-21 06:01 xia_scw_vpc-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      579 b- defN 23-Apr-21 06:01 xia_scw_vpc-0.0.3.dist-info/RECORD
+7 files, 253485 bytes uncompressed, 105897 bytes compressed:  58.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
 Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_vpc-0.0.2.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.2.dist-info/METADATA
+Filename: xia_scw_vpc-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.0.2.dist-info/WHEEL
+Filename: xia_scw_vpc-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.0.2.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.0.2.dist-info/RECORD
+Filename: xia_scw_vpc-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `xia_scw_vpc-0.0.2.dist-info/METADATA` & `xia_scw_vpc-0.0.3.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-scw-vpc
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-vpc/0.0.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

