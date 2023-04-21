# Comparing `tmp/Emmett-Sentry-0.2.0.tar.gz` & `tmp/emmett_sentry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Emmett-Sentry-0.2.0.tar", max compression
+gzip compressed data, was "emmett_sentry-0.3.0.tar", max compression
```

## Comparing `Emmett-Sentry-0.2.0.tar` & `emmett_sentry-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1486 2022-03-10 13:40:03.973695 Emmett-Sentry-0.2.0/LICENSE
--rw-r--r--   0        0        0     1324 2022-03-10 13:40:03.973695 Emmett-Sentry-0.2.0/README.md
--rw-r--r--   0        0        0       24 2022-03-10 13:40:03.973695 Emmett-Sentry-0.2.0/emmett_sentry/__init__.py
--rw-r--r--   0        0        0       22 2022-03-10 13:40:03.977695 Emmett-Sentry-0.2.0/emmett_sentry/__version__.py
--rw-r--r--   0        0        0     2284 2022-03-10 13:40:03.977695 Emmett-Sentry-0.2.0/emmett_sentry/ext.py
--rw-r--r--   0        0        0     6833 2022-03-10 13:40:03.977695 Emmett-Sentry-0.2.0/emmett_sentry/helpers.py
--rw-r--r--   0        0        0     1321 2022-03-10 13:40:03.977695 Emmett-Sentry-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2089 2022-03-10 13:40:09.095159 Emmett-Sentry-0.2.0/setup.py
--rw-r--r--   0        0        0     2550 2022-03-10 13:40:09.095543 Emmett-Sentry-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1486 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1393 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/README.md
+-rw-r--r--   0        0        0       24 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/__version__.py
+-rw-r--r--   0        0        0     2354 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/ext.py
+-rw-r--r--   0        0        0     7672 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/emmett_sentry/helpers.py
+-rw-r--r--   0        0        0     1298 2023-04-21 10:06:32.939689 emmett_sentry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 emmett_sentry-0.3.0/setup.py
+-rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 emmett_sentry-0.3.0/PKG-INFO
```

### Comparing `Emmett-Sentry-0.2.0/LICENSE` & `emmett_sentry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Emmett-Sentry-0.2.0/README.md` & `emmett_sentry-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 | dsn | | Sentry project's DSN |
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
 | enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
 | traces\_sample\_rate | | Traces sampling rate |
+| trace\_websockets | `False` | Enable tracing on websocket routes |
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

### Comparing `Emmett-Sentry-0.2.0/emmett_sentry/ext.py` & `emmett_sentry-0.3.0/emmett_sentry/ext.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     default_config = dict(
         dsn="",
         environment="development",
         release=None,
         auto_load=True,
         enable_tracing=False,
         sample_rate=1.0,
-        traces_sample_rate=None
+        traces_sample_rate=None,
+        trace_websockets=False
     )
     _initialized = False
     _errmsg = "You need to configure Sentry extension before using its methods"
 
     def on_load(self):
         self._scopes = {}
         self._before_send_callbacks = []
@@ -45,15 +46,16 @@
             dsn=self.config.dsn,
             environment=self.config.environment,
             release=self.config.release,
             sample_rate=self.config.sample_rate,
             traces_sample_rate=self.config.traces_sample_rate,
             before_send=self._before_send
         )
-        patch_routers(self)
+        if self.config.auto_load:
+            patch_routers(self)
         self._initialized = True
 
     def _before_send(self, event, hint):
         for callback in self._before_send_callbacks:
             event = callback(event, hint)
             if not event:
                 break
```

### Comparing `Emmett-Sentry-0.2.0/emmett_sentry/helpers.py` & `emmett_sentry-0.3.0/emmett_sentry/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 """
 
 import urllib
 
 from functools import wraps
 
 from emmett import current
+from emmett.asgi.wrappers import Request as ASGIRequest, Websocket as ASGIWebsocket
 from emmett.http import HTTPResponse
+from emmett.rsgi.wrappers import Request as RSGIRequest, Websocket as RSGIWebsocket
 from sentry_sdk.hub import Hub, _should_send_default_pii
 from sentry_sdk.integrations._wsgi_common import _filter_headers
 from sentry_sdk.tracing import Transaction
 from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
 
 
 def _capture_exception(hub, exception):
@@ -34,28 +36,39 @@
 def _capture_message(hub, message, level = None):
     hub.capture_message(
         message,
         level=level
     )
 
 
+def _process_common_asgi(data, wrapper):
+    data["query_string"] = urllib.parse.unquote(
+        wrapper._scope["query_string"].decode("latin-1")
+    )
+
+def _process_common_rsgi(data, wrapper):
+    data["query_string"] = urllib.parse.unquote(wrapper._scope.query_string)
+
+
 def _process_common(data, wrapper):
     data["url"] = "%s://%s%s" % (
         wrapper.scheme,
         wrapper.host,
         wrapper.path
     )
-    data["query_string"] = urllib.parse.unquote(
-        wrapper._scope["query_string"].decode("latin-1")
-    )
     data["env"] = {}
     data["headers"] = _filter_headers(dict(wrapper.headers.items()))
 
-    if wrapper._scope.get("client") and _should_send_default_pii():
-        data["env"]["REMOTE_ADDR"] = wrapper._scope["client"][0]
+    if _should_send_default_pii():
+        data["env"]["REMOTE_ADDR"] = wrapper.client
+
+    if isinstance(wrapper, (ASGIRequest, ASGIWebsocket)):
+        _process_common_asgi(data, wrapper)
+    elif isinstance(wrapper, (RSGIRequest, RSGIWebsocket)):
+        _process_common_rsgi(data, wrapper)
 
 
 def _process_http(event, hint):
     if not hasattr(current, "request"):
         return event
 
     wrapper = current.request
@@ -113,19 +126,23 @@
     async def wrap(*args, **kwargs):
         with Hub(Hub.current) as hub:
             with hub.push_scope() as scope:
                 scope.add_event_processor(_process_http)
                 for key, builder in ext._scopes.items():
                     scope.set_extra(key, await builder())
 
+                proto = (
+                    "rsgi" if hasattr(current.request._scope, "rsgi_version") else
+                    "asgi"
+                )
                 txn = Transaction.continue_from_headers(
-                    current.request._scope["headers"],
+                    current.request.headers,
                     op="http.server"
                 )
-                txn.set_tag("asgi.type", "http")
+                txn.set_tag(f"{proto}.type", "http")
 
                 with hub.start_transaction(txn):
                     try:
                         return await dispatch_method(*args, **kwargs)
                     except HTTPResponse:
                         raise
                     except Exception as exc:
@@ -159,19 +176,23 @@
     async def wrap(*args, **kwargs):
         with Hub(Hub.current) as hub:
             with hub.push_scope() as scope:
                 scope.add_event_processor(_process_ws)
                 for key, builder in ext._scopes.items():
                     scope.set_extra(key, await builder())
 
+                proto = (
+                    "rsgi" if hasattr(current.websocket._scope, "rsgi_version") else
+                    "asgi"
+                )
                 txn = Transaction.continue_from_headers(
-                    current.request._scope["headers"],
+                    current.websocket.headers,
                     op="websocket.server"
                 )
-                txn.set_tag("asgi.type", "websocket")
+                txn.set_tag(f"{proto}.type", "websocket")
 
                 with hub.start_transaction(txn):
                     try:
                         return await dispatch_method(*args, **kwargs)
                     except Exception as exc:
                         _capture_exception(hub, exc)
                         raise
@@ -192,16 +213,17 @@
         )
 
     return _routing_rec_http
 
 
 def _build_routing_rec_ws(ext, rec_cls):
     wrapper = (
-        _build_ws_dispatcher_wrapper_txn if ext.config.enable_tracing else
-        _build_ws_dispatcher_wrapper_err
+        _build_ws_dispatcher_wrapper_txn if (
+            ext.config.enable_tracing and ext.config.trace_websockets
+        ) else _build_ws_dispatcher_wrapper_err
     )
 
     def _routing_rec_ws(router, name, match, dispatch, flow_recv, flow_send):
         return rec_cls(
             name=name,
             match=match,
             dispatch=wrapper(ext, dispatch),
```

### Comparing `Emmett-Sentry-0.2.0/pyproject.toml` & `emmett_sentry-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
-name = "Emmett-Sentry"
-version = "0.2.0"
+name = "emmett-sentry"
+version = "0.3.0"
 description = "Sentry extension for Emmett framework"
-authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
+authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/sentry"
 repository = "https://github.com/emmett-framework/sentry"
 
 keywords = ["sentry", "logging", "emmett"]
@@ -14,33 +14,32 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 include = [
     "LICENSE"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-emmett = "^2.1.0"
-sentry-sdk = "^1.5.0"
+python = "^3.8"
+emmett = "^2.5.0"
+sentry-sdk = "^1.20.0"
 
 [tool.poetry.dev-dependencies]
-pylint = "^2.4.4"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/emmett-framework/sentry/issues"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `Emmett-Sentry-0.2.0/setup.py` & `emmett_sentry-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['emmett_sentry']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['emmett>=2.1.0,<3.0.0', 'sentry-sdk>=1.5.0,<2.0.0']
+['emmett>=2.5.0,<3.0.0', 'sentry-sdk>=1.20.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'emmett-sentry',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Sentry extension for Emmett framework',
-    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| traces\\_sample\\_rate | | Traces sampling rate |\n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
+    'long_description': '# Emmett-Sentry\n\nEmmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.\n\n[![pip version](https://img.shields.io/pypi/v/emmett-sentry.svg?style=flat)](https://pypi.python.org/pypi/emmett-sentry) \n\n## Installation\n\nYou can install Emmett-Sentry using pip:\n\n    pip install emmett-sentry\n\nAnd add it to your Emmett application:\n\n```python\nfrom emmett_sentry import Sentry\n\nsentry = app.use_extension(Sentry)\n```\n\n## Configuration\n\nHere is the complete list of parameters of the extension configuration:\n\n| param | default | description |\n| --- | --- | --- |\n| dsn | | Sentry project\'s DSN |\n| environment | development | Application environment |\n| release | | Application release |\n| auto\\_load | `True` | Automatically inject extension on routes |\n| enable\\_tracing | `False` | Enable tracing on routes |\n| sample\\_rate | 1 | Error sampling rate |\n| traces\\_sample\\_rate | | Traces sampling rate |\n| trace\\_websockets | `False` | Enable tracing on websocket routes |\n\n## Usage\n\nThe extension exposes two methods to manually track events:\n\n- exception\n- message\n\nYou call these methods directly within your code:\n\n```python\n# track an error\ntry:\n    1 / 0\nexcept Exception:\n    sentry.exception()\n\n# track a message\nsentry.message("some event", level="info")\n```\n\n## License\n\nEmmett-Sentry is released under BSD license.\n',
     'author': 'Giovanni Barillari',
-    'author_email': 'gi0baro@d4net.org',
-    'maintainer': None,
-    'maintainer_email': None,
+    'author_email': 'g@baro.dev',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/emmett-framework/sentry',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `Emmett-Sentry-0.2.0/PKG-INFO` & `emmett_sentry-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: emmett-sentry
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sentry extension for Emmett framework
 Home-page: https://github.com/emmett-framework/sentry
 License: BSD-3-Clause
 Keywords: sentry,logging,emmett
 Author: Giovanni Barillari
-Author-email: gi0baro@d4net.org
-Requires-Python: >=3.7,<4.0
+Author-email: g@baro.dev
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: emmett (>=2.1.0,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.5.0,<2.0.0)
+Requires-Dist: emmett (>=2.5.0,<3.0.0)
+Requires-Dist: sentry-sdk (>=1.20.0,<2.0.0)
 Project-URL: Issue Tracker, https://github.com/emmett-framework/sentry/issues
 Project-URL: Repository, https://github.com/emmett-framework/sentry
 Description-Content-Type: text/markdown
 
 # Emmett-Sentry
 
 Emmett-Sentry is an [Emmett framework](https://emmett.sh) extension integrating [Sentry](https://sentry.io) monitoring platform.
@@ -56,14 +61,15 @@
 | dsn | | Sentry project's DSN |
 | environment | development | Application environment |
 | release | | Application release |
 | auto\_load | `True` | Automatically inject extension on routes |
 | enable\_tracing | `False` | Enable tracing on routes |
 | sample\_rate | 1 | Error sampling rate |
 | traces\_sample\_rate | | Traces sampling rate |
+| trace\_websockets | `False` | Enable tracing on websocket routes |
 
 ## Usage
 
 The extension exposes two methods to manually track events:
 
 - exception
 - message
```

