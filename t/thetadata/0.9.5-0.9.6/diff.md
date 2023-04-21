# Comparing `tmp/thetadata-0.9.5.tar.gz` & `tmp/thetadata-0.9.6.tar.gz`

## Comparing `thetadata-0.9.5.tar` & `thetadata-0.9.6.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.5/mkdocs.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.5/setup.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.5/.github/workflows/main.yml
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/__init__.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/connection_msgs.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/explanation.md
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/how-to-guides.md
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/index.md
--rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/logo.png
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/manipulate_df.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/manipulate_series.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/reference.md
--rw-r--r--   0        0        0    27736 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/tutorials.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/__init__.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/cancel_streams.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/eod.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/get_last.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/list_roots.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/open_interest_streaming.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/quote_1min.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/quote_tick.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/trade_streaming.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/options/trade_streaming_full.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/eod.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/get_last.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/list_roots.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/quote_1min.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.5/docs/stocks/quote_tick.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.5/tests/__init__.py
--rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.5/tests/test_client.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.5/tests/test_docs.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/__init__.py
--rw-r--r--   0        0        0    58526 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/client.py
--rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/enums.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/exceptions.py
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/parsing.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/py.typed
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.5/thetadata/terminal.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.5/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.5/LICENSE
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 thetadata-0.9.5/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 thetadata-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 thetadata-0.9.6/mkdocs.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 thetadata-0.9.6/setup.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 thetadata-0.9.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thetadata-0.9.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/connection_msgs.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/explanation.md
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/how-to-guides.md
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/index.md
+-rw-r--r--   0        0        0    51619 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/logo.png
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/manipulate_df.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/manipulate_series.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/reference.md
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/tutorials.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/__init__.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/cancel_streams.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/eod.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/get_last.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/list_roots.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/open_interest_streaming.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_1min.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_streaming.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/quote_tick.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/trade_streaming.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/options/trade_streaming_full.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/eod.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/get_last.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/list_roots.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/quote_1min.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 thetadata-0.9.6/docs/stocks/quote_tick.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/__init__.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/test_client.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 thetadata-0.9.6/tests/test_docs.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/__init__.py
+-rw-r--r--   0        0        0    58526 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/client.py
+-rw-r--r--   0        0        0    20277 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/enums.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/exceptions.py
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/parsing.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/py.typed
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 thetadata-0.9.6/thetadata/terminal.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 thetadata-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 thetadata-0.9.6/LICENSE
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 thetadata-0.9.6/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 thetadata-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 thetadata-0.9.6/PKG-INFO
```

### Comparing `thetadata-0.9.5/mkdocs.yml` & `thetadata-0.9.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/.github/workflows/main.yml` & `thetadata-0.9.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/.github/workflows/python-publish.yml` & `thetadata-0.9.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/connection_msgs.py` & `thetadata-0.9.6/docs/options/open_interest_streaming.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from datetime import date
-
-from thetadata import ThetaClient, OptionRight, StreamMsg, StreamMsgType
+from thetadata import ThetaClient, StreamMsg, StreamMsgType
 
 
 def streaming():
     # Credentials now required because get_last is only available to ThetaData Standard & Pro subscribers.
     client = ThetaClient(username="MyThetaDataEmail", passwd="MyThetaDataPassword")
 
     client.connect_stream(callback)  # You can stop streaming by calling client.close_stream
-    client.req_full_trade_stream_opt()  # Subscribes to every option trade.
+    client.req_full_open_interest_stream()  # requests every option open interest update
 
 
 # User generated method that gets called each time a message from the stream arrives.
 def callback(msg: StreamMsg):
-    if msg.type == StreamMsgType.DISCONNECTED or msg.type == StreamMsgType.RECONNECTED:
-        print(msg.type.__str__())  # Handle disconnect / reconnect.
+    msg.type = msg.type
+
+    if msg.type == StreamMsgType.OPEN_INTEREST:
+        print('con:' + msg.contract.to_string() + ' open_interest: ' + msg.open_interest.to_string())
 
 
 if __name__ == "__main__":
     streaming()
```

### Comparing `thetadata-0.9.5/docs/explanation.md` & `thetadata-0.9.6/docs/explanation.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/how-to-guides.md` & `thetadata-0.9.6/docs/how-to-guides.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/index.md` & `thetadata-0.9.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/logo.png` & `thetadata-0.9.6/docs/logo.png`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/manipulate_series.py` & `thetadata-0.9.6/docs/manipulate_series.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/tutorials.md` & `thetadata-0.9.6/docs/tutorials.md`

 * *Files 6% similar despite different names*

```diff
@@ -249,17 +249,50 @@
 
 You must implement a callback method as shown in the first example below. Each time a 
 ``StreamMsg`` is received, this method will get called. A ``StreamMsg`` has a ``StreamMsgType``, which
 can be used to determine the purpose of the message.
 
 #### Limitations
 
-The Pro tier has the ability to request a trade stream for every option contract in
-existence and is able to have up to 15K quote streams. The Standard tier is only allowed
-5K quote streams and 10K trade streams. Other tiers do not have access to streaming at this time.
+The Pro tier has the ability to request a trade stream for every option contract in existence and is able to 
+request up to 20K quote streams. The Standard tier can request 10K quote streams and 20K trade streams.
+Other tiers do not have access to streaming at this time.
+
+### Option Quotes
+
+Below requests to receive continuous updates for quote for an AAPL option contract. Notice 
+that these options are probably expired, so you may need to change the expiration date.
+
+=== "trade_streaming.py"
+
+    ```python
+    --8<-- "docs/options/quote_streaming.py"
+    ```
+
+=== "Output"
+
+    ```bash
+    > python trade_streaming.py
+    ---------------------------------------------------------------------------
+    con:    root: AAPL isOption: True exp: 2023-07-21 strike: 170.0 isCall: True
+    quote:  ms_of_day: 57061764 bid_size: 202 bid_exchange: EDGX bid_price: 6.35 bid_condition: NATIONAL_BBO ask_size: 742 ask_exchange: C2OX ask_price: 6.45 ask_condition: NATIONAL_BBO date: 2023-04-21
+    ---------------------------------------------------------------------------
+    con:    root: AAPL isOption: True exp: 2023-07-21 strike: 170.0 isCall: True
+    quote:  ms_of_day: 57061816 bid_size: 202 bid_exchange: EDGX bid_price: 6.35 bid_condition: NATIONAL_BBO ask_size: 742 ask_exchange: C2OX ask_price: 6.45 ask_condition: NATIONAL_BBO date: 2023-04-21
+    ---------------------------------------------------------------------------
+    con:    root: AAPL isOption: True exp: 2023-07-21 strike: 170.0 isCall: True
+    quote:  ms_of_day: 57061974 bid_size: 202 bid_exchange: EDGX bid_price: 6.35 bid_condition: NATIONAL_BBO ask_size: 742 ask_exchange: C2OX ask_price: 6.45 ask_condition: NATIONAL_BBO date: 2023-04-21
+    ---------------------------------------------------------------------------
+    con:    root: AAPL isOption: True exp: 2023-07-21 strike: 170.0 isCall: True
+    quote:  ms_of_day: 57061974 bid_size: 254 bid_exchange: C2OX bid_price: 6.35 bid_condition: NATIONAL_BBO ask_size: 742 ask_exchange: C2OX ask_price: 6.45 ask_condition: NATIONAL_BBO date: 2023-04-21
+    ---------------------------------------------------------------------------
+    con:    root: AAPL isOption: True exp: 2023-07-21 strike: 170.0 isCall: True
+    quote:  ms_of_day: 57062025 bid_size: 322 bid_exchange: C2OX bid_price: 6.35 bid_condition: NATIONAL_BBO ask_size: 742 ask_exchange: C2OX ask_price: 6.45 ask_condition: NATIONAL_BBO date: 2023-04-21
+    ---------------------------------------------------------------------------
+    ```
 
 ### Option Trades
 
 Below requests to receive continuous updates for trades for a NVDA option contract. Notice 
 that these options are probably expired, so you may need to change the expiration date.
 
 === "trade_streaming.py"
@@ -324,15 +357,16 @@
     last quote at time of trade: ms_of_day: 46429598 bid_size: 39 bid_exchange: XBOS bid_price: 9.55 bid_condition: NATIONAL_BBO ask_size: 39 ask_exchange: XBOS ask_price: 10.05 ask_condition: NATIONAL_BBO date: 2022-12-27
     ---------------------------------------------------------------------------
     ```
 
 ### Every Open Interest
 
 Below requests to receive continuous updates for every option open interest. This method is only
-available to PRO subscribers.
+available to PRO subscribers. Open Interest is generally reported at 06:30 ET. It is generally not updated during
+the trading day.
 
 === "open_interest_streaming.py"
 
     ```python
     --8<-- "docs/options/open_interest_streaming.py"
     ```
```

### Comparing `thetadata-0.9.5/docs/options/cancel_streams.py` & `thetadata-0.9.6/docs/options/cancel_streams.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/options/eod.py` & `thetadata-0.9.6/docs/options/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/options/get_last.py` & `thetadata-0.9.6/docs/options/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/options/quote_1min.py` & `thetadata-0.9.6/docs/options/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/options/quote_tick.py` & `thetadata-0.9.6/docs/options/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/options/trade_streaming.py` & `thetadata-0.9.6/docs/options/trade_streaming_full.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from datetime import date
-
-from thetadata import ThetaClient, OptionRight, StreamMsg, StreamMsgType
+from thetadata import ThetaClient, StreamMsg, StreamMsgType, StreamResponseType
 
 
 def streaming():
-    # Credentials now required because get_last is only available to ThetaData Standard & Pro subscribers.
+    # Credentials now required because streaming is only available to ThetaData Standard & Pro subscribers.
     client = ThetaClient(username="MyThetaDataEmail", passwd="MyThetaDataPassword")
 
     client.connect_stream(callback)  # You can stop streaming by calling client.close_stream
-    # This contract is likely expired! Replace it with a contract that isn't expired
-    client.req_trade_stream_opt("NVDA", date(2023, 1, 13), 150, OptionRight.CALL)
+    req_id = client.req_full_trade_stream_opt()  # Requests every option trade (async).
+
+    # Verify that the request to stream was successful.
+    response = client.verify(req_id)
+    if response == StreamResponseType.SUBSCRIBED:
+        print('Request to stream full trades successful.')
+    elif response == StreamResponseType.INVALID_PERMS:
+        print('Invalid permissions to stream full trades. Theta Data Options Pro account required.')
+    else:
+        print('Unexpected stream response: ' + str(response))
 
 
 # User generated method that gets called each time a message from the stream arrives.
 def callback(msg: StreamMsg):
     msg.type = msg.type
 
     if msg.type == StreamMsgType.TRADE:
```

### Comparing `thetadata-0.9.5/docs/stocks/eod.py` & `thetadata-0.9.6/docs/stocks/eod.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/stocks/get_last.py` & `thetadata-0.9.6/docs/stocks/get_last.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/stocks/quote_1min.py` & `thetadata-0.9.6/docs/stocks/quote_1min.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/docs/stocks/quote_tick.py` & `thetadata-0.9.6/docs/stocks/quote_tick.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/tests/test_client.py` & `thetadata-0.9.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/tests/test_docs.py` & `thetadata-0.9.6/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/thetadata/client.py` & `thetadata-0.9.6/thetadata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     TickBody,
     ListBody,
     parse_list_REST, parse_flexible_REST, parse_hist_REST, parse_hist_REST_stream, parse_hist_REST_stream_ijson,
 )
 from .terminal import check_download, launch_terminal
 
 _NOT_CONNECTED_MSG = "You must establish a connection first."
-_VERSION = '0.9.5'
+_VERSION = '0.9.6'
 URL_BASE = "http://127.0.0.1:25510/"
 
 
 def _format_strike(strike: float) -> int:
     """Round USD to the nearest tenth of a cent, acceptable by the terminal."""
     return round(strike * 1000)
```

### Comparing `thetadata-0.9.5/thetadata/enums.py` & `thetadata-0.9.6/thetadata/enums.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/thetadata/exceptions.py` & `thetadata-0.9.6/thetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/thetadata/parsing.py` & `thetadata-0.9.6/thetadata/parsing.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/thetadata/terminal.py` & `thetadata-0.9.6/thetadata/terminal.py`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/LICENSE` & `thetadata-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `thetadata-0.9.5/README.md` & `thetadata-0.9.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 The [Thetadata](https://thetadata.net) Python API provides low latency US equities & options data that may be used for
 market research or algorithmic trading applications.
 
 Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) for more details.
 
 ## Installation
 
-Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you.
+Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you. Python 10 or higher is **highly** recommended.
 
 `pip install thetadata`
 
 Please see our [official installation instructions](https://thetadata-api.github.io/thetadata-python/tutorials/#installation)
 to get started.
 
 ## Contributing
```

### Comparing `thetadata-0.9.5/pyproject.toml` & `thetadata-0.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thetadata"
-version = "0.9.5"
+version = "0.9.6"
 authors = [
   { name="Bailey Danseglio", email="bailey@thetadata.net" },
   { name="Adler Weber", email="redacted@thetadata.net" },
 ]
 description = "Python API for Thetadata"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "tqdm",
```

### Comparing `thetadata-0.9.5/PKG-INFO` & `thetadata-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thetadata
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python API for Thetadata
 Project-URL: Homepage, https://thetadata.net
 Project-URL: Source, https://thetadata-api.github.io/thetadata-python/reference/
 Project-URL: Bug Tracker, https://github.com/ThetaData-API/thetadata-python/issues
 Project-URL: Documentation, https://thetadata-api.github.io/thetadata-python/
 Author-email: Bailey Danseglio <bailey@thetadata.net>, Adler Weber <redacted@thetadata.net>
 License: MIT License
@@ -28,15 +28,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Requires-Dist: ijson
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: wget
 Provides-Extra: docs
@@ -54,15 +54,15 @@
 The [Thetadata](https://thetadata.net) Python API provides low latency US equities & options data that may be used for
 market research or algorithmic trading applications.
 
 Please see this repository's [documentation](https://thetadata-api.github.io/thetadata-python) for more details.
 
 ## Installation
 
-Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you.
+Java 11 or higher is required. If you are on Windows, Java 19 will automatically be installed for you. Python 10 or higher is **highly** recommended.
 
 `pip install thetadata`
 
 Please see our [official installation instructions](https://thetadata-api.github.io/thetadata-python/tutorials/#installation)
 to get started.
 
 ## Contributing
```

