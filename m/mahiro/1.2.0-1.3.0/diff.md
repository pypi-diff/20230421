# Comparing `tmp/mahiro-1.2.0.tar.gz` & `tmp/mahiro-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mahiro-1.2.0.tar", last modified: Sat Apr 15 20:09:03 2023, max compression
+gzip compressed data, was "mahiro-1.3.0.tar", last modified: Fri Apr 21 12:01:42 2023, max compression
```

## Comparing `mahiro-1.2.0.tar` & `mahiro-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.618352 mahiro-1.2.0/
--rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.2.0/LICENSE
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 20:09:03.617374 mahiro-1.2.0/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.2.0/README.md
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.612288 mahiro-1.2.0/mahiro/
--rw-r--r--   0 ryu        (501) staff       (20)       79 2023-04-15 14:58:09.000000 mahiro-1.2.0/mahiro/__init__.py
--rw-r--r--   0 ryu        (501) staff       (20)      955 2023-04-15 15:41:29.000000 mahiro-1.2.0/mahiro/main.py
--rw-r--r--   0 ryu        (501) staff       (20)     4088 2023-04-15 20:07:58.000000 mahiro-1.2.0/mahiro/models.py
--rw-r--r--   0 ryu        (501) staff       (20)     1871 2023-04-15 15:40:57.000000 mahiro-1.2.0/mahiro/send.py
-drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-15 20:09:03.616459 mahiro-1.2.0/mahiro.egg-info/
--rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/PKG-INFO
--rw-r--r--   0 ryu        (501) staff       (20)      241 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/SOURCES.txt
--rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/dependency_links.txt
--rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/requires.txt
--rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-15 20:09:03.000000 mahiro-1.2.0/mahiro.egg-info/top_level.txt
--rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-15 20:09:03.618522 mahiro-1.2.0/setup.cfg
--rw-r--r--   0 ryu        (501) staff       (20)      690 2023-04-15 20:08:25.000000 mahiro-1.2.0/setup.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.705186 mahiro-1.3.0/
+-rw-r--r--   0 ryu        (501) staff       (20)     1064 2023-04-15 13:55:07.000000 mahiro-1.3.0/LICENSE
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 12:01:42.704753 mahiro-1.3.0/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      105 2023-04-15 14:22:50.000000 mahiro-1.3.0/README.md
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.701047 mahiro-1.3.0/mahiro/
+-rw-r--r--   0 ryu        (501) staff       (20)       79 2023-04-15 14:58:09.000000 mahiro-1.3.0/mahiro/__init__.py
+-rw-r--r--   0 ryu        (501) staff       (20)     1330 2023-04-21 11:31:45.000000 mahiro-1.3.0/mahiro/main.py
+-rw-r--r--   0 ryu        (501) staff       (20)     4325 2023-04-21 11:55:24.000000 mahiro-1.3.0/mahiro/models.py
+-rw-r--r--   0 ryu        (501) staff       (20)     2316 2023-04-21 11:54:59.000000 mahiro-1.3.0/mahiro/send.py
+drwxr-xr-x   0 ryu        (501) staff       (20)        0 2023-04-21 12:01:42.704118 mahiro-1.3.0/mahiro.egg-info/
+-rw-r--r--   0 ryu        (501) staff       (20)      399 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/PKG-INFO
+-rw-r--r--   0 ryu        (501) staff       (20)      241 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/SOURCES.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        1 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/dependency_links.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       78 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/requires.txt
+-rw-r--r--   0 ryu        (501) staff       (20)        7 2023-04-21 12:01:42.000000 mahiro-1.3.0/mahiro.egg-info/top_level.txt
+-rw-r--r--   0 ryu        (501) staff       (20)       38 2023-04-21 12:01:42.705343 mahiro-1.3.0/setup.cfg
+-rw-r--r--   0 ryu        (501) staff       (20)      690 2023-04-21 12:01:03.000000 mahiro-1.3.0/setup.py
```

### Comparing `mahiro-1.2.0/LICENSE` & `mahiro-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mahiro-1.2.0/mahiro/main.py` & `mahiro-1.3.0/mahiro/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,58 @@
 from fastapi import FastAPI
-from .models import GroupMessage, FriendMessage, MessageContainer
+from .models import GroupMessage, FriendMessage, MessageContainer, Auth
 import uvicorn
 import os
 
 app = FastAPI()
 
 g_container = MessageContainer()
 
+
 @app.post("/recive/group")
 async def recive_group(data: GroupMessage):
     await g_container.call_group(ctx=data)
 
     return {"code": 200}
 
 
 @app.post("/recive/friend")
 async def recive_friend(data: FriendMessage):
     await g_container.call_friend(ctx=data)
 
     return {"code": 200}
 
 
+@app.post("/recive/auth")
+async def recive_auth(data: Auth):
+    print("Auth token received")
+    g_container.set_token(data.token)
+    print("Registering all plugins to node...")
+    g_container.register_all_plugins()
+    return {"code": 200}
+
+
+@app.get("/recive/health")
+async def recive_health():
+    return {"code": 200}
+
+
 MAHIRO_PYTHON_PORT = os.getenv("MAHIRO_PYTHON_PORT", 8099)
 
-class Mahiro:
 
-    container = g_container
+class Mahiro:
+    container: MessageContainer = g_container
 
     def __init__(self):
         pass
 
     def run(
         self,
         port: int = MAHIRO_PYTHON_PORT,
         host: str = "0.0.0.0",
         reload: bool = False,
     ):
         print("Mahiro Python Bridge is running on port", port)
-        print('Registering all plugins...')
-        self.container.register_all_plugins()
+        # trigger get token url
+        print("Triggering get token...")
+        self.container.want_get_token()
         uvicorn.run(app=app, port=port, host=host, reload=reload)
```

### Comparing `mahiro-1.2.0/mahiro/models.py` & `mahiro-1.3.0/mahiro/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from pydantic import BaseModel
-from .send import Sender, AtUin, Image
+from .send import Sender, AtUin, Image, MAHIRO_TOKEN_HEADER
 import requests
-from typing import Awaitable
+from typing import Awaitable, List, Dict
 from termcolor import colored
 import asyncio
+import time
+
 
 class Msg(BaseModel):
     SubMsgType: int
     Content: str = ""
-    AtUinLists: list[AtUin] = []
-    Images: list[Image] = []
+    AtUinLists: List[AtUin] = []
+    Images: List[Image] = []
     # todo: add types
     Video: dict = {}
     Voice: dict = {}
 
 
 class SubMsgType:
     mixed = 0
     xml = 12
     video = 19
     json = 51
 
 
 # group msg
 class GroupMessageConfigs(BaseModel):
-    availablePlugins: list[str] = []
+    availablePlugins: List[str] = []
 
 
 class GroupMessage(BaseModel):
     userId: int
     userNickname: str = ""
     groupId: int
     groupNickname: str = ""
@@ -51,18 +53,18 @@
 
     def __init__(self, ctx: GroupMessage, sender: Sender, extra: GroupMessageExtra):
         self.ctx = ctx
         self.sender = sender
         self.extra = extra
 
     @staticmethod
-    def create_group_message_mahiro(id: str, ctx: GroupMessage):
+    def create_group_message_mahiro(id: str, ctx: GroupMessage, token: str):
         is_text = ctx.msg.SubMsgType == SubMsgType.mixed
         extra = GroupMessageExtra(is_text=is_text)
-        sender = Sender(id=id, qq=ctx.qq)
+        sender = Sender(id=id, qq=ctx.qq, token=token)
         return GroupMessageMahiro(ctx=ctx, sender=sender, extra=extra)
 
 
 # friend msg
 class FriendMessage(BaseModel):
     userId: int
     userName: str = ""
@@ -73,45 +75,53 @@
 class FriendMessageMahiro:
     ctx: FriendMessage
     sender: Sender
 
     def __init__(self, ctx: FriendMessage, sender: Sender):
         self.ctx = ctx
         self.sender = sender
-    
+
     @staticmethod
-    def create_friend_message_mahiro(id: str, ctx: FriendMessage):
-        sender = Sender(id=id, qq=ctx.qq)
+    def create_friend_message_mahiro(id: str, ctx: FriendMessage, token: str):
+        sender = Sender(id=id, qq=ctx.qq, token=token)
         return FriendMessageMahiro(ctx=ctx, sender=sender)
 
 
 class MessageContainer:
-    instances: dict[str, Awaitable] = {}
-    friend_instances: dict[str, Awaitable] = {}
+    instances: Dict[str, Awaitable] = {}
+    friend_instances: Dict[str, Awaitable] = {}
+    __token: str = ""
 
     def __init__(self):
         pass
 
+    def set_token(self, token: str):
+        self.__token = token
+
     def __register_plugin_to_node(self, id: str):
+        headers = {}
+        headers[MAHIRO_TOKEN_HEADER] = self.__token
+        requests.post(
+            Sender.REGISTER_PLUGIN_URL,
+            json={"name": id},
+            headers=headers,
+        )
+        print(f"register plugin [{id}] to node success")
+
+    def want_get_token(self):
         try:
-            requests.post(
-                Sender.REGISTER_PLUGIN_URL,
-                json={"name": id},
+            requests.get(
+                Sender.GET_TOKEN_URL,
             )
-            print(f"register plugin [{id}] to node success")
         except Exception as e:
-            print("register plugin to node error: ", e)
-            print('\n\n')
-            print(colored('------------- Important -------------', 'red'))
-            print(colored('Please start Mahiro node server first, ', 'red'))
-            print(colored('Then start Mahiro python bridge server.', 'red'))
-            print(colored('-------------------------------------', 'red'))
-            print('\n\n')
-            raise e
-        
+            print(colored("get token error: ", "red"), e)
+            print("Retry after 5 seconds...")
+            time.sleep(5)
+            self.want_get_token()
+
     def register_all_plugins(self):
         for key in self.instances:
             self.__register_plugin_to_node(id=key)
 
     def add_group(self, id: str, callback: Awaitable):
         """
         register group message plugin
@@ -128,22 +138,30 @@
     async def call_group(self, ctx: GroupMessage):
         tasks = []
         available_plugins = ctx.configs.availablePlugins
         for key in available_plugins:
             if key not in self.instances:
                 continue
             # create mahiro
-            mahiro = GroupMessageMahiro.create_group_message_mahiro(id=key, ctx=ctx)
+            mahiro = GroupMessageMahiro.create_group_message_mahiro(
+                id=key, ctx=ctx, token=self.__token
+            )
             # call
             tasks.append(self.instances[key](mahiro))
         if len(tasks) > 0:
             await asyncio.gather(*tasks)
 
     async def call_friend(self, ctx: FriendMessage):
         tasks = []
         for key in self.friend_instances:
             # create mahiro
-            mahiro = FriendMessageMahiro.create_friend_message_mahiro(id=key, ctx=ctx)
+            mahiro = FriendMessageMahiro.create_friend_message_mahiro(
+                id=key, ctx=ctx, token=self.__token
+            )
             # call
             tasks.append(self.friend_instances[key](mahiro))
         if len(tasks) > 0:
-            await asyncio.gather(*tasks)
+            await asyncio.gather(*tasks)
+
+
+class Auth(BaseModel):
+    token: str
```

### Comparing `mahiro-1.2.0/mahiro/send.py` & `mahiro-1.3.0/mahiro/send.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import requests
 from pydantic import BaseModel
+from typing import List
 
 UP_STREAM_URL = os.environ.get("MAHIRO_NODE_URL", "http://0.0.0.0:8098")
+MAHIRO_TOKEN_HEADER = "x-mahiro-token"
 
 
 class AtUin(BaseModel):
     Uin: int
     Nick: str = ""
 
 
@@ -14,67 +16,79 @@
     FileId: int
     FileMd5: str
     FileSize: int
 
 
 class Sender:
     id: str
+    __token: str
     # from qq
     qq: int
 
     __GROUP_URL = f"{UP_STREAM_URL}/api/v1/recive/group"
     __FRIEND_URL = f"{UP_STREAM_URL}/api/v1/recive/friend"
     REGISTER_PLUGIN_URL = f"{UP_STREAM_URL}/api/v1/panel/plugin/register"
+    GET_TOKEN_URL = f"{UP_STREAM_URL}/api/v1/panel/auth/gettoken"
 
-    def __init__(self, id: str, qq: int):
+    def __init__(self, id: str, qq: int, token: str):
         self.id = id
         self.qq = qq
+        self.__token = token
 
     def __create_configs(self):
         return {"id": self.id}
 
+    def __create_headers(self):
+        headers = {}
+        headers[MAHIRO_TOKEN_HEADER] = self.__token
+        return headers
+
     def send_to_group(
         self,
         group_id: int,
         msg: str = "",
-        imgs: list[Image] = [],
-        ats: list[AtUin] = [],
+        imgs: List[Image] = [],
+        ats: List[AtUin] = [],
         fast_image: str = None,
     ):
         json = {
             "groupId": group_id,
             "msg": {
                 "Content": msg,
                 "Images": imgs,
                 "AtUinLists": ats,
             },
             "qq": self.qq,
             "configs": self.__create_configs(),
         }
         if fast_image:
             json["fastImage"] = fast_image
-        print('send_to_group to', json['groupId'])
-        return requests.post(
+        print("send_to_group to", json["groupId"])
+        requests.post(
             self.__GROUP_URL,
             json=json,
+            timeout=5,
+            headers=self.__create_headers(),
         )
 
     def send_to_friend(
         self,
         user_id: int,
         msg: str = "",
-        imgs: list[Image] = [],
+        imgs: List[Image] = [],
         fast_image: str = None,
     ):
         json = {
             "userId": user_id,
             "msg": {"Content": msg, "Images": imgs},
             "qq": self.qq,
             "configs": self.__create_configs(),
         }
         if fast_image:
             json["fastImage"] = fast_image
-        print('send_to_friend to', json['userId'])
+        print("send_to_friend to", json["userId"])
         requests.post(
             self.__FRIEND_URL,
             json=json,
+            timeout=5,
+            headers=self.__create_headers(),
         )
```

### Comparing `mahiro-1.2.0/setup.py` & `mahiro-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return "\n".join(data)
 
 setup(
     name="mahiro",
     description="Python bridge for Mahiro",
     long_description=read_files(["README.md"]),
     long_description_content_type="text/markdown",
-    version="1.2.0",
+    version="1.3.0",
     author="fz6m",
     author_email="i@fz6m.com",
     url="https://github.com/opq-osc/mahiro",
     license="MIT",
     keywords=["OPQ", "OPQBot", "mahiro"],
     packages=find_packages(),
     install_requires=read_files(["requirements.txt"]),
```

