# Comparing `tmp/pravega-0.3.2-cp39-none-win_amd64.whl.zip` & `tmp/pravega-0.3.3-cp38-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 5232489 bytes, number of entries: 5
--rw-r--r--  4.6 unx     3301 b- defN 22-Sep-16 05:42 pravega-0.3.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Sep-16 05:42 pravega-0.3.2.dist-info/WHEEL
--rw-r--r--  4.6 unx       64 b- defN 22-Sep-16 05:42 pravega_client/__init__.py
--rwxr-xr-x  4.6 unx 15210496 b- defN 22-Sep-16 05:42 pravega_client/pravega_client.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      396 b- defN 22-Sep-16 05:42 pravega-0.3.2.dist-info/RECORD
-5 files, 15214352 bytes uncompressed, 5231757 bytes compressed:  65.6%
+Zip file size: 5412953 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     3301 b- defN 23-Apr-21 04:50 pravega-0.3.3.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Apr-21 04:50 pravega-0.3.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx       64 b- defN 23-Apr-21 04:50 pravega_client/__init__.py
+-rwxr-xr-x  4.6 unx 15856640 b- defN 23-Apr-21 04:50 pravega_client/pravega_client.cp38-win_amd64.pyd
+-rw-r--r--  4.6 unx      396 b- defN 23-Apr-21 04:50 pravega-0.3.3.dist-info/RECORD
+5 files, 15860496 bytes uncompressed, 5412221 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pravega-0.3.2.dist-info/METADATA
+Filename: pravega-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: pravega-0.3.2.dist-info/WHEEL
+Filename: pravega-0.3.3.dist-info/WHEEL
 Comment: 
 
 Filename: pravega_client/__init__.py
 Comment: 
 
-Filename: pravega_client/pravega_client.cp39-win_amd64.pyd
+Filename: pravega_client/pravega_client.cp38-win_amd64.pyd
 Comment: 
 
-Filename: pravega-0.3.2.dist-info/RECORD
+Filename: pravega-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pravega-0.3.2.dist-info/METADATA` & `pravega-0.3.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pravega
-Version: 0.3.2
+Version: 0.3.3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Summary: Pravega client
 Keywords: streaming,client,pravega
 Author: Pravega Community
 License: Apache-2.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://pravega.github.io/pravega-client-rust/
 Project-URL: Source Code, https://github.com/pravega/pravega-client-rust
+Project-URL: Homepage, https://pravega.github.io/pravega-client-rust/
 
 ![CIbuild](https://github.com/pravega/pravega-client-rust/workflows/CIbuild/badge.svg)
 [![codecov](https://codecov.io/gh/pravega/pravega-client-rust/branch/master/graph/badge.svg?token=XEjqMkINCV)](https://codecov.io/gh/pravega/pravega-client-rust)
 
 # Pravega Python client.
 
 This project provides a way to interact with [Pravega](http://pravega.io) using Python client.
```

