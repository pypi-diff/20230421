# Comparing `tmp/xia_engine_terraform_gcs-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform_gcs-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 123185 bytes, number of entries: 7
--rw-r--r--  2.0 unx      378 b- defN 23-Apr-17 18:11 xia_engine_terraform_gcs/__init__.py
--rw-r--r--  2.0 unx   292352 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      674 b- defN 23-Apr-17 18:14 xia_engine_terraform_gcs-0.0.4.dist-info/RECORD
-7 files, 294406 bytes uncompressed, 121963 bytes compressed:  58.6%
+Zip file size: 124570 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-21 09:20 xia_engine_terraform_gcs/__init__.py
+-rw-r--r--  2.0 unx   295424 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      674 b- defN 23-Apr-21 09:23 xia_engine_terraform_gcs-0.0.5.dist-info/RECORD
+7 files, 297478 bytes uncompressed, 123348 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform_gcs/__init__.py
 Comment: 
 
 Filename: xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.4.dist-info/LICENSE.txt
+Filename: xia_engine_terraform_gcs-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.4.dist-info/METADATA
+Filename: xia_engine_terraform_gcs-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.4.dist-info/WHEEL
+Filename: xia_engine_terraform_gcs-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.4.dist-info/top_level.txt
+Filename: xia_engine_terraform_gcs-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.0.4.dist-info/RECORD
+Filename: xia_engine_terraform_gcs-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform_gcs/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformGcsEngine", "TerraformGcsConnectParam", "TerraformGcsClient",
     "ScwTerraformGcsEngine", "ScwTerraformGcsConnectParam"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_engine_terraform_gcs-0.0.4.dist-info/METADATA` & `xia_engine_terraform_gcs-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform-gcs
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_terraform_gcs-0.0.4.dist-info/RECORD` & `xia_engine_terraform_gcs-0.0.5.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform_gcs/__init__.py,sha256=MgwvTHtpFEkP8ldrz4Krcr2K0Ow3bMUz9BJU6rpG61g,378
-xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd,sha256=2chdi48g4Dp1J2Pu3EbDKo0X5HwdnP1Cl2OY-WSNmtw,292352
-xia_engine_terraform_gcs-0.0.4.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
-xia_engine_terraform_gcs-0.0.4.dist-info/METADATA,sha256=-Wn_3gXCL5iiPjKPKdiYBLfxNSIWtzz3PxfjcA-fB7s,726
-xia_engine_terraform_gcs-0.0.4.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_engine_terraform_gcs-0.0.4.dist-info/top_level.txt,sha256=iRljnR7jo0lVXDe6suGjsY4FzFzjk-Xas_iLcd7D2EU,25
-xia_engine_terraform_gcs-0.0.4.dist-info/RECORD,,
+xia_engine_terraform_gcs/__init__.py,sha256=mB1j0aJxmN3PElKy_xBfLpxVWKanXtwPGsKsgEqnlDI,378
+xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd,sha256=xUNqbAbpkxgseB2fWbIhSG0ofHoS6C7E8yF8BdwU8cY,295424
+xia_engine_terraform_gcs-0.0.5.dist-info/LICENSE.txt,sha256=30wWxpufZqbxK7WdwZRoX8iA_veQA4gbl5oih3j5vFs,152
+xia_engine_terraform_gcs-0.0.5.dist-info/METADATA,sha256=Rzr4Xf4-CUpjhBHn4aHN82lE9Ch50TZ21LDMzHYJTh4,726
+xia_engine_terraform_gcs-0.0.5.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_engine_terraform_gcs-0.0.5.dist-info/top_level.txt,sha256=iRljnR7jo0lVXDe6suGjsY4FzFzjk-Xas_iLcd7D2EU,25
+xia_engine_terraform_gcs-0.0.5.dist-info/RECORD,,
```

