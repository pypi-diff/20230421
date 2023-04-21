# Comparing `tmp/SocketSwap-0.1.1-py2.py3-none-any.whl.zip` & `tmp/SocketSwap-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5616 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      436 b- defN 23-Apr-18 19:59 SocketSwap/__init__.py
--rw-rw-rw-  2.0 fat     1146 b- defN 23-Apr-18 19:59 SocketSwap/context_manager.py
+Zip file size: 5949 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      311 b- defN 23-Apr-21 14:15 SocketSwap/__init__.py
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-20 14:11 SocketSwap/context_manager.py
 -rw-rw-rw-  2.0 fat     7907 b- defN 23-Apr-18 19:59 SocketSwap/proxy.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1067 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      642 b- defN 23-Apr-18 20:00 SocketSwap-0.1.1.dist-info/RECORD
-8 files, 12375 bytes uncompressed, 4498 bytes compressed:  63.7%
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1857 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      642 b- defN 23-Apr-21 14:16 SocketSwap-0.1.2.dist-info/RECORD
+8 files, 13042 bytes uncompressed, 4831 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: SocketSwap/context_manager.py
 Comment: 
 
 Filename: SocketSwap/proxy.py
 Comment: 
 
-Filename: SocketSwap-0.1.1.dist-info/LICENSE
+Filename: SocketSwap-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: SocketSwap-0.1.1.dist-info/METADATA
+Filename: SocketSwap-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: SocketSwap-0.1.1.dist-info/WHEEL
+Filename: SocketSwap-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: SocketSwap-0.1.1.dist-info/top_level.txt
+Filename: SocketSwap-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: SocketSwap-0.1.1.dist-info/RECORD
+Filename: SocketSwap-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SocketSwap/__init__.py

```diff
@@ -4,17 +4,12 @@
 SocketSwap is a python package that allows to proxy any third-party libraries traffic through a local TCP Proxy
 """
 
 __version__ = "0.1.0"
 __author__ = 'fyx99'
 __credits__ = 'No credits'
 
-import socketswap.proxy 
-from socketswap.proxy import start_local_proxy
-from socketswap.context_manager import ProxySwapContext
+from SocketSwap.context_manager import SocketSwapContext
 
 __all__ = [
-    socketswap.proxy,
-    start_local_proxy,
-    
-    ProxySwapContext
+    SocketSwapContext
 ]
```

## SocketSwap/context_manager.py

```diff
@@ -5,15 +5,15 @@
 import time
 
 
 # def wrap_start_proxy(args):
 #     start_local_proxy(*args)
 
 
-class ProxySwapContext:
+class SocketSwapContext:
     
     def __init__(self, *args):
         self.args = args
     
     def __enter__(self):
         print("Starting Proxy Server")
         self.proxy_process = multiprocessing.Process(target=start_local_proxy, args=(self.args))
@@ -34,12 +34,12 @@
     remote_socket.connect((target_host, target_port))
     return remote_socket
 
 if __name__ == '__main__':
     # for testing
     
     
-    with ProxySwapContext(conn_factory, "127.0.0.1", 2222):
+    with SocketSwapContext(conn_factory, "127.0.0.1", 2222):
         for i in range(1000):
             print(i)
             time.sleep(3)
```

## Comparing `SocketSwap-0.1.1.dist-info/LICENSE` & `SocketSwap-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SocketSwap-0.1.1.dist-info/RECORD` & `SocketSwap-0.1.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-SocketSwap/__init__.py,sha256=5B8yXcyn0DQIgC5jZMnhZDbgDY4I0DOe3XjaprUhWHI,436
-SocketSwap/context_manager.py,sha256=C_1pM_f9-QgO_AQ-k2UXzuqZjaaRTfjq3VKH-e7vpNA,1146
+SocketSwap/__init__.py,sha256=64HZufssVBc8rthVa3qdXtdh4lnUtVlvYfqnGF8Tvu8,311
+SocketSwap/context_manager.py,sha256=X0LezqjrTxf1UKRwo4f2a0UfTt8uxPOmZ80YE08d_Pc,1148
 SocketSwap/proxy.py,sha256=R8YobQ-TXQJ-WQPoUoSlSlGIuwIsZbOqbadMRwyRygw,7907
-SocketSwap-0.1.1.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
-SocketSwap-0.1.1.dist-info/METADATA,sha256=H-MFfkVPHTfgdFMLKz3ttJ7xOkTMckzQP6Dbdx9DttA,1067
-SocketSwap-0.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-SocketSwap-0.1.1.dist-info/top_level.txt,sha256=sGI9LWTAw3Bu2u37_lcKmZtgzwly_gHlFHYKhZTWVDM,11
-SocketSwap-0.1.1.dist-info/RECORD,,
+SocketSwap-0.1.2.dist-info/LICENSE,sha256=23tRc0wLCYQHwSFTDYEAJnQxRfETM7yum1i0Qhl_lpU,1056
+SocketSwap-0.1.2.dist-info/METADATA,sha256=PpsJnp1pvV9wH5z_VTTzjUW-_8SRmAQBK_sk2ajawtA,1857
+SocketSwap-0.1.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+SocketSwap-0.1.2.dist-info/top_level.txt,sha256=sGI9LWTAw3Bu2u37_lcKmZtgzwly_gHlFHYKhZTWVDM,11
+SocketSwap-0.1.2.dist-info/RECORD,,
```

