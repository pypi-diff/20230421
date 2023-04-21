# Comparing `tmp/jupylite_duckdb-0.0.2-py3-none-any.whl.zip` & `tmp/jupylite_duckdb-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3833 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-21 01:26 jupylite_duckdb/__init__.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-21 01:26 jupylite_duckdb/_version.py
+Zip file size: 3834 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-21 01:33 jupylite_duckdb/__init__.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Apr-21 01:39 jupylite_duckdb/_version.py
 -rw-rw-rw-  2.0 fat     3354 b- defN 23-Apr-21 01:07 jupylite_duckdb/jdw.py
--rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      668 b- defN 23-Apr-21 01:27 jupylite_duckdb-0.0.2.dist-info/RECORD
-8 files, 6192 bytes uncompressed, 2653 bytes compressed:  57.2%
+-rw-rw-rw-  2.0 fat     1495 b- defN 23-Apr-21 01:40 jupylite_duckdb-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Apr-21 01:40 jupylite_duckdb-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 01:40 jupylite_duckdb-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Apr-21 01:40 jupylite_duckdb-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      668 b- defN 23-Apr-21 01:40 jupylite_duckdb-0.0.3.dist-info/RECORD
+8 files, 6192 bytes uncompressed, 2654 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: jupylite_duckdb/_version.py
 Comment: 
 
 Filename: jupylite_duckdb/jdw.py
 Comment: 
 
-Filename: jupylite_duckdb-0.0.2.dist-info/LICENSE
+Filename: jupylite_duckdb-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: jupylite_duckdb-0.0.2.dist-info/METADATA
+Filename: jupylite_duckdb-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: jupylite_duckdb-0.0.2.dist-info/WHEEL
+Filename: jupylite_duckdb-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: jupylite_duckdb-0.0.2.dist-info/top_level.txt
+Filename: jupylite_duckdb-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: jupylite_duckdb-0.0.2.dist-info/RECORD
+Filename: jupylite_duckdb-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jupylite_duckdb/_version.py

```diff
@@ -1 +1 @@
-__version__="0.0.2"
+__version__="0.0.3"
```

## Comparing `jupylite_duckdb-0.0.2.dist-info/LICENSE` & `jupylite_duckdb-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jupylite_duckdb-0.0.2.dist-info/RECORD` & `jupylite_duckdb-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 jupylite_duckdb/__init__.py,sha256=63DJdYAwG3_kumZPUNkRrenlKyU3GCBUUGPtoXJoelM,64
-jupylite_duckdb/_version.py,sha256=DpbRCq1IY9iJDmSYzWUXi2b9EjbIDdCaXVy6HIKPHek,21
+jupylite_duckdb/_version.py,sha256=PRoALGP9h73tfLSNvhmNGpW4G-W1SFB20tLsfamwYRc,21
 jupylite_duckdb/jdw.py,sha256=3SojnoS1wjwZFqhjT9MbNwYdy4bO384ukKx6RVF___g,3354
-jupylite_duckdb-0.0.2.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
-jupylite_duckdb-0.0.2.dist-info/METADATA,sha256=PJqgrLzjiWFAqhU1jX0sgW0rli003J-2Lrb9VW6XHoA,482
-jupylite_duckdb-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-jupylite_duckdb-0.0.2.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
-jupylite_duckdb-0.0.2.dist-info/RECORD,,
+jupylite_duckdb-0.0.3.dist-info/LICENSE,sha256=WJMtiY9u9JD8FJ18a6_psLMXvrOIA7F-mYphCuyGFvw,1495
+jupylite_duckdb-0.0.3.dist-info/METADATA,sha256=iRUOowNJVGYSBoytOIGzshuNvD5RRimO5TVYh1wZeGE,482
+jupylite_duckdb-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+jupylite_duckdb-0.0.3.dist-info/top_level.txt,sha256=y1GybQE7FyRTQPGLf2lE9dStC--h8ZozxhgXQRxz490,16
+jupylite_duckdb-0.0.3.dist-info/RECORD,,
```

