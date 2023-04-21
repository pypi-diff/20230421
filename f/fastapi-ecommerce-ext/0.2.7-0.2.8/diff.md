# Comparing `tmp/fastapi_ecommerce_ext-0.2.7.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.2.7.tar", last modified: Wed Apr 19 15:59:01 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.8.tar", last modified: Thu Apr 20 17:16:55 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.2.7.tar` & `fastapi_ecommerce_ext-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:59:01.388521 fastapi_ecommerce_ext-0.2.7/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-19 15:59:01.388521 fastapi_ecommerce_ext-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:59:01.376521 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:59:01.387520 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:59:01.385521 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-19 15:59:01.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-19 15:59:01.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:59:01.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-19 15:59:01.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-19 15:59:01.000000 fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-19 15:59:01.389521 fastapi_ecommerce_ext-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-04-19 15:58:57.000000 fastapi_ecommerce_ext-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      382 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.660941 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     2874 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      382 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-20 17:11:58.000000 fastapi_ecommerce_ext-0.2.8/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.2.7/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/configure.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,23 +44,11 @@
         access_log_path,
         serialize=True,
         level=logging_level,
         enqueue=True,
         backtrace=True,
         diagnose=True,
         encoding="UTF-8",
-        rotation="500 MB",
-        retention="14 days",
-        compression="zip",
-    )
-    logger.add(
-        error_log_path,
-        serialize=True,
-        level=logging.ERROR,
-        enqueue=True,
-        backtrace=True,
-        diagnose=True,
-        encoding="UTF-8",
-        rotation="500 MB",
-        retention="14 days",
+        rotation="256 MB",
+        retention="7 days",
         compression="zip",
     )
```

### Comparing `fastapi_ecommerce_ext-0.2.7/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import time
 from typing import Callable
 
 from loguru import logger
 from starlette import status
 from starlette.concurrency import iterate_in_threadpool
-from starlette.middleware.base import _StreamingResponse
+from starlette.middleware.base import StreamingResponse
 from starlette.requests import Request
 from starlette.responses import Response, JSONResponse
 from starlette.routing import Match
 
 
 class LoguruLoggingMiddleware:
     async def __call__(self, request: Request, call_next: Callable):
@@ -24,22 +24,22 @@
             response = JSONResponse(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 content={"detail": f"{e.__class__.__name__} - {e.args}"},
                 media_type="application/json",
             )
         return await self.http(request, response)
 
-    async def http(self, request: Request, response: Response | JSONResponse):
+    async def http(self, request: Request, response: Response | StreamingResponse):
         status_color = self.__colorize_response_status(response.status_code)
         msg = (
             f"{request.client.host}:{request.client.port} - "
             f"{request.method} {request.url} {response.status_code}"
         )
         if 500 <= response.status_code <= 599:
-            if isinstance(response, _StreamingResponse):
+            if isinstance(response, StreamingResponse):
                 response_body = [
                     section async for section in response.body_iterator
                 ]
                 response.body_iterator = iterate_in_threadpool(
                     iter(response_body)
                 )
                 msg += f" - response: {response_body[0].decode()}"
@@ -49,18 +49,16 @@
             headers = []
             for route in request.app.router.routes:
                 match, scope = route.matches(request)
                 if match == Match.FULL:
                     for name, value in scope["path_params"].items():
                         headers.append(f"{name}: {value}")
             if len(headers) > 0:
-                logger.opt(colors=True).info(
-                    f"<{status_color}>- Params: {headers}</{status_color}>"
-                )
-        logger.opt(colors=True).info(f"<{status_color}>{msg}</{status_color}>")
+                logger.info(f"- Params: {headers}")
+        logger.info(msg)
         return response
 
     @staticmethod
     def __colorize_response_status(status_code: int):
         if 200 <= status_code <= 299:
             color = "light-white"
         elif 300 <= status_code <= 399:
```

### Comparing `fastapi_ecommerce_ext-0.2.7/setup.py` & `fastapi_ecommerce_ext-0.2.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "v0.2.7"
+version = "0.2.8"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```

