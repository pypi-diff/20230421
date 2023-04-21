# Comparing `tmp/ortoolpy-0.5.0-py3-none-any.whl.zip` & `tmp/ortoolpy-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 27779 bytes, number of entries: 8
+Zip file size: 27776 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     1216 b- defN 80-Jan-01 00:00 ortoolpy/__init__.py
 -rw-r--r--  2.0 unx     3325 b- defN 80-Jan-01 00:00 ortoolpy/cover_by_rect.py
 -rw-r--r--  2.0 unx    50154 b- defN 80-Jan-01 00:00 ortoolpy/etc.py
 -rw-r--r--  2.0 unx    28688 b- defN 80-Jan-01 00:00 ortoolpy/optimization/__init__.py
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 ortoolpy-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1555 b- defN 80-Jan-01 00:00 ortoolpy-0.5.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      622 b- defN 16-Jan-01 00:00 ortoolpy-0.5.0.dist-info/RECORD
-8 files, 96405 bytes uncompressed, 26711 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 ortoolpy-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 ortoolpy-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1552 b- defN 80-Jan-01 00:00 ortoolpy-0.6.0.dist-info/METADATA
+?rw-r--r--  2.0 unx      622 b- defN 16-Jan-01 00:00 ortoolpy-0.6.0.dist-info/RECORD
+8 files, 96402 bytes uncompressed, 26708 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: ortoolpy/etc.py
 Comment: 
 
 Filename: ortoolpy/optimization/__init__.py
 Comment: 
 
-Filename: ortoolpy-0.5.0.dist-info/LICENSE
+Filename: ortoolpy-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: ortoolpy-0.5.0.dist-info/WHEEL
+Filename: ortoolpy-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: ortoolpy-0.5.0.dist-info/METADATA
+Filename: ortoolpy-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: ortoolpy-0.5.0.dist-info/RECORD
+Filename: ortoolpy-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ortoolpy-0.5.0.dist-info/LICENSE` & `ortoolpy-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ortoolpy-0.5.0.dist-info/METADATA` & `ortoolpy-0.6.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortoolpy
-Version: 0.5.0
+Version: 0.6.0
 Summary: `ortoolpy` is a package for Operations Research.
 Home-page: https://github.com/SaitoTsutomu/ortoolpy
 License: Apache-2.0
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -12,16 +12,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
-Requires-Dist: more-itertools (>=9.0,<10.0)
-Requires-Dist: pandas (>=1.5,<2.0)
+Requires-Dist: more-itertools (>=9.1,<10.0)
+Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: pulp (>=2.7,<3.0)
 Description-Content-Type: text/x-rst
 
 `ortoolpy` is a package for Operations Research.
 It is user's responsibility for the use of `ortoolpy`.
 
 ::
```

