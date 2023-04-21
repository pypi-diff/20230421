# Comparing `tmp/fastapi_ecommerce_ext-0.3.0.tar.gz` & `tmp/fastapi_ecommerce_ext-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.3.0.tar", last modified: Fri Apr 21 03:15:52 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.3.1.tar", last modified: Fri Apr 21 03:18:40 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.3.0.tar` & `fastapi_ecommerce_ext-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:15:52.698911 fastapi_ecommerce_ext-0.3.0/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0      382 2023-04-21 03:15:52.699910 fastapi_ecommerce_ext-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:15:52.687911 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-21 03:15:52.698911 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     2663 2023-04-21 03:15:51.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:15:52.695911 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      382 2023-04-21 03:15:52.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-21 03:15:52.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:15:52.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 03:15:52.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 03:15:52.000000 fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 03:15:52.699910 fastapi_ecommerce_ext-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-21 03:15:51.000000 fastapi_ecommerce_ext-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:18:40.185480 fastapi_ecommerce_ext-0.3.1/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:18:40.185480 fastapi_ecommerce_ext-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:18:40.175478 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-21 03:18:40.184487 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     2650 2023-04-21 03:18:38.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:18:40.182477 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:18:40.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-21 03:18:40.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:18:40.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 03:18:40.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-21 03:18:40.000000 fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-21 03:18:40.186478 fastapi_ecommerce_ext-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-21 03:18:38.000000 fastapi_ecommerce_ext-0.3.1/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.3.0/LICENSE.txt` & `fastapi_ecommerce_ext-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.0/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.3.1/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,20 +49,20 @@
             if len(headers) > 0:
                 logger.info(f"- Params: {headers}")
         logger.info(self.log_format(request))
         return request
 
     @staticmethod
     async def log_after_response(request: Request, response: Response | StreamingResponse):
-        msg = ""
+        msg = " - response: "
         if isinstance(response, StreamingResponse):
             response_body = [
                 section async for section in response.body_iterator
             ]
             response.body_iterator = iterate_in_threadpool(
                 iter(response_body)
             )
-            msg += f" - response: {response_body[0].decode()}"
+            msg += f"{response_body[0].decode()}"
         elif isinstance(response, Response):
-            msg += f" - response: {json.loads(response.body)}"
+            msg += f"{json.loads(response.body)}"
         logger.info(msg)
         return response
```

### Comparing `fastapi_ecommerce_ext-0.3.0/setup.py` & `fastapi_ecommerce_ext-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "0.3.0"
+version = "0.3.1"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```

