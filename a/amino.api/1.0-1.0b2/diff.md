# Comparing `tmp/amino.api-1.0.tar.gz` & `tmp/amino.api-1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.0.tar", last modified: Wed Apr 19 17:23:01 2023, max compression
+gzip compressed data, was "amino.api-1.0b2.tar", last modified: Thu Apr 20 21:06:36 2023, max compression
```

## Comparing `amino.api-1.0.tar` & `amino.api-1.0b2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:23:01.937274 amino.api-1.0/
--rw-rw-rw-   0        0        0      556 2023-04-19 17:23:01.938268 amino.api-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       40 2023-04-18 11:48:20.000000 amino.api-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 17:23:01.889751 amino.api-1.0/amino/
--rw-rw-rw-   0        0        0      855 2023-04-19 17:14:09.000000 amino.api-1.0/amino/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-19 15:48:32.000000 amino.api-1.0/amino/client.py
--rw-rw-rw-   0        0        0     5596 2023-04-19 16:13:18.000000 amino.api-1.0/amino/full_client.py
--rw-rw-rw-   0        0        0     1090 2023-04-19 11:06:56.000000 amino.api-1.0/amino/local_client.py
--rw-rw-rw-   0        0        0    11244 2023-04-19 16:24:07.000000 amino.api-1.0/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:23:01.936270 amino.api-1.0/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 12:11:03.000000 amino.api-1.0/amino/utils/__init__.py
--rw-rw-rw-   0        0        0      770 2023-04-19 10:34:16.000000 amino.api-1.0/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     5141 2023-04-19 15:37:56.000000 amino.api-1.0/amino/utils/helpers.py
--rw-rw-rw-   0        0        0     3747 2023-04-19 10:53:03.000000 amino.api-1.0/amino/utils/objects.py
--rw-rw-rw-   0        0        0     1909 2023-04-19 15:23:01.000000 amino.api-1.0/amino/utils/requester.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:23:01.913756 amino.api-1.0/amino.api.egg-info/
--rw-rw-rw-   0        0        0      556 2023-04-19 17:23:00.000000 amino.api-1.0/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-19 17:23:00.000000 amino.api-1.0/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:23:00.000000 amino.api-1.0/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 17:23:00.000000 amino.api-1.0/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 17:23:00.000000 amino.api-1.0/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:23:01.939273 amino.api-1.0/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-04-18 11:57:56.000000 amino.api-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.853437 amino.api-1.0b2/
+-rw-rw-rw-   0        0        0      558 2023-04-20 21:06:36.853437 amino.api-1.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2023-04-18 11:48:20.000000 amino.api-1.0b2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.800821 amino.api-1.0b2/amino/
+-rw-rw-rw-   0        0        0      860 2023-04-20 10:21:20.000000 amino.api-1.0b2/amino/__init__.py
+-rw-rw-rw-   0        0        0     9436 2023-04-20 20:43:38.000000 amino.api-1.0b2/amino/client.py
+-rw-rw-rw-   0        0        0    10084 2023-04-20 20:56:23.000000 amino.api-1.0b2/amino/full_client.py
+-rw-rw-rw-   0        0        0     3582 2023-04-20 11:50:55.000000 amino.api-1.0b2/amino/local_client.py
+-rw-rw-rw-   0        0        0    11406 2023-04-20 11:36:48.000000 amino.api-1.0b2/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.852437 amino.api-1.0b2/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-18 12:11:03.000000 amino.api-1.0b2/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-04-20 08:49:05.000000 amino.api-1.0b2/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7350 2023-04-20 16:39:36.000000 amino.api-1.0b2/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0     8804 2023-04-20 20:54:36.000000 amino.api-1.0b2/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2117 2023-04-20 16:31:41.000000 amino.api-1.0b2/amino/utils/requester.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:06:36.825825 amino.api-1.0b2/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 21:06:35.000000 amino.api-1.0b2/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:06:36.855430 amino.api-1.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2023-04-20 21:06:25.000000 amino.api-1.0b2/setup.py
```

### Comparing `amino.api-1.0/PKG-INFO` & `amino.api-1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.0
+Version: 1.0b2
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino New Start</h1>
```

### Comparing `amino.api-1.0/amino/__init__.py` & `amino.api-1.0b2/amino/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.py-api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.0'
-__newest__ = '1.0'#loads(get("https://pypi.org/pypi//json").text)["info"]["version"]
+__version__ = '1.0b2'
+__newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `amino.api-1.0/amino/socket.py` & `amino.api-1.0b2/amino/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from time import sleep, time
 from json import loads, dumps
 from websocket import WebSocketApp, enableTrace
 from threading import Thread
 from sys import _getframe as getframe
 from random import randint
+from traceback import format_exc
 
 from .utils import objects
 from .utils.exceptions import SocketNotStarted
 
 class SocketHandler:
 	def __init__(self, req, sock_trace: bool = False, debug: bool = False):
 		self.socket_url = "wss://ws1.narvii.com"
 		self.debug = debug
-		print(self.debug)
 		self.socket = None
 		self.reconnectTime = 60
 		self.active = False
 		self.socket_thread = None
 		self.req = req
 		if self.socket_enabled:
 			self.reconnect_thread = Thread(target=self.reconnect)
@@ -73,15 +73,19 @@
 					print(f"[socket][reconnect_handler] Reconnecting Socket")
 
 				self.close()
 				self.connect()
 
 
 	def handle_message(self, ws, data):
-		return self.resolve(data)
+		data = loads(data)
+		try:
+			self.resolve(data)
+		except:
+			print(format_exc())
 
 	def send(self, data):
 		if self.debug:
 			print(f"[socket][send] Sending Data : {data}")
 		if not self.socket_thread:
 			if self.debug:
 				print(f"[socket][send][error] Socket not started !")
@@ -167,16 +171,16 @@
 		return self.chat_actions_start.get(key, self.default)(data)
 
 	def _resolve_chat_action_end(self, data):
 		key = data['o'].get('actions', 0)
 		return self.chat_actions_end.get(key, self.default)(data)
 
 	def resolve(self, data):
-		data = loads(data)
-		return self.methods.get(data["t"], self.default)(data)
+		self.on_reslove(data)
+		self.methods.get(data["t"], self.default)(data)
 
 	def call(self, type, data):
 		if type in self.handlers:
 			for handler in self.handlers[type]:
 				handler(data)
 
 	def event(self, type):
@@ -236,9 +240,10 @@
 	def on_chat_tipping_disabled(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 	def on_timestamp_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 	def on_welcome_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 	def on_invite_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 
 	def on_user_typing_start(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 	def on_user_typing_end(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
+	def on_reslove(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]))
 
 	def default(self, data): self.call(getframe(0).f_code.co_name, data)
```

### Comparing `amino.api-1.0/amino/utils/exceptions.py` & `amino.api-1.0b2/amino/utils/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 		Exception.__init__(*args, **kwargs)
 
 class SocketNotStarted(Exception):
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
 
+class IncorrectType(Exception):
+	def __init__(*args, **kwargs):
+		Exception.__init__(*args, **kwargs)
+
+
+
 errors = {
 }
 
 def check_exceptions(data):
 	try:
 		data = loads(data)
 		try:code = data["api:statuscode"]
```

### Comparing `amino.api-1.0/amino/utils/requester.py` & `amino.api-1.0b2/amino/utils/requester.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 from requests import Session
 
 from .helpers import Generator
 from .exceptions import InvalidFunctionСall, InvalidSessionType
 from .exceptions import check_exceptions
 
 class Requester:
-	def __init__(self, session: Union[ClientSession, Session], deviceId: str = None, auto_device: bool = False):
+	def __init__(self, session: Union[ClientSession, Session], deviceId: str = None, auto_device: bool = False, proxies: dict = None, verify = None):
 		self.api = "https://service.narvii.com/api/v1"
 		self.sid = None
 		self.deviceId = deviceId
 		self.gen = Generator(auto_device)
 		self.session = session
+		self.proxies = proxies
+		self.verify = verify
 
 		if isinstance(self.session, ClientSession):self.session_type = "async"
 		elif isinstance(self.session, Session):self.session_type = "sync"
 		else:raise InvalidSessionType(type(self.session))
 
 	def _set(self, act: int, sid: str = None, deviceId: str = None):
 		if act == 1:self.sid=sid
 		if act == 2:self.deviceId=deviceId
 
 
-	def make_request(self, method: str, endpoint: str, body = None, proxies: dict = None, verify = None, type=None):
-		if self.session_type!="sync":raise InvalidFunctionСall("You cannot select this function, your session type is sync")
+	def make_request(self, method: str, endpoint: str, body = None, type=None, successfully: int = 200, headers = None):
+		if self.session_type!="sync":raise InvalidFunctionСall("You cannot select this function, your session type is async")
 		
-		response = self.session.request(method, f"{self.api}{endpoint}", proxies=proxies, verify=verify, data=body, headers=self.gen.get_headers(sid=self.sid, data=body, deviceId=self.deviceId, content_type=type))
-		return check_exceptions(response.text) if response.status_code != 200 else response
+		response = self.session.request(method, f"{self.api}{endpoint}", proxies=self.proxies, verify=self.verify, data=body, headers=headers if headers else self.gen.get_headers(sid=self.sid, data=body, deviceId=self.deviceId, content_type=type))
+		return check_exceptions(response.text) if response.status_code != successfully else response
 
 
-	async def make_async_request(self, method: str, endpoint: str, body = None, type=None):
-		if self.session_type!="sync":raise InvalidFunctionСall("You cannot select this function, your session type is async")
-		response = await self.session.request(method, f"{self.api}{endpoint}", data=dumps(body) if body else None, headers=self.gen.get_headers(sid=self.sid, data=body, deviceId=self.deviceId, content_type=type))
-		return check_exceptions(await response.text()) if response.status != 200 else response
+	async def make_async_request(self, method: str, endpoint: str, body = None, type=None, successfully: int = 200, headers = None):
+		if self.session_type!="sync":raise InvalidFunctionСall("You cannot select this function, your session type is sync")
+		response = await self.session.request(method, f"{self.api}{endpoint}", data=dumps(body) if body else None, headers=headers if headers else self.gen.get_headers(sid=self.sid, data=body, deviceId=self.deviceId, content_type=type))
+		return check_exceptions(await response.text()) if response.status != successfully else response
```

### Comparing `amino.api-1.0/amino.api.egg-info/PKG-INFO` & `amino.api-1.0b2/amino.api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.api
-Version: 1.0
+Version: 1.0b2
 Summary: Library for creating amino bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/amino.api
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip
 Description: <h1 align="center">Amino New Start</h1>
```

