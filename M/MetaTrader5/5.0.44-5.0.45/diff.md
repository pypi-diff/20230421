# Comparing `tmp/MetaTrader5-5.0.44-cp39-cp39-win_amd64.whl.zip` & `tmp/MetaTrader5-5.0.45-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 57102 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    17517 b- defN 23-Feb-15 00:27 MetaTrader5/__init__.py
--rw-rw-rw-  2.0 fat   138752 b- defN 23-Feb-15 00:27 MetaTrader5/_core.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1065 b- defN 23-Feb-15 00:27 MetaTrader5-5.0.44.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2336 b- defN 23-Feb-15 00:27 MetaTrader5-5.0.44.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-15 00:27 MetaTrader5-5.0.44.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Feb-15 00:27 MetaTrader5-5.0.44.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      592 b- defN 23-Feb-15 00:27 MetaTrader5-5.0.44.dist-info/RECORD
-7 files, 160374 bytes uncompressed, 56054 bytes compressed:  65.0%
+Zip file size: 57158 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    17680 b- defN 23-Apr-21 14:33 MetaTrader5/__init__.py
+-rw-rw-rw-  2.0 fat   138752 b- defN 23-Apr-21 14:33 MetaTrader5/_core.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1065 b- defN 23-Apr-21 14:33 MetaTrader5-5.0.45.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-Apr-21 14:33 MetaTrader5-5.0.45.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-21 14:33 MetaTrader5-5.0.45.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-21 14:33 MetaTrader5-5.0.45.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      592 b- defN 23-Apr-21 14:33 MetaTrader5-5.0.45.dist-info/RECORD
+7 files, 160537 bytes uncompressed, 56110 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: MetaTrader5/__init__.py
 Comment: 
 
 Filename: MetaTrader5/_core.cp39-win_amd64.pyd
 Comment: 
 
-Filename: MetaTrader5-5.0.44.dist-info/LICENSE.txt
+Filename: MetaTrader5-5.0.45.dist-info/LICENSE.txt
 Comment: 
 
-Filename: MetaTrader5-5.0.44.dist-info/METADATA
+Filename: MetaTrader5-5.0.45.dist-info/METADATA
 Comment: 
 
-Filename: MetaTrader5-5.0.44.dist-info/WHEEL
+Filename: MetaTrader5-5.0.45.dist-info/WHEEL
 Comment: 
 
-Filename: MetaTrader5-5.0.44.dist-info/top_level.txt
+Filename: MetaTrader5-5.0.45.dist-info/top_level.txt
 Comment: 
 
-Filename: MetaTrader5-5.0.44.dist-info/RECORD
+Filename: MetaTrader5-5.0.45.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## MetaTrader5/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '5.0.44'
+__version__ = '5.0.45'
 __author__  = 'MetaQuotes Ltd.'
 
 # timeframes
 TIMEFRAME_M1                        = 1
 TIMEFRAME_M2                        = 2
 TIMEFRAME_M3                        = 3
 TIMEFRAME_M4                        = 4
@@ -60,17 +60,18 @@
 ORDER_STATE_FILLED                  = 4      # Order fully executed
 ORDER_STATE_REJECTED                = 5      # Order rejected
 ORDER_STATE_EXPIRED                 = 6      # Order expired
 ORDER_STATE_REQUEST_ADD             = 7      # Order is being registered (placing to the trading system)
 ORDER_STATE_REQUEST_MODIFY          = 8      # Order is being modified (changing its parameters)
 ORDER_STATE_REQUEST_CANCEL          = 9      # Order is being deleted (deleting from the trading system)
 # ENUM_ORDER_TYPE_FILLING
-ORDER_FILLING_FOK                   = 0
-ORDER_FILLING_IOC                   = 1
-ORDER_FILLING_RETURN                = 2
+ORDER_FILLING_FOK                   = 0      # Fill Or Kill order
+ORDER_FILLING_IOC                   = 1      # Immediately Or Cancel
+ORDER_FILLING_RETURN                = 2      # Return remaining volume to book
+ORDER_FILLING_BOC                   = 3      # Book Or Cancel order
 # ENUM_ORDER_TYPE_TIME
 ORDER_TIME_GTC                      = 0      # Good till cancel order
 ORDER_TIME_DAY                      = 1      # Good till current trade day order
 ORDER_TIME_SPECIFIED                = 2      # Good till expired order
 ORDER_TIME_SPECIFIED_DAY            = 3      # The order will be effective till 23:59:59 of the specified day. If this time is outside a trading session, the order expires in the nearest trading time.
 # ENUM_ORDER_REASON
 ORDER_REASON_CLIENT                 = 0      # The order was placed from a desktop terminal
```

## Comparing `MetaTrader5-5.0.44.dist-info/LICENSE.txt` & `MetaTrader5-5.0.45.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `MetaTrader5-5.0.44.dist-info/METADATA` & `MetaTrader5-5.0.45.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MetaTrader5
-Version: 5.0.44
+Version: 5.0.45
 Summary: API Connector to MetaTrader 5 Terminal
 Home-page: https://www.metatrader5.com
 Author: MetaQuotes Ltd.
 Author-email: plugins@metaquotes.net
 Maintainer: MetaQuotes Ltd.
 Maintainer-email: plugins@metaquotes.net
 License: MIT
```

