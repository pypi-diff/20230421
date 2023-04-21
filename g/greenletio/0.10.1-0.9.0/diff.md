# Comparing `tmp/greenletio-0.10.1.tar.gz` & `tmp/greenletio-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenletio-0.10.1.tar", last modified: Fri Apr 21 19:27:28 2023, max compression
+gzip compressed data, was "/home/miguelgrinberg/Documents/dev/greenletio/dist/tmp4gzf851z/greenletio-0.9.0.tar", last modified: Wed Aug 18 08:44:38 2021, max compression
```

## Comparing `greenletio-0.10.1.tar` & `greenletio-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,26 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.351567 greenletio-0.10.1/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2020-07-15 11:38:09.000000 greenletio-0.10.1/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2070 2023-04-21 19:27:28.351809 greenletio-0.10.1/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1480 2021-06-06 19:25:27.000000 greenletio-0.10.1/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-03 11:04:26.000000 greenletio-0.10.1/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      779 2023-04-21 19:27:28.352913 greenletio-0.10.1/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-06-03 11:06:28.000000 greenletio-0.10.1/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.325259 greenletio-0.10.1/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.334068 greenletio-0.10.1/src/greenletio/
--rw-r--r--   0 mgrinberg   (502) staff       (20)      113 2021-08-21 22:51:28.000000 greenletio-0.10.1/src/greenletio/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     4627 2023-04-21 19:15:19.000000 greenletio-0.10.1/src/greenletio/core.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.344603 greenletio-0.10.1/src/greenletio/green/
--rw-r--r--   0 mgrinberg   (502) staff       (20)        0 2020-08-03 12:52:37.000000 greenletio-0.10.1/src/greenletio/green/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     9129 2021-06-02 16:15:09.000000 greenletio-0.10.1/src/greenletio/green/socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6623 2020-08-02 10:58:40.000000 greenletio-0.10.1/src/greenletio/green/ssl.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    10269 2023-04-21 17:17:03.000000 greenletio-0.10.1/src/greenletio/green/threading.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      244 2020-08-02 11:00:27.000000 greenletio-0.10.1/src/greenletio/green/time.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      639 2021-08-21 22:51:28.000000 greenletio-0.10.1/src/greenletio/io.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2645 2021-08-21 22:51:28.000000 greenletio-0.10.1/src/greenletio/patcher.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)      618 2022-11-27 23:39:05.000000 greenletio-0.10.1/src/greenletio/run.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1425 2023-04-21 18:34:41.000000 greenletio-0.10.1/src/greenletio/x.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.338956 greenletio-0.10.1/src/greenletio.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2070 2023-04-21 19:27:28.000000 greenletio-0.10.1/src/greenletio.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      675 2023-04-21 19:27:28.000000 greenletio-0.10.1/src/greenletio.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2023-04-21 19:27:28.000000 greenletio-0.10.1/src/greenletio.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-03 11:07:00.000000 greenletio-0.10.1/src/greenletio.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)        9 2023-04-21 19:27:28.000000 greenletio-0.10.1/src/greenletio.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       11 2023-04-21 19:27:28.000000 greenletio-0.10.1/src/greenletio.egg-info/top_level.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2023-04-21 19:27:28.350638 greenletio-0.10.1/tests/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     5682 2023-04-21 18:41:52.000000 greenletio-0.10.1/tests/test_core.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2869 2020-08-02 22:55:41.000000 greenletio-0.10.1/tests/test_patcher.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2677 2021-08-21 22:51:28.000000 greenletio-0.10.1/tests/test_socket.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     2510 2021-08-21 22:51:28.000000 greenletio-0.10.1/tests/test_ssl.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)     6664 2021-08-21 22:51:28.000000 greenletio-0.10.1/tests/test_threading.py
+drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-08-18 08:44:38.000000 greenletio-0.9.0/
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1072 2020-08-01 12:06:03.000000 greenletio-0.9.0/LICENSE
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2106 2021-08-18 08:44:38.000000 greenletio-0.9.0/PKG-INFO
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     1480 2021-06-09 09:38:10.000000 greenletio-0.9.0/README.md
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      104 2021-06-09 09:38:10.000000 greenletio-0.9.0/pyproject.toml
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      778 2021-08-18 08:44:38.000000 greenletio-0.9.0/setup.cfg
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)       38 2021-06-09 09:38:10.000000 greenletio-0.9.0/setup.py
+drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/
+drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio/
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      113 2021-08-18 07:49:22.000000 greenletio-0.9.0/src/greenletio/__init__.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     3953 2021-08-18 07:49:22.000000 greenletio-0.9.0/src/greenletio/core.py
+drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio/green/
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-06-09 09:38:10.000000 greenletio-0.9.0/src/greenletio/green/__init__.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     9129 2021-06-09 09:38:10.000000 greenletio-0.9.0/src/greenletio/green/socket.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     6623 2021-06-09 09:38:10.000000 greenletio-0.9.0/src/greenletio/green/ssl.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)    10288 2021-08-18 07:58:11.000000 greenletio-0.9.0/src/greenletio/green/threading.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      244 2021-06-09 09:38:10.000000 greenletio-0.9.0/src/greenletio/green/time.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      639 2021-08-18 07:49:22.000000 greenletio-0.9.0/src/greenletio/io.py
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2645 2021-08-12 22:53:12.000000 greenletio-0.9.0/src/greenletio/patcher.py
+drwxr-xr-x   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        0 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)     2106 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/PKG-INFO
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)      529 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/SOURCES.txt
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        1 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/dependency_links.txt
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        1 2021-08-08 13:16:16.000000 greenletio-0.9.0/src/greenletio.egg-info/not-zip-safe
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)        9 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/requires.txt
+-rw-r--r--   0 miguelgrinberg  (1000) miguelgrinberg  (1000)       11 2021-08-18 08:44:38.000000 greenletio-0.9.0/src/greenletio.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `greenletio-0.10.1/LICENSE` & `greenletio-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/PKG-INFO` & `greenletio-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: greenletio
-Version: 0.10.1
+Version: 0.9.0
 Summary: Asyncio integration with sync code using greenlets.
 Home-page: https://github.com/miguelgrinberg/greenletio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/greenletio/issues
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,7 +72,9 @@
 
 ## Resources
 
 - [Documentation](http://greenletio.readthedocs.io/en/latest/)
 - [PyPI](https://pypi.python.org/pypi/greenletio)
 - [Change Log](https://github.com/miguelgrinberg/greenletio/blob/main/CHANGES.md)
 
+
+
```

### Comparing `greenletio-0.10.1/README.md` & `greenletio-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/setup.cfg` & `greenletio-0.9.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = greenletio
-version = 0.10.1
+version = 0.9.0
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Asyncio integration with sync code using greenlets.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/greenletio
 project_urls =
```

### Comparing `greenletio-0.10.1/src/greenletio/core.py` & `greenletio-0.9.0/src/greenletio/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import asyncio
-import contextvars
 import functools
 import sys
 from greenlet import greenlet, getcurrent
 
 
 class GreenletBridge:
-    stop = object()
-
     def __init__(self):
         self.bridge_greenlet = None
 
     def run(self):
         async def async_run():
             gl = getcurrent().parent
             coro = gl.switch()
-            while gl and coro != self.stop:  # pragma: no branch
+            while gl and coro != ():  # pragma: no branch
                 try:
                     result = await coro
                 except:  # noqa: E722
                     coro = gl.throw(*sys.exc_info())
                 else:
                     coro = gl.switch(result)
 
@@ -33,31 +30,36 @@
         loop.run_until_complete(async_run())
         self.bridge_greenlet = None
 
     def start(self):
         if self.bridge_greenlet:
             return self.bridge_greenlet
         if asyncio.get_event_loop().is_running():
-            # we shouldn't be here if a loop is already running!
+            # we shouldn't be here is a loop is already running!
             return greenlet.getcurrent()
 
-        self.bridge_greenlet = greenlet(self.run)
-        self.bridge_greenlet.switch()
+        self.switch()
         return self.bridge_greenlet
 
     def stop(self):
         if self.bridge_greenlet:
-            self.bridge_greenlet.switch(self.stop)
+            self.bridge_greenlet.switch()
             self.bridge_greenlet = None
 
+    def switch(self):
+        if self.bridge_greenlet is not None:
+            raise RuntimeError('Bridge already started.')
+        self.bridge_greenlet = greenlet(self.run)
+        return self.bridge_greenlet.switch()
+
 
 bridge = GreenletBridge()
 
 
-def async_(fn=None, *, with_context=False):
+def async_(fn):
     """Convert a standard function to an async function that can be awaited.
 
     This function creates an async wrapper for a standard function, allowing
     callers to invoke the function as an awaitable. Example::
 
         def fn():
             pass
@@ -70,55 +72,31 @@
         @async_
         def fn():
             pass
 
         async def main():
             await fn()
 
-    If you are using context variables, you can use the ``with_context`` option
-    to ensure that the context is preserved when the function is called::
-
-        @async_(with_context=True)
-        def fn():
-            pass
-
     :param fn: the standard function to convert to async.
     """
-    if fn is None:
-        return lambda fn: async_(fn, with_context=with_context)
-
     @functools.wraps(fn)
-    async def decorator(*args, **kwargs):
-        gl = greenlet(fn)
-
-        async def run():
+    def decorator(*args, **kwargs):
+        async def wrapper(fn, *args, **kwargs):
+            gl = greenlet(fn)
             coro = gl.switch(*args, **kwargs)
             while gl:
                 try:
                     result = await coro
                 except:  # noqa: E722
-                    # this catches exceptions from async functions awaited in
-                    # sync code, and re-raises them in the greenlet
                     coro = gl.throw(*sys.exc_info())
                 else:
                     coro = gl.switch(result)
-            return coro
-
-        if with_context:
-            gl.gr_context = contextvars.copy_context()
-            try:
-                result = await run()
-            finally:
-                # restore the context
-                for var in gl.gr_context:
-                    var.set(gl.gr_context[var])
-        else:
-            result = await run()
 
-        return result
+            return coro
+        return wrapper(fn, *args, **kwargs)
 
     return decorator
 
 
 def await_(coro_or_fn):
     """Wait for an async function to complete in a standard function, without
     blocking the asyncio loop.
```

### Comparing `greenletio-0.10.1/src/greenletio/green/socket.py` & `greenletio-0.9.0/src/greenletio/green/socket.py`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/src/greenletio/green/ssl.py` & `greenletio-0.9.0/src/greenletio/green/ssl.py`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/src/greenletio/green/threading.py` & `greenletio-0.9.0/src/greenletio/green/threading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import collections
 import weakref
 import greenlet
-from greenletio.core import await_, async_
+from greenletio.core import bridge, await_, async_
 from greenletio.patcher import copy_globals
 import threading as _original_threading_
 
 copy_globals(_original_threading_, globals())
 
 _active = {}
 
@@ -218,15 +218,15 @@
 class Thread(_original_threading_.Thread):
     def __init__(self, group=None, target=None, name=None, args=(),
                  kwargs=None, *, daemon=None):
         assert group is None, "group argument must be None for now"
         if kwargs is None:
             kwargs = {}
         self._target = target
-        self._name = str(name or _original_threading_._newname('GThread-%d'))
+        self._name = str(name or _original_threading_._newname())
         self._args = args
         self._kwargs = kwargs
         self._daemonic = False
         self._ident = None
         self._started = Event()
         self._ended = Event()
         self._is_stopped = False
@@ -239,14 +239,15 @@
 
         if self._started.is_set():
             raise RuntimeError("threads can only be started once")
 
         async def bootstrap():
             await async_(self._bootstrap)()
 
+        bridge.start()
         self.task = asyncio.ensure_future(bootstrap())
         self._started.set()
 
     def _set_ident(self):
         self._ident = get_ident()
 
     def _bootstrap(self):
```

### Comparing `greenletio-0.10.1/src/greenletio/io.py` & `greenletio-0.9.0/src/greenletio/io.py`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/src/greenletio/patcher.py` & `greenletio-0.9.0/src/greenletio/patcher.py`

 * *Files identical despite different names*

### Comparing `greenletio-0.10.1/src/greenletio.egg-info/PKG-INFO` & `greenletio-0.9.0/src/greenletio.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: greenletio
-Version: 0.10.1
+Version: 0.9.0
 Summary: Asyncio integration with sync code using greenlets.
 Home-page: https://github.com/miguelgrinberg/greenletio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/greenletio/issues
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -70,7 +72,9 @@
 
 ## Resources
 
 - [Documentation](http://greenletio.readthedocs.io/en/latest/)
 - [PyPI](https://pypi.python.org/pypi/greenletio)
 - [Change Log](https://github.com/miguelgrinberg/greenletio/blob/main/CHANGES.md)
 
+
+
```

### Comparing `greenletio-0.10.1/src/greenletio.egg-info/SOURCES.txt` & `greenletio-0.9.0/src/greenletio.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,18 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/greenletio/__init__.py
 src/greenletio/core.py
 src/greenletio/io.py
 src/greenletio/patcher.py
-src/greenletio/run.py
-src/greenletio/x.py
 src/greenletio.egg-info/PKG-INFO
 src/greenletio.egg-info/SOURCES.txt
 src/greenletio.egg-info/dependency_links.txt
 src/greenletio.egg-info/not-zip-safe
 src/greenletio.egg-info/requires.txt
 src/greenletio.egg-info/top_level.txt
 src/greenletio/green/__init__.py
 src/greenletio/green/socket.py
 src/greenletio/green/ssl.py
 src/greenletio/green/threading.py
-src/greenletio/green/time.py
-tests/test_core.py
-tests/test_patcher.py
-tests/test_socket.py
-tests/test_ssl.py
-tests/test_threading.py
+src/greenletio/green/time.py
```

