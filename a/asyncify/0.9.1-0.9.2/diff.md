# Comparing `tmp/asyncify-0.9.1.tar.gz` & `tmp/asyncify-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncify-0.9.1.tar", max compression
+gzip compressed data, was "asyncify-0.9.2.tar", max compression
```

## Comparing `asyncify-0.9.1.tar` & `asyncify-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      591 2022-05-03 21:42:23.468562 asyncify-0.9.1/asyncify/__init__.py
--rw-r--r--   0        0        0      237 2022-02-04 21:32:32.115440 asyncify-0.9.1/asyncify/__main__.py
--rw-r--r--   0        0        0      819 2022-02-04 21:32:32.113814 asyncify-0.9.1/asyncify/_anyio.py
--rw-r--r--   0        0        0      192 2022-05-17 17:10:23.571412 asyncify-0.9.1/asyncify/_meta.py
--rw-r--r--   0        0        0      545 2022-02-04 21:32:32.116593 asyncify-0.9.1/asyncify/aios/__init__.py
--rw-r--r--   0        0        0      609 2022-02-04 21:32:32.115440 asyncify-0.9.1/asyncify/aios/_path.py
--rw-r--r--   0        0        0     9378 2022-05-03 21:42:23.468562 asyncify-0.9.1/asyncify/core.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.792943 asyncify-0.9.1/asyncify/py.typed
--rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.412347 asyncify-0.9.1/LICENSE
--rw-r--r--   0        0        0     1762 2022-05-17 17:10:00.118023 asyncify-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1049 2022-05-03 21:42:21.323730 asyncify-0.9.1/README.md
--rw-r--r--   0        0        0     1834 2022-05-17 17:10:39.523637 asyncify-0.9.1/setup.py
--rw-r--r--   0        0        0     2040 2022-05-17 17:10:39.523637 asyncify-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-04-20 23:19:54.379920 asyncify-0.9.2/asyncify/__about__.py
+-rw-r--r--   0        0        0      595 2023-04-20 20:51:48.590192 asyncify-0.9.2/asyncify/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-20 20:51:48.619562 asyncify-0.9.2/asyncify/__main__.py
+-rw-r--r--   0        0        0      819 2022-02-04 21:32:32.113814 asyncify-0.9.2/asyncify/_anyio.py
+-rw-r--r--   0        0        0      355 2023-04-20 20:38:23.571136 asyncify-0.9.2/asyncify/_meta.py
+-rw-r--r--   0        0        0      545 2022-02-04 21:32:32.116593 asyncify-0.9.2/asyncify/aios/__init__.py
+-rw-r--r--   0        0        0      609 2022-02-04 21:32:32.115440 asyncify-0.9.2/asyncify/aios/_path.py
+-rw-r--r--   0        0        0     9771 2023-03-31 17:46:06.855340 asyncify-0.9.2/asyncify/core.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.792943 asyncify-0.9.2/asyncify/py.typed
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.412347 asyncify-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2063 2023-04-20 23:19:49.647811 asyncify-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1052 2022-09-19 18:35:16.980214 asyncify-0.9.2/README.md
+-rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 asyncify-0.9.2/PKG-INFO
```

### Comparing `asyncify-0.9.1/asyncify/_anyio.py` & `asyncify-0.9.2/asyncify/_anyio.py`

 * *Files identical despite different names*

### Comparing `asyncify-0.9.1/asyncify/aios/__init__.py` & `asyncify-0.9.2/asyncify/aios/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncify-0.9.1/asyncify/aios/_path.py` & `asyncify-0.9.2/asyncify/aios/_path.py`

 * *Files identical despite different names*

### Comparing `asyncify-0.9.1/asyncify/core.py` & `asyncify-0.9.2/asyncify/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """Asyncify core"""
 
 import asyncio
-import sys
+import warnings
 
 from asyncio import AbstractEventLoop, get_event_loop, run as asyncio_run
 from functools import partial, wraps
 from inspect import isawaitable
 
 from xtyping import (
     TYPE_CHECKING,
@@ -116,14 +116,16 @@
     loop: Optional[AbstractEventLoop] = None,
     executor: Optional[Any] = None,
 ) -> Callable[P, Awaitable[T]]:
     """Makes a sync function async
 
     Args:
         funk: Function to make into an async coroutine
+        loop: Event loop in which to run/execute
+        executor: Executor to with which to execute
 
     Returns:
         An asynchronous function
 
     Examples:
         >>> from asyncify import asyncify
         >>> def add(a, b):
@@ -194,39 +196,48 @@
             loop.set_debug(debug)  # pragma: no cover
         return loop.run_until_complete(aw)
     finally:
         loop.close()
         asyncio.set_event_loop(None)
 
 
-def run(aw: Awaitable[T], *, debug: Optional[bool] = None, **kwargs: Any) -> T:
+def run(
+    aw: Coroutine[Any, Any, T], *, debug: Optional[bool] = None, **kwargs: Any
+) -> T:
     """Run an async/awaitable function (Polyfill asyncio.run)
 
     Emulate `asyncio.run()` for snakes below python 3.7; `asyncio.run` was
     added in python3.7.
 
     Args:
         aw (Awaitable[T]): Async/awaitable function to run
         debug (Optional[bool]): If True run event loop in debug mode
+        **kwargs: keyword arguments to be passed to the wrapped function
 
     Returns:
         T: Return the result of running the async function
 
     Examples:
         >>> async def add(a, b):
         ...     return a + b
         ...
         >>> from asyncify.core import run
         >>> run(add(1, 4))
         5
 
     """
-    if sys.version_info >= (3, 7):
-        return asyncio.run(aw, debug=debug)
-    return _run(aw=aw, debug=debug)  # pragma: no cover
+    # If python is 3.6
+    if not hasattr(asyncio, "run"):  # pragma: no cover
+        warnings.warn(
+            "asyncify no longer supports python3.6...",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return _run(aw, debug=debug)
+    return asyncio_run(aw, debug=debug)
 
 
 def is_async(obj: Any) -> bool:
     """Return True if function/object is async/awaitable
 
     Args:
         obj: Object (probably a function) that could be async
@@ -315,20 +326,23 @@
         raise ValueError(
             f"anyio not installed, backend must be 'asyncio' not '{backend}'"
         )
     _backend_options = backend_options or {}
     _debug = _backend_options.get("debug", False)
     if callable(awaitable_or_func) and not asyncio.iscoroutine(awaitable_or_func):
         return asyncio_run(
-            cast(Awaitable[T_Retval], awaitable_or_func(*args)), debug=_debug
+            awaitable_or_func(*args),
+            debug=_debug,
         )
 
     if args:
         raise ValueError("args must be empty when calling a coroutine")
-    return asyncio_run(cast(Awaitable[T_Retval], awaitable_or_func), debug=_debug)
+    return asyncio_run(
+        cast(Coroutine[Any, Any, T_Retval], awaitable_or_func), debug=_debug
+    )
 
 
 def aiorun(
     awaitable_or_func: Union[
         Awaitable[T_Retval], Callable[..., Coroutine[Any, Any, T_Retval]]
     ],
     *args: object,
@@ -342,11 +356,11 @@
         if not ANYIO
         else aiorun_anyio(
             awaitable_or_func, *args, backend=backend, backend_options=backend_options
         )
     )
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     import doctest
 
     doctest.testmod()
```

### Comparing `asyncify-0.9.1/LICENSE` & `asyncify-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncify-0.9.1/README.md` & `asyncify-0.9.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 
 **TLDR:** Sync 2 Async decorator
 
 **Install:** `pip install asyncify`
 
 **Usage:**
 
-
-
 ```python
 import asyncify
+
 # OR
 from asyncify import asyncify
 from asyncify import run  # asyncio.run polyfill for python36
 
+
 def add(a, b):
     return a + b
 
+
 assert add(1, 2) == 3
 
+
 @asyncify
 def add_async(a, b):
     return a + b
 
+
 res = await add_async(1, 2)
 assert res == 3
 ```
```

### Comparing `asyncify-0.9.1/PKG-INFO` & `asyncify-0.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: asyncify
-Version: 0.9.1
+Version: 0.9.2
 Summary: sync 2 async
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/asyncify
 License: MIT
 Keywords: async,asyncify,asyncio,dgpy
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: funkify (>=0.4.0,<0.5.0)
 Requires-Dist: xtyping (>=0.5.0)
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
@@ -37,28 +41,31 @@
 
 **TLDR:** Sync 2 Async decorator
 
 **Install:** `pip install asyncify`
 
 **Usage:**
 
-
-
 ```python
 import asyncify
+
 # OR
 from asyncify import asyncify
 from asyncify import run  # asyncio.run polyfill for python36
 
+
 def add(a, b):
     return a + b
 
+
 assert add(1, 2) == 3
 
+
 @asyncify
 def add_async(a, b):
     return a + b
 
+
 res = await add_async(1, 2)
 assert res == 3
 ```
```

