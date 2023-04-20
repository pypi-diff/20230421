# Comparing `tmp/lager-0.3.0-py3-none-any.whl.zip` & `tmp/lager-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5309 bytes, number of entries: 10
--rw-r--r--  2.0 fat      519 b- defN 80-Jan-01 00:00 lager/__init__.py
+Zip file size: 5272 bytes, number of entries: 10
+-rw-r--r--  2.0 fat      580 b- defN 80-Jan-01 00:00 lager/__init__.py
 -rw-r--r--  2.0 fat      335 b- defN 80-Jan-01 00:00 lager/_version.py
--rw-r--r--  2.0 fat     1224 b- defN 80-Jan-01 00:00 lager/const.py
--rw-r--r--  2.0 fat     3252 b- defN 80-Jan-01 00:00 lager/core.py
--rw-r--r--  2.0 fat     1344 b- defN 80-Jan-01 00:00 lager/httpx.py
--rw-r--r--  2.0 fat      991 b- defN 80-Jan-01 00:00 lager/pydantic.py
--rw-r--r--  2.0 fat     1056 b- defN 80-Jan-01 00:00 lager-0.3.0.dist-info/LICENSE
-?rw-r--r--  2.0 fat       83 b- defN 16-Jan-01 00:00 lager-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat      511 b- defN 16-Jan-01 00:00 lager-0.3.0.dist-info/METADATA
-?rw-r--r--  2.0 fat      716 b- defN 16-Jan-01 00:00 lager-0.3.0.dist-info/RECORD
-10 files, 10031 bytes uncompressed, 4115 bytes compressed:  59.0%
+-rw-r--r--  2.0 fat     1092 b- defN 80-Jan-01 00:00 lager/const.py
+-rw-r--r--  2.0 fat     3195 b- defN 80-Jan-01 00:00 lager/core.py
+-rw-r--r--  2.0 fat     1290 b- defN 80-Jan-01 00:00 lager/httpx.py
+-rw-r--r--  2.0 fat      997 b- defN 80-Jan-01 00:00 lager/pydantic.py
+-rw-r--r--  2.0 fat     1056 b- defN 80-Jan-01 00:00 lager-0.4.0.dist-info/LICENSE
+?rw-r--r--  2.0 fat       83 b- defN 16-Jan-01 00:00 lager-0.4.0.dist-info/WHEEL
+?rw-r--r--  2.0 fat      511 b- defN 16-Jan-01 00:00 lager-0.4.0.dist-info/METADATA
+?rw-r--r--  2.0 fat      716 b- defN 16-Jan-01 00:00 lager-0.4.0.dist-info/RECORD
+10 files, 9855 bytes uncompressed, 4078 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: lager/httpx.py
 Comment: 
 
 Filename: lager/pydantic.py
 Comment: 
 
-Filename: lager-0.3.0.dist-info/LICENSE
+Filename: lager-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: lager-0.3.0.dist-info/WHEEL
+Filename: lager-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: lager-0.3.0.dist-info/METADATA
+Filename: lager-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: lager-0.3.0.dist-info/RECORD
+Filename: lager-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lager/__init__.py

```diff
@@ -4,21 +4,26 @@
     VERSION_INFO,
     VERSION_MAJOR,
     VERSION_MINOR,
     VERSION_PATCH,
     __version__,
 )
 from lager.const import LAGER_PORT, LOGURU_DEFAULT_FMT, TORNADO_FMT
-from lager.core import LN, LOG, flog, handlers, ln, log, loglevel
+from lager.core import LN, LOG, flog, handlers, ln, log, logger, loglevel
 
 
 __all__ = [
     'LAGER_PORT',
     'VERSION_MAJOR',
     'VERSION_MINOR',
     'VERSION_PATCH',
     'VERSION_INFO',
     '__version__',
     'LOGURU_DEFAULT_FMT',
     'TORNADO_FMT',
-    'loglevel'
-    ]
+    'loglevel',
+    'logger',
+    'LOG',
+    'log',
+    'LN',
+    'ln',
+]
```

## lager/_version.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """`lager` version"""
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH = [int(el) for el in __version__.split('.')]
 VERSION_INFO = (VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH)
 
 __all__ = [
     "VERSION_MAJOR",
     "VERSION_MINOR",
     "VERSION_PATCH",
```

## lager/const.py

```diff
@@ -1,53 +1,53 @@
 # -*- coding: utf-8 -*-
 """Constants go here!"""
 LAGER_PORT = 52437
 
-TORNADO_FMT= "".join(
+TORNADO_FMT = "".join(
     [
         "<level>",
         "[{level.name[0]} ",
         "{time:YYMMDDTHH:mm:ss} ",
         "{name}:{module}:{line}]",
         "</level> ",
         "{message}",
-        ]
-    )
+    ]
+)
 
 LOGURU_DEFAULT_FMT = "".join(
     [
         "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green>",
         " | ",
         "<level>{level: <8}</level>",
         " | ",
         "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan>",
         " - ",
         "<level>{message}</level>",
-        ]
-    )
+    ]
+)
 
 LOG_LEVELS = {
-    "notset"  : "NOTSET",
-    "n"       : "NOTSET",
-    "debug"   : "DEBUG",
-    "d"       : "DEBUG",
-    "info"    : "INFO",
-    "i"       : "INFO",
-    "s"       : "SUCCESS",
-    "success" : "SUCCESS",
-    "warning" : "WARNING",
-    "warn"    : "WARNING",
-    "w"       : "WARNING",
-    "error"   : "ERROR",
-    "e"       : "ERROR",
+    "notset": "NOTSET",
+    "n": "NOTSET",
+    "debug": "DEBUG",
+    "d": "DEBUG",
+    "info": "INFO",
+    "i": "INFO",
+    "s": "SUCCESS",
+    "success": "SUCCESS",
+    "warning": "WARNING",
+    "warn": "WARNING",
+    "w": "WARNING",
+    "error": "ERROR",
+    "e": "ERROR",
     "critical": "CRITICAL",
-    "fatal"   : "CRITICAL",
-    "c"       : "CRITICAL",
+    "fatal": "CRITICAL",
+    "c": "CRITICAL",
     # enum/enum-strings
-    "0"       : "NOTSET",
-    "10"      : "DEBUG",
-    "20"      : "INFO",
-    "25"      : "SUCCESS",
-    "30"      : "WARNING",
-    "40"      : "ERROR",
-    "50"      : "CRITICAL",
-    }
+    "0": "NOTSET",
+    "10": "DEBUG",
+    "20": "INFO",
+    "25": "SUCCESS",
+    "30": "WARNING",
+    "40": "ERROR",
+    "50": "CRITICAL",
+}
```

## lager/core.py

```diff
@@ -7,24 +7,15 @@
 from typing import Union
 
 from loguru import logger
 
 from lager.const import LOG_LEVELS
 
 
-__all__ = [
-    'loglevel',
-    'flog',
-    'handlers',
-    'logger',
-    'log',
-    'LOG',
-    'ln',
-    'LN'
-    ]
+__all__ = ['loglevel', 'flog', 'handlers', 'logger', 'log', 'LOG', 'ln', 'LN']
 
 logger.t = logger.trace
 logger.d = logger.debug
 logger.i = logger.info
 logger.s = logger.success
 logger.w = logger.warning
 logger.e = logger.error
@@ -38,14 +29,15 @@
 LN = logger
 
 
 def loglevel(level: Union[str, int]) -> str:
     """Convert log-level abrev to a valid loguru log level"""
     return LOG_LEVELS[str(level).strip("'").strip('"').lower()]
 
+
 def flog(funk=None, level="debug", enter=True, exit=True):
     """Log function (sync/async) enter and exit using this decorator
 
     Args:
         funk (Callable): Function to decorate
         level (Union[int, str]): Log level
         enter (bool): Log function entry if True
@@ -66,72 +58,68 @@
         async def add_async(a, b):
             return a + b
         import asyncio
         asyncio.run(add_async(1, 4))
 
     """
 
-
     def _flog(funk):
         name = funk.__name__
 
-
         @wraps(funk)
         def _flog_decorator(*args, **kwargs):
             logger_ = logger.opt(depth=1)
             if enter:
                 logger_.log(
                     loglevel(level),
                     "FLOG-ENTER > '{}' (args={}, kwargs={})",
                     name,
                     args,
                     kwargs,
-                    )
+                )
             ti = time()
             result = funk(*args, **kwargs)
             tf = time()
             if exit:
                 logger_.log(
                     loglevel(level),
                     "FLOG-EXIT < '{}' (return={}, dt_sec={})",
                     name,
                     result,
                     tf - ti,
-                    )
+                )
             return result
 
-
         @wraps(funk)
         async def _flog_decorator_async(*args, **kwargs):
             logger_ = logger.opt(depth=7)
             if enter:
                 logger_.log(
                     loglevel(level),
                     "FLOG-ENTER > '{}' (args={}, kwargs={})",
                     name,
                     args,
                     kwargs,
-                    )
+                )
             ti = time()
             result = await funk(*args, **kwargs)
             tf = time()
             if exit:
                 logger_.log(
                     loglevel(level),
                     "FLOG-EXIT < '{}' (return={}, dt_sec={})",
                     name,
                     result,
                     tf - ti,
-                    )
+                )
             return result
 
-
         if asyncio.iscoroutinefunction(funk) or asyncio.iscoroutine(funk):
             return _flog_decorator_async
         return _flog_decorator
 
-
     return _flog(funk) if funk else _flog
 
+
 def handlers():
     """Return all handlers"""
     return logger._core.handlers
```

## lager/httpx.py

```diff
@@ -6,47 +6,41 @@
 import httpx
 
 
 SINKS = []
 
 
 class HttpxSink(object):
-
-
     def __init__(self, url, *args, **kwargs):
         self.url = url
         self.client = httpx.AsyncClient(*args, **kwargs)
         SINKS.append(self)
 
-
     async def __call__(self, msg):
         print(msg)
-        httpx.post(self.url, data={
-            'msg': msg
-            })
+        httpx.post(self.url, data={'msg': msg})
 
     async def handle(self, message):
         print('async handling', message)
         print(self.url, self.client)
         print(dir(self.client))
         # async with self.client as c:
         #     await c.post(url=self.url, data={'msg': message})
-        await self.client.post(url=self.url, data={
-            'msg': message
-            })
-
+        await self.client.post(url=self.url, data={'msg': message})
 
     async def await_delete_channels(self):
         await self.client.aclose()
 
     # @atexit.register
     # def shutdown(self):
     #     print("Shutting down")
     #     loop = asyncio.get_event_loop()
     #     loop.run_until_complete(self.await_delete_channels())
+
+
 #
 # @atexit.register
 # def shutdown():
 #     print("Shutting down")
 #
 #
 #     async def _shutdown():
```

## lager/pydantic.py

```diff
@@ -7,32 +7,37 @@
 from jsonbourne.pydantic import JsonBaseModel
 
 
 class RecordFile(JsonBaseModel):
     name: str
     path: str
 
+
 class RecordLevel(JsonBaseModel):
     name: str
     no: int
     icon: str
 
+
 class RecordThread(JsonBaseModel):
     id: int
     name: str
 
+
 class RecordProcess(JsonBaseModel):
     id: int
     name: str
 
+
 class RecordException(JsonBaseModel):
     type: Optional[Type[BaseException]]
     value: Optional[BaseException]
     traceback: Optional[TracebackType]
 
+
 class Record(JsonBaseModel):
     elapsed: timedelta
     exception: Optional[RecordException]
     extra: dict
     file: RecordFile
     function: str
     level: RecordLevel
@@ -40,9 +45,10 @@
     message: str
     module: str
     name: Union[str, None]
     process: RecordProcess
     thread: RecordThread
     time: datetime
 
+
 class Message(JsonBaseModel):
     record: Record
```

## Comparing `lager-0.3.0.dist-info/LICENSE` & `lager-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

