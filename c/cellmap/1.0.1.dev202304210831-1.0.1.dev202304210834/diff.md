# Comparing `tmp/cellmap-1.0.1.dev202304210831-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304210834-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390444 bytes, number of entries: 6
+Zip file size: 1390443 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    63141 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210831.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210831.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304210831.dist-info/RECORD
-6 files, 4512505 bytes uncompressed, 1389558 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    63146 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210834.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210834.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304210834.dist-info/RECORD
+6 files, 4512510 bytes uncompressed, 1389557 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210831.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304210834.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210831.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304210834.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210831.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304210834.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -41,15 +41,15 @@
     else:
         judge_vol_tri_ = vol_ < np.percentile(vol_,100-cutedge_vol)
     if cutedge_length == None:
         judge_length_edge_ = length_edge_ < cut_std*np.std(length_edge_)
         judge_length_tri_= length_ < cut_std*np.std(length_)
     else:
         judge_length_edge_ = length_edge_ < np.percentile(length_edge_,100-cutedge_length)
-        judge_length_tri_ = length_ < np.percentile(length_,100-cutedge_length)
+        judge_length_tri_ = length_ < np.percentile(length_edge_,100-cutedge_length)
     if return_type == 'edges': return tri_.edges[judge_length_edge_].T
     if return_type == 'triangles':
         idx_mask_ = judge_vol_tri_ & judge_length_tri_
         tri_.set_mask(idx_mask_==False)
         return tri_,idx_mask_
```

## Comparing `cellmap-1.0.1.dev202304210831.dist-info/METADATA` & `cellmap-1.0.1.dev202304210834.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304210831
+Version: 1.0.1.dev202304210834
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

