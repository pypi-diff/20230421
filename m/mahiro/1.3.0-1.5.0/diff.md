# Comparing `tmp/mahiro-1.3.0.tar.gz` & `tmp/mahiro-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahiro-1.3.0.tar", last modified: Fri Apr 21 12:01:42 2023, max compression
+gzip compressed data, was "mahiro-1.5.0.tar", last modified: Fri Apr 21 17:34:41 2023, max compression
```

## Comparing `mahiro-1.3.0.tar` & `mahiro-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.705186 mahiro-1.3.0/
--rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.3.0/LICENSE
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 12:01:42.704753 mahiro-1.3.0/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.3.0/README.md
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.701047 mahiro-1.3.0/mahiro/
--rw-r--r--   0 ryu        (501) staff       (20)       79 2023-04-15 14:58:09.000000 mahiro-1.3.0/mahiro/__init__.py
--rw-r--r--   0 ryu        (501) staff       (20)     1330 2023-04-21 11:31:45.000000 mahiro-1.3.0/mahiro/main.py
--rw-r--r--   0 ryu        (501) staff       (20)     4325 2023-04-21 11:55:24.000000 mahiro-1.3.0/mahiro/models.py
--rw-r--r--   0 ryu        (501) staff       (20)     2316 2023-04-21 11:54:59.000000 mahiro-1.3.0/mahiro/send.py
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.704118 mahiro-1.3.0/mahiro.egg-info/
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      241 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/SOURCES.txt
--rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/dependency_links.txt
--rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/requires.txt
--rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/top_level.txt
--rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-21 12:01:42.705343 mahiro-1.3.0/setup.cfg
--rw-r--r--   0 ryu        (501) staff       (20)      690 2023-04-21 12:01:03.000000 mahiro-1.3.0/setup.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 17:34:41.866594 mahiro-1.5.0/
+-rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.5.0/LICENSE
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 17:34:41.865989 mahiro-1.5.0/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.5.0/README.md
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 17:34:41.860208 mahiro-1.5.0/mahiro/
+-rw-r--r--   0 ryu        (501) staff       (20)      112 2023-04-21 17:12:55.000000 mahiro-1.5.0/mahiro/__init__.py
+-rw-r--r--   0 ryu        (501) staff       (20)     1388 2023-04-21 17:13:43.000000 mahiro-1.5.0/mahiro/main.py
+-rw-r--r--   0 ryu        (501) staff       (20)     4449 2023-04-21 17:13:22.000000 mahiro-1.5.0/mahiro/models.py
+-rw-r--r--   0 ryu        (501) staff       (20)     2316 2023-04-21 17:13:27.000000 mahiro-1.5.0/mahiro/send.py
+-rw-r--r--   0 ryu        (501) staff       (20)       22 2023-04-21 17:25:56.000000 mahiro-1.5.0/mahiro/version.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 17:34:41.865157 mahiro-1.5.0/mahiro.egg-info/
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 17:34:41.000000 mahiro-1.5.0/mahiro.egg-info/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      259 2023-04-21 17:34:41.000000 mahiro-1.5.0/mahiro.egg-info/SOURCES.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-21 17:34:41.000000 mahiro-1.5.0/mahiro.egg-info/dependency_links.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-21 17:34:41.000000 mahiro-1.5.0/mahiro.egg-info/requires.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-21 17:34:41.000000 mahiro-1.5.0/mahiro.egg-info/top_level.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-21 17:34:41.866822 mahiro-1.5.0/setup.cfg
+-rw-r--r--   0 ryu        (501) staff       (20)      733 2023-04-21 17:34:28.000000 mahiro-1.5.0/setup.py
```

### Comparing `mahiro-1.3.0/LICENSE` & `mahiro-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mahiro-1.3.0/mahiro/main.py` & `mahiro-1.5.0/mahiro/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
+import uvicorn
 from fastapi import FastAPI
+
 from .models import GroupMessage, FriendMessage, MessageContainer, Auth
-import uvicorn
-import os
+from .version import __VERSION__
 
 app = FastAPI()
 
 g_container = MessageContainer()
 
 
 @app.post("/recive/group")
@@ -29,15 +31,15 @@
     print("Registering all plugins to node...")
     g_container.register_all_plugins()
     return {"code": 200}
 
 
 @app.get("/recive/health")
 async def recive_health():
-    return {"code": 200}
+    return {"code": 200, "version": __VERSION__}
 
 
 MAHIRO_PYTHON_PORT = os.getenv("MAHIRO_PYTHON_PORT", 8099)
 
 
 class Mahiro:
     container: MessageContainer = g_container
```

### Comparing `mahiro-1.3.0/mahiro/models.py` & `mahiro-1.5.0/mahiro/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from pydantic import BaseModel
-from .send import Sender, AtUin, Image, MAHIRO_TOKEN_HEADER
+import time
 import requests
-from typing import Awaitable, List, Dict
-from termcolor import colored
 import asyncio
-import time
+from termcolor import colored
+from pydantic import BaseModel
+from typing import Awaitable, List, Dict
 
+from .send import Sender, AtUin, Image, MAHIRO_TOKEN_HEADER
 
 class Msg(BaseModel):
     SubMsgType: int
     Content: str = ""
     AtUinLists: List[AtUin] = []
     Images: List[Image] = []
     # todo: add types
@@ -31,16 +31,20 @@
 
 class GroupMessage(BaseModel):
     userId: int
     userNickname: str = ""
     groupId: int
     groupNickname: str = ""
     msg: Msg
-    qq: int
+    # internal fields
     configs: GroupMessageConfigs
+    # bot qq
+    qq: int
+    # opq raw data
+    raw: dict = {}
 
 
 class GroupMessageExtra:
     is_text: bool
 
     def __init__(self, is_text: bool):
         self.is_text = is_text
@@ -65,15 +69,18 @@
 
 
 # friend msg
 class FriendMessage(BaseModel):
     userId: int
     userName: str = ""
     msg: Msg
+    # bot qq
     qq: int
+    # opq raw data
+    raw: dict = {}
 
 
 class FriendMessageMahiro:
     ctx: FriendMessage
     sender: Sender
 
     def __init__(self, ctx: FriendMessage, sender: Sender):
```

### Comparing `mahiro-1.3.0/mahiro/send.py` & `mahiro-1.5.0/mahiro/send.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
-from pydantic import BaseModel
 from typing import List
+from pydantic import BaseModel
 
 UP_STREAM_URL = os.environ.get("MAHIRO_NODE_URL", "http://0.0.0.0:8098")
 MAHIRO_TOKEN_HEADER = "x-mahiro-token"
 
 
 class AtUin(BaseModel):
     Uin: int
```

