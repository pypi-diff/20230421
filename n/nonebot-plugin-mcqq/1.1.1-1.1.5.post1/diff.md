# Comparing `tmp/nonebot-plugin-mcqq-1.1.1.tar.gz` & `tmp/nonebot-plugin-mcqq-1.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-1.1.1.tar", last modified: Wed Feb 15 13:30:11 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-1.1.5.post1.tar", last modified: Fri Apr 21 09:59:51 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-1.1.1.tar` & `nonebot-plugin-mcqq-1.1.5.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 13:30:11.035151 nonebot-plugin-mcqq-1.1.1/
--rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2641 2023-02-15 13:30:11.034180 nonebot-plugin-mcqq-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2023-01-26 17:04:35.000000 nonebot-plugin-mcqq-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-15 13:30:11.016201 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq/
--rw-rw-rw-   0        0        0      825 2023-01-13 05:35:44.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq/__init__.py
--rw-rw-rw-   0        0        0     4147 2023-02-15 10:45:36.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq/data_source.py
--rw-rw-rw-   0        0        0     7926 2023-02-02 06:27:05.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-15 13:30:11.032158 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/
--rw-rw-rw-   0        0        0     2641 2023-02-15 13:30:10.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-02-15 13:30:11.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 13:30:10.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-02-15 13:30:10.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-15 13:30:10.000000 nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-15 13:30:11.035151 nonebot-plugin-mcqq-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-02-15 13:29:48.000000 nonebot-plugin-mcqq-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/
+-rw-rw-rw-   0        0        0    35184 2022-08-07 15:18:53.000000 nonebot-plugin-mcqq-1.1.5.post1/LICENSE
+-rw-rw-rw-   0        0        0     2647 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2146 2023-01-26 17:04:35.000000 nonebot-plugin-mcqq-1.1.5.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.269679 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/
+-rw-rw-rw-   0        0        0      911 2023-04-21 09:31:25.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/__init__.py
+-rw-rw-rw-   0        0        0     2422 2023-04-21 09:32:08.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/data_source.py
+-rw-rw-rw-   0        0        0     1023 2023-04-21 09:31:25.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:59:51.279688 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/
+-rw-rw-rw-   0        0        0     2647 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-21 09:59:51.000000 nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:59:51.280689 nonebot-plugin-mcqq-1.1.5.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-04-21 09:58:44.000000 nonebot-plugin-mcqq-1.1.5.post1/setup.py
```

### Comparing `nonebot-plugin-mcqq-1.1.1/LICENSE` & `nonebot-plugin-mcqq-1.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.1/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.1
+Version: 1.1.5.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.1/README.md` & `nonebot-plugin-mcqq-1.1.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq/__init__.py` & `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from nonebot import on_message, get_driver
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
 from nonebot_plugin_guild_patch import GuildMessageEvent
-
-from .data_source import send_msg_to_mc, start_ws_server, stop_ws_server
-from .utils import msg_rule
 from typing import Union
+from mcqq_tool.mcqq import send_msg_to_mc
+from .data_source import start_ws_server, stop_ws_server
+from .utils import msg_rule, plugin_config
 
 mc_qq = on_message(priority=5, rule=msg_rule, block=False)
 
 driver = get_driver()
 
 
 # bot连接时
@@ -23,8 +23,8 @@
     # 关闭 WebSocket 服务器
     await stop_ws_server()
 
 
 # 收到 群/频 道消息时
 @mc_qq.handle()
 async def handle_first_receive(bot: Bot, event: Union[GroupMessageEvent, GuildMessageEvent]):
-    await send_msg_to_mc(bot=bot, event=event)
+    await send_msg_to_mc(bot=bot, event=event, server_list=plugin_config.mc_qq_servers_list)
```

### Comparing `nonebot-plugin-mcqq-1.1.1/nonebot_plugin_mcqq.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-1.1.5.post1/nonebot_plugin_mcqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq
-Version: 1.1.1
+Version: 1.1.5.post1
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-1.1.1/setup.py` & `nonebot-plugin-mcqq-1.1.5.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.1",  # 程序版本
+    version="1.1.5-post1",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.10
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        'mcqq-tool>=0.0.1',
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
     ],
 )
```

