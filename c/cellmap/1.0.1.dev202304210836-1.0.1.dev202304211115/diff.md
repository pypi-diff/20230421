# Comparing `tmp/cellmap-1.0.1.dev202304210836-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304211115-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1390449 bytes, number of entries: 6
+Zip file size: 1390450 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    63188 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210836.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304210836.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304210836.dist-info/RECORD
-6 files, 4512552 bytes uncompressed, 1389563 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    63190 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304211115.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304211115.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304211115.dist-info/RECORD
+6 files, 4512554 bytes uncompressed, 1389564 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210836.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304211115.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210836.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304211115.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304210836.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304211115.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -21,15 +21,15 @@
 
 
 
 def create_graph(
     X,
     cutedge_vol = None,
     cutedge_length = None,
-    cut_std = 2,
+    cut_std = 2.5,
     return_type = 'edges',
 ):
     tri_ = matplotlib.tri.Triangulation(X[:,0],X[:,1])
     X_src_,X_trg_ = X[tri_.edges[:,0]],X[tri_.edges[:,1]]
     length_edge_ = np.linalg.norm(X_src_-X_trg_,axis=1)
     x1,y1 = X[tri_.triangles[:,0],0],X[tri_.triangles[:,0],1]
     x2,y2 = X[tri_.triangles[:,1],0],X[tri_.triangles[:,1],1]
```

## Comparing `cellmap-1.0.1.dev202304210836.dist-info/METADATA` & `cellmap-1.0.1.dev202304211115.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304210836
+Version: 1.0.1.dev202304211115
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

