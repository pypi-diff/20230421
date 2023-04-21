# Comparing `tmp/async_etcd3gw-0.3.tar.gz` & `tmp/async_etcd3gw-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_etcd3gw-0.3.tar", last modified: Wed Apr 19 09:22:21 2023, max compression
+gzip compressed data, was "async_etcd3gw-0.4.tar", last modified: Fri Apr 21 20:57:10 2023, max compression
```

## Comparing `async_etcd3gw-0.3.tar` & `async_etcd3gw-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-19 09:22:21.304426 async_etcd3gw-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/async_etcd3gw/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/async_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/async_etcd3gw/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/async_etcd3gw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:22:21.000000 async_etcd3gw-0.3/async_etcd3gw.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 09:22:21.304426 async_etcd3gw-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:22:21.300426 async_etcd3gw-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/tests/test_async_etcd3gw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 09:21:54.000000 async_etcd3gw-0.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.862848 async_etcd3gw-0.4/async_etcd3gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/async_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/async_etcd3gw/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/async_etcd3gw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:57:10.000000 async_etcd3gw-0.4/async_etcd3gw.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:57:10.866848 async_etcd3gw-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/tests/test_async_etcd3gw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-21 20:56:47.000000 async_etcd3gw-0.4/tests/test_client.py
```

### Comparing `async_etcd3gw-0.3/LICENSE` & `async_etcd3gw-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/PKG-INFO` & `async_etcd3gw-0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_etcd3gw
-Version: 0.3
+Version: 0.4
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
@@ -75,10 +75,12 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
+* [etcd](https://etcd.io)
+* [etcd gRPC API](https://etcd.io/docs/v3.5/learning/api/)
 * [etcd3gw, An etcd3 grpc-gateway v3 API Python client](https://opendev.org/openstack/etcd3gw)
 * [etcd gRPC gateway](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)
 * [AIOHTTP, Asynchronous HTTP Client/Server for asyncio and Python.](https://docs.aiohttp.org/en/stable/)
```

### Comparing `async_etcd3gw-0.3/README.md` & `async_etcd3gw-0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,10 +47,12 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
+* [etcd](https://etcd.io)
+* [etcd gRPC API](https://etcd.io/docs/v3.5/learning/api/)
 * [etcd3gw, An etcd3 grpc-gateway v3 API Python client](https://opendev.org/openstack/etcd3gw)
 * [etcd gRPC gateway](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)
 * [AIOHTTP, Asynchronous HTTP Client/Server for asyncio and Python.](https://docs.aiohttp.org/en/stable/)
```

### Comparing `async_etcd3gw-0.3/async_etcd3gw/__init__.py` & `async_etcd3gw-0.4/async_etcd3gw/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #    https://opendev.org/openstack/etcd3gw/src/tag/2.1.0/etcd3gw/__init__.py
 
 from . import utils
 from .async_client import AsyncEtcd3Client, async_client
 from .async_lease import AsyncLease
 from .async_lock import AsyncLock
 
-__version__ = "0.3"
+__version__ = "0.4"
 
 __all__ = (
     "AsyncEtcd3Client",
     "AsyncLease",
     "AsyncLock",
     "async_client",
     "utils",
```

### Comparing `async_etcd3gw-0.3/async_etcd3gw/async_client.py` & `async_etcd3gw-0.4/async_etcd3gw/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "DEFAULT_API_PATH",
     "DEFAULT_PORT",
     "DEFAULT_PROTOCOL",
 ]
 
 _SORT_ORDER = ["none", "ascend", "descend"]
 _SORT_TARGET = ["key", "version", "create", "mod", "value"]
-DEFAULT_API_PATH = "/v3alpha/"
+DEFAULT_API_PATH = "/v3/"
 DEFAULT_PORT = 2379
 DEFAULT_PROTOCOL = "http"
 
 # gRPC gateway endpoints:
 #
 # - etcd v3.2 or before uses only [CLIENT-URL]/v3alpha/*
 # - etcd v3.3 uses [CLIENT-URL]/v3beta/* while keeping [CLIENT-URL]/v3alpha/*
@@ -66,14 +66,15 @@
         """Construct an client to talk to etcd3's grpc-gateway's /v3 HTTP API
 
         Args:
             host (str): The etcd hostname.
             port (int): The etcd port.
             protocol (str): The etcd protocol (http/https).
             timeout (int): The default timeout.
+            api_path (str): The api path.
         """
         self.host = host
         self.port = port
         self.protocol = protocol
         self.api_path = api_path
 
         if timeout is not None:
```

### Comparing `async_etcd3gw-0.3/async_etcd3gw/async_lease.py` & `async_etcd3gw-0.4/async_etcd3gw/async_lease.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/async_etcd3gw/async_lock.py` & `async_etcd3gw-0.4/async_etcd3gw/async_lock.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/async_etcd3gw/async_watch.py` & `async_etcd3gw-0.4/async_etcd3gw/async_watch.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/async_etcd3gw/exceptions.py` & `async_etcd3gw-0.4/async_etcd3gw/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/async_etcd3gw/utils.py` & `async_etcd3gw-0.4/async_etcd3gw/utils.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/async_etcd3gw.egg-info/PKG-INFO` & `async_etcd3gw-0.4/async_etcd3gw.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-etcd3gw
-Version: 0.3
+Version: 0.4
 Summary: An async Python client for etcd3 grpc-gateway v3 API
 Home-page: https://github.com/DLBD-Department/async_etcd3gw
 Author: Alkemy spa
 Author-email: DLBDDepartment@alkemy.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DLBD-Department/async_etcd3gw/issues
 Project-URL: Source Code, https://github.com/DLBD-Department/async_etcd3gw
@@ -75,10 +75,12 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 ### Links
 
+* [etcd](https://etcd.io)
+* [etcd gRPC API](https://etcd.io/docs/v3.5/learning/api/)
 * [etcd3gw, An etcd3 grpc-gateway v3 API Python client](https://opendev.org/openstack/etcd3gw)
 * [etcd gRPC gateway](https://etcd.io/docs/v3.5/dev-guide/api_grpc_gateway/)
 * [AIOHTTP, Asynchronous HTTP Client/Server for asyncio and Python.](https://docs.aiohttp.org/en/stable/)
```

### Comparing `async_etcd3gw-0.3/setup.cfg` & `async_etcd3gw-0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/tests/test_async_etcd3gw.py` & `async_etcd3gw-0.4/tests/test_async_etcd3gw.py`

 * *Files identical despite different names*

### Comparing `async_etcd3gw-0.3/tests/test_client.py` & `async_etcd3gw-0.4/tests/test_client.py`

 * *Files identical despite different names*

