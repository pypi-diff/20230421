# Comparing `tmp/dbus_fast-1.85.0.tar.gz` & `tmp/dbus-fast-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbus_fast-1.85.0.tar", max compression
+gzip compressed data, was "dbus-fast-1.9.0.tar", max compression
```

## Comparing `dbus_fast-1.85.0.tar` & `dbus-fast-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,31 @@
--rw-r--r--   0        0        0     1083 2023-04-21 00:35:14.110922 dbus_fast-1.85.0/LICENSE
--rw-r--r--   0        0        0     9404 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/README.md
--rw-r--r--   0        0        0     1252 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/build_ext.py
--rw-r--r--   0        0        0     2608 2023-04-21 00:35:15.026926 dbus_fast-1.85.0/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/__init__.py
--rw-r--r--   0        0        0      401 2023-04-21 00:35:14.978926 dbus_fast-1.85.0/src/dbus_fast/__version__.py
--rw-r--r--   0        0        0        0 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/__init__.py
--rw-r--r--   0        0        0      211 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/_cython_compat.py
--rw-r--r--   0        0        0     3521 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/address.py
--rw-r--r--   0        0        0      275 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/constants.py
--rw-r--r--   0        0        0     2463 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/marshaller.pxd
--rw-r--r--   0        0        0     7785 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/marshaller.py
--rw-r--r--   0        0        0     5298 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/unmarshaller.pxd
--rw-r--r--   0        0        0    25709 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/unmarshaller.py
--rw-r--r--   0        0        0     5660 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/_private/util.py
--rw-r--r--   0        0        0       90 2023-04-21 00:35:14.114922 dbus_fast-1.85.0/src/dbus_fast/aio/__init__.py
--rw-r--r--   0        0        0    17715 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/aio/message_bus.py
--rw-r--r--   0        0        0      100 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/aio/message_reader.pxd
--rw-r--r--   0        0        0     1181 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/aio/message_reader.py
--rw-r--r--   0        0        0     7045 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/aio/proxy_object.py
--rw-r--r--   0        0        0     4285 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/auth.py
--rw-r--r--   0        0        0     5490 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/constants.py
--rw-r--r--   0        0        0     1982 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/errors.py
--rw-r--r--   0        0        0       90 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/glib/__init__.py
--rw-r--r--   0        0        0    16304 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/glib/message_bus.py
--rw-r--r--   0        0        0    10724 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/glib/proxy_object.py
--rw-r--r--   0        0        0    22462 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/introspection.py
--rw-r--r--   0        0        0       53 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/main.py
--rw-r--r--   0        0        0     1215 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/message.pxd
--rw-r--r--   0        0        0    11736 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/message.py
--rw-r--r--   0        0        0     1333 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/message_bus.pxd
--rw-r--r--   0        0        0    46761 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/message_bus.py
--rw-r--r--   0        0        0    14104 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/proxy_object.py
--rw-r--r--   0        0        0        0 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/py.typed
--rw-r--r--   0        0        0      524 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/service.pxd
--rw-r--r--   0        0        0    22206 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/service.py
--rw-r--r--   0        0        0      352 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/signature.pxd
--rw-r--r--   0        0        0    16584 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/signature.py
--rw-r--r--   0        0        0      181 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/unpack.pxd
--rw-r--r--   0        0        0      622 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/unpack.py
--rw-r--r--   0        0        0     5144 2023-04-21 00:35:14.118923 dbus_fast-1.85.0/src/dbus_fast/validators.py
--rw-r--r--   0        0        0    10563 1970-01-01 00:00:00.000000 dbus_fast-1.85.0/setup.py
--rw-r--r--   0        0        0    10672 1970-01-01 00:00:00.000000 dbus_fast-1.85.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-24 07:50:15.357764 dbus-fast-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9471 2022-09-24 07:50:15.357764 dbus-fast-1.9.0/README.md
+-rw-r--r--   0        0        0     2580 2022-09-24 07:50:16.317766 dbus-fast-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      961 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/__init__.py
+-rw-r--r--   0        0        0      400 2022-09-24 07:50:16.261766 dbus-fast-1.9.0/src/dbus_fast/__version__.py
+-rw-r--r--   0        0        0        0 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/__init__.py
+-rw-r--r--   0        0        0     3521 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/address.py
+-rw-r--r--   0        0        0      346 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/constants.py
+-rw-r--r--   0        0        0     5457 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/marshaller.py
+-rw-r--r--   0        0        0    12731 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/unmarshaller.py
+-rw-r--r--   0        0        0     5628 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/_private/util.py
+-rw-r--r--   0        0        0       90 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/aio/__init__.py
+-rw-r--r--   0        0        0    17472 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/aio/message_bus.py
+-rw-r--r--   0        0        0     6776 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/aio/proxy_object.py
+-rw-r--r--   0        0        0     3646 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/auth.py
+-rw-r--r--   0        0        0     5288 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/constants.py
+-rw-r--r--   0        0        0     1739 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/errors.py
+-rw-r--r--   0        0        0       90 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/glib/__init__.py
+-rw-r--r--   0        0        0    15979 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/glib/message_bus.py
+-rw-r--r--   0        0        0    10727 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/glib/proxy_object.py
+-rw-r--r--   0        0        0    22457 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/introspection.py
+-rw-r--r--   0        0        0       53 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/main.py
+-rw-r--r--   0        0        0    11783 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/message.py
+-rw-r--r--   0        0        0    43305 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/message_bus.py
+-rw-r--r--   0        0        0    13748 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/proxy_object.py
+-rw-r--r--   0        0        0        0 2022-09-24 07:50:15.361764 dbus-fast-1.9.0/src/dbus_fast/py.typed
+-rw-r--r--   0        0        0    20512 2022-09-24 07:50:15.365764 dbus-fast-1.9.0/src/dbus_fast/service.py
+-rw-r--r--   0        0        0    16377 2022-09-24 07:50:15.365764 dbus-fast-1.9.0/src/dbus_fast/signature.py
+-rw-r--r--   0        0        0     4991 2022-09-24 07:50:15.365764 dbus-fast-1.9.0/src/dbus_fast/validators.py
+-rw-r--r--   0        0        0    10842 1970-01-01 00:00:00.000000 dbus-fast-1.9.0/setup.py
+-rw-r--r--   0        0        0    11000 1970-01-01 00:00:00.000000 dbus-fast-1.9.0/PKG-INFO
```

### Comparing `dbus_fast-1.85.0/LICENSE` & `dbus-fast-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.85.0/README.md` & `dbus-fast-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,15 @@
 
 Desktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.
 
 Desktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.
 
 dbus-fast plans to improve over other DBus libraries for Python in the following ways:
 
-- Zero dependencies and pure Python 3
-- An optional cython extension is available to speed up (un)marshalling
+- Zero dependencies and pure Python 3.
 - Focus on performance
 - Support for multiple IO backends including asyncio and the GLib main loop.
 - Nonblocking IO suitable for GUI development.
 - Target the latest language features of Python for beautiful services and clients.
 - Complete implementation of the DBus type system without ever guessing types.
 - Integration tests for all features of the library.
 - Completely documented public API.
@@ -75,14 +74,16 @@
 This example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.
 
 ```python
 from dbus_fast.aio import MessageBus
 
 import asyncio
 
+loop = asyncio.get_event_loop()
+
 
 async def main():
     bus = await MessageBus().connect()
     # the introspection xml would normally be included in your project, but
     # this is convenient for development
     introspection = await bus.introspect('org.mpris.MediaPlayer2.vlc', '/org/mpris/MediaPlayer2')
 
@@ -101,17 +102,17 @@
     # listen to signals
     def on_properties_changed(interface_name, changed_properties, invalidated_properties):
         for changed, variant in changed_properties.items():
             print(f'property changed: {changed} - {variant.value}')
 
     properties.on_properties_changed(on_properties_changed)
 
-    await asyncio.Event().wait()
+    await loop.create_future()
 
-asyncio.run(main())
+loop.run_until_complete(main())
 ```
 
 ## The Service Interface
 
 To define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.
 
 For more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).
@@ -154,17 +155,17 @@
 async def main():
     bus = await MessageBus().connect()
     interface = ExampleInterface('test.interface')
     bus.export('/test/path', interface)
     # now that we are ready to handle requests, we can request name from D-Bus
     await bus.request_name('test.name')
     # wait indefinitely
-    await asyncio.Event().wait()
+    await asyncio.get_event_loop().create_future()
 
-asyncio.run(main())
+asyncio.get_event_loop().run_until_complete(main())
 ```
 
 ## The Low-Level Interface
 
 The low-level interface works with DBus messages directly.
 
 For more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).
@@ -172,14 +173,16 @@
 ```python
 from dbus_fast.message import Message, MessageType
 from dbus_fast.aio import MessageBus
 
 import asyncio
 import json
 
+loop = asyncio.get_event_loop()
+
 
 async def main():
     bus = await MessageBus().connect()
 
     reply = await bus.call(
         Message(destination='org.freedesktop.DBus',
                 path='/org/freedesktop/DBus',
@@ -188,24 +191,24 @@
 
     if reply.message_type == MessageType.ERROR:
         raise Exception(reply.body[0])
 
     print(json.dumps(reply.body[0], indent=2))
 
 
-asyncio.run(main())
+loop.run_until_complete(main())
 ```
 
 ## Projects that use python-dbus-fast
 
 - [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)
 
 ## Contributing
 
-Contributions are welcome. Development happens on [Github](https://github.com/Bluetooth-Devices/dbus-fast).
+Contributions are welcome. Development happens on [Github](https://github.com/altdesktop/python-dbus-fast).
 
 Before you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.
 
 ## Copyright
 
 You can use this code under an MIT license (see LICENSE).
```

### Comparing `dbus_fast-1.85.0/pyproject.toml` & `dbus-fast-1.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbus-fast"
-version = "1.85.0"
+version = "1.9.0"
 description = "A faster version of dbus-next"
 authors = ["Bluetooth Devices Authors <bluetooth@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/dbus-fast"
 documentation = "https://dbus-fast.readthedocs.io"
 classifiers = [
@@ -14,43 +14,45 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "dbus_fast", from = "src" },
 ]
 
-[tool.poetry.build]
-generate-setup-file = true
-script = "build_ext.py"
-
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bluetooth-devices/dbus-fast/issues"
 "Changelog" = "https://github.com/bluetooth-devices/dbus-fast/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-async-timeout = {version = ">=3.0.0", python = "<3.11"}
 
-# duplicated in docs/requirements.txt for readthedocs compatibility
-[tool.poetry.group.docs.dependencies]
-myst-parser = "^0.18.0"
-sphinx = "^5.1.1"
-sphinx-rtd-theme = "^1.0.0"
-sphinxcontrib-asyncio = "^0.3.0"
-sphinxcontrib-fulltoc = "^1.2.0"
+# Documentation Dependencies
+sphinxcontrib-asyncio = {version = "^0.3.0", extras = ["docs"]}
+sphinxcontrib-fulltoc = {version = "^1.2.0", extras = ["docs"]}
+Sphinx = {version = "^5.1.1", extras = ["docs"]}
+myst-parser = {version = "^0.18.0", extras = ["docs"]}
+sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"]}
+
+[tool.poetry.extras]
+docs = [
+    "myst-parser",
+    "sphinx",
+    "sphinx-rtd-theme",
+    "sphinxcontrib-asyncio",
+    "sphinxcontrib-fulltoc"
+]
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 pytest-asyncio = "^0.19.0"
+
+[tool.poetry.group.dev.dependencies]
 pycairo = "^1.21.0"
 PyGObject = "^3.42.2"
-Cython = "^0.29.32"
-setuptools = "^65.4.1"
-pytest-timeout = "^2.1.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/dbus_fast/__version__.py:__version__"
 build_command = "pip install poetry && poetry build"
 
@@ -71,15 +73,15 @@
 
 [tool.isort]
 profile = "black"
 known_first_party = ["dbus_fast", "tests"]
 
 [tool.mypy]
 check_untyped_defs = true
-disallow_any_generics = false  # turn this on when we drop 3.7/3.8 support
+disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 mypy_path = "src/"
 no_implicit_optional = true
 show_error_codes = true
 warn_unreachable = true
 warn_unused_ignores = true
@@ -93,9 +95,9 @@
 allow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = "docs.*"
 ignore_errors = true
 
 [build-system]
-requires = ['setuptools>=65.4.1', 'wheel', 'Cython', "poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/_private/address.py` & `dbus-fast-1.9.0/src/dbus_fast/_private/address.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.85.0/src/dbus_fast/_private/util.py` & `dbus-fast-1.9.0/src/dbus_fast/_private/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import ast
 import inspect
-from typing import Any, List, Tuple, Union
+from typing import Any, List, Union
 
-from ..signature import SignatureTree, Variant, get_signature_tree
+from ..signature import SignatureTree, Variant
 
 
 def signature_contains_type(
     signature: Union[str, SignatureTree], body: List[Any], token: str
 ) -> bool:
     """For a given signature and body, check to see if it contains any members
     with the given token"""
     if type(signature) is str:
-        signature = get_signature_tree(signature)
+        signature = SignatureTree._get(signature)
 
     queue = []
     contains_variants = False
     for st in signature.types:
         queue.append(st)
 
     while True:
@@ -46,21 +46,21 @@
             queue.extend(member)
         elif type(member) is dict:
             queue.extend(member.values())
 
 
 def replace_fds_with_idx(
     signature: Union[str, SignatureTree], body: List[Any]
-) -> Tuple[List[Any], List[int]]:
+) -> (List[Any], List[int]):
     """Take the high level body format and convert it into the low level body
     format. Type 'h' refers directly to the fd in the body. Replace that with
     an index and return the corresponding list of unix fds that can be set on
     the Message"""
     if type(signature) is str:
-        signature = get_signature_tree(signature)
+        signature = SignatureTree._get(signature)
 
     if not signature_contains_type(signature, body, "h"):
         return body, []
 
     unix_fds = []
 
     def _replace(fd):
@@ -78,15 +78,15 @@
 def replace_idx_with_fds(
     signature: Union[str, SignatureTree], body: List[Any], unix_fds: List[int]
 ) -> List[Any]:
     """Take the low level body format and return the high level body format.
     Type 'h' refers to an index in the unix_fds array. Replace those with the
     actual file descriptor or `None` if one does not exist."""
     if type(signature) is str:
-        signature = get_signature_tree(signature)
+        signature = SignatureTree._get(signature)
 
     if not signature_contains_type(signature, body, "h"):
         return body
 
     def _replace(idx):
         try:
             return unix_fds[idx]
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/aio/message_bus.py` & `dbus-fast-1.9.0/src/dbus_fast/aio/message_bus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,74 +1,66 @@
 import array
 import asyncio
 import logging
 import socket
-import sys
-from collections import deque
+from asyncio import Queue
 from copy import copy
 from typing import Any, Optional
 
-if sys.version_info[:2] < (3, 11):
-    from async_timeout import timeout as asyncio_timeout
-else:
-    from asyncio import timeout as asyncio_timeout
-
 from .. import introspection as intr
+from .._private.unmarshaller import Unmarshaller
 from ..auth import Authenticator, AuthExternal
 from ..constants import (
     BusType,
     MessageFlag,
     MessageType,
     NameFlag,
     ReleaseNameReply,
     RequestNameReply,
 )
 from ..errors import AuthError
 from ..message import Message
 from ..message_bus import BaseMessageBus
 from ..service import ServiceInterface
-from .message_reader import build_message_reader
 from .proxy_object import ProxyObject
 
-NO_REPLY_EXPECTED_VALUE = MessageFlag.NO_REPLY_EXPECTED.value
-
 
 def _future_set_exception(fut: asyncio.Future, exc: Exception) -> None:
     if fut is not None and not fut.done():
         fut.set_exception(exc)
 
 
 def _future_set_result(fut: asyncio.Future, result: Any) -> None:
     if fut is not None and not fut.done():
         fut.set_result(result)
 
 
 class _MessageWriter:
     def __init__(self, bus: "MessageBus") -> None:
-        self.messages = deque()
+        self.messages = Queue()
         self.negotiate_unix_fd = bus._negotiate_unix_fd
         self.bus = bus
         self.sock = bus._sock
         self.loop = bus._loop
         self.buf = None
         self.fd = bus._fd
         self.offset = 0
         self.unix_fds = None
         self.fut: Optional[asyncio.Future] = None
 
     def write_callback(self, remove_writer: bool = True) -> None:
         try:
             while True:
                 if self.buf is None:
-                    if not self.messages:
+                    if self.messages.qsize() == 0:
                         # nothing more to write
                         if remove_writer:
                             self.loop.remove_writer(self.fd)
                         return
-                    buf, unix_fds, fut = self.messages.pop()
+                    buf, unix_fds, fut = self.messages.get_nowait()
                     self.unix_fds = unix_fds
                     self.buf = memoryview(buf)
                     self.offset = 0
                     self.fut = fut
 
                 if self.unix_fds and self.negotiate_unix_fd:
                     ancdata = [
@@ -93,41 +85,41 @@
         except Exception as e:
             if self.bus._user_disconnect:
                 _future_set_result(self.fut, None)
             else:
                 _future_set_exception(self.fut, e)
             self.bus._finalize(e)
 
-    def buffer_message(self, msg: Message, future=None) -> None:
-        self.messages.append(
+    def buffer_message(self, msg: Message, future=None):
+        self.messages.put_nowait(
             (
-                msg._marshall(self.negotiate_unix_fd),
+                msg._marshall(negotiate_unix_fd=self.negotiate_unix_fd),
                 copy(msg.unix_fds),
                 future,
             )
         )
 
-    def _write_without_remove_writer(self) -> None:
+    def _write_without_remove_writer(self):
         """Call the write callback without removing the writer."""
         self.write_callback(remove_writer=False)
 
-    def schedule_write(self, msg: Message = None, future=None) -> None:
-        queue_is_empty = not self.messages
+    def schedule_write(self, msg: Message = None, future=None):
+        queue_is_empty = self.messages.qsize() == 0
         if msg is not None:
             self.buffer_message(msg, future)
         if self.bus.unique_name:
             # Optimization: try to send now if the queue
             # is empty. With bleak this usually means we
             # can send right away 99% of the time which
             # is a huge improvement in latency.
             if queue_is_empty:
                 self._write_without_remove_writer()
             if (
                 self.buf is not None
-                or self.messages
+                or self.messages.qsize() != 0
                 or not self.fut
                 or not self.fut.done()
             ):
                 self.loop.add_writer(self.fd, self.write_callback)
 
 
 class MessageBus(BaseMessageBus):
@@ -156,25 +148,25 @@
         be :class:`None` until the message bus connects.
     :vartype unique_name: str
     :ivar connected: True if this message bus is expected to be able to send
         and receive messages.
     :vartype connected: bool
     """
 
-    __slots__ = ("_loop", "_auth", "_writer", "_disconnect_future")
-
     def __init__(
         self,
         bus_address: str = None,
         bus_type: BusType = BusType.SESSION,
         auth: Authenticator = None,
-        negotiate_unix_fd: bool = False,
-    ) -> None:
-        super().__init__(bus_address, bus_type, ProxyObject, negotiate_unix_fd)
-        self._loop = asyncio.get_running_loop()
+        negotiate_unix_fd=False,
+    ):
+        super().__init__(bus_address, bus_type, ProxyObject)
+        self._negotiate_unix_fd = negotiate_unix_fd
+        self._loop = asyncio.get_event_loop()
+        self._unmarshaller = self._create_unmarshaller()
 
         self._writer = _MessageWriter(self)
 
         if auth is None:
             self._auth = AuthExternal()
         else:
             self._auth = auth
@@ -194,23 +186,15 @@
               the DBus daemon failed.
             - :class:`Exception` - If there was a connection error.
         """
         await self._authenticate()
 
         future = self._loop.create_future()
 
-        self._loop.add_reader(
-            self._fd,
-            build_message_reader(
-                self._stream,
-                self._sock if self._negotiate_unix_fd else None,
-                self._process_message,
-                self._finalize,
-            ),
-        )
+        self._loop.add_reader(self._fd, self._message_reader)
 
         def on_hello(reply, err):
             try:
                 if err:
                     raise err
                 self.unique_name = reply.body[0]
                 self._writer.schedule_write()
@@ -225,15 +209,15 @@
             path="/org/freedesktop/DBus",
             interface="org.freedesktop.DBus",
             member="Hello",
             serial=self.next_serial(),
         )
 
         self._method_return_handlers[hello_msg.serial] = on_hello
-        self._stream.write(hello_msg._marshall(False))
+        self._stream.write(hello_msg._marshall())
         self._stream.flush()
 
         return await future
 
     async def introspect(
         self, bus_name: str, path: str, timeout: float = 30.0
     ) -> intr.Node:
@@ -269,16 +253,15 @@
             if err:
                 _future_set_exception(future, err)
             else:
                 _future_set_result(future, reply)
 
         super().introspect(bus_name, path, reply_handler)
 
-        async with asyncio_timeout(timeout):
-            return await future
+        return await asyncio.wait_for(future, timeout=timeout)
 
     async def request_name(
         self, name: str, flags: NameFlag = NameFlag.NONE
     ) -> RequestNameReply:
         """Request that this message bus owns the given name.
 
         :param name: The name to request.
@@ -347,15 +330,15 @@
             ``None`` after the message is sent.
         :rtype: :class:`Message <dbus_fast.Message>` or :class:`None` if no reply is expected.
 
         :raises:
             - :class:`Exception` - If a connection error occurred.
         """
         if (
-            msg.flags.value & NO_REPLY_EXPECTED_VALUE
+            msg.flags & MessageFlag.NO_REPLY_EXPECTED
             or msg.message_type is not MessageType.METHOD_CALL
         ):
             await self.send(msg)
             return None
 
         future = self._loop.create_future()
 
@@ -368,15 +351,15 @@
 
         self._call(msg, reply_handler, check_callback=False)
 
         await future
 
         return future.result()
 
-    def send(self, msg: Message) -> asyncio.Future:
+    def send(self, msg: Message):
         """Asynchronously send a message on the message bus.
 
         .. note:: This method may change to a couroutine function in the 1.0
             release of the library.
 
         :param msg: The message to send.
         :type msg: :class:`Message <dbus_fast.Message>`
@@ -428,23 +411,32 @@
 
             args = ServiceInterface._msg_body_to_args(msg)
             fut = asyncio.ensure_future(method.fn(interface, *args))
             fut.add_done_callback(done)
 
         return handler
 
-    async def _auth_readline(self) -> str:
+    def _message_reader(self):
+        try:
+            while True:
+                if self._unmarshaller.unmarshall():
+                    self._on_message(self._unmarshaller.message)
+                    self._unmarshaller = self._create_unmarshaller()
+                else:
+                    break
+        except Exception as e:
+            self._finalize(e)
+
+    async def _auth_readline(self):
         buf = b""
         while buf[-2:] != b"\r\n":
-            # The auth protocol is line based, so we can read until we get a
-            # newline.
-            buf += await self._loop.sock_recv(self._sock, 1024)
+            buf += await self._loop.sock_recv(self._sock, 2)
         return buf[:-2].decode()
 
-    async def _authenticate(self) -> None:
+    async def _authenticate(self):
         await self._loop.sock_sendall(self._sock, b"\0")
 
         first_line = self._auth._authentication_start(
             negotiate_unix_fd=self._negotiate_unix_fd
         )
 
         if first_line is not None:
@@ -458,30 +450,33 @@
             response = self._auth._receive_line(await self._auth_readline())
             if response is not None:
                 await self._loop.sock_sendall(
                     self._sock, Authenticator._format_line(response)
                 )
                 self._stream.flush()
             if response == "BEGIN":
-                # The first octet received by the server after the \r\n of the BEGIN command
-                # from the client must be the first octet of the authenticated/encrypted stream
-                # of D-Bus messages.
                 break
 
-    def disconnect(self) -> None:
+    def disconnect(self):
         """Disconnect the message bus by closing the underlying connection asynchronously.
 
         All pending  and future calls will error with a connection error.
         """
         super().disconnect()
         try:
             self._sock.close()
         except Exception:
             logging.warning("could not close socket", exc_info=True)
 
+    def _create_unmarshaller(self) -> Unmarshaller:
+        sock = None
+        if self._negotiate_unix_fd:
+            sock = self._sock
+        return Unmarshaller(self._stream, sock)
+
     def _finalize(self, err: Optional[Exception] = None) -> None:
         try:
             self._loop.remove_reader(self._fd)
         except Exception:
             logging.warning("could not remove message reader", exc_info=True)
         try:
             self._loop.remove_writer(self._fd)
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/aio/proxy_object.py` & `dbus-fast-1.9.0/src/dbus_fast/aio/proxy_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import xml.etree.ElementTree as ET
-from typing import TYPE_CHECKING, Any, List, Union
+from typing import List, Union
 
 from .. import introspection as intr
 from .._private.util import replace_fds_with_idx, replace_idx_with_fds
-from ..constants import ErrorType, MessageFlag
+from ..constants import ErrorType
 from ..errors import DBusError
-from ..message import Message
+from ..message import Message, MessageFlag
 from ..message_bus import BaseMessageBus
 from ..proxy_object import BaseProxyInterface, BaseProxyObject
 from ..signature import Variant
-from ..unpack import unpack_variants as unpack
-
-if TYPE_CHECKING:
-    from .message_bus import MessageBus as AioMessageBus
-
-NO_REPLY_EXPECTED_VALUE = MessageFlag.NO_REPLY_EXPECTED.value
+from ..signature import unpack_variants as unpack
 
 
 class ProxyInterface(BaseProxyInterface):
     """A class representing a proxy to an interface exported on the bus by
     another client for the asyncio :class:`MessageBus
     <dbus_fast.aio.MessageBus>` implementation.
 
@@ -75,17 +70,15 @@
     DBus property getters and setters are exposed as coroutines. The ``value``
     must correspond to the type of the property in the interface definition.
 
     If the service returns an error for a DBus call, a :class:`DBusError
     <dbus_fast.DBusError>` will be raised with information about the error.
     """
 
-    bus: "AioMessageBus"
-
-    def _add_method(self, intr_method: intr.Method) -> None:
+    def _add_method(self, intr_method):
         async def method_fn(
             *args, flags=MessageFlag.NONE, unpack_variants: bool = False
         ):
             input_body, unix_fds = replace_fds_with_idx(
                 intr_method.in_signature, list(args)
             )
 
@@ -98,15 +91,15 @@
                     signature=intr_method.in_signature,
                     body=input_body,
                     flags=flags,
                     unix_fds=unix_fds,
                 )
             )
 
-            if flags is not None and flags.value & NO_REPLY_EXPECTED_VALUE:
+            if flags & MessageFlag.NO_REPLY_EXPECTED:
                 return None
 
             BaseProxyInterface._check_method_return(msg, intr_method.out_signature)
 
             out_len = len(intr_method.out_args)
 
             body = replace_idx_with_fds(msg.signature_tree, msg.body, msg.unix_fds)
@@ -122,16 +115,16 @@
             return body
 
         method_name = f"call_{BaseProxyInterface._to_snake_case(intr_method.name)}"
         setattr(self, method_name, method_fn)
 
     def _add_property(
         self,
-        intr_property: intr.Property,
-    ) -> None:
+        intr_property,
+    ):
         async def property_getter(
             *, flags=MessageFlag.NONE, unpack_variants: bool = False
         ):
             msg = await self.bus.call(
                 Message(
                     destination=self.bus_name,
                     path=self.path,
@@ -153,15 +146,15 @@
 
             body = replace_idx_with_fds("v", msg.body, msg.unix_fds)[0].value
 
             if unpack_variants:
                 return unpack(body)
             return body
 
-        async def property_setter(val: Any) -> None:
+        async def property_setter(val):
             variant = Variant(intr_property.signature, val)
 
             body, unix_fds = replace_fds_with_idx(
                 "ssv", [self.introspection.name, intr_property.name, variant]
             )
 
             msg = await self.bus.call(
@@ -191,15 +184,15 @@
 
     def __init__(
         self,
         bus_name: str,
         path: str,
         introspection: Union[intr.Node, str, ET.Element],
         bus: BaseMessageBus,
-    ) -> None:
+    ):
         super().__init__(bus_name, path, introspection, bus, ProxyInterface)
 
     def get_interface(self, name: str) -> ProxyInterface:
         return super().get_interface(name)
 
     def get_children(self) -> List["ProxyObject"]:
         return super().get_children()
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/auth.py` & `dbus-fast-1.9.0/src/dbus_fast/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,101 @@
 import enum
 import os
-from typing import List, Optional, Tuple
 
 from .errors import AuthError
 
-UID_NOT_SPECIFIED = -1
-
 # The auth interface here is unstable. I would like to eventually open this up
 # for people to define their own custom authentication protocols, but I'm not
 # familiar with what's needed for that exactly. To work with any message bus
 # implementation would require abstracting out all the IO. Async operations
 # might be challenging because different IO backends have different ways of
 # doing that. I might just end up giving the raw socket and leaving it all up
 # to the user, but it would be nice to have a little guidance in the interface
 # since a lot of it is strongly specified. If you have a need for this, contact
-# the project maintainer to help stabilize this interface.
+# the project maintainer to help stabalize this interface.
 
 
 class _AuthResponse(enum.Enum):
     OK = "OK"
     REJECTED = "REJECTED"
     DATA = "DATA"
     ERROR = "ERROR"
     AGREE_UNIX_FD = "AGREE_UNIX_FD"
 
     @classmethod
-    def parse(klass, line: str) -> Tuple["_AuthResponse", List[str]]:
+    def parse(klass, line):
         args = line.split(" ")
         response = klass(args[0])
         return response, args[1:]
 
 
 # UNSTABLE
 class Authenticator:
     """The base class for authenticators for :class:`MessageBus <dbus_fast.message_bus.BaseMessageBus>` authentication.
 
     In the future, the library may allow extending this class for custom authentication protocols.
 
     :seealso: https://dbus.freedesktop.org/doc/dbus-specification.html#auth-protocol
     """
 
-    def _authentication_start(self, negotiate_unix_fd: bool = False) -> str:
+    def _authentication_start(self, negotiate_unix_fd=False):
         raise NotImplementedError(
             "authentication_start() must be implemented in the inheriting class"
         )
 
-    def _receive_line(self, line: str) -> str:
+    def _receive_line(self, line):
         raise NotImplementedError(
             "receive_line() must be implemented in the inheriting class"
         )
 
     @staticmethod
-    def _format_line(line: str) -> bytes:
+    def _format_line(line):
         return f"{line}\r\n".encode()
 
 
 class AuthExternal(Authenticator):
     """An authenticator class for the external auth protocol for use with the
     :class:`MessageBus <dbus_fast.message_bus.BaseMessageBus>`.
 
-    :param uid: The uid to use when connecting to the message bus. Use UID_NOT_SPECIFIED to use the uid known to the kernel.
-    :vartype uid: int
-
     :sealso: https://dbus.freedesktop.org/doc/dbus-specification.html#auth-protocol
     """
 
-    def __init__(self, uid: int = None) -> None:
-        self.negotiate_unix_fd: bool = False
-        self.negotiating_fds: bool = False
-        self.uid: Optional[int] = uid
+    def __init__(self):
+        self.negotiate_unix_fd = False
+        self.negotiating_fds = False
 
-    def _authentication_start(self, negotiate_unix_fd: bool = False) -> str:
+    def _authentication_start(self, negotiate_unix_fd=False) -> str:
         self.negotiate_unix_fd = negotiate_unix_fd
-        uid = self.uid
-        if uid == UID_NOT_SPECIFIED:
-            return "AUTH EXTERNAL"
-        if uid is None:
-            uid = os.getuid()
-        hex_uid = str(uid).encode().hex()
+        hex_uid = str(os.getuid()).encode().hex()
         return f"AUTH EXTERNAL {hex_uid}"
 
-    def _receive_line(self, line: str) -> str:
+    def _receive_line(self, line: str):
         response, args = _AuthResponse.parse(line)
 
         if response is _AuthResponse.OK:
             if self.negotiate_unix_fd:
                 self.negotiating_fds = True
                 return "NEGOTIATE_UNIX_FD"
             else:
                 return "BEGIN"
 
         if response is _AuthResponse.AGREE_UNIX_FD:
             return "BEGIN"
 
-        if response is _AuthResponse.DATA and self.uid == UID_NOT_SPECIFIED:
-            return "DATA"
-
         raise AuthError(f"authentication failed: {response.value}: {args}")
 
 
 class AuthAnnonymous(Authenticator):
     """An authenticator class for the annonymous auth protocol for use with the
     :class:`MessageBus <dbus_fast.message_bus.BaseMessageBus>`.
 
     :sealso: https://dbus.freedesktop.org/doc/dbus-specification.html#auth-protocol
     """
 
-    def _authentication_start(self, negotiate_unix_fd: bool = False) -> str:
+    def _authentication_start(self, negotiate_unix_fd=False) -> str:
         if negotiate_unix_fd:
             raise AuthError(
                 "annonymous authentication does not support negotiating unix fds right now"
             )
 
         return "AUTH ANONYMOUS"
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/constants.py` & `dbus-fast-1.9.0/src/dbus_fast/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,15 @@
 
     NONE = 0
     NO_REPLY_EXPECTED = 1  #: The method call does not expect a method return.
     NO_AUTOSTART = 2
     ALLOW_INTERACTIVE_AUTHORIZATION = 4
 
 
-# This is written out because of https://github.com/python/cpython/issues/98976
-MESSAGE_FLAG_MAP = {
-    0: MessageFlag.NONE,
-    1: MessageFlag.NO_REPLY_EXPECTED,
-    2: MessageFlag.NO_AUTOSTART,
-    4: MessageFlag.ALLOW_INTERACTIVE_AUTHORIZATION,
-}
+MESSAGE_FLAG_MAP = {field.value: field for field in MessageFlag}
 
 
 class NameFlag(IntFlag):
     """A flag that affects the behavior of a name request."""
 
     NONE = 0
     ALLOW_REPLACEMENT = 1  #: If another client requests this name, let them have it.
@@ -71,19 +65,19 @@
     the ``org.freedesktop.DBus.Properties`` interface.
     """
 
     READ = "read"  #: The property is readonly.
     WRITE = "write"  #: The property is writeonly.
     READWRITE = "readwrite"  #: The property can be read or written to.
 
-    def readable(self) -> bool:
+    def readable(self):
         """Get whether the property can be read."""
         return self == PropertyAccess.READ or self == PropertyAccess.READWRITE
 
-    def writable(self) -> bool:
+    def writable(self):
         """Get whether the property can be written to."""
         return self == PropertyAccess.WRITE or self == PropertyAccess.READWRITE
 
 
 class ArgDirection(Enum):
     """For an introspected argument, indicates whether it is an input parameter or a return value."""
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/errors.py` & `dbus-fast-1.9.0/src/dbus_fast/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from typing import Optional, Union
-
-
 class SignatureBodyMismatchError(ValueError):
     pass
 
 
 class InvalidSignatureError(ValueError):
     pass
 
@@ -30,55 +27,53 @@
 
 
 class SignalDisabledError(Exception):
     pass
 
 
 class InvalidBusNameError(TypeError):
-    def __init__(self, name: str) -> None:
+    def __init__(self, name):
         super().__init__(f"invalid bus name: {name}")
 
 
 class InvalidObjectPathError(TypeError):
-    def __init__(self, path: str) -> None:
+    def __init__(self, path):
         super().__init__(f"invalid object path: {path}")
 
 
 class InvalidInterfaceNameError(TypeError):
-    def __init__(self, name: str) -> None:
+    def __init__(self, name):
         super().__init__(f"invalid interface name: {name}")
 
 
 class InvalidMemberNameError(TypeError):
-    def __init__(self, member: str) -> None:
+    def __init__(self, member):
         super().__init__(f"invalid member name: {member}")
 
 
 from .constants import ErrorType, MessageType
 from .message import Message
 from .validators import assert_interface_name_valid
 
 
 class DBusError(Exception):
-    def __init__(
-        self, type_: Union[ErrorType, str], text: str, reply: Optional[Message] = None
-    ) -> None:
+    def __init__(self, type_, text, reply=None):
         super().__init__(text)
 
         if type(type_) is ErrorType:
             type_ = type_.value
 
-        assert_interface_name_valid(type_)  # type: ignore[arg-type]
+        assert_interface_name_valid(type_)
         if reply is not None and type(reply) is not Message:
             raise TypeError("reply must be of type Message")
 
         self.type = type_
         self.text = text
         self.reply = reply
 
     @staticmethod
-    def _from_message(msg: Message) -> "DBusError":
+    def _from_message(msg):
         assert msg.message_type == MessageType.ERROR
-        return DBusError(msg.error_name or "unknown", msg.body[0], reply=msg)
+        return DBusError(msg.error_name, msg.body[0], reply=msg)
 
-    def _as_message(self, msg: Message) -> Message:
+    def _as_message(self, msg):
         return Message.new_error(msg, self.type, self.text)
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/glib/message_bus.py` & `dbus-fast-1.9.0/src/dbus_fast/glib/message_bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import io
-import logging
-import traceback
 from typing import Callable, Optional
 
 from .. import introspection as intr
 from .._private.unmarshaller import Unmarshaller
 from ..auth import Authenticator, AuthExternal
 from ..constants import (
     BusType,
@@ -45,17 +43,16 @@
 
     def dispatch(self, callback, user_data):
         try:
             while self.bus._stream.readable():
                 if not self.unmarshaller:
                     self.unmarshaller = Unmarshaller(self.bus._stream)
 
-                message = self.unmarshaller.unmarshall()
-                if message:
-                    callback(message)
+                if self.unmarshaller.unmarshall():
+                    callback(self.unmarshaller.message)
                     self.unmarshaller = None
                 else:
                     break
         except Exception as e:
             self.bus.disconnect()
             self.bus._finalize(e)
             return GLib.SOURCE_REMOVE
@@ -95,15 +92,15 @@
 
             self.bus._stream.flush()
 
             if not self.bus._buffered_messages:
                 return GLib.SOURCE_REMOVE
             else:
                 message = self.bus._buffered_messages.pop(0)
-                self.message_stream = io.BytesIO(message._marshall(False))
+                self.message_stream = io.BytesIO(message._marshall())
                 return GLib.SOURCE_CONTINUE
         except BlockingIOError:
             return GLib.SOURCE_CONTINUE
         except Exception as e:
             self.bus._finalize(e)
             return GLib.SOURCE_REMOVE
 
@@ -172,22 +169,14 @@
         self._buffered_messages = []
 
         if auth is None:
             self._auth = AuthExternal()
         else:
             self._auth = auth
 
-    def _on_message(self, msg: Message) -> None:
-        try:
-            self._process_message(msg)
-        except Exception as e:
-            logging.error(
-                f"got unexpected error processing a message: {e}.\n{traceback.format_exc()}"
-            )
-
     def connect(
         self, connect_notify: Callable[["MessageBus", Optional[Exception]], None] = None
     ):
         """Connect this message bus to the DBus daemon.
 
         This method or the synchronous version must be called before the
         message bus can be used.
@@ -230,15 +219,15 @@
                 path="/org/freedesktop/DBus",
                 interface="org.freedesktop.DBus",
                 member="Hello",
                 serial=self.next_serial(),
             )
 
             self._method_return_handlers[hello_msg.serial] = on_hello
-            self._stream.write(hello_msg._marshall(False))
+            self._stream.write(hello_msg._marshall())
             self._stream.flush()
 
         self._authenticate(authenticate_notify)
 
     def connect_sync(self) -> "MessageBus":
         """Connect this message bus to the DBus daemon.
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/glib/proxy_object.py` & `dbus-fast-1.9.0/src/dbus_fast/glib/proxy_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .. import introspection as intr
 from ..constants import ErrorType
 from ..errors import DBusError
 from ..message import Message
 from ..message_bus import BaseMessageBus
 from ..proxy_object import BaseProxyInterface, BaseProxyObject
 from ..signature import Variant
-from ..unpack import unpack_variants as unpack
+from ..signature import unpack_variants as unpack
 
 # glib is optional
 try:
     from gi.repository import GLib
 except ImportError:
     pass
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/introspection.py` & `dbus-fast-1.9.0/src/dbus_fast/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xml.etree.ElementTree as ET
 from typing import List, Union
 
 from .constants import ArgDirection, PropertyAccess
 from .errors import InvalidIntrospectionError
-from .signature import SignatureType, get_signature_tree
+from .signature import SignatureTree, SignatureType
 from .validators import assert_interface_name_valid, assert_member_name_valid
 
 # https://dbus.freedesktop.org/doc/dbus-specification.html#introspection-format
 # TODO annotations
 
 
 class Arg:
@@ -38,15 +38,15 @@
             assert_member_name_valid(name)
 
         type_ = None
         if type(signature) is SignatureType:
             type_ = signature
             signature = signature.signature
         else:
-            tree = get_signature_tree(signature)
+            tree = SignatureTree._get(signature)
             if len(tree.types) != 1:
                 raise InvalidIntrospectionError(
                     f"an argument must have a single complete type. (has {len(tree.types)} types)"
                 )
             type_ = tree.types[0]
 
         self.type = type_
@@ -244,15 +244,15 @@
         self,
         name: str,
         signature: str,
         access: PropertyAccess = PropertyAccess.READWRITE,
     ):
         assert_member_name_valid(name)
 
-        tree = get_signature_tree(signature)
+        tree = SignatureTree._get(signature)
         if len(tree.types) != 1:
             raise InvalidIntrospectionError(
                 f"properties must have a single complete type. (has {len(tree.types)} types)"
             )
 
         self.name = name
         self.signature = signature
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/message.py` & `dbus-fast-1.9.0/src/dbus_fast/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, List, Optional, Union
+from typing import Any, List
 
 from ._private.constants import LITTLE_ENDIAN, PROTOCOL_VERSION, HeaderField
 from ._private.marshaller import Marshaller
 from .constants import ErrorType, MessageFlag, MessageType
 from .errors import InvalidMessageError
-from .signature import SignatureTree, Variant, get_signature_tree
+from .signature import SignatureTree, Variant
 from .validators import (
     assert_bus_name_valid,
     assert_interface_name_valid,
     assert_member_name_valid,
     assert_object_path_valid,
 )
 
@@ -24,16 +24,14 @@
 HEADER_MEMBER = HeaderField.MEMBER.value
 HEADER_ERROR_NAME = HeaderField.ERROR_NAME.value
 HEADER_REPLY_SERIAL = HeaderField.REPLY_SERIAL.value
 HEADER_DESTINATION = HeaderField.DESTINATION.value
 HEADER_SIGNATURE = HeaderField.SIGNATURE.value
 HEADER_UNIX_FDS = HeaderField.UNIX_FDS.value
 
-MESSAGE_FLAG = MessageFlag
-
 
 class Message:
     """A class for sending and receiving messages through the
     :class:`MessageBus <dbus_fast.message_bus.BaseMessageBus>` with the
     low-level api.
 
     A ``Message`` can be constructed by the user to send over the message bus.
@@ -93,74 +91,76 @@
         "signature_tree",
         "body",
         "serial",
     )
 
     def __init__(
         self,
-        destination: Optional[str] = None,
-        path: Optional[str] = None,
-        interface: Optional[str] = None,
-        member: Optional[str] = None,
+        destination: str = None,
+        path: str = None,
+        interface: str = None,
+        member: str = None,
         message_type: MessageType = MessageType.METHOD_CALL,
-        flags: Union[MessageFlag, int] = MessageFlag.NONE,
-        error_name: Optional[Union[str, ErrorType]] = None,
-        reply_serial: int = 0,
-        sender: Optional[str] = None,
+        flags: MessageFlag = MessageFlag.NONE,
+        error_name: str = None,
+        reply_serial: int = None,
+        sender: str = None,
         unix_fds: List[int] = [],
-        signature: Optional[Union[SignatureTree, str]] = None,
+        signature: str = "",
         body: List[Any] = [],
         serial: int = 0,
         validate: bool = True,
-    ) -> None:
+    ):
         self.destination = destination
         self.path = path
         self.interface = interface
         self.member = member
         self.message_type = message_type
-        self.flags = flags if type(flags) is MESSAGE_FLAG else MESSAGE_FLAG(flags)
+        self.flags = (
+            flags if type(flags) is MessageFlag else MessageFlag(bytes([flags]))
+        )
         self.error_name = (
-            str(error_name.value) if type(error_name) is ErrorType else error_name
+            error_name if type(error_name) is not ErrorType else error_name.value
         )
-        self.reply_serial = reply_serial or 0
+        self.reply_serial = reply_serial
         self.sender = sender
         self.unix_fds = unix_fds
-        if type(signature) is SignatureTree:
-            self.signature = signature.signature
-            self.signature_tree = signature
-        else:
-            self.signature = signature or ""  # type: ignore[assignment]
-            self.signature_tree = get_signature_tree(signature or "")
+        self.signature = (
+            signature.signature if type(signature) is SignatureTree else signature
+        )
+        self.signature_tree = (
+            signature
+            if type(signature) is SignatureTree
+            else SignatureTree._get(signature)
+        )
         self.body = body
-        self.serial = serial or 0
+        self.serial = serial
 
         if not validate:
             return
         if self.destination is not None:
             assert_bus_name_valid(self.destination)
         if self.interface is not None:
             assert_interface_name_valid(self.interface)
         if self.path is not None:
             assert_object_path_valid(self.path)
         if self.member is not None:
             assert_member_name_valid(self.member)
         if self.error_name is not None:
-            assert_interface_name_valid(self.error_name)  # type: ignore[arg-type]
+            assert_interface_name_valid(self.error_name)
 
         required_fields = REQUIRED_FIELDS.get(self.message_type)
         if not required_fields:
             raise InvalidMessageError(f"got unknown message type: {self.message_type}")
         for field in required_fields:
             if not getattr(self, field):
                 raise InvalidMessageError(f"missing required field: {field}")
 
     @staticmethod
-    def new_error(
-        msg: "Message", error_name: Union[str, ErrorType], error_text: str
-    ) -> "Message":
+    def new_error(msg: "Message", error_name: str, error_text: str) -> "Message":
         """A convenience constructor to create an error message in reply to the given message.
 
         :param msg: The message this error is in reply to.
         :type msg: :class:`Message`
         :param error_name: The name of this error. Must be a valid interface name.
         :type error_name: str
         :param error_text: Human-readable text for the error.
@@ -215,16 +215,16 @@
 
     @staticmethod
     def new_signal(
         path: str,
         interface: str,
         member: str,
         signature: str = "",
-        body: Optional[List[Any]] = None,
-        unix_fds: Optional[List[int]] = None,
+        body: List[Any] = None,
+        unix_fds: List[int] = None,
     ) -> "Message":
         """A convenience constructor to create a new signal message.
 
         :param path: The path of this signal.
         :type path: str
         :param interface: The interface of this signal.
         :type interface: str
@@ -242,59 +242,77 @@
 
         :raises:
             - :class:`InvalidSignatureError` - If the signature is not a valid signature.
             - :class:`InvalidObjectPathError` - If ``path`` is not a valid object path.
             - :class:`InvalidInterfaceNameError` - If ``interface`` is not a valid interface name.
             - :class:`InvalidMemberNameError` - If ``member`` is not a valid member name.
         """
+        body = body if body else []
         return Message(
             message_type=MessageType.SIGNAL,
             interface=interface,
             path=path,
             member=member,
             signature=signature,
-            body=body or [],
-            unix_fds=unix_fds or [],
+            body=body,
+            unix_fds=unix_fds,
         )
 
-    def _marshall(self, negotiate_unix_fd: bool) -> bytearray:
-        """Marshall this message into a byte array."""
+    def _matches(self, **kwargs):
+        for attr, val in kwargs.items():
+            if getattr(self, attr) != val:
+                return False
+
+        return True
+
+    def _marshall(self, negotiate_unix_fd=False):
         # TODO maximum message size is 134217728 (128 MiB)
         body_block = Marshaller(self.signature, self.body)
-        body_buffer = body_block._marshall()
+        body_block.marshall()
 
         fields = []
 
         # No verify here since the marshaller will raise an exception if the
         # Variant is invalid.
 
         if self.path:
-            fields.append([HEADER_PATH, Variant("o", self.path, False)])
+            fields.append([HEADER_PATH, Variant("o", self.path, verify=False)])
         if self.interface:
-            fields.append([HEADER_INTERFACE, Variant("s", self.interface, False)])
+            fields.append(
+                [HEADER_INTERFACE, Variant("s", self.interface, verify=False)]
+            )
         if self.member:
-            fields.append([HEADER_MEMBER, Variant("s", self.member, False)])
+            fields.append([HEADER_MEMBER, Variant("s", self.member, verify=False)])
         if self.error_name:
-            fields.append([HEADER_ERROR_NAME, Variant("s", self.error_name, False)])
+            fields.append(
+                [HEADER_ERROR_NAME, Variant("s", self.error_name, verify=False)]
+            )
         if self.reply_serial:
-            fields.append([HEADER_REPLY_SERIAL, Variant("u", self.reply_serial, False)])
+            fields.append(
+                [HEADER_REPLY_SERIAL, Variant("u", self.reply_serial, verify=False)]
+            )
         if self.destination:
-            fields.append([HEADER_DESTINATION, Variant("s", self.destination, False)])
+            fields.append(
+                [HEADER_DESTINATION, Variant("s", self.destination, verify=False)]
+            )
         if self.signature:
-            fields.append([HEADER_SIGNATURE, Variant("g", self.signature, False)])
+            fields.append(
+                [HEADER_SIGNATURE, Variant("g", self.signature, verify=False)]
+            )
         if self.unix_fds and negotiate_unix_fd:
-            fields.append([HEADER_UNIX_FDS, Variant("u", len(self.unix_fds), False)])
+            fields.append(
+                [HEADER_UNIX_FDS, Variant("u", len(self.unix_fds), verify=False)]
+            )
 
         header_body = [
             LITTLE_ENDIAN,
             self.message_type.value,
             self.flags.value,
             PROTOCOL_VERSION,
-            len(body_buffer),
+            len(body_block.buffer),
             self.serial,
             fields,
         ]
         header_block = Marshaller("yyyyuua(yv)", header_body)
-        header_block._marshall()
-        header_block._align(8)
-        header_buffer = header_block._buffer()
-        return header_buffer + body_buffer
+        header_block.marshall()
+        header_block.align(8)
+        return header_block.buffer + body_block.buffer
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/message_bus.py` & `dbus-fast-1.9.0/src/dbus_fast/message_bus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import logging
 import socket
 import traceback
 import xml.etree.ElementTree as ET
-from types import TracebackType
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Callable, Optional, Type, Union
 
 from . import introspection as intr
 from ._private.address import get_bus_address, parse_address
 from ._private.util import replace_fds_with_idx, replace_idx_with_fds
 from .constants import (
     BusType,
     ErrorType,
@@ -17,78 +16,18 @@
     NameFlag,
     ReleaseNameReply,
     RequestNameReply,
 )
 from .errors import DBusError, InvalidAddressError
 from .message import Message
 from .proxy_object import BaseProxyObject
-from .service import ServiceInterface, _Method
+from .service import ServiceInterface
 from .signature import Variant
 from .validators import assert_bus_name_valid, assert_object_path_valid
 
-MESSAGE_TYPE_CALL = MessageType.METHOD_CALL
-MESSAGE_TYPE_SIGNAL = MessageType.SIGNAL
-NO_REPLY_EXPECTED_VALUE = MessageFlag.NO_REPLY_EXPECTED.value
-
-
-def _expects_reply(msg) -> bool:
-    return not (msg.flags.value & NO_REPLY_EXPECTED_VALUE)
-
-
-class SendReply:
-    """A context manager to send a reply to a message."""
-
-    __slots__ = ("_bus", "_msg")
-
-    def __init__(self, bus: "BaseMessageBus", msg: Message) -> None:
-        """Create a new reply context manager."""
-        self._bus = bus
-        self._msg = msg
-
-    def __enter__(self):
-        return self
-
-    def __call__(self, reply: Message) -> None:
-        if _expects_reply(self._msg):
-            self._bus.send(reply)
-
-    def _exit(
-        self,
-        exc_type: Optional[Type[Exception]],
-        exc_value: Optional[Exception],
-        tb: Optional[TracebackType],
-    ) -> bool:
-        if exc_type is None:
-            return False
-
-        if issubclass(exc_type, DBusError):
-            self(exc_value._as_message(self._msg))  # type: ignore[union-attr]
-            return True
-
-        if issubclass(exc_type, Exception):
-            self(
-                Message.new_error(
-                    self._msg,
-                    ErrorType.SERVICE_ERROR,
-                    f"The service interface raised an error: {exc_value}.\n{traceback.format_tb(tb)}",
-                )
-            )
-            return True
-
-    def __exit__(
-        self,
-        exc_type: Optional[Type[Exception]],
-        exc_value: Optional[Exception],
-        tb: Optional[TracebackType],
-    ) -> bool:
-        return self._exit(exc_type, exc_value, tb)
-
-    def send_error(self, exc: Exception) -> None:
-        self._exit(exc.__class__, exc, exc.__traceback__)
-
 
 class BaseMessageBus:
     """An abstract class to manage a connection to a DBus message bus.
 
     The message bus class is the entry point into all the features of the
     library. It sets up a connection to the DBus daemon and exposes an
     interface to send and receive messages and expose services.
@@ -112,90 +51,63 @@
         be :class:`None` until the message bus connects.
     :vartype unique_name: str
     :ivar connected: True if this message bus is expected to be able to send
         and receive messages.
     :vartype connected: bool
     """
 
-    __slots__ = (
-        "unique_name",
-        "_disconnected",
-        "_user_disconnect",
-        "_method_return_handlers",
-        "_serial",
-        "_user_message_handlers",
-        "_name_owners",
-        "_path_exports",
-        "_bus_address",
-        "_name_owner_match_rule",
-        "_match_rules",
-        "_high_level_client_initialized",
-        "_ProxyObject",
-        "_machine_id",
-        "_negotiate_unix_fd",
-        "_sock",
-        "_stream",
-        "_fd",
-    )
-
     def __init__(
         self,
         bus_address: Optional[str] = None,
         bus_type: BusType = BusType.SESSION,
         ProxyObject: Optional[Type[BaseProxyObject]] = None,
-        negotiate_unix_fd: bool = False,
-    ) -> None:
-        self.unique_name: Optional[str] = None
+    ):
+        self.unique_name = None
         self._disconnected = False
-        self._negotiate_unix_fd = negotiate_unix_fd
 
         # True if the user disconnected himself, so don't throw errors out of
         # the main loop.
         self._user_disconnect = False
 
-        self._method_return_handlers: Dict[
-            int, Callable[[Optional[Message], Optional[Exception]], None]
-        ] = {}
+        self._method_return_handlers = {}
         self._serial = 0
-        self._user_message_handlers: List[
-            Callable[[Message], Union[Message, bool, None]]
-        ] = []
+        self._user_message_handlers = []
         # the key is the name and the value is the unique name of the owner.
         # This cache is kept up to date by the NameOwnerChanged signal and is
         # used to route messages to the correct proxy object. (used for the
         # high level client only)
-        self._name_owners: Dict[str, str] = {}
+        self._name_owners = {}
         # used for the high level service
-        self._path_exports: Dict[str, list[ServiceInterface]] = {}
+        self._path_exports = {}
         self._bus_address = (
             parse_address(bus_address)
             if bus_address
             else parse_address(get_bus_address(bus_type))
         )
         # the bus implementations need this rule for the high level client to
         # work correctly.
         self._name_owner_match_rule = "sender='org.freedesktop.DBus',interface='org.freedesktop.DBus',path='/org/freedesktop/DBus',member='NameOwnerChanged'"
         # _match_rules: the keys are match rules and the values are ref counts
         # (used for the high level client only)
-        self._match_rules: Dict[str, int] = {}
+        self._match_rules = {}
         self._high_level_client_initialized = False
         self._ProxyObject = ProxyObject
 
         # machine id is lazy loaded
-        self._machine_id: Optional[int] = None
+        self._machine_id = None
 
         self._setup_socket()
 
     @property
-    def connected(self) -> bool:
+    def connected(self):
         if self.unique_name is None or self._disconnected or self._user_disconnect:
             return False
         return True
 
-    def export(self, path: str, interface: ServiceInterface) -> None:
+    def export(self, path: str, interface: ServiceInterface):
         """Export the service interface on this message bus to make it available
         to other clients.
 
         :param path: The object path to export this interface on.
         :type path: str
         :param interface: The service interface to export.
         :type interface: :class:`ServiceInterface
@@ -215,20 +127,20 @@
         for f in self._path_exports[path]:
             if f.name == interface.name:
                 raise ValueError(
                     f'An interface with this name is already exported on this bus at path "{path}": "{interface.name}"'
                 )
 
         self._path_exports[path].append(interface)
-        ServiceInterface._add_bus(interface, self, self._make_method_handler)
+        ServiceInterface._add_bus(interface, self)
         self._emit_interface_added(path, interface)
 
     def unexport(
         self, path: str, interface: Optional[Union[ServiceInterface, str]] = None
-    ) -> None:
+    ):
         """Unexport the path or service interface to make it no longer
         available to clients.
 
         :param path: The object path to unexport.
         :type path: str
         :param interface: The interface instance or the name of the interface
             to unexport. If ``None``, unexport every interface on the path.
@@ -274,15 +186,15 @@
         self._emit_interface_removed(path, removed_interfaces)
 
     def introspect(
         self,
         bus_name: str,
         path: str,
         callback: Callable[[Optional[intr.Node], Optional[Exception]], None],
-    ) -> None:
+    ):
         """Get introspection data for the node at the given path from the given
         bus name.
 
         Calls the standard ``org.freedesktop.DBus.Introspectable.Introspect``
         on the bus for the path.
 
         :param bus_name: The name to introspect.
@@ -295,18 +207,18 @@
 
         :raises:
             - :class:`InvalidObjectPathError <dbus_fast.InvalidObjectPathError>` - If the given object path is not valid.
             - :class:`InvalidBusNameError <dbus_fast.InvalidBusNameError>` - If the given bus name is not valid.
         """
         BaseMessageBus._check_callback_type(callback)
 
-        def reply_notify(reply: Optional[Message], err: Optional[Exception]) -> None:
+        def reply_notify(reply, err):
             try:
                 BaseMessageBus._check_method_return(reply, err, "s")
-                result = intr.Node.parse(reply.body[0])  # type: ignore[union-attr]
+                result = intr.Node.parse(reply.body[0])
             except Exception as e:
                 callback(None, e)
                 return
 
             callback(result, None)
 
         self._call(
@@ -315,35 +227,30 @@
                 path=path,
                 interface="org.freedesktop.DBus.Introspectable",
                 member="Introspect",
             ),
             reply_notify,
         )
 
-    def _emit_interface_added(self, path: str, interface: ServiceInterface) -> None:
+    def _emit_interface_added(self, path, interface):
         """Emit the ``org.freedesktop.DBus.ObjectManager.InterfacesAdded`` signal.
 
         This signal is intended to be used to alert clients when
         a new interface has been added.
 
         :param path: Path of exported object.
         :type path: str
         :param interface: Exported service interface.
         :type interface: :class:`ServiceInterface
             <dbus_fast.service.ServiceInterface>`
         """
         if self._disconnected:
             return
 
-        def get_properties_callback(
-            interface: ServiceInterface,
-            result: Any,
-            user_data: Any,
-            e: Optional[Exception],
-        ) -> None:
+        def get_properties_callback(interface, result, user_data, e):
             if e is not None:
                 try:
                     raise e
                 except Exception:
                     logging.error(
                         "An exception ocurred when emitting ObjectManager.InterfacesAdded for %s. "
                         "Some properties will not be included in the signal.",
@@ -361,15 +268,15 @@
                     signature="oa{sa{sv}}",
                     body=[path, body],
                 )
             )
 
         ServiceInterface._get_all_property_values(interface, get_properties_callback)
 
-    def _emit_interface_removed(self, path: str, removed_interfaces: List[str]) -> None:
+    def _emit_interface_removed(self, path, removed_interfaces):
         """Emit the ``org.freedesktop.DBus.ObjectManager.InterfacesRemoved` signal.
 
         This signal is intended to be used to alert clients when
         a interface has been removed.
 
         :param path: Path of removed (unexported) object.
         :type path: str
@@ -392,15 +299,15 @@
     def request_name(
         self,
         name: str,
         flags: NameFlag = NameFlag.NONE,
         callback: Optional[
             Callable[[Optional[RequestNameReply], Optional[Exception]], None]
         ] = None,
-    ) -> None:
+    ):
         """Request that this message bus owns the given name.
 
         :param name: The name to request.
         :type name: str
         :param flags: Name flags that affect the behavior of the name request.
         :type flags: :class:`NameFlag <dbus_fast.NameFlag>`
         :param callback: A callback that will be called with the reply of the
@@ -411,49 +318,46 @@
             - :class:`InvalidBusNameError <dbus_fast.InvalidBusNameError>` - If the given bus name is not valid.
         """
         assert_bus_name_valid(name)
 
         if callback is not None:
             BaseMessageBus._check_callback_type(callback)
 
-        if type(flags) is not NameFlag:
-            flags = NameFlag(flags)
-
-        message = Message(
-            destination="org.freedesktop.DBus",
-            path="/org/freedesktop/DBus",
-            interface="org.freedesktop.DBus",
-            member="RequestName",
-            signature="su",
-            body=[name, flags],
-        )
-
-        if callback is None:
-            self._call(message, None)
-            return
-
-        def reply_notify(reply: Optional[Message], err: Optional[Exception]) -> None:
+        def reply_notify(reply, err):
             try:
                 BaseMessageBus._check_method_return(reply, err, "u")
-                result = RequestNameReply(reply.body[0])  # type: ignore[union-attr]
+                result = RequestNameReply(reply.body[0])
             except Exception as e:
-                callback(None, e)  # type: ignore[misc]
+                callback(None, e)
                 return
 
-            callback(result, None)  # type: ignore[misc]
+            callback(result, None)
+
+        if type(flags) is not NameFlag:
+            flags = NameFlag(flags)
 
-        self._call(message, reply_notify)
+        self._call(
+            Message(
+                destination="org.freedesktop.DBus",
+                path="/org/freedesktop/DBus",
+                interface="org.freedesktop.DBus",
+                member="RequestName",
+                signature="su",
+                body=[name, flags],
+            ),
+            reply_notify if callback else None,
+        )
 
     def release_name(
         self,
         name: str,
         callback: Optional[
             Callable[[Optional[ReleaseNameReply], Optional[Exception]], None]
         ] = None,
-    ) -> None:
+    ):
         """Request that this message bus release the given name.
 
         :param name: The name to release.
         :type name: str
         :param callback: A callback that will be called with the reply of the
             release request as a :class:`ReleaseNameReply
             <dbus_fast.ReleaseNameReply>`.
@@ -463,38 +367,35 @@
             - :class:`InvalidBusNameError <dbus_fast.InvalidBusNameError>` - If the given bus name is not valid.
         """
         assert_bus_name_valid(name)
 
         if callback is not None:
             BaseMessageBus._check_callback_type(callback)
 
-        message = Message(
-            destination="org.freedesktop.DBus",
-            path="/org/freedesktop/DBus",
-            interface="org.freedesktop.DBus",
-            member="ReleaseName",
-            signature="s",
-            body=[name],
-        )
-
-        if callback is None:
-            self._call(message, None)
-            return
-
-        def reply_notify(reply: Optional[Message], err: Optional[Exception]) -> None:
+        def reply_notify(reply, err):
             try:
                 BaseMessageBus._check_method_return(reply, err, "u")
-                result = ReleaseNameReply(reply.body[0])  # type: ignore[union-attr]
+                result = ReleaseNameReply(reply.body[0])
             except Exception as e:
-                callback(None, e)  # type: ignore[misc]
+                callback(None, e)
                 return
 
-            callback(result, None)  # type: ignore[misc]
+            callback(result, None)
 
-        self._call(message, reply_notify)
+        self._call(
+            Message(
+                destination="org.freedesktop.DBus",
+                path="/org/freedesktop/DBus",
+                interface="org.freedesktop.DBus",
+                member="ReleaseName",
+                signature="s",
+                body=[name],
+            ),
+            reply_notify if callback else None,
+        )
 
     def get_proxy_object(
         self, bus_name: str, path: str, introspection: Union[intr.Node, str, ET.Element]
     ) -> BaseProxyObject:
         """Get a proxy object for the path exported on the bus that owns the
         name. The object is expected to export the interfaces and nodes
         specified in the introspection data.
@@ -522,15 +423,15 @@
                 "the message bus implementation did not provide a proxy object class"
             )
 
         self._init_high_level_client()
 
         return self._ProxyObject(bus_name, path, introspection, self)
 
-    def disconnect(self) -> None:
+    def disconnect(self):
         """Disconnect the message bus by closing the underlying connection asynchronously.
 
         All pending  and future calls will error with a connection error.
         """
         self._user_disconnect = True
         try:
             self._sock.shutdown(socket.SHUT_RDWR)
@@ -546,15 +447,15 @@
         :rtype: int
         """
         self._serial += 1
         return self._serial
 
     def add_message_handler(
         self, handler: Callable[[Message], Optional[Union[Message, bool]]]
-    ) -> None:
+    ):
         """Add a custom message handler for incoming messages.
 
         The handler should be a callable that takes a :class:`Message
         <dbus_fast.Message>`. If the message is a method call, you may return
         another Message as a reply and it will be marked as handled. You may
         also return ``True`` to mark the message as handled without sending a
         reply.
@@ -571,38 +472,38 @@
         if len(handler_signature.parameters) != 1:
             raise TypeError(error_text)
 
         self._user_message_handlers.append(handler)
 
     def remove_message_handler(
         self, handler: Callable[[Message], Optional[Union[Message, bool]]]
-    ) -> None:
+    ):
         """Remove a message handler that was previously added by
         :func:`add_message_handler()
         <dbus_fast.message_bus.BaseMessageBus.add_message_handler>`.
 
         :param handler: A message handler.
         :type handler: :class:`Callable`
         """
         for i, h in enumerate(self._user_message_handlers):
             if h == handler:
                 del self._user_message_handlers[i]
-                return
+                break
 
     def send(self, msg: Message) -> None:
         """Asynchronously send a message on the message bus.
 
         :param msg: The message to send.
         :type msg: :class:`Message <dbus_fast.Message>`
         """
         raise NotImplementedError(
             'the "send" method must be implemented in the inheriting class'
         )
 
-    def _finalize(self, err: Optional[Exception]) -> None:
+    def _finalize(self, err):
         """should be called after the socket disconnects with the disconnection
         error to clean up resources and put the bus in a disconnected state"""
         if self._disconnected:
             return
 
         self._disconnected = True
 
@@ -626,22 +527,16 @@
             for iface in exports:
                 if iface is interface:
                     return True
 
         return False
 
     def _interface_signal_notify(
-        self,
-        interface: ServiceInterface,
-        interface_name: str,
-        member: str,
-        signature: str,
-        body: List[Any],
-        unix_fds: List[int] = [],
-    ) -> None:
+        self, interface, interface_name, member, signature, body, unix_fds=[]
+    ):
         path = None
         for p, ifaces in self._path_exports.items():
             for i in ifaces:
                 if i is interface:
                     path = p
 
         if path is None:
@@ -656,15 +551,15 @@
                 member=member,
                 signature=signature,
                 body=body,
                 unix_fds=unix_fds,
             )
         )
 
-    def _introspect_export_path(self, path: str) -> intr.Node:
+    def _introspect_export_path(self, path):
         assert_object_path_valid(path)
 
         if path in self._path_exports:
             node = intr.Node.default(path)
             for interface in self._path_exports[path]:
                 node.interfaces.append(interface.introspect())
         else:
@@ -683,15 +578,15 @@
 
             children.add(child_name)
 
         node.nodes = [intr.Node(name) for name in children if name]
 
         return node
 
-    def _setup_socket(self) -> None:
+    def _setup_socket(self):
         err = None
 
         for transport, options in self._bus_address:
             filename = None
             ip_addr = ""
             ip_port = 0
 
@@ -699,15 +594,15 @@
                 self._sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
                 self._stream = self._sock.makefile("rwb")
                 self._fd = self._sock.fileno()
 
                 if "path" in options:
                     filename = options["path"]
                 elif "abstract" in options:
-                    filename = b"\0" + options["abstract"].encode()
+                    filename = f'\0{options["abstract"]}'
                 else:
                     raise InvalidAddressError(
                         "got unix transport with unknown path specifier"
                     )
 
                 try:
                     self._sock.connect(filename)
@@ -735,234 +630,248 @@
 
             else:
                 raise InvalidAddressError(f"got unknown address transport: {transport}")
 
         if err:
             raise err
 
-    def _call(
-        self,
-        msg: Message,
-        callback: Optional[Callable[[Optional[Message], Optional[Exception]], None]],
-        check_callback: bool = True,
-    ) -> None:
+    def _call(self, msg, callback, check_callback: bool = True) -> None:
         if check_callback:
             BaseMessageBus._check_callback_type(callback)
 
         if not msg.serial:
             msg.serial = self.next_serial()
 
-        def reply_notify(reply: Optional[Message], err: Optional[Exception]) -> None:
-            if reply and msg.destination and reply.sender:
+        def reply_notify(reply, err):
+            if reply:
                 self._name_owners[msg.destination] = reply.sender
-            callback(reply, err)  # type: ignore[misc]
+            callback(reply, err)
 
-        no_reply_expected = not _expects_reply(msg)
+        no_reply_expected = msg.flags & MessageFlag.NO_REPLY_EXPECTED
 
         # Make sure the return reply handler is installed
         # before sending the message to avoid a race condition
         # where the reply is lost in case the backend can
         # send it right away.
         if not no_reply_expected:
             self._method_return_handlers[msg.serial] = reply_notify
 
         self.send(msg)
 
         if no_reply_expected:
-            callback(None, None)  # type: ignore[misc]
+            callback(None, None)
 
     @staticmethod
-    def _check_callback_type(callback: Callable) -> None:
+    def _check_callback_type(callback):
         """Raise a TypeError if the user gives an invalid callback as a parameter"""
 
         text = "a callback must be callable with two parameters"
 
         if not callable(callback):
             raise TypeError(text)
 
         fn_signature = inspect.signature(callback)
         if len(fn_signature.parameters) != 2:
             raise TypeError(text)
 
     @staticmethod
-    def _check_method_return(
-        msg: Optional[Message], err: Optional[Exception], signature: str
-    ) -> None:
+    def _check_method_return(msg, err, signature):
         if err:
             raise err
-        elif msg is None:
-            raise DBusError(
-                ErrorType.INTERNAL_ERROR, "invalid message type for method call", msg
-            )
         elif (
             msg.message_type == MessageType.METHOD_RETURN and msg.signature == signature
         ):
             return
         elif msg.message_type == MessageType.ERROR:
             raise DBusError._from_message(msg)
         else:
             raise DBusError(
                 ErrorType.INTERNAL_ERROR, "invalid message type for method call", msg
             )
 
-    def _process_message(self, msg) -> None:
+    def _on_message(self, msg):
+        try:
+            self._process_message(msg)
+        except Exception as e:
+            logging.error(
+                f"got unexpected error processing a message: {e}.\n{traceback.format_exc()}"
+            )
+
+    def _send_reply(self, msg):
+        bus = self
+
+        class SendReply:
+            def __enter__(self):
+                return self
+
+            def __call__(self, reply):
+                if msg.flags & MessageFlag.NO_REPLY_EXPECTED:
+                    return
+
+                bus.send(reply)
+
+            def _exit(self, exc_type, exc_value, tb):
+                if exc_type is None:
+                    return
+
+                if issubclass(exc_type, DBusError):
+                    self(exc_value._as_message(msg))
+                    return True
+
+                if issubclass(exc_type, Exception):
+                    self(
+                        Message.new_error(
+                            msg,
+                            ErrorType.SERVICE_ERROR,
+                            f"The service interface raised an error: {exc_value}.\n{traceback.format_tb(tb)}",
+                        )
+                    )
+                    return True
+
+            def __exit__(self, exc_type, exc_value, tb):
+                self._exit(exc_type, exc_value, tb)
+
+            def send_error(self, exc):
+                self._exit(exc.__class__, exc, exc.__traceback__)
+
+        return SendReply()
+
+    def _process_message(self, msg):
         handled = False
-        for user_handler in self._user_message_handlers:
+
+        for handler in self._user_message_handlers:
             try:
-                result = user_handler(msg)
+                result = handler(msg)
                 if result:
                     if type(result) is Message:
                         self.send(result)
                     handled = True
                     break
             except DBusError as e:
-                if msg.message_type is MESSAGE_TYPE_CALL:
+                if msg.message_type == MessageType.METHOD_CALL:
                     self.send(e._as_message(msg))
                     handled = True
                     break
                 else:
                     logging.error(
                         f"A message handler raised an exception: {e}.\n{traceback.format_exc()}"
                     )
             except Exception as e:
                 logging.error(
                     f"A message handler raised an exception: {e}.\n{traceback.format_exc()}"
                 )
-                if msg.message_type is MESSAGE_TYPE_CALL:
+                if msg.message_type == MessageType.METHOD_CALL:
                     self.send(
                         Message.new_error(
                             msg,
                             ErrorType.INTERNAL_ERROR,
                             f"An internal error occurred: {e}.\n{traceback.format_exc()}",
                         )
                     )
                     handled = True
                     break
 
-        if msg.message_type is MESSAGE_TYPE_SIGNAL:
-            if (
-                msg.member == "NameOwnerChanged"
-                and msg.sender == "org.freedesktop.DBus"
-                and msg.path == "/org/freedesktop/DBus"
-                and msg.interface == "org.freedesktop.DBus"
+        if msg.message_type == MessageType.SIGNAL:
+            if msg._matches(
+                member="NameOwnerChanged",  # least likely to match
+                sender="org.freedesktop.DBus",
+                path="/org/freedesktop/DBus",
+                interface="org.freedesktop.DBus",
             ):
                 [name, old_owner, new_owner] = msg.body
                 if new_owner:
                     self._name_owners[name] = new_owner
                 elif name in self._name_owners:
                     del self._name_owners[name]
-            return
 
-        if msg.message_type is MESSAGE_TYPE_CALL:
+        elif msg.message_type == MessageType.METHOD_CALL:
             if not handled:
                 handler = self._find_message_handler(msg)
 
-                send_reply = SendReply(self, msg)
+                send_reply = self._send_reply(msg)
 
                 with send_reply:
                     if handler:
                         handler(msg, send_reply)
                     else:
                         send_reply(
                             Message.new_error(
                                 msg,
                                 ErrorType.UNKNOWN_METHOD,
                                 f'{msg.interface}.{msg.member} with signature "{msg.signature}" could not be found',
                             )
                         )
-            return
 
-        # An ERROR or a METHOD_RETURN
-        if msg.reply_serial in self._method_return_handlers:
-            if not handled:
-                return_handler = self._method_return_handlers[msg.reply_serial]
-                return_handler(msg, None)
-            del self._method_return_handlers[msg.reply_serial]
-
-    def _make_method_handler(
-        self, interface: ServiceInterface, method: _Method
-    ) -> Callable[[Message, Callable[[Message], None]], None]:
-        def handler(msg: Message, send_reply: Callable[[Message], None]) -> None:
+        else:
+            # An ERROR or a METHOD_RETURN
+            if msg.reply_serial in self._method_return_handlers:
+                if not handled:
+                    handler = self._method_return_handlers[msg.reply_serial]
+                    handler(msg, None)
+                del self._method_return_handlers[msg.reply_serial]
+
+    def _make_method_handler(self, interface, method):
+        def handler(msg, send_reply):
             args = ServiceInterface._msg_body_to_args(msg)
             result = method.fn(interface, *args)
             body, fds = ServiceInterface._fn_result_to_body(
-                result,
-                signature_tree=method.out_signature_tree,
-                replace_fds=self._negotiate_unix_fd,
-            )
-            send_reply(
-                Message(
-                    message_type=MessageType.METHOD_RETURN,
-                    reply_serial=msg.serial,
-                    destination=msg.sender,
-                    signature=method.out_signature,
-                    body=body,
-                    unix_fds=fds,
-                )
+                result, signature_tree=method.out_signature_tree
             )
+            send_reply(Message.new_method_return(msg, method.out_signature, body, fds))
 
         return handler
 
-    def _find_message_handler(
-        self, msg
-    ) -> Optional[Callable[[Message, Callable], None]]:
-        handler: Optional[Callable[[Message, Callable], None]] = None
-
-        if (
-            msg.interface == "org.freedesktop.DBus.Introspectable"
-            and msg.member == "Introspect"
-            and msg.signature == ""
+    def _find_message_handler(self, msg):
+        handler = None
+
+        if msg._matches(
+            interface="org.freedesktop.DBus.Introspectable",
+            member="Introspect",
+            signature="",
         ):
             handler = self._default_introspect_handler
 
-        elif msg.interface == "org.freedesktop.DBus.Properties":
+        elif msg._matches(interface="org.freedesktop.DBus.Properties"):
             handler = self._default_properties_handler
 
-        elif msg.interface == "org.freedesktop.DBus.Peer":
-            if msg.member == "Ping" and msg.signature == "":
+        elif msg._matches(interface="org.freedesktop.DBus.Peer"):
+            if msg._matches(member="Ping", signature=""):
                 handler = self._default_ping_handler
-            elif msg.member == "GetMachineId" and msg.signature == "":
+            elif msg._matches(member="GetMachineId", signature=""):
                 handler = self._default_get_machine_id_handler
-        elif (
-            msg.interface == "org.freedesktop.DBus.ObjectManager"
-            and msg.member == "GetManagedObjects"
+        elif msg._matches(
+            interface="org.freedesktop.DBus.ObjectManager", member="GetManagedObjects"
         ):
             handler = self._default_get_managed_objects_handler
 
-        elif msg.path:
+        else:
             for interface in self._path_exports.get(msg.path, []):
                 for method in ServiceInterface._get_methods(interface):
                     if method.disabled:
                         continue
-                    if (
-                        msg.interface == interface.name
-                        and msg.member == method.name
-                        and msg.signature == method.in_signature
+                    if msg._matches(
+                        interface=interface.name,
+                        member=method.name,
+                        signature=method.in_signature,
                     ):
-                        handler = ServiceInterface._get_handler(interface, method, self)
+                        handler = self._make_method_handler(interface, method)
                         break
                 if handler:
                     break
 
         return handler
 
-    def _default_introspect_handler(
-        self, msg: Message, send_reply: Callable[[Message], None]
-    ) -> None:
+    def _default_introspect_handler(self, msg, send_reply):
         introspection = self._introspect_export_path(msg.path).tostring()
         send_reply(Message.new_method_return(msg, "s", [introspection]))
 
-    def _default_ping_handler(
-        self, msg: Message, send_reply: Callable[[Message], None]
-    ) -> None:
+    def _default_ping_handler(self, msg, send_reply):
         send_reply(Message.new_method_return(msg))
 
-    def _default_get_machine_id_handler(
-        self, msg: Message, send_reply: Callable[[Message], None]
-    ) -> None:
+    def _default_get_machine_id_handler(self, msg, send_reply):
         if self._machine_id:
             send_reply(Message.new_method_return(msg, "s", self._machine_id))
             return
 
         def reply_handler(reply, err):
             if err:
                 # the bus has been disconnected, cannot send a reply
@@ -985,17 +894,15 @@
                 interface="org.freedesktop.DBus.Peer",
                 member="GetMachineId",
             ),
             reply_handler,
             check_callback=False,
         )
 
-    def _default_get_managed_objects_handler(
-        self, msg: Message, send_reply: Callable[[Message], None]
-    ) -> None:
+    def _default_get_managed_objects_handler(self, msg, send_reply):
         result = {}
         result_signature = "a{oa{sa{sv}}}"
         error_handled = False
 
         def is_result_complete():
             if not result:
                 return True
@@ -1037,17 +944,15 @@
 
         for node in nodes:
             for interface in self._path_exports[node]:
                 ServiceInterface._get_all_property_values(
                     interface, get_all_properties_callback, node
                 )
 
-    def _default_properties_handler(
-        self, msg: Message, send_reply: Callable[[Message], None]
-    ) -> None:
+    def _default_properties_handler(self, msg, send_reply):
         methods = {"Get": "ss", "Set": "ssv", "GetAll": "s"}
         if msg.member not in methods or methods[msg.member] != msg.signature:
             raise DBusError(
                 ErrorType.UNKNOWN_METHOD,
                 f'properties interface doesn\'t have method "{msg.member}" with signature "{msg.signature}"',
             )
 
@@ -1181,15 +1086,15 @@
             ServiceInterface._get_all_property_values(
                 interface, get_all_properties_callback
             )
 
         else:
             assert False
 
-    def _init_high_level_client(self) -> None:
+    def _init_high_level_client(self):
         """The high level client is initialized when the first proxy object is
         gotten. Currently just sets up the match rules for the name owner cache
         so signals can be routed to the right objects."""
         if self._high_level_client_initialized:
             return
         self._high_level_client_initialized = True
 
@@ -1225,15 +1130,15 @@
 
         if match_rule in self._match_rules:
             self._match_rules[match_rule] += 1
             return
 
         self._match_rules[match_rule] = 1
 
-        def add_match_notify(msg: Message, err: Optional[Exception]) -> None:
+        def add_match_notify(msg, err):
             if err:
                 logging.error(f'add match request failed. match="{match_rule}", {err}')
             if msg.message_type == MessageType.ERROR:
                 logging.error(
                     f'add match request failed. match="{match_rule}", {msg.body[0]}'
                 )
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/proxy_object.py` & `dbus-fast-1.9.0/src/dbus_fast/proxy_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 import inspect
 import logging
 import re
 import xml.etree.ElementTree as ET
 from dataclasses import dataclass
-from functools import lru_cache
-from typing import Callable, Coroutine, Dict, List, Optional, Type, Union
+from typing import Callable, Coroutine, Dict, List, Type, Union
 
 from . import introspection as intr
 from . import message_bus
 from ._private.util import replace_idx_with_fds
 from .constants import ErrorType, MessageType
 from .errors import DBusError, InterfaceNotFoundError
 from .message import Message
-from .unpack import unpack_variants as unpack
+from .signature import unpack_variants as unpack
 from .validators import assert_bus_name_valid, assert_object_path_valid
 
 
 @dataclass
 class SignalHandler:
     """Signal handler."""
 
@@ -47,64 +46,59 @@
     :vartype path: str
     :ivar introspection: Parsed introspection data for the proxy interface.
     :vartype introspection: :class:`Node <dbus_fast.introspection.Interface>`
     :ivar bus: The message bus this proxy interface is connected to.
     :vartype bus: :class:`BaseMessageBus <dbus_fast.message_bus.BaseMessageBus>`
     """
 
-    def __init__(
-        self,
-        bus_name: str,
-        path: str,
-        introspection: intr.Interface,
-        bus: "message_bus.BaseMessageBus",
-    ) -> None:
+    def __init__(self, bus_name, path, introspection, bus):
 
         self.bus_name = bus_name
         self.path = path
         self.introspection = introspection
         self.bus = bus
         self._signal_handlers: Dict[str, List[SignalHandler]] = {}
         self._signal_match_rule = f"type='signal',sender={bus_name},interface={introspection.name},path={path}"
 
     _underscorer1 = re.compile(r"(.)([A-Z][a-z]+)")
     _underscorer2 = re.compile(r"([a-z0-9])([A-Z])")
 
     @staticmethod
-    @lru_cache(maxsize=128)
-    def _to_snake_case(member: str) -> str:
+    def _to_snake_case(member):
         subbed = BaseProxyInterface._underscorer1.sub(r"\1_\2", member)
         return BaseProxyInterface._underscorer2.sub(r"\1_\2", subbed).lower()
 
     @staticmethod
-    def _check_method_return(msg: Message, signature: Optional[str] = None):
+    def _check_method_return(msg, signature=None):
         if msg.message_type == MessageType.ERROR:
             raise DBusError._from_message(msg)
         elif msg.message_type != MessageType.METHOD_RETURN:
             raise DBusError(
                 ErrorType.CLIENT_ERROR, "method call didnt return a method return", msg
             )
         elif signature is not None and msg.signature != signature:
             raise DBusError(
                 ErrorType.CLIENT_ERROR,
                 f'method call returned unexpected signature: "{msg.signature}"',
                 msg,
             )
 
-    def _add_method(self, intr_method: intr.Method) -> None:
+    def _add_method(self, intr_method):
         raise NotImplementedError("this must be implemented in the inheriting class")
 
-    def _add_property(self, intr_property: intr.Property) -> None:
+    def _add_property(self, intr_property):
         raise NotImplementedError("this must be implemented in the inheriting class")
 
-    def _message_handler(self, msg: Message) -> None:
+    def _message_handler(self, msg):
         if (
-            msg.message_type != MessageType.SIGNAL
-            or msg.interface != self.introspection.name
-            or msg.path != self.path
+            not msg._matches(
+                message_type=MessageType.SIGNAL,
+                interface=self.introspection.name,
+                path=self.path,
+            )
             or msg.member not in self._signal_handlers
         ):
             return
 
         if (
             msg.sender != self.bus_name
             and self.bus._name_owners.get(self.bus_name, "") != msg.sender
@@ -135,16 +129,16 @@
             else:
                 data = body
 
             cb_result = handler.fn(*data)
             if isinstance(cb_result, Coroutine):
                 asyncio.create_task(cb_result)
 
-    def _add_signal(self, intr_signal: intr.Signal, interface: intr.Interface) -> None:
-        def on_signal_fn(fn: Callable, *, unpack_variants: bool = False):
+    def _add_signal(self, intr_signal, interface):
+        def on_signal_fn(fn, *, unpack_variants: bool = False):
             fn_signature = inspect.signature(fn)
             if 0 < len(
                 [
                     par
                     for par in fn_signature.parameters.values()
                     if par.kind == inspect.Parameter.KEYWORD_ONLY
                     and par.default == inspect.Parameter.empty
@@ -175,15 +169,15 @@
             if intr_signal.name not in self._signal_handlers:
                 self._signal_handlers[intr_signal.name] = []
 
             self._signal_handlers[intr_signal.name].append(
                 SignalHandler(fn, unpack_variants)
             )
 
-        def off_signal_fn(fn: Callable, *, unpack_variants: bool = False) -> None:
+        def off_signal_fn(fn, *, unpack_variants: bool = False):
             try:
                 i = self._signal_handlers[intr_signal.name].index(
                     SignalHandler(fn, unpack_variants)
                 )
                 del self._signal_handlers[intr_signal.name][i]
                 if not self._signal_handlers[intr_signal.name]:
                     del self._signal_handlers[intr_signal.name]
@@ -237,15 +231,15 @@
     def __init__(
         self,
         bus_name: str,
         path: str,
         introspection: Union[intr.Node, str, ET.Element],
         bus: "message_bus.BaseMessageBus",
         ProxyInterface: Type[BaseProxyInterface],
-    ) -> None:
+    ):
         assert_object_path_valid(path)
         assert_bus_name_valid(bus_name)
 
         if not isinstance(bus, message_bus.BaseMessageBus):
             raise TypeError("bus must be an instance of BaseMessageBus")
         if not issubclass(ProxyInterface, BaseProxyInterface):
             raise TypeError("ProxyInterface must be an instance of BaseProxyInterface")
@@ -298,15 +292,15 @@
         for intr_method in intr_interface.methods:
             interface._add_method(intr_method)
         for intr_property in intr_interface.properties:
             interface._add_property(intr_property)
         for intr_signal in intr_interface.signals:
             interface._add_signal(intr_signal, interface)
 
-        def get_owner_notify(msg: Message, err: Optional[Exception]) -> None:
+        def get_owner_notify(msg, err):
             if err:
                 logging.error(f'getting name owner for "{name}" failed, {err}')
                 return
             if msg.message_type == MessageType.ERROR:
                 if msg.error_name != ErrorType.NAME_HAS_NO_OWNER.value:
                     logging.error(
                         f'getting name owner for "{name}" failed, {msg.body[0]}'
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/service.py` & `dbus-fast-1.9.0/src/dbus_fast/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,23 @@
 import asyncio
 import copy
 import inspect
 from functools import wraps
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    no_type_check_decorator,
-)
+from typing import Any, Dict, List, no_type_check_decorator
 
 from . import introspection as intr
 from ._private.util import (
     parse_annotation,
     replace_fds_with_idx,
     replace_idx_with_fds,
     signature_contains_type,
 )
 from .constants import PropertyAccess
 from .errors import SignalDisabledError
-from .message import Message
-from .signature import (
-    SignatureBodyMismatchError,
-    SignatureTree,
-    Variant,
-    get_signature_tree,
-)
-
-if TYPE_CHECKING:
-    from .message_bus import BaseMessageBus
+from .signature import SignatureBodyMismatchError, SignatureTree, Variant
 
 
 class _Method:
     def __init__(self, fn, name, disabled=False):
         in_signature = ""
         out_signature = ""
 
@@ -54,25 +35,25 @@
                 )
             in_args.append(intr.Arg(annotation, intr.ArgDirection.IN, param.name))
             in_signature += annotation
 
         out_args = []
         out_signature = parse_annotation(inspection.return_annotation)
         if out_signature:
-            for type_ in get_signature_tree(out_signature).types:
+            for type_ in SignatureTree._get(out_signature).types:
                 out_args.append(intr.Arg(type_, intr.ArgDirection.OUT))
 
         self.name = name
         self.fn = fn
         self.disabled = disabled
         self.introspection = intr.Method(name, in_args, out_args)
         self.in_signature = in_signature
         self.out_signature = out_signature
-        self.in_signature_tree = get_signature_tree(in_signature)
-        self.out_signature_tree = get_signature_tree(out_signature)
+        self.in_signature_tree = SignatureTree._get(in_signature)
+        self.out_signature_tree = SignatureTree._get(out_signature)
 
 
 def method(name: str = None, disabled: bool = False):
     """A decorator to mark a class method of a :class:`ServiceInterface` to be a DBus service method.
 
     The parameters and return value must each be annotated with a signature
     string of a single complete DBus type.
@@ -131,20 +112,20 @@
         signature = ""
         signature_tree = None
 
         return_annotation = parse_annotation(inspection.return_annotation)
 
         if return_annotation:
             signature = return_annotation
-            signature_tree = get_signature_tree(signature)
+            signature_tree = SignatureTree._get(signature)
             for type_ in signature_tree.types:
                 args.append(intr.Arg(type_, intr.ArgDirection.OUT))
         else:
             signature = ""
-            signature_tree = get_signature_tree("")
+            signature_tree = SignatureTree._get("")
 
         self.signature = signature
         self.signature_tree = signature_tree
         self.name = name
         self.disabled = disabled
         self.introspection = intr.Signal(self.name, args)
 
@@ -241,15 +222,15 @@
 
         if not return_annotation:
             raise ValueError(
                 "the property must specify the dbus type string as a return annotation string"
             )
 
         self.signature = return_annotation
-        tree = get_signature_tree(return_annotation)
+        tree = SignatureTree._get(return_annotation)
 
         if len(tree.types) != 1:
             raise ValueError("the property signature must be a single complete type")
 
         self.type = tree.types[0]
 
         if "options" in kwargs:
@@ -342,22 +323,18 @@
         valid interface name.
     :vartype name: str
     """
 
     def __init__(self, name: str):
         # TODO cannot be overridden by a dbus member
         self.name = name
-        self.__methods: List[_Method] = []
-        self.__properties: List[_Property] = []
-        self.__signals: List[_Signal] = []
+        self.__methods = []
+        self.__properties = []
+        self.__signals = []
         self.__buses = set()
-        self.__handlers: dict[
-            BaseMessageBus,
-            dict[_Method, Callable[[Message, Callable[[Message], None]], None]],
-        ] = {}
 
         for name, member in inspect.getmembers(type(self)):
             member_dict = getattr(member, "__dict__", {})
             if type(member) is _Property:
                 # XXX The getter and the setter may show up as different
                 # members if they have different names. But if they have the
                 # same name, they will be the same member. So we try to merge
@@ -444,72 +421,51 @@
                 prop.introspection
                 for prop in ServiceInterface._get_properties(self)
                 if not prop.disabled
             ],
         )
 
     @staticmethod
-    def _get_properties(interface: "ServiceInterface") -> List[_Property]:
+    def _get_properties(interface):
         return interface.__properties
 
     @staticmethod
-    def _get_methods(interface: "ServiceInterface") -> List[_Method]:
+    def _get_methods(interface):
         return interface.__methods
 
     @staticmethod
-    def _get_signals(interface: "ServiceInterface") -> List[_Signal]:
+    def _get_signals(interface):
         return interface.__signals
 
     @staticmethod
-    def _get_buses(interface: "ServiceInterface") -> Set["BaseMessageBus"]:
+    def _get_buses(interface):
         return interface.__buses
 
     @staticmethod
-    def _get_handler(
-        interface: "ServiceInterface", method: _Method, bus: "BaseMessageBus"
-    ) -> Callable[[Message, Callable[[Message], None]], None]:
-        return interface.__handlers[bus][method]
-
-    @staticmethod
-    def _add_bus(
-        interface: "ServiceInterface",
-        bus: "BaseMessageBus",
-        maker: Callable[
-            ["ServiceInterface", _Method],
-            Callable[[Message, Callable[[Message], None]], None],
-        ],
-    ) -> None:
+    def _add_bus(interface, bus):
         interface.__buses.add(bus)
-        interface.__handlers[bus] = {
-            method: maker(interface, method) for method in interface.__methods
-        }
 
     @staticmethod
-    def _remove_bus(interface: "ServiceInterface", bus: "BaseMessageBus") -> None:
+    def _remove_bus(interface, bus):
         interface.__buses.remove(bus)
-        del interface.__handlers[bus]
 
     @staticmethod
-    def _msg_body_to_args(msg: Message) -> List[Any]:
-        if not msg.unix_fds or not signature_contains_type(
-            msg.signature_tree, msg.body, "h"
-        ):
+    def _msg_body_to_args(msg):
+        if signature_contains_type(msg.signature_tree, msg.body, "h"):
+            # XXX: This deep copy could be expensive if messages are very
+            # large. We could optimize this by only copying what we change
+            # here.
+            return replace_idx_with_fds(
+                msg.signature_tree, copy.deepcopy(msg.body), msg.unix_fds
+            )
+        else:
             return msg.body
 
-        # XXX: This deep copy could be expensive if messages are very
-        # large. We could optimize this by only copying what we change
-        # here.
-        return replace_idx_with_fds(
-            msg.signature_tree, copy.deepcopy(msg.body), msg.unix_fds
-        )
-
     @staticmethod
-    def _fn_result_to_body(
-        result: List[Any], signature_tree: SignatureTree, replace_fds: bool = True
-    ) -> Tuple[List[Any], List[int]]:
+    def _fn_result_to_body(result, signature_tree):
         """The high level interfaces may return single values which may be
         wrapped in a list to be a message body. Also they may return fds
         directly for type 'h' which need to be put into an external list."""
         out_len = len(signature_tree.types)
         if result is None:
             result = []
         else:
@@ -522,30 +478,26 @@
                     )
 
         if out_len != len(result):
             raise SignatureBodyMismatchError(
                 f"Signature and function return mismatch, expected {len(signature_tree.types)} arguments but got {len(result)}"
             )
 
-        if not replace_fds:
-            return result, []
         return replace_fds_with_idx(signature_tree, result)
 
     @staticmethod
-    def _handle_signal(
-        interface: "ServiceInterface", signal: _Signal, result: List[Any]
-    ) -> None:
+    def _handle_signal(interface, signal, result):
         body, fds = ServiceInterface._fn_result_to_body(result, signal.signature_tree)
         for bus in ServiceInterface._get_buses(interface):
             bus._interface_signal_notify(
                 interface, interface.name, signal.name, signal.signature, body, fds
             )
 
     @staticmethod
-    def _get_property_value(interface: "ServiceInterface", prop: _Property, callback):
+    def _get_property_value(interface, prop, callback):
         # XXX MUST CHECK TYPE RETURNED BY GETTER
         try:
             if asyncio.iscoroutinefunction(prop.prop_getter):
                 task = asyncio.ensure_future(prop.prop_getter(interface))
 
                 def get_property_callback(task):
                     try:
@@ -562,15 +514,15 @@
             callback(
                 interface, prop, getattr(interface, prop.prop_getter.__name__), None
             )
         except Exception as e:
             callback(interface, prop, None, e)
 
     @staticmethod
-    def _set_property_value(interface: "ServiceInterface", prop, value, callback):
+    def _set_property_value(interface, prop, value, callback):
         # XXX MUST CHECK TYPE TO SET
         try:
             if asyncio.iscoroutinefunction(prop.prop_setter):
                 task = asyncio.ensure_future(prop.prop_setter(interface, value))
 
                 def set_property_callback(task):
                     try:
@@ -586,35 +538,28 @@
 
             setattr(interface, prop.prop_setter.__name__, value)
             callback(interface, prop, None)
         except Exception as e:
             callback(interface, prop, e)
 
     @staticmethod
-    def _get_all_property_values(
-        interface: "ServiceInterface", callback, user_data=None
-    ):
+    def _get_all_property_values(interface, callback, user_data=None):
         result = {}
         result_error = None
 
         for prop in ServiceInterface._get_properties(interface):
             if prop.disabled or not prop.access.readable():
                 continue
             result[prop.name] = None
 
         if not result:
             callback(interface, result, user_data, None)
             return
 
-        def get_property_callback(
-            interface: "ServiceInterface",
-            prop: _Property,
-            value: Any,
-            e: Optional[Exception],
-        ) -> None:
+        def get_property_callback(interface, prop, value, e):
             nonlocal result_error
             if e is not None:
                 result_error = e
                 del result[prop.name]
             else:
                 try:
                     result[prop.name] = Variant(prop.signature, value)
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/signature.py` & `dbus-fast-1.9.0/src/dbus_fast/signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from functools import lru_cache
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, List, Union
 
 from .errors import InvalidSignatureError, SignatureBodyMismatchError
 from .validators import is_object_path_valid
 
 
+def unpack_variants(data: Any):
+    """Unpack variants and remove signature info."""
+    if isinstance(data, Variant):
+        return unpack_variants(data.value)
+    if isinstance(data, dict):
+        return {k: unpack_variants(v) for k, v in data.items()}
+    if isinstance(data, list):
+        return [unpack_variants(item) for item in data]
+    return data
+
+
 class SignatureType:
     """A class that represents a single complete type within a signature.
 
     This class is not meant to be constructed directly. Use the :class:`SignatureTree`
     class to parse signatures.
 
     :ivar ~.signature: The signature of this complete type.
@@ -17,27 +28,27 @@
     :ivar children: A list of child types if this is a container type. Arrays \
     have one child type, dict entries have two child types (key and value), and \
     structs have child types equal to the number of struct members.
     :vartype children: list(:class:`SignatureType`)
     """
 
     _tokens = "ybnqiuxtdsogavh({"
-    __slots__ = ("token", "children", "_signature")
 
     def __init__(self, token: str) -> None:
         self.token = token
         self.children: List[SignatureType] = []
-        self._signature: Optional[str] = None
+        self._signature = None
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other):
         if type(other) is SignatureType:
             return self.signature == other.signature
-        return super().__eq__(other)
+        else:
+            return super().__eq__(other)
 
-    def _collapse(self) -> str:
+    def _collapse(self):
         if self.token not in "a({":
             return self.token
 
         signature = [self.token]
 
         for child in self.children:
             signature.append(child._collapse())
@@ -53,17 +64,17 @@
     def signature(self) -> str:
         if self._signature is not None:
             return self._signature
         self._signature = self._collapse()
         return self._signature
 
     @staticmethod
-    def _parse_next(signature: str) -> Tuple["SignatureType", str]:
+    def _parse_next(signature):
         if not signature:
-            raise InvalidSignatureError("Cannot parse an empty signature")
+            return (None, "")
 
         token = signature[0]
 
         if token not in SignatureType._tokens:
             raise InvalidSignatureError(f'got unexpected token: "{token}"')
 
         # container types
@@ -98,142 +109,142 @@
                 raise InvalidSignatureError('missing closing "}" for dict entry')
             self.children.append(value_child)
             return (self, signature[1:])
 
         # basic type
         return (SignatureType(token), signature[1:])
 
-    def _verify_byte(self, body: Any) -> None:
+    def _verify_byte(self, body):
         BYTE_MIN = 0x00
         BYTE_MAX = 0xFF
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus BYTE type "y" must be Python type "int", got {type(body)}'
             )
         if body < BYTE_MIN or body > BYTE_MAX:
             raise SignatureBodyMismatchError(
                 f"DBus BYTE type must be between {BYTE_MIN} and {BYTE_MAX}"
             )
 
-    def _verify_boolean(self, body: Any) -> None:
+    def _verify_boolean(self, body):
         if not isinstance(body, bool):
             raise SignatureBodyMismatchError(
                 f'DBus BOOLEAN type "b" must be Python type "bool", got {type(body)}'
             )
 
-    def _verify_int16(self, body: Any) -> None:
+    def _verify_int16(self, body):
         INT16_MIN = -0x7FFF - 1
         INT16_MAX = 0x7FFF
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus INT16 type "n" must be Python type "int", got {type(body)}'
             )
         elif body > INT16_MAX or body < INT16_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus INT16 type "n" must be between {INT16_MIN} and {INT16_MAX}'
             )
 
-    def _verify_uint16(self, body: Any) -> None:
+    def _verify_uint16(self, body):
         UINT16_MIN = 0
         UINT16_MAX = 0xFFFF
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus UINT16 type "q" must be Python type "int", got {type(body)}'
             )
         elif body > UINT16_MAX or body < UINT16_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus UINT16 type "q" must be between {UINT16_MIN} and {UINT16_MAX}'
             )
 
-    def _verify_int32(self, body: int) -> None:
+    def _verify_int32(self, body):
         INT32_MIN = -0x7FFFFFFF - 1
         INT32_MAX = 0x7FFFFFFF
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus INT32 type "i" must be Python type "int", got {type(body)}'
             )
         elif body > INT32_MAX or body < INT32_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus INT32 type "i" must be between {INT32_MIN} and {INT32_MAX}'
             )
 
-    def _verify_uint32(self, body: Any) -> None:
+    def _verify_uint32(self, body):
         UINT32_MIN = 0
         UINT32_MAX = 0xFFFFFFFF
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus UINT32 type "u" must be Python type "int", got {type(body)}'
             )
         elif body > UINT32_MAX or body < UINT32_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus UINT32 type "u" must be between {UINT32_MIN} and {UINT32_MAX}'
             )
 
-    def _verify_int64(self, body: Any) -> None:
+    def _verify_int64(self, body):
         INT64_MAX = 9223372036854775807
         INT64_MIN = -INT64_MAX - 1
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus INT64 type "x" must be Python type "int", got {type(body)}'
             )
         elif body > INT64_MAX or body < INT64_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus INT64 type "x" must be between {INT64_MIN} and {INT64_MAX}'
             )
 
-    def _verify_uint64(self, body: Any) -> None:
+    def _verify_uint64(self, body):
         UINT64_MIN = 0
         UINT64_MAX = 18446744073709551615
         if not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus UINT64 type "t" must be Python type "int", got {type(body)}'
             )
         elif body > UINT64_MAX or body < UINT64_MIN:
             raise SignatureBodyMismatchError(
                 f'DBus UINT64 type "t" must be between {UINT64_MIN} and {UINT64_MAX}'
             )
 
-    def _verify_double(self, body: Any) -> None:
-        if not isinstance(body, (float, int)):
+    def _verify_double(self, body):
+        if not isinstance(body, float) and not isinstance(body, int):
             raise SignatureBodyMismatchError(
                 f'DBus DOUBLE type "d" must be Python type "float" or "int", got {type(body)}'
             )
 
-    def _verify_unix_fd(self, body: Any) -> None:
+    def _verify_unix_fd(self, body):
         try:
             self._verify_uint32(body)
         except SignatureBodyMismatchError:
             raise SignatureBodyMismatchError(
                 'DBus UNIX_FD type "h" must be a valid UINT32'
             )
 
-    def _verify_object_path(self, body: Any) -> None:
+    def _verify_object_path(self, body):
         if not is_object_path_valid(body):
             raise SignatureBodyMismatchError(
                 'DBus OBJECT_PATH type "o" must be a valid object path'
             )
 
-    def _verify_string(self, body: Any) -> None:
+    def _verify_string(self, body):
         if not isinstance(body, str):
             raise SignatureBodyMismatchError(
                 f'DBus STRING type "s" must be Python type "str", got {type(body)}'
             )
 
-    def _verify_signature(self, body: Any) -> None:
+    def _verify_signature(self, body):
         # I guess we could run it through the SignatureTree parser instead
         if not isinstance(body, str):
             raise SignatureBodyMismatchError(
                 f'DBus SIGNATURE type "g" must be Python type "str", got {type(body)}'
             )
         if len(body.encode()) > 0xFF:
             raise SignatureBodyMismatchError(
                 'DBus SIGNATURE type "g" must be less than 256 bytes'
             )
 
-    def _verify_array(self, body: Any) -> None:
+    def _verify_array(self, body):
         child_type = self.children[0]
 
         if child_type.token == "{":
             if not isinstance(body, dict):
                 raise SignatureBodyMismatchError(
                     f'DBus ARRAY type "a" with DICT_ENTRY child must be Python type "dict", got {type(body)}'
                 )
@@ -250,30 +261,30 @@
             if not isinstance(body, list):
                 raise SignatureBodyMismatchError(
                     f'DBus ARRAY type "a" must be Python type "list", got {type(body)}'
                 )
             for member in body:
                 child_type.verify(member)
 
-    def _verify_struct(self, body: Any) -> None:
+    def _verify_struct(self, body):
         # TODO allow tuples
         if not isinstance(body, list):
             raise SignatureBodyMismatchError(
                 f'DBus STRUCT type "(" must be Python type "list", got {type(body)}'
             )
 
         if len(body) != len(self.children):
             raise SignatureBodyMismatchError(
                 'DBus STRUCT type "(" must have Python list members equal to the number of struct type members'
             )
 
         for i, member in enumerate(body):
             self.children[i].verify(member)
 
-    def _verify_variant(self, body: Any) -> None:
+    def _verify_variant(self, body):
         # a variant signature and value is valid by construction
         if not isinstance(body, Variant):
             raise SignatureBodyMismatchError(
                 f'DBus VARIANT type "v" must be Python type "Variant", got {type(body)}'
             )
 
     def verify(self, body: Any) -> bool:
@@ -289,15 +300,15 @@
         if validator:
             validator(self, body)
         else:
             raise Exception(f"cannot verify type with token {self.token}")
 
         return True
 
-    validators: Dict[str, Callable[["SignatureType", Any], None]] = {
+    validators = {
         "y": _verify_byte,
         "b": _verify_boolean,
         "n": _verify_int16,
         "q": _verify_uint16,
         "i": _verify_int32,
         "u": _verify_uint32,
         "x": _verify_int64,
@@ -325,34 +336,38 @@
     :ivar ~.signature: The signature of this signature tree.
     :vartype ~.signature: str
 
     :raises:
         :class:`InvalidSignatureError` if the given signature is not valid.
     """
 
-    __slots__ = ("signature", "types")
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _get(signature: str = "") -> "SignatureTree":
+        return SignatureTree(signature)
 
-    def __init__(self, signature: str = "") -> None:
+    def __init__(self, signature: str = ""):
         self.signature = signature
 
         self.types: List[SignatureType] = []
 
         if len(signature) > 0xFF:
             raise InvalidSignatureError("A signature must be less than 256 characters")
 
         while signature:
             (type_, signature) = SignatureType._parse_next(signature)
             self.types.append(type_)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other):
         if type(other) is SignatureTree:
             return self.signature == other.signature
-        return super().__eq__(other)
+        else:
+            return super().__eq__(other)
 
-    def verify(self, body: List[Any]) -> bool:
+    def verify(self, body: List[Any]):
         """Verifies that the give body matches this signature tree
 
         :param body: the body to verify for this tree
         :type body: list(Any)
 
         :returns: True if the signature matches the body or an exception if not.
 
@@ -377,15 +392,18 @@
     """A class to represent a DBus variant (type "v").
 
     This class is used in message bodies to represent variants. The user can
     expect a value in the body with type "v" to use this class and can
     construct this class directly for use in message bodies sent over the bus.
 
     :ivar signature: The signature for this variant. Must be a single complete type.
-    :vartype signature: str or SignatureTree or SignatureType
+    :vartype signature: str
+
+    :ivar signature_type: The parsed signature of this variant.
+    :vartype signature_type: :class:`SignatureType`
 
     :ivar value: The value of this variant. Must correspond to the signature.
     :vartype value: Any
 
     :raises:
         :class:`InvalidSignatureError` if the signature is not valid.
         :class:`SignatureBodyMismatchError` if the signature does not match the body.
@@ -394,55 +412,49 @@
     __slots__ = ("type", "signature", "value")
 
     def __init__(
         self,
         signature: Union[str, SignatureTree, SignatureType],
         value: Any,
         verify: bool = True,
-    ) -> None:
-        """Init a new Variant."""
+    ):
+        signature_str = ""
+        signature_tree = None
+        signature_type = None
+
         if type(signature) is SignatureTree:
             signature_tree = signature
-            self.signature = signature_tree.signature
-            self.type = signature_tree.types[0]
         elif type(signature) is SignatureType:
-            signature_tree = None
-            self.signature = signature.signature
-            self.type = signature
+            signature_type = signature
+            signature_str = signature.signature
         elif type(signature) is str:
-            signature_tree = get_signature_tree(signature)
-            self.signature = signature
-            self.type = signature_tree.types[0]
+            signature_tree = SignatureTree._get(signature)
         else:
             raise TypeError(
                 "signature must be a SignatureTree, SignatureType, or a string"
             )
-        self.value = value
-        if verify:
-            if signature_tree and len(signature_tree.types) != 1:
+
+        if signature_tree:
+            if verify and len(signature_tree.types) != 1:
                 raise ValueError(
                     "variants must have a signature for a single complete type"
                 )
-            self.type.verify(value)
+            signature_str = signature_tree.signature
+            signature_type = signature_tree.types[0]
 
-    def __eq__(self, other: Any) -> bool:
+        if verify:
+            signature_type.verify(value)
+
+        self.type = signature_type
+        self.signature = signature_str
+        self.value = value
+
+    def __eq__(self, other):
         if type(other) is Variant:
             return self.signature == other.signature and self.value == other.value
-        return super().__eq__(other)
+        else:
+            return super().__eq__(other)
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "<dbus_fast.signature.Variant ('{}', {})>".format(
             self.type.signature, self.value
         )
-
-
-@lru_cache(maxsize=None)
-def get_signature_tree(signature: str) -> SignatureTree:
-    """Get a signature tree for the given signature.
-
-    :param signature: The signature to get a tree for.
-    :type signature: str
-
-    :returns: The signature tree for the given signature.
-    :rtype: :class:`SignatureTree`
-    """
-    return SignatureTree(signature)
```

### Comparing `dbus_fast-1.85.0/src/dbus_fast/validators.py` & `dbus-fast-1.9.0/src/dbus_fast/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     :param name: The bus name to validate.
     :type name: str
 
     :returns: Whether the name is a valid bus name.
     :rtype: bool
     """
     if not isinstance(name, str):
-        return False  # type: ignore[unreachable]
+        return False
 
     if not name or len(name) > 255:
         return False
 
     if name.startswith(":"):
         # a unique bus name
         return True
@@ -58,15 +58,15 @@
     :param path: The object path to validate.
     :type path: str
 
     :returns: Whether the object path is valid.
     :rtype: bool
     """
     if not isinstance(path, str):
-        return False  # type: ignore[unreachable]
+        return False
 
     if not path:
         return False
 
     if not path.startswith("/"):
         return False
 
@@ -89,15 +89,15 @@
     :param name: The interface name to validate.
     :type name: str
 
     :returns: Whether the name is a valid interface name.
     :rtype: bool
     """
     if not isinstance(name, str):
-        return False  # type: ignore[unreachable]
+        return False
 
     if not name or len(name) > 255:
         return False
 
     if name.startswith("."):
         return False
 
@@ -120,71 +120,71 @@
     :param member: The member name to validate.
     :type member: str
 
     :returns: Whether the name is a valid member name.
     :rtype: bool
     """
     if not isinstance(member, str):
-        return False  # type: ignore[unreachable]
+        return False
 
     if not member or len(member) > 255:
         return False
 
     if _member_re.search(member) is None:
         return False
 
     return True
 
 
-def assert_bus_name_valid(name: str) -> None:
+def assert_bus_name_valid(name: str):
     """Raise an error if this is not a valid bus name.
 
     .. seealso:: https://dbus.freedesktop.org/doc/dbus-specification.html#message-protocol-names-bus
 
     :param name: The bus name to validate.
     :type name: str
 
     :raises:
         - :class:`InvalidBusNameError` - If this is not a valid bus name.
     """
     if not is_bus_name_valid(name):
         raise InvalidBusNameError(name)
 
 
-def assert_object_path_valid(path: str) -> None:
+def assert_object_path_valid(path: str):
     """Raise an error if this is not a valid object path.
 
     .. seealso:: https://dbus.freedesktop.org/doc/dbus-specification.html#message-protocol-marshaling-object-path
 
     :param path: The object path to validate.
     :type path: str
 
     :raises:
         - :class:`InvalidObjectPathError` - If this is not a valid object path.
     """
     if not is_object_path_valid(path):
         raise InvalidObjectPathError(path)
 
 
-def assert_interface_name_valid(name: str) -> None:
+def assert_interface_name_valid(name: str):
     """Raise an error if this is not a valid interface name.
 
     .. seealso:: https://dbus.freedesktop.org/doc/dbus-specification.html#message-protocol-names-interface
 
     :param name: The interface name to validate.
     :type name: str
 
     :raises:
         - :class:`InvalidInterfaceNameError` - If this is not a valid object path.
     """
     if not is_interface_name_valid(name):
         raise InvalidInterfaceNameError(name)
 
 
-def assert_member_name_valid(member: str) -> None:
+def assert_member_name_valid(member):
     """Raise an error if this is not a valid member name.
 
     .. seealso:: https://dbus.freedesktop.org/doc/dbus-specification.html#message-protocol-names-member
 
     :param member: The member name to validate.
     :type member: str
```

### Comparing `dbus_fast-1.85.0/setup.py` & `dbus-fast-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 packages = \
 ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio', 'dbus_fast.glib']
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
-{':python_version < "3.11"': ['async-timeout>=3.0.0']}
+{':extra == "docs"': ['sphinxcontrib-asyncio[docs]>=0.3.0,<0.4.0',
+                      'sphinxcontrib-fulltoc[docs]>=1.2.0,<2.0.0',
+                      'Sphinx[docs]>=5.1.1,<6.0.0',
+                      'myst-parser[docs]>=0.18.0,<0.19.0',
+                      'sphinx-rtd-theme[docs]>=1.0.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'dbus-fast',
-    'version': '1.85.0',
+    'version': '1.9.0',
     'description': 'A faster version of dbus-next',
-    'long_description': '# dbus-fast\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/dbus-fast/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/dbus-fast/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://dbus-fast.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/dbus-fast.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/dbus-fast">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/dbus-fast.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/dbus-fast/">\n    <img src="https://img.shields.io/pypi/v/dbus-fast.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/dbus-fast.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/dbus-fast.svg?style=flat-square" alt="License">\n</p>\n\nA faster version of dbus-next originally from the [great DBus next library](https://github.com/altdesktop/python-dbus-next) ❤️\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install dbus-fast`\n\n[Documentation](https://dbus-fast.readthedocs.io/en/latest/)\n\ndbus-fast is a Python library for DBus that aims to be a performant fully featured high level library primarily geared towards integration of applications into Linux desktop and mobile environments.\n\nDesktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.\n\nDesktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.\n\ndbus-fast plans to improve over other DBus libraries for Python in the following ways:\n\n- Zero dependencies and pure Python 3\n- An optional cython extension is available to speed up (un)marshalling\n- Focus on performance\n- Support for multiple IO backends including asyncio and the GLib main loop.\n- Nonblocking IO suitable for GUI development.\n- Target the latest language features of Python for beautiful services and clients.\n- Complete implementation of the DBus type system without ever guessing types.\n- Integration tests for all features of the library.\n- Completely documented public API.\n\n## Installing\n\nThis library is available on PyPi as [dbus-fast](https://pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-fast\n```\n\n## The Client Interface\n\nTo use a service on the bus, the library constructs a proxy object you can use to call methods, get and set properties, and listen to signals.\n\nFor more information, see the [overview for the high-level client](https://dbus-fast.readthedocs.io/en/latest/high-level-client/index.html).\n\nThis example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.\n\n```python\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\n\n\nasync def main():\n    bus = await MessageBus().connect()\n    # the introspection xml would normally be included in your project, but\n    # this is convenient for development\n    introspection = await bus.introspect(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\')\n\n    obj = bus.get_proxy_object(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\', introspection)\n    player = obj.get_interface(\'org.mpris.MediaPlayer2.Player\')\n    properties = obj.get_interface(\'org.freedesktop.DBus.Properties\')\n\n    # call methods on the interface (this causes the media player to play)\n    await player.call_play()\n\n    volume = await player.get_volume()\n    print(f\'current volume: {volume}, setting to 0.5\')\n\n    await player.set_volume(0.5)\n\n    # listen to signals\n    def on_properties_changed(interface_name, changed_properties, invalidated_properties):\n        for changed, variant in changed_properties.items():\n            print(f\'property changed: {changed} - {variant.value}\')\n\n    properties.on_properties_changed(on_properties_changed)\n\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Service Interface\n\nTo define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.\n\nFor more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).\n\n```python\nfrom dbus_fast.service import ServiceInterface, method, dbus_property, signal, Variant\nfrom dbus_fast.aio MessageBus\n\nimport asyncio\n\nclass ExampleInterface(ServiceInterface):\n    def __init__(self, name):\n        super().__init__(name)\n        self._string_prop = \'kevin\'\n\n    @method()\n    def Echo(self, what: \'s\') -> \'s\':\n        return what\n\n    @method()\n    def GetVariantDict() -> \'a{sv}\':\n        return {\n            \'foo\': Variant(\'s\', \'bar\'),\n            \'bat\': Variant(\'x\', -55),\n            \'a_list\': Variant(\'as\', [\'hello\', \'world\'])\n        }\n\n    @dbus_property()\n    def string_prop(self) -> \'s\':\n        return self._string_prop\n\n    @string_prop.setter\n    def string_prop_setter(self, val: \'s\'):\n        self._string_prop = val\n\n    @signal()\n    def signal_simple(self) -> \'s\':\n        return \'hello\'\n\nasync def main():\n    bus = await MessageBus().connect()\n    interface = ExampleInterface(\'test.interface\')\n    bus.export(\'/test/path\', interface)\n    # now that we are ready to handle requests, we can request name from D-Bus\n    await bus.request_name(\'test.name\')\n    # wait indefinitely\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Low-Level Interface\n\nThe low-level interface works with DBus messages directly.\n\nFor more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).\n\n```python\nfrom dbus_fast.message import Message, MessageType\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\nimport json\n\n\nasync def main():\n    bus = await MessageBus().connect()\n\n    reply = await bus.call(\n        Message(destination=\'org.freedesktop.DBus\',\n                path=\'/org/freedesktop/DBus\',\n                interface=\'org.freedesktop.DBus\',\n                member=\'ListNames\'))\n\n    if reply.message_type == MessageType.ERROR:\n        raise Exception(reply.body[0])\n\n    print(json.dumps(reply.body[0], indent=2))\n\n\nasyncio.run(main())\n```\n\n## Projects that use python-dbus-fast\n\n- [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)\n\n## Contributing\n\nContributions are welcome. Development happens on [Github](https://github.com/Bluetooth-Devices/dbus-fast).\n\nBefore you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.\n\n## Copyright\n\nYou can use this code under an MIT license (see LICENSE).\n\n- © 2019, Tony Crisci\n- © 2022, Bluetooth Devices authors\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
+    'long_description': '# dbus-fast\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/dbus-fast/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/dbus-fast/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://dbus-fast.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/dbus-fast.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/dbus-fast">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/dbus-fast.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/dbus-fast/">\n    <img src="https://img.shields.io/pypi/v/dbus-fast.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/dbus-fast.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/dbus-fast.svg?style=flat-square" alt="License">\n</p>\n\nA faster version of dbus-next originally from the [great DBus next library](https://github.com/altdesktop/python-dbus-next) ❤️\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install dbus-fast`\n\n[Documentation](https://dbus-fast.readthedocs.io/en/latest/)\n\ndbus-fast is a Python library for DBus that aims to be a performant fully featured high level library primarily geared towards integration of applications into Linux desktop and mobile environments.\n\nDesktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.\n\nDesktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.\n\ndbus-fast plans to improve over other DBus libraries for Python in the following ways:\n\n- Zero dependencies and pure Python 3.\n- Focus on performance\n- Support for multiple IO backends including asyncio and the GLib main loop.\n- Nonblocking IO suitable for GUI development.\n- Target the latest language features of Python for beautiful services and clients.\n- Complete implementation of the DBus type system without ever guessing types.\n- Integration tests for all features of the library.\n- Completely documented public API.\n\n## Installing\n\nThis library is available on PyPi as [dbus-fast](https://pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-fast\n```\n\n## The Client Interface\n\nTo use a service on the bus, the library constructs a proxy object you can use to call methods, get and set properties, and listen to signals.\n\nFor more information, see the [overview for the high-level client](https://dbus-fast.readthedocs.io/en/latest/high-level-client/index.html).\n\nThis example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.\n\n```python\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\n\nloop = asyncio.get_event_loop()\n\n\nasync def main():\n    bus = await MessageBus().connect()\n    # the introspection xml would normally be included in your project, but\n    # this is convenient for development\n    introspection = await bus.introspect(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\')\n\n    obj = bus.get_proxy_object(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\', introspection)\n    player = obj.get_interface(\'org.mpris.MediaPlayer2.Player\')\n    properties = obj.get_interface(\'org.freedesktop.DBus.Properties\')\n\n    # call methods on the interface (this causes the media player to play)\n    await player.call_play()\n\n    volume = await player.get_volume()\n    print(f\'current volume: {volume}, setting to 0.5\')\n\n    await player.set_volume(0.5)\n\n    # listen to signals\n    def on_properties_changed(interface_name, changed_properties, invalidated_properties):\n        for changed, variant in changed_properties.items():\n            print(f\'property changed: {changed} - {variant.value}\')\n\n    properties.on_properties_changed(on_properties_changed)\n\n    await loop.create_future()\n\nloop.run_until_complete(main())\n```\n\n## The Service Interface\n\nTo define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.\n\nFor more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).\n\n```python\nfrom dbus_fast.service import ServiceInterface, method, dbus_property, signal, Variant\nfrom dbus_fast.aio MessageBus\n\nimport asyncio\n\nclass ExampleInterface(ServiceInterface):\n    def __init__(self, name):\n        super().__init__(name)\n        self._string_prop = \'kevin\'\n\n    @method()\n    def Echo(self, what: \'s\') -> \'s\':\n        return what\n\n    @method()\n    def GetVariantDict() -> \'a{sv}\':\n        return {\n            \'foo\': Variant(\'s\', \'bar\'),\n            \'bat\': Variant(\'x\', -55),\n            \'a_list\': Variant(\'as\', [\'hello\', \'world\'])\n        }\n\n    @dbus_property()\n    def string_prop(self) -> \'s\':\n        return self._string_prop\n\n    @string_prop.setter\n    def string_prop_setter(self, val: \'s\'):\n        self._string_prop = val\n\n    @signal()\n    def signal_simple(self) -> \'s\':\n        return \'hello\'\n\nasync def main():\n    bus = await MessageBus().connect()\n    interface = ExampleInterface(\'test.interface\')\n    bus.export(\'/test/path\', interface)\n    # now that we are ready to handle requests, we can request name from D-Bus\n    await bus.request_name(\'test.name\')\n    # wait indefinitely\n    await asyncio.get_event_loop().create_future()\n\nasyncio.get_event_loop().run_until_complete(main())\n```\n\n## The Low-Level Interface\n\nThe low-level interface works with DBus messages directly.\n\nFor more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).\n\n```python\nfrom dbus_fast.message import Message, MessageType\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\nimport json\n\nloop = asyncio.get_event_loop()\n\n\nasync def main():\n    bus = await MessageBus().connect()\n\n    reply = await bus.call(\n        Message(destination=\'org.freedesktop.DBus\',\n                path=\'/org/freedesktop/DBus\',\n                interface=\'org.freedesktop.DBus\',\n                member=\'ListNames\'))\n\n    if reply.message_type == MessageType.ERROR:\n        raise Exception(reply.body[0])\n\n    print(json.dumps(reply.body[0], indent=2))\n\n\nloop.run_until_complete(main())\n```\n\n## Projects that use python-dbus-fast\n\n- [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)\n\n## Contributing\n\nContributions are welcome. Development happens on [Github](https://github.com/altdesktop/python-dbus-fast).\n\nBefore you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.\n\n## Copyright\n\nYou can use this code under an MIT license (see LICENSE).\n\n- © 2019, Tony Crisci\n- © 2022, Bluetooth Devices authors\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'Bluetooth Devices Authors',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/dbus-fast',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
-from build_ext import *
-build(setup_kwargs)
+
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio',
-'dbus_fast.glib'] package_data = \ {'': ['*']} extras_require = \ {':
-python_version < "3.11"': ['async-timeout>=3.0.0']} setup_kwargs = { 'name':
-'dbus-fast', 'version': '1.85.0', 'description': 'A faster version of dbus-
-next', 'long_description': '# dbus-fast\n\n
+'dbus_fast.glib'] package_data = \ {'': ['*']} extras_require = \ {':extra ==
+"docs"': ['sphinxcontrib-asyncio[docs]>=0.3.0,<0.4.0', 'sphinxcontrib-fulltoc
+[docs]>=1.2.0,<2.0.0', 'Sphinx[docs]>=5.1.1,<6.0.0', 'myst-parser
+[docs]>=0.18.0,<0.19.0', 'sphinx-rtd-theme[docs]>=1.0.0,<2.0.0']} setup_kwargs
+= { 'name': 'dbus-fast', 'version': '1.9.0', 'description': 'A faster version
+of dbus-next', 'long_description': '# dbus-fast\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
 \n\nA faster version of dbus-next originally from the [great DBus next library]
@@ -19,88 +21,90 @@
 towards integration of applications into Linux desktop and mobile
 environments.\n\nDesktop application developers can use this library for
 integrating their applications into desktop environments by implementing common
 DBus standard interfaces or creating custom plugin interfaces.\n\nDesktop users
 can use this library to create their own scripts and utilities to interact with
 those interfaces for customization of their desktop environment.\n\ndbus-fast
 plans to improve over other DBus libraries for Python in the following ways:
-\n\n- Zero dependencies and pure Python 3\n- An optional cython extension is
-available to speed up (un)marshalling\n- Focus on performance\n- Support for
-multiple IO backends including asyncio and the GLib main loop.\n- Nonblocking
-IO suitable for GUI development.\n- Target the latest language features of
-Python for beautiful services and clients.\n- Complete implementation of the
-DBus type system without ever guessing types.\n- Integration tests for all
-features of the library.\n- Completely documented public API.\n\n##
-Installing\n\nThis library is available on PyPi as [dbus-fast](https://
-pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-fast\n```\n\n## The
-Client Interface\n\nTo use a service on the bus, the library constructs a proxy
-object you can use to call methods, get and set properties, and listen to
-signals.\n\nFor more information, see the [overview for the high-level client]
-(https://dbus-fast.readthedocs.io/en/latest/high-level-client/
-index.html).\n\nThis example connects to a media player and controls it with
-the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus
-interface.\n\n```python\nfrom dbus_fast.aio import MessageBus\n\nimport
-asyncio\n\n\nasync def main():\n bus = await MessageBus().connect()\n # the
-introspection xml would normally be included in your project, but\n # this is
-convenient for development\n introspection = await bus.introspect
+\n\n- Zero dependencies and pure Python 3.\n- Focus on performance\n- Support
+for multiple IO backends including asyncio and the GLib main loop.\n-
+Nonblocking IO suitable for GUI development.\n- Target the latest language
+features of Python for beautiful services and clients.\n- Complete
+implementation of the DBus type system without ever guessing types.\n-
+Integration tests for all features of the library.\n- Completely documented
+public API.\n\n## Installing\n\nThis library is available on PyPi as [dbus-
+fast](https://pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-
+fast\n```\n\n## The Client Interface\n\nTo use a service on the bus, the
+library constructs a proxy object you can use to call methods, get and set
+properties, and listen to signals.\n\nFor more information, see the [overview
+for the high-level client](https://dbus-fast.readthedocs.io/en/latest/high-
+level-client/index.html).\n\nThis example connects to a media player and
+controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/
+latest/) DBus interface.\n\n```python\nfrom dbus_fast.aio import
+MessageBus\n\nimport asyncio\n\nloop = asyncio.get_event_loop()\n\n\nasync def
+main():\n bus = await MessageBus().connect()\n # the introspection xml would
+normally be included in your project, but\n # this is convenient for
+development\n introspection = await bus.introspect
 (\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\')\n\n obj =
 bus.get_proxy_object(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/
 MediaPlayer2\', introspection)\n player = obj.get_interface
 (\'org.mpris.MediaPlayer2.Player\')\n properties = obj.get_interface
 (\'org.freedesktop.DBus.Properties\')\n\n # call methods on the interface (this
 causes the media player to play)\n await player.call_play()\n\n volume = await
 player.get_volume()\n print(f\'current volume: {volume}, setting to 0.5\')\n\n
 await player.set_volume(0.5)\n\n # listen to signals\n def
 on_properties_changed(interface_name, changed_properties,
 invalidated_properties):\n for changed, variant in changed_properties.items():
 \n print(f\'property changed: {changed} - {variant.value}\')\n\n
-properties.on_properties_changed(on_properties_changed)\n\n await asyncio.Event
-().wait()\n\nasyncio.run(main())\n```\n\n## The Service Interface\n\nTo define
-a service on the bus, use the `ServiceInterface` class and decorate class
-methods to specify DBus methods, properties, and signals with their type
-signatures.\n\nFor more information, see the [overview for the high-level
-service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/
-index.html).\n\n```python\nfrom dbus_fast.service import ServiceInterface,
-method, dbus_property, signal, Variant\nfrom dbus_fast.aio MessageBus\n\nimport
-asyncio\n\nclass ExampleInterface(ServiceInterface):\n def __init__(self,
-name):\n super().__init__(name)\n self._string_prop = \'kevin\'\n\n @method()\n
-def Echo(self, what: \'s\') -> \'s\':\n return what\n\n @method()\n def
-GetVariantDict() -> \'a{sv}\':\n return {\n \'foo\': Variant(\'s\', \'bar\'),\n
-\'bat\': Variant(\'x\', -55),\n \'a_list\': Variant(\'as\', [\'hello\',
-\'world\'])\n }\n\n @dbus_property()\n def string_prop(self) -> \'s\':\n return
-self._string_prop\n\n @string_prop.setter\n def string_prop_setter(self, val:
-\'s\'):\n self._string_prop = val\n\n @signal()\n def signal_simple(self) -
-> \'s\':\n return \'hello\'\n\nasync def main():\n bus = await MessageBus
-().connect()\n interface = ExampleInterface(\'test.interface\')\n bus.export
-(\'/test/path\', interface)\n # now that we are ready to handle requests, we
-can request name from D-Bus\n await bus.request_name(\'test.name\')\n # wait
-indefinitely\n await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n##
-The Low-Level Interface\n\nThe low-level interface works with DBus messages
-directly.\n\nFor more information, see the [overview for the low-level
-interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-
-interface/index.html).\n\n```python\nfrom dbus_fast.message import Message,
+properties.on_properties_changed(on_properties_changed)\n\n await
+loop.create_future()\n\nloop.run_until_complete(main())\n```\n\n## The Service
+Interface\n\nTo define a service on the bus, use the `ServiceInterface` class
+and decorate class methods to specify DBus methods, properties, and signals
+with their type signatures.\n\nFor more information, see the [overview for the
+high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-
+level-service/index.html).\n\n```python\nfrom dbus_fast.service import
+ServiceInterface, method, dbus_property, signal, Variant\nfrom dbus_fast.aio
+MessageBus\n\nimport asyncio\n\nclass ExampleInterface(ServiceInterface):\n def
+__init__(self, name):\n super().__init__(name)\n self._string_prop =
+\'kevin\'\n\n @method()\n def Echo(self, what: \'s\') -> \'s\':\n return
+what\n\n @method()\n def GetVariantDict() -> \'a{sv}\':\n return {\n \'foo\':
+Variant(\'s\', \'bar\'),\n \'bat\': Variant(\'x\', -55),\n \'a_list\': Variant
+(\'as\', [\'hello\', \'world\'])\n }\n\n @dbus_property()\n def string_prop
+(self) -> \'s\':\n return self._string_prop\n\n @string_prop.setter\n def
+string_prop_setter(self, val: \'s\'):\n self._string_prop = val\n\n @signal()\n
+def signal_simple(self) -> \'s\':\n return \'hello\'\n\nasync def main():\n bus
+= await MessageBus().connect()\n interface = ExampleInterface
+(\'test.interface\')\n bus.export(\'/test/path\', interface)\n # now that we
+are ready to handle requests, we can request name from D-Bus\n await
+bus.request_name(\'test.name\')\n # wait indefinitely\n await
+asyncio.get_event_loop().create_future()\n\nasyncio.get_event_loop
+().run_until_complete(main())\n```\n\n## The Low-Level Interface\n\nThe low-
+level interface works with DBus messages directly.\n\nFor more information, see
+the [overview for the low-level interface](https://python-dbus-
+fast.readthedocs.io/en/latest/low-level-interface/
+index.html).\n\n```python\nfrom dbus_fast.message import Message,
 MessageType\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\nimport
-json\n\n\nasync def main():\n bus = await MessageBus().connect()\n\n reply =
-await bus.call(\n Message(destination=\'org.freedesktop.DBus\',\n path=\'/org/
-freedesktop/DBus\',\n interface=\'org.freedesktop.DBus\',\n
-member=\'ListNames\'))\n\n if reply.message_type == MessageType.ERROR:\n raise
-Exception(reply.body[0])\n\n print(json.dumps(reply.body[0],
-indent=2))\n\n\nasyncio.run(main())\n```\n\n## Projects that use python-dbus-
-fast\n\n- [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-
-adapters)\n\n## Contributing\n\nContributions are welcome. Development happens
-on [Github](https://github.com/Bluetooth-Devices/dbus-fast).\n\nBefore you
-commit, run `pre-commit run --all-files` to run the linter, code formatter, and
-the test suite.\n\n## Copyright\n\nYou can use this code under an MIT license
-(see LICENSE).\n\n- Â© 2019, Tony Crisci\n- Â© 2022, Bluetooth Devices
-authors\n\n## Contributors â¨\n\nThanks goes to these wonderful people ([emoji
-key](https://allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n\n\n\n\nThis
-project follows the [all-contributors](https://github.com/all-contributors/all-
-contributors) specification. Contributions of any kind welcome!\n\n##
-Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/
-audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://
-github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
-'author': 'Bluetooth Devices Authors', 'author_email': 'bluetooth@koston.org',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://github.com/
-bluetooth-devices/dbus-fast', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'extras_require': extras_require,
-'python_requires': '>=3.7,<4.0', } from build_ext import * build(setup_kwargs)
-setup(**setup_kwargs)
+json\n\nloop = asyncio.get_event_loop()\n\n\nasync def main():\n bus = await
+MessageBus().connect()\n\n reply = await bus.call(\n Message
+(destination=\'org.freedesktop.DBus\',\n path=\'/org/freedesktop/DBus\',\n
+interface=\'org.freedesktop.DBus\',\n member=\'ListNames\'))\n\n if
+reply.message_type == MessageType.ERROR:\n raise Exception(reply.body[0])\n\n
+print(json.dumps(reply.body[0], indent=2))\n\n\nloop.run_until_complete(main
+())\n```\n\n## Projects that use python-dbus-fast\n\n- [Bluetooth Adapters]
+(https://github.com/bluetooth-devices/bluetooth-adapters)\n\n##
+Contributing\n\nContributions are welcome. Development happens on [Github]
+(https://github.com/altdesktop/python-dbus-fast).\n\nBefore you commit, run
+`pre-commit run --all-files` to run the linter, code formatter, and the test
+suite.\n\n## Copyright\n\nYou can use this code under an MIT license (see
+LICENSE).\n\n- Â© 2019, Tony Crisci\n- Â© 2022, Bluetooth Devices authors\n\n##
+Contributors â¨\n\nThanks goes to these wonderful people ([emoji key](https://
+allcontributors.org/docs/en/emoji-key)):\n\n\n\n\n\n\n\n\nThis project follows
+the [all-contributors](https://github.com/all-contributors/all-contributors)
+specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
+was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and
+the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/
+cookiecutter-pypackage)\nproject template.\n', 'author': 'Bluetooth Devices
+Authors', 'author_email': 'bluetooth@koston.org', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/bluetooth-devices/dbus-
+fast', 'package_dir': package_dir, 'packages': packages, 'package_data':
+package_data, 'extras_require': extras_require, 'python_requires':
+'>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `dbus_fast-1.85.0/PKG-INFO` & `dbus-fast-1.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbus-fast
-Version: 1.85.0
+Version: 1.9.0
 Summary: A faster version of dbus-next
 Home-page: https://github.com/bluetooth-devices/dbus-fast
 License: MIT
 Author: Bluetooth Devices Authors
 Author-email: bluetooth@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,17 +13,21 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: async-timeout (>=3.0.0) ; python_version < "3.11"
+Provides-Extra: docs
+Requires-Dist: Sphinx[docs] (>=5.1.1,<6.0.0); extra == "docs"
+Requires-Dist: myst-parser[docs] (>=0.18.0,<0.19.0); extra == "docs"
+Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0); extra == "docs"
+Requires-Dist: sphinxcontrib-asyncio[docs] (>=0.3.0,<0.4.0); extra == "docs"
+Requires-Dist: sphinxcontrib-fulltoc[docs] (>=1.2.0,<2.0.0); extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/dbus-fast/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/dbus-fast/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://dbus-fast.readthedocs.io
 Project-URL: Repository, https://github.com/bluetooth-devices/dbus-fast
 Description-Content-Type: text/markdown
 
 # dbus-fast
@@ -72,16 +76,15 @@
 
 Desktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.
 
 Desktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.
 
 dbus-fast plans to improve over other DBus libraries for Python in the following ways:
 
-- Zero dependencies and pure Python 3
-- An optional cython extension is available to speed up (un)marshalling
+- Zero dependencies and pure Python 3.
 - Focus on performance
 - Support for multiple IO backends including asyncio and the GLib main loop.
 - Nonblocking IO suitable for GUI development.
 - Target the latest language features of Python for beautiful services and clients.
 - Complete implementation of the DBus type system without ever guessing types.
 - Integration tests for all features of the library.
 - Completely documented public API.
@@ -103,14 +106,16 @@
 This example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.
 
 ```python
 from dbus_fast.aio import MessageBus
 
 import asyncio
 
+loop = asyncio.get_event_loop()
+
 
 async def main():
     bus = await MessageBus().connect()
     # the introspection xml would normally be included in your project, but
     # this is convenient for development
     introspection = await bus.introspect('org.mpris.MediaPlayer2.vlc', '/org/mpris/MediaPlayer2')
 
@@ -129,17 +134,17 @@
     # listen to signals
     def on_properties_changed(interface_name, changed_properties, invalidated_properties):
         for changed, variant in changed_properties.items():
             print(f'property changed: {changed} - {variant.value}')
 
     properties.on_properties_changed(on_properties_changed)
 
-    await asyncio.Event().wait()
+    await loop.create_future()
 
-asyncio.run(main())
+loop.run_until_complete(main())
 ```
 
 ## The Service Interface
 
 To define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.
 
 For more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).
@@ -182,17 +187,17 @@
 async def main():
     bus = await MessageBus().connect()
     interface = ExampleInterface('test.interface')
     bus.export('/test/path', interface)
     # now that we are ready to handle requests, we can request name from D-Bus
     await bus.request_name('test.name')
     # wait indefinitely
-    await asyncio.Event().wait()
+    await asyncio.get_event_loop().create_future()
 
-asyncio.run(main())
+asyncio.get_event_loop().run_until_complete(main())
 ```
 
 ## The Low-Level Interface
 
 The low-level interface works with DBus messages directly.
 
 For more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).
@@ -200,14 +205,16 @@
 ```python
 from dbus_fast.message import Message, MessageType
 from dbus_fast.aio import MessageBus
 
 import asyncio
 import json
 
+loop = asyncio.get_event_loop()
+
 
 async def main():
     bus = await MessageBus().connect()
 
     reply = await bus.call(
         Message(destination='org.freedesktop.DBus',
                 path='/org/freedesktop/DBus',
@@ -216,24 +223,24 @@
 
     if reply.message_type == MessageType.ERROR:
         raise Exception(reply.body[0])
 
     print(json.dumps(reply.body[0], indent=2))
 
 
-asyncio.run(main())
+loop.run_until_complete(main())
 ```
 
 ## Projects that use python-dbus-fast
 
 - [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)
 
 ## Contributing
 
-Contributions are welcome. Development happens on [Github](https://github.com/Bluetooth-Devices/dbus-fast).
+Contributions are welcome. Development happens on [Github](https://github.com/altdesktop/python-dbus-fast).
 
 Before you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.
 
 ## Copyright
 
 You can use this code under an MIT license (see LICENSE).
```

