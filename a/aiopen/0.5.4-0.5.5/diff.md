# Comparing `tmp/aiopen-0.5.4.tar.gz` & `tmp/aiopen-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopen-0.5.4.tar", max compression
+gzip compressed data, was "aiopen-0.5.5.tar", max compression
```

## Comparing `aiopen-0.5.4.tar` & `aiopen-0.5.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      277 2022-02-04 21:32:32.100387 aiopen-0.5.4/aiopen/__init__.py
--rw-r--r--   0        0        0      233 2022-02-04 21:32:32.101386 aiopen-0.5.4/aiopen/__main__.py
--rw-r--r--   0        0        0     2848 2022-05-03 21:42:21.323730 aiopen-0.5.4/aiopen/_anyio.py
--rw-r--r--   0        0        0      191 2022-05-03 21:42:21.323730 aiopen-0.5.4/aiopen/_meta.py
--rw-r--r--   0        0        0    10624 2022-05-03 21:42:21.323730 aiopen-0.5.4/aiopen/core.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.781952 aiopen-0.5.4/aiopen/py.typed
--rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.409298 aiopen-0.5.4/LICENSE
--rw-r--r--   0        0        0     1614 2022-05-11 18:20:20.652127 aiopen-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1420 2022-05-03 21:42:21.323730 aiopen-0.5.4/README.md
--rw-r--r--   0        0        0     2212 2022-05-26 20:02:11.855083 aiopen-0.5.4/setup.py
--rw-r--r--   0        0        0     2407 2022-05-26 20:02:11.855083 aiopen-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      268 2023-04-20 23:19:54.379920 aiopen-0.5.5/aiopen/__about__.py
+-rw-r--r--   0        0        0      281 2023-04-20 20:48:15.122367 aiopen-0.5.5/aiopen/__init__.py
+-rw-r--r--   0        0        0      477 2023-04-20 20:48:27.266169 aiopen-0.5.5/aiopen/__main__.py
+-rw-r--r--   0        0        0     2827 2023-04-19 19:17:33.708721 aiopen-0.5.5/aiopen/_anyio.py
+-rw-r--r--   0        0        0      349 2023-04-20 20:38:23.568136 aiopen-0.5.5/aiopen/_meta.py
+-rw-r--r--   0        0        0    10927 2023-04-18 11:41:47.324748 aiopen-0.5.5/aiopen/core.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.781952 aiopen-0.5.5/aiopen/py.typed
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.409298 aiopen-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2532 2023-04-20 23:19:49.227680 aiopen-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1414 2022-09-19 18:35:16.979213 aiopen-0.5.5/README.md
+-rw-r--r--   0        0        0     2603 1970-01-01 00:00:00.000000 aiopen-0.5.5/PKG-INFO
```

### Comparing `aiopen-0.5.4/aiopen/_anyio.py` & `aiopen-0.5.5/aiopen/_anyio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # -*- coding: utf-8 -*-
 """Async io base functions and utilities
 
 Inspired by aiofiles
 """
 from __future__ import annotations
 
+from os import PathLike
 from types import TracebackType
 from typing import AnyStr, Awaitable, Callable, Type, Union, overload
 
-from anyio._core._fileio import (  # type: ignore[attr-defined]
-    AsyncFile,
-    PathLike,
-    open_file,
-)
+from anyio import AsyncFile, open_file
 
 from xtyping import Generic, OpenBinaryMode, OpenTextMode, Optional
 
 
 class AsyncFileContextManager(Generic[AnyStr]):
     __slots__ = ("_coro", "_obj")
     _coro: Awaitable[AsyncFile[AnyStr]]
@@ -78,15 +75,15 @@
     closefd: bool = ...,
     opener: Optional[Callable[[str, int], int]] = ...,
 ) -> AsyncFileContextManager[str]:
     ...
 
 
 def aiopen(
-    file: Union[str, PathLike, int],
+    file: Union[str, PathLike, int],  # type: ignore[type-arg]
     mode: str = "r",
     buffering: int = -1,
     encoding: Optional[str] = None,
     errors: Optional[str] = None,
     newline: Optional[str] = None,
     closefd: bool = True,
     opener: Optional[Callable[[str, int], int]] = None,
```

### Comparing `aiopen-0.5.4/aiopen/core.py` & `aiopen-0.5.5/aiopen/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self._executor, partial(fn, *args, **kwargs)
         )
         return cast(T, retval)
 
     return cast(Callable[P, Awaitable[T]], _async_funk)
 
 
-class AsyncBase(Generic[AnyStr]):
+class AsyncBase(Generic[AnyStr]):  # pragma: no cover
     _file: Union[BufferedWriter, TextIOWrapper, FileIO, BufferedRandom, BufferedReader]
     _loop: AbstractEventLoop
     _executor: Optional[BaseEventLoop] = None
 
     def __init__(
         self,
         file: Union[
@@ -165,15 +165,15 @@
         else:
             raise AttributeError("detach() method is not available")
 
     @aio_hoist
     def peek(self, *args: Any, **kwargs: Any) -> Any:
         if isinstance(self._file, BufferedReader):
             return self._file.peek(*args, **kwargs)
-        raise IOError("peek() method is not available")
+        raise OSError("peek() method is not available")
 
 
 # TODO: Fix generics...
 class AsyncBaseDetachable(AsyncBase):  # type: ignore[type-arg]
     _file: Union[BufferedReader, BufferedRandom, BufferedWriter, TextIOWrapper]
 
     def detach(self) -> Any:
@@ -236,15 +236,15 @@
     file: Union[
         TextIOBase, BufferedWriter, BufferedReader, BufferedRandom, FileIO, Any
     ],
     *,
     loop: AbstractEventLoop,
     executor: Any = None,
 ) -> Union[TextIOWrapperAsync, BufferedIOAsyncBase, BufferedReaderAsync, FileIOAsync]:
-    raise TypeError("Unsupported io type: {}.".format(file))
+    raise TypeError(f"Unsupported io type: {file}.")
 
 
 @_aiopen_dispatch.register(TextIOBase)
 def _textio_base_dispatcher(
     file: FileIO, *, loop: AbstractEventLoop, executor: Any = None
 ) -> TextIOWrapperAsync:
     return TextIOWrapperAsync(file, loop=loop, executor=executor)
@@ -410,15 +410,25 @@
     newline: None = None,
     closefd: bool = True,
     opener: None = None,
     *,
     loop: Optional[AbstractEventLoop] = None,
     executor: Any = None,
 ) -> AiopenContextManager:
-    """Async version of the `open` builtin"""
+    """Async version of the `open` builtin
+
+    Examples:
+        >>> async def main():
+        ...     async with aiopen("test.txt", "w") as f:
+        ...         await f.write("test")
+        ...     async with aiopen("test.txt", "r") as f:
+        ...         assert await f.read() == "test"
+        >>> asyncio.run(main())
+
+    """
     return AiopenContextManager(
         _aiopen(
             str(file),
             mode=mode,
             buffering=buffering,
             encoding=encoding,
             errors=errors,
```

### Comparing `aiopen-0.5.4/LICENSE` & `aiopen-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopen-0.5.4/README.md` & `aiopen-0.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 
 **Install:** `pip install aiopen`
 
 Async-open
 
 **Why not use aiofiles?**
 
- - Wanted more type annotations
- - aiofiles uses ye ole `@coroutine` decorator -- aiopen uses python3.6+ `async/await`
- - aiopen is a callable module, so you can do:
- 	- `import aiopen`
- 	- `async with aiopen('afile.txt', 'w') as f: await f.write('some text!')`
- 	- `async with aiopen('afile.txt', 'r') as f: content = await f.read()`
-
+- Wanted more type annotations
+- aiofiles uses ye ole `@coroutine` decorator -- aiopen uses python3.6+ `async/await`
+- aiopen is a callable module, so you can do:
+  - `import aiopen`
+  - `async with aiopen('afile.txt', 'w') as f: await f.write('some text!')`
+  - `async with aiopen('afile.txt', 'r') as f: content = await f.read()`
 
 (Big shouts out to the aiofiles people, aiopen is entirely based off of aiofiles)
 
-
 ## Usage:
 
 Just import it! The module is also callable!
 
 ```python
 import aiopen
 
 async with aiopen('afile.txt', 'w') as f:
     await f.write('some text!')
 
 async with aiopen('afile.txt', 'r') as f:
     content = await f.read()
     print(content)
-
 ```
```

### Comparing `aiopen-0.5.4/PKG-INFO` & `aiopen-0.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: aiopen
-Version: 0.5.4
+Version: 0.5.5
 Summary: Async file io
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/aiopen
 License: MIT
 Keywords: anyio,fs,aiopen,async,dgpy
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
@@ -37,34 +41,31 @@
 
 **Install:** `pip install aiopen`
 
 Async-open
 
 **Why not use aiofiles?**
 
- - Wanted more type annotations
- - aiofiles uses ye ole `@coroutine` decorator -- aiopen uses python3.6+ `async/await`
- - aiopen is a callable module, so you can do:
- 	- `import aiopen`
- 	- `async with aiopen('afile.txt', 'w') as f: await f.write('some text!')`
- 	- `async with aiopen('afile.txt', 'r') as f: content = await f.read()`
-
+- Wanted more type annotations
+- aiofiles uses ye ole `@coroutine` decorator -- aiopen uses python3.6+ `async/await`
+- aiopen is a callable module, so you can do:
+  - `import aiopen`
+  - `async with aiopen('afile.txt', 'w') as f: await f.write('some text!')`
+  - `async with aiopen('afile.txt', 'r') as f: content = await f.read()`
 
 (Big shouts out to the aiofiles people, aiopen is entirely based off of aiofiles)
 
-
 ## Usage:
 
 Just import it! The module is also callable!
 
 ```python
 import aiopen
 
 async with aiopen('afile.txt', 'w') as f:
     await f.write('some text!')
 
 async with aiopen('afile.txt', 'r') as f:
     content = await f.read()
     print(content)
-
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
-Metadata-Version: 2.1 Name: aiopen Version: 0.5.4 Summary: Async file io Home-
+Metadata-Version: 2.1 Name: aiopen Version: 0.5.5 Summary: Async file io Home-
 page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/aiopen
 License: MIT Keywords: anyio,fs,aiopen,async,dgpy Author: jesse Author-email:
 jesse@dgi.com Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Typing :: Typed Requires-Dist: funkify (>=0.4.0,<0.5.0) Requires-
-Dist: xtyping (>=0.5.0) Project-URL: Repository, https://github.com/dynamic-
-graphics-inc/dgpy-libs Description-Content-Type: text/markdown [drawing] #
-aiopen [![Wheel](https://img.shields.io/pypi/wheel/aiopen.svg)](https://
-img.shields.io/pypi/wheel/aiopen.svg) [![Version](https://img.shields.io/pypi/
-v/aiopen.svg)](https://img.shields.io/pypi/v/aiopen.svg) [![py_versions](https:
-//img.shields.io/pypi/pyversions/aiopen.svg)](https://img.shields.io/pypi/
-pyversions/aiopen.svg) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) **Install:** `pip
-install aiopen` Async-open **Why not use aiofiles?** - Wanted more type
-annotations - aiofiles uses ye ole `@coroutine` decorator -- aiopen uses
-python3.6+ `async/await` - aiopen is a callable module, so you can do: -
-`import aiopen` - `async with aiopen('afile.txt', 'w') as f: await f.write
-('some text!')` - `async with aiopen('afile.txt', 'r') as f: content = await
-f.read()` (Big shouts out to the aiofiles people, aiopen is entirely based off
-of aiofiles) ## Usage: Just import it! The module is also callable! ```python
-import aiopen async with aiopen('afile.txt', 'w') as f: await f.write('some
-text!') async with aiopen('afile.txt', 'r') as f: content = await f.read()
-print(content) ```
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Typing :: Typed
+Requires-Dist: funkify (>=0.4.0,<0.5.0) Requires-Dist: xtyping (>=0.5.0)
+Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
+Description-Content-Type: text/markdown [drawing] # aiopen [![Wheel](https://
+img.shields.io/pypi/wheel/aiopen.svg)](https://img.shields.io/pypi/wheel/
+aiopen.svg) [![Version](https://img.shields.io/pypi/v/aiopen.svg)](https://
+img.shields.io/pypi/v/aiopen.svg) [![py_versions](https://img.shields.io/pypi/
+pyversions/aiopen.svg)](https://img.shields.io/pypi/pyversions/aiopen.svg) [!
+[Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg)](https://github.com/psf/black) **Install:** `pip install aiopen`
+Async-open **Why not use aiofiles?** - Wanted more type annotations - aiofiles
+uses ye ole `@coroutine` decorator -- aiopen uses python3.6+ `async/await` -
+aiopen is a callable module, so you can do: - `import aiopen` - `async with
+aiopen('afile.txt', 'w') as f: await f.write('some text!')` - `async with
+aiopen('afile.txt', 'r') as f: content = await f.read()` (Big shouts out to the
+aiofiles people, aiopen is entirely based off of aiofiles) ## Usage: Just
+import it! The module is also callable! ```python import aiopen async with
+aiopen('afile.txt', 'w') as f: await f.write('some text!') async with aiopen
+('afile.txt', 'r') as f: content = await f.read() print(content) ```
```

