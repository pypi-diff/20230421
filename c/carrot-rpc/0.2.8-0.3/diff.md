# Comparing `tmp/carrot_rpc-0.2.8-py3-none-any.whl.zip` & `tmp/carrot_rpc-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 5355 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       60 b- defN 21-Oct-28 14:23 carrot/__init__.py
--rw-rw-r--  2.0 unx     6054 b- defN 22-Oct-25 20:19 carrot/carrot.py
--rw-r--r--  2.0 unx     1094 b- defN 22-Oct-25 20:21 carrot_rpc-0.2.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4052 b- defN 22-Oct-25 20:21 carrot_rpc-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-25 20:21 carrot_rpc-0.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 22-Oct-25 20:21 carrot_rpc-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      546 b- defN 22-Oct-25 20:21 carrot_rpc-0.2.8.dist-info/RECORD
-7 files, 11905 bytes uncompressed, 4385 bytes compressed:  63.2%
+Zip file size: 6978 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx       58 b- defN 23-Apr-21 07:11 carrot/__init__.py
+-rwxr-xr-x  2.0 unx     6054 b- defN 22-Oct-25 20:19 carrot/carrot.py
+-rw-rw-r--  2.0 unx     5866 b- defN 23-Apr-21 07:17 carrot/src.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-Apr-21 07:20 carrot_rpc-0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3915 b- defN 23-Apr-21 07:20 carrot_rpc-0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 07:20 carrot_rpc-0.3.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx        7 b- defN 23-Apr-21 07:20 carrot_rpc-0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      606 b- defN 23-Apr-21 07:20 carrot_rpc-0.3.dist-info/RECORD
+8 files, 17692 bytes uncompressed, 5926 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: carrot/__init__.py
 Comment: 
 
 Filename: carrot/carrot.py
 Comment: 
 
-Filename: carrot_rpc-0.2.8.dist-info/LICENSE
+Filename: carrot/src.py
 Comment: 
 
-Filename: carrot_rpc-0.2.8.dist-info/METADATA
+Filename: carrot_rpc-0.3.dist-info/LICENSE
 Comment: 
 
-Filename: carrot_rpc-0.2.8.dist-info/WHEEL
+Filename: carrot_rpc-0.3.dist-info/METADATA
 Comment: 
 
-Filename: carrot_rpc-0.2.8.dist-info/top_level.txt
+Filename: carrot_rpc-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: carrot_rpc-0.2.8.dist-info/RECORD
+Filename: carrot_rpc-0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: carrot_rpc-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carrot/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .carrot import Carrot
-from .carrot import carrot_ask
+from .src import CarrotCall
+from .src import carrot_ask
```

## Comparing `carrot_rpc-0.2.8.dist-info/LICENSE` & `carrot_rpc-0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `carrot_rpc-0.2.8.dist-info/METADATA` & `carrot_rpc-0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: carrot-rpc
-Version: 0.2.8
+Version: 0.3
 Summary: Carrot-RPC it is a python asyncio RPC server/client for RabbitMQ with pydantic schema that allows you to make RPC calls.
 Home-page: https://github.com/Sobolev5/carrot-rpc
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiormq (>=6.4.2)
-Requires-Dist: simple-print (>=1.4.7)
+Requires-Dist: simple-print (>=1.7.0)
 Requires-Dist: orjson (>=3.8.0)
 Requires-Dist: pydantic (>=1.10.2)
 
 # Carrot
 Carrot-RPC it is a python asyncio RPC server/client for RabbitMQ that allows you to make RPC calls.  
 *Note:* This project in active development and can be unstable.  
 You can see live example here: http://5.187.4.179:5888/
@@ -34,15 +34,15 @@
 ```
 
 
 ## Microservice A which call
 
 ```python
 import asyncio
-from carrot import Carrot
+from carrot import CarrotCall
 from simple_print import sprint
 
 # set amqp connection:
 AMQP_URI = "amqp://admin:password@127.0.0.1/vhost"
 
 # defer function which call «MICROSERVICE_SUM»:
 async def call_sum_a_and_b():
@@ -50,22 +50,22 @@
     # make dict request:
     dct = {}
     dct["caller"] = "Function on microservice_interface which call RPC in microservice_sum"
     dct["number_a"] = int(data["number_a"])
     dct["number_b"] = int(data["number_b"])
 
     # defer carrot instance and make rpc call:
-    carrot = await Carrot(AMQP_URI).connect()
+    carrot = await CarrotCall(AMQP_URI).connect()
     response_from_another_microservice = await carrot.call(dct, "microservice_sum:sum_a_and_b", timeout=5)    
     # first arg is dict with data
     # second arg it routing key (through default AMQP exchange) 
     # third arg is optional (response timeout in seconds, 5 seconds by default) 
 
     # get response dict from microservice «MICROSERVICE_SUM»
-    sprint(f'Sum a and b: {response_from_another_microservice["sum"]}', c="yellow", p=1, f=1)
+    sprint(f'Sum a and b: {response_from_another_microservice["sum"]}', c="yellow")
 
     # you can send request to another microservice without reply (like standart call):
     await carrot.call(dct, "microservice_sum:sum_a_and_b", without_reply=True)
     # in this case «MICROSERVICE_SUM» just calculate sum and do not send response to caller.   
 
 
 loop = asyncio.get_event_loop()
@@ -94,25 +94,25 @@
     caller: str
     number_a: int
     number_b: int
 
 # decorate called function with pydantic schema
 @carrot_ask(SumAAndB)
 async def sum_a_and_b(incoming_dict: dict) -> dict:
-    sprint(incoming_dict, c="yellow", p=1, f=1)
+    sprint(incoming_dict, c="green")
     dct = {}
     dct["caller"] = "i am sum_a_and_b function mounted on microservice_sum"
     dct["sum"] = incoming_dict["number_a"] + incoming_dict["number_b"]
     return dct
 
 # make amqp router:
 async def amqp_router():
     connection = await aiormq.connect(AMQP_URI)
     channel = await connection.channel()
-    sprint(f"AMQP:     ready [yes]", c="green", p=1, f=1)
+    sprint(f"AMQP:     ready [yes]", c="green")
     sum_a_and_b__declared = await channel.queue_declare(f"microservice_sum:sum_a_and_b", durable=False)
     await channel.basic_consume(sum_a_and_b__declared.queue, sum_a_and_b, no_ack=False)  
     
 
 class App(FastAPI):
     def __init__(self, *args, **kwargs):
         loop = asyncio.get_event_loop()
@@ -120,22 +120,20 @@
         super().__init__(*args, **kwargs)
 
 app = App()
 
 ```
 
 ## Full working example with docker-compose
-https://github.com/Sobolev5/FastAPI-plus-RabbitMQ
+https://github.com/Sobolev5/Carrot-RPC-Example
 
 
 ## TODO
 tests, docstrings, extended documentation
 
 
-# Try my free time tracker
-My free time tracker for developers [Workhours.space](https://workhours.space/).
```

