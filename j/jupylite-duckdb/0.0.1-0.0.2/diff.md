# Comparing `tmp/jupylite_duckdb-0.0.1-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3841 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-21 01:07 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-21 00:08 jupylite_duckdb/_version.py
+Zip file size: 3833 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-21 01:26 jupylite_duckdb/__init__.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-21 01:26 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     3354 b- defN 23-Apr-21 01:07 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-21 01:16 jupylite_duckdb-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Apr-21 01:16 jupylite_duckdb-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 01:16 jupylite_duckdb-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-21 01:16 jupylite_duckdb-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      668 b- defN 23-Apr-21 01:16 jupylite_duckdb-0.0.1.dist-info/RECORD
-8 files, 6200 bytes uncompressed, 2661 bytes compressed:  57.1%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      668 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/RECORD
+8 files, 6192 bytes uncompressed, 2653 bytes compressed:  57.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: jupylite_duckdb/_version.py
 Comment: 
 
 Filename: jupylite_duckdb/jdw.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.1.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.1.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.1.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.1.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.1.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/__init__.py

```diff
@@ -1 +1 @@
-from jupyterlite_duckdb_wasm.jdw import connect, query  # type: ignore
+from jupylite_duckdb.jdw import connect, query  # type: ignore
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.1"
+__version__="0.0.2"
```

## Comparing `jupylite_duckdb-0.0.1.dist-info/LICENSE` & `jupylite_duckdb-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

