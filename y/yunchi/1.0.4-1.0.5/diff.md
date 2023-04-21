# Comparing `tmp/yunchi-1.0.4-cp38-cp38-win_amd64.whl.zip` & `tmp/yunchi-1.0.5-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,21 @@
-Zip file size: 650228 bytes, number of entries: 26
--rw-rw-rw-  2.0 fat     3032 b- defN 23-Apr-06 06:47 main.py
+Zip file size: 454023 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat      188 b- defN 23-Apr-14 03:05 yunchi/__init__.py
 -rw-rw-rw-  2.0 fat      150 b- defN 23-Apr-14 03:00 yunchi/api.py
--rw-rw-rw-  2.0 fat   270336 b- defN 23-Apr-21 03:04 yunchi/data.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   270336 b- defN 23-Apr-21 08:29 yunchi/data.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     9403 b- defN 23-Mar-31 07:27 yunchi/model.py
--rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 03:04 yunchi/quote.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   177152 b- defN 23-Apr-06 07:23 yunchi/quote_api.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 03:04 yunchi/sdk.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   107008 b- defN 23-Apr-21 03:04 yunchi/strategy.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   107008 b- defN 23-Apr-06 07:23 yunchi/strategy_api.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   254464 b- defN 23-Apr-21 03:04 yunchi/trade.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   167936 b- defN 23-Apr-06 07:23 yunchi/trade_api.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat      153 b- defN 23-Apr-06 07:29 yunchi/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 08:29 yunchi/quote.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 08:29 yunchi/sdk.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   107008 b- defN 23-Apr-21 08:29 yunchi/strategy.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   254464 b- defN 23-Apr-21 08:29 yunchi/trade.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     9745 b- defN 23-Apr-06 07:48 yunchi/pb/Quotation.proto
 -rw-rw-rw-  2.0 fat   102268 b- defN 23-Mar-10 07:41 yunchi/pb/Quotation_pb2.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-Apr-14 01:57 yunchi/pb/__init__.py
 -rw-rw-rw-  2.0 fat   352070 b- defN 23-Apr-14 01:58 yunchi/pb/api_pb2.py
 -rw-rw-rw-  2.0 fat    35275 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.api.proto
 -rw-rw-rw-  2.0 fat    10950 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.type.proto
 -rw-rw-rw-  2.0 fat    49067 b- defN 23-Apr-14 01:57 yunchi/pb/type_pb2.py
--rw-rw-rw-  2.0 fat    37174 b- defN 23-Apr-06 07:29 yunchi/pb/__pycache__/Quotation_pb2.cpython-38.pyc
--rw-rw-rw-  2.0 fat      156 b- defN 23-Apr-06 07:29 yunchi/pb/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-  2.0 fat      466 b- defN 23-Apr-21 03:04 yunchi-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-21 03:04 yunchi-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-21 03:04 yunchi-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2179 b- defN 23-Apr-21 03:04 yunchi-1.0.4.dist-info/RECORD
-26 files, 2049671 bytes uncompressed, 646756 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat      466 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1523 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/RECORD
+19 files, 1556404 bytes uncompressed, 451587 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: main.py
-Comment: 
-
 Filename: yunchi/__init__.py
 Comment: 
 
 Filename: yunchi/api.py
 Comment: 
 
 Filename: yunchi/data.cp38-win_amd64.pyd
@@ -12,35 +9,23 @@
 
 Filename: yunchi/model.py
 Comment: 
 
 Filename: yunchi/quote.cp38-win_amd64.pyd
 Comment: 
 
-Filename: yunchi/quote_api.cp38-win_amd64.pyd
-Comment: 
-
 Filename: yunchi/sdk.cp38-win_amd64.pyd
 Comment: 
 
 Filename: yunchi/strategy.cp38-win_amd64.pyd
 Comment: 
 
-Filename: yunchi/strategy_api.cp38-win_amd64.pyd
-Comment: 
-
 Filename: yunchi/trade.cp38-win_amd64.pyd
 Comment: 
 
-Filename: yunchi/trade_api.cp38-win_amd64.pyd
-Comment: 
-
-Filename: yunchi/__pycache__/__init__.cpython-38.pyc
-Comment: 
-
 Filename: yunchi/pb/Quotation.proto
 Comment: 
 
 Filename: yunchi/pb/Quotation_pb2.py
 Comment: 
 
 Filename: yunchi/pb/__init__.py
@@ -54,26 +39,20 @@
 
 Filename: yunchi/pb/dtp.type.proto
 Comment: 
 
 Filename: yunchi/pb/type_pb2.py
 Comment: 
 
-Filename: yunchi/pb/__pycache__/Quotation_pb2.cpython-38.pyc
-Comment: 
-
-Filename: yunchi/pb/__pycache__/__init__.cpython-38.pyc
-Comment: 
-
-Filename: yunchi-1.0.4.dist-info/METADATA
+Filename: yunchi-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: yunchi-1.0.4.dist-info/WHEEL
+Filename: yunchi-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: yunchi-1.0.4.dist-info/top_level.txt
+Filename: yunchi-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: yunchi-1.0.4.dist-info/RECORD
+Filename: yunchi-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

