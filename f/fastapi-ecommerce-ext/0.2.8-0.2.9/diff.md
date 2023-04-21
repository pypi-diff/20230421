# Comparing `tmp/fastapi_ecommerce_ext-0.2.8.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.2.8.tar", last modified: Thu Apr 20 17:16:55 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.9.tar", last modified: Fri Apr 21 03:12:45 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.2.8.tar` & `fastapi_ecommerce_ext-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0      382 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.660941 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     2874 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      382 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-20 17:16:55.000000 fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 17:16:55.663356 fastapi_ecommerce_ext-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-20 17:11:58.000000 fastapi_ecommerce_ext-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:12:45.134692 fastapi_ecommerce_ext-0.2.9/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:12:45.134692 fastapi_ecommerce_ext-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:12:45.121697 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-21 03:12:45.133693 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     2731 2023-04-21 03:10:31.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:12:45.130692 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:12:45.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-21 03:12:45.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:12:45.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 03:12:45.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-21 03:12:45.000000 fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-21 03:12:45.135198 fastapi_ecommerce_ext-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-21 03:12:43.000000 fastapi_ecommerce_ext-0.2.9/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.2.8/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.8/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.9/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,63 +10,58 @@
 from starlette.responses import Response, JSONResponse
 from starlette.routing import Match
 
 
 class LoguruLoggingMiddleware:
     async def __call__(self, request: Request, call_next: Callable):
         try:
+            await self.log_before_response(request)
             st = time.time()
             response = await call_next(request)
             elapsed = f"{time.time() - st:0.10f} sec"
             response.headers.append("X-Response-Time", elapsed)
         except Exception as e:
             if request.app.debug:
                 logger.exception(e)
             response = JSONResponse(
                 status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
                 content={"detail": f"{e.__class__.__name__} - {e.args}"},
                 media_type="application/json",
             )
-        return await self.http(request, response)
+        return await self.log_after_response(request, response)
 
-    async def http(self, request: Request, response: Response | StreamingResponse):
-        status_color = self.__colorize_response_status(response.status_code)
+    @staticmethod
+    def log_format(request: Request):
+        return f"{request.client.host}:{request.client.port} - {request.method} {request.url}"
+
+    async def log_before_response(self, request: Request):
         msg = (
             f"{request.client.host}:{request.client.port} - "
-            f"{request.method} {request.url} {response.status_code}"
+            f"{request.method} {request.url}"
         )
+        if request.app.debug:
+            headers = []
+            for route in request.app.router.routes:
+                match, scope = route.matches(request)
+                if match == Match.FULL:
+                    for name, value in scope["path_params"].items():
+                        headers.append(f"{name}: {value}")
+            if len(headers) > 0:
+                logger.info(f"- Params: {headers}")
+        logger.info(self.log_format(request))
+        return request
+
+    async def log_after_response(self, request: Request, response: Response | StreamingResponse):
+        msg = self.log_format(request)
         if 500 <= response.status_code <= 599:
             if isinstance(response, StreamingResponse):
                 response_body = [
                     section async for section in response.body_iterator
                 ]
                 response.body_iterator = iterate_in_threadpool(
                     iter(response_body)
                 )
                 msg += f" - response: {response_body[0].decode()}"
             elif isinstance(response, Response):
                 msg += f" - response: {json.loads(response.body)}"
-        if request.app.debug:
-            headers = []
-            for route in request.app.router.routes:
-                match, scope = route.matches(request)
-                if match == Match.FULL:
-                    for name, value in scope["path_params"].items():
-                        headers.append(f"{name}: {value}")
-            if len(headers) > 0:
-                logger.info(f"- Params: {headers}")
         logger.info(msg)
         return response
-
-    @staticmethod
-    def __colorize_response_status(status_code: int):
-        if 200 <= status_code <= 299:
-            color = "light-white"
-        elif 300 <= status_code <= 399:
-            color = "light-magenta"
-        elif 400 <= status_code <= 499:
-            color = "fg 255,150,38"
-        elif 500 <= status_code <= 599:
-            color = "light-red"
-        else:
-            color = "light-white"
-        return color
```

### Comparing `fastapi_ecommerce_ext-0.2.8/setup.py` & `fastapi_ecommerce_ext-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "0.2.8"
+version = "0.2.9"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```

