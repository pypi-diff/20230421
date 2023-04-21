# Comparing `tmp/socket_request-1.1.6-py3-none-any.whl.zip` & `tmp/socket_request-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 26736 bytes, number of entries: 14
+Zip file size: 26752 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1231 b- defN 22-Dec-05 03:00 socket_request/__init__.py
 -rw-r--r--  2.0 unx     1486 b- defN 22-Dec-05 03:05 socket_request/__main__.py
--rw-r--r--  2.0 unx      343 b- defN 23-Mar-29 08:17 socket_request/__version__.py
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 02:59 socket_request/__version__.py
 -rw-r--r--  2.0 unx    11299 b- defN 23-Mar-29 08:16 socket_request/control_chain_cli.py
 -rw-r--r--  2.0 unx    14629 b- defN 23-Mar-27 02:49 socket_request/core/connect_sock.py
 -rw-r--r--  2.0 unx    23349 b- defN 23-Mar-29 08:15 socket_request/core/control_chain.py
--rw-r--r--  2.0 unx     8720 b- defN 22-Sep-30 06:43 socket_request/core/docker_sock.py
+-rw-r--r--  2.0 unx     8865 b- defN 23-Apr-21 02:59 socket_request/core/docker_sock.py
 -rw-r--r--  2.0 unx     6948 b- defN 22-Dec-05 02:40 socket_request/utils/data.py
 -rw-r--r--  2.0 unx    14402 b- defN 23-Mar-29 06:57 socket_request/utils/utils.py
--rw-r--r--  2.0 unx     4389 b- defN 23-Mar-29 08:17 socket_request-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-29 08:17 socket_request-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Mar-29 08:17 socket_request-1.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Mar-29 08:17 socket_request-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1222 b- defN 23-Mar-29 08:17 socket_request-1.1.6.dist-info/RECORD
-14 files, 88197 bytes uncompressed, 24688 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx     4389 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1222 b- defN 23-Apr-21 02:59 socket_request-1.1.7.dist-info/RECORD
+14 files, 88342 bytes uncompressed, 24704 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: socket_request/utils/data.py
 Comment: 
 
 Filename: socket_request/utils/utils.py
 Comment: 
 
-Filename: socket_request-1.1.6.dist-info/METADATA
+Filename: socket_request-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: socket_request-1.1.6.dist-info/WHEEL
+Filename: socket_request-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: socket_request-1.1.6.dist-info/entry_points.txt
+Filename: socket_request-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: socket_request-1.1.6.dist-info/top_level.txt
+Filename: socket_request-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: socket_request-1.1.6.dist-info/RECORD
+Filename: socket_request-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## socket_request/__version__.py

```diff
@@ -1,9 +1,9 @@
 ####
 __title__ = 'socket_request'
 __description__ = 'socket_request is building and parsing HTTP requests with UNIX domain sockets.'
 __url__ = 'https://github.com/jinwoo-j/socket_request'
-__version__ = '1.1.6'
+__version__ = '1.1.7'
 __author__ = 'Jinwoo Jeong'
 __author_email__ = 'jinwoo@parametacorp.com'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2021 JINWOO'
```

## socket_request/core/docker_sock.py

```diff
@@ -15,15 +15,16 @@
             unix_socket="/var/run/docker.sock",
             url="/",
             timeout=5,
             debug=False,
             auto_prepare=False,
             wait_state=False,
             simple_name=True,
-            logger=None
+            logger=None,
+            default_return_keys=[]
 
     ):
         super().__init__(unix_socket=unix_socket, timeout=timeout, debug=debug)
 
         self.return_merged_values = None
         self.url = url
         self.unix_socket = unix_socket
@@ -38,15 +39,18 @@
         self.files = {}
         self.detail = False
         self.debug = debug
         self.simple_name = simple_name
         self.auto_prepare = auto_prepare
         self.wait_state = wait_state
         self.logger = logger
-        self.default_return_keys = ["Image", "State", "Status"]
+        if default_return_keys:
+            self.default_return_keys = default_return_keys
+        else:
+            self.default_return_keys = ["Image", "State", "Status"]
         self.container_list = []
         self.return_keys = list(set(self.default_return_keys) | {"Id", "Names"})
         self.return_lower_keys = [key.lower() for key in self.return_keys]
         self.stats_keys = ["used_memory", "available_memory", "memory_usage", "number_cpus", "cpu_usage"]
         self.columns = self.return_lower_keys + self.stats_keys
```

## Comparing `socket_request-1.1.6.dist-info/METADATA` & `socket_request-1.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: socket-request
-Version: 1.1.6
+Version: 1.1.7
 Summary: socket_request is building and parsing HTTP requests with UNIX domain sockets.
 Home-page: https://github.com/jinwoo-j/socket_request
 Author: Jinwoo Jeong
 Author-email: jinwoo@parametacorp.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: halo (>=0.0.31)
 Requires-Dist: devtools (>=0.6.1)
 Requires-Dist: argparse (>=1.4.0)
 Requires-Dist: requests (>=2.20.0)
-Requires-Dist: pawnlib (==0.1.37)
+Requires-Dist: pawnlib (>=0.1.62)
 
 # socket_request
 
 socket_request is build and parses HTTP requests with unix domain sockets.
 
 ### Installing socket_request
```

