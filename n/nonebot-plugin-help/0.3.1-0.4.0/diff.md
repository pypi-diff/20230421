# Comparing `tmp/nonebot-plugin-help-0.3.1.tar.gz` & `tmp/nonebot_plugin_help-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-help-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_help-0.4.0.tar", max compression
```

## Comparing `nonebot-plugin-help-0.3.1.tar` & `nonebot_plugin_help-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot-plugin-help-0.3.1/LICENSE
--rw-r--r--   0        0        0     1314 2022-06-22 18:07:33.467310 nonebot-plugin-help-0.3.1/nonebot_plugin_help/__init__.py
--rw-r--r--   0        0        0     5136 2022-06-22 18:11:59.155534 nonebot-plugin-help-0.3.1/nonebot_plugin_help/handler.py
--rw-r--r--   0        0        0      619 2022-06-22 18:17:05.558820 nonebot-plugin-help-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6474 2022-06-22 18:15:15.186661 nonebot-plugin-help-0.3.1/README.md
--rw-r--r--   0        0        0     7250 2022-06-22 18:17:10.699801 nonebot-plugin-help-0.3.1/setup.py
--rw-r--r--   0        0        0     7071 2022-06-22 18:17:10.699801 nonebot-plugin-help-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-06-21 14:58:39.859249 nonebot_plugin_help-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1314 2023-04-21 15:38:27.260766 nonebot_plugin_help-0.4.0/nonebot_plugin_help/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-21 15:54:22.509482 nonebot_plugin_help-0.4.0/nonebot_plugin_help/config.py
+-rw-r--r--   0        0        0     5114 2023-04-21 15:55:29.018660 nonebot_plugin_help-0.4.0/nonebot_plugin_help/handler.py
+-rw-r--r--   0        0        0      577 2023-04-21 16:04:48.599018 nonebot_plugin_help-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6433 2023-04-21 16:03:21.346614 nonebot_plugin_help-0.4.0/README.md
+-rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 nonebot_plugin_help-0.4.0/PKG-INFO
```

### Comparing `nonebot-plugin-help-0.3.1/LICENSE` & `nonebot_plugin_help-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-help-0.3.1/nonebot_plugin_help/__init__.py` & `nonebot_plugin_help-0.4.0/nonebot_plugin_help/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .handler import helper
 
 
 default_start = list(nonebot.get_driver().config.command_start)[0]
 
 # Legacy way of self registering (use custom attributes)
 # Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
-__help_version__ = '0.3.1'
+__help_version__ = '0.4.0'
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
 __help_plugin_name__ = "Nonebot2 Help Menu"
 # Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
 __usage__ = f'''欢迎使用Nonebot2 Help Menu
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 '''
@@ -28,9 +28,9 @@
 本插件提供公共帮助菜单能力
 此Bot配置的命令前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 
 {default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <插件名>  # 调取目标插件帮助信息
 ''',
-    extra={'version': '0.3.1'}
+    extra={'version': '0.3.2'}
 )
```

### Comparing `nonebot-plugin-help-0.3.1/nonebot_plugin_help/handler.py` & `nonebot_plugin_help-0.4.0/nonebot_plugin_help/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import nonebot.plugin
 from nonebot import on_command
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, Arg
 from nonebot.adapters import Event
-from nonebot.adapters.onebot.v11.message import Message, MessageSegment
+from nonebot.adapters import Message
+
+from .config import Config
 
 default_start = list(nonebot.get_driver().config.command_start)[0]
-helper = on_command("help", priority=1, aliases={"帮助"})
+plugin_config = Config.parse_obj(nonebot.get_driver().config)
+
+helper = on_command("help", priority=plugin_config.help_priority, aliases={"帮助"}, block=plugin_config.help_block)
 # Matcher level info registering, still active in-use
 helper.__help_name__ = 'help'
 helper.__help_info__ = f'''{default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <plugin_name>  # 调取目标插件帮助信息'''
 
 
 @helper.handle()
 async def handle_first_receive(event: Event, matcher: Matcher, args: Message = CommandArg()):
-    at = MessageSegment.at(event.get_user_id())
     if args:
         matcher.set_arg("content", args)
     else:
-        await matcher.finish(Message(at + f'''欢迎使用Nonebot2 Help Menu
+        await matcher.finish(f'''欢迎使用Nonebot2 Help Menu
 支持使用的前缀：{" ".join(list(nonebot.get_driver().config.command_start))}
 {default_start}help  # 获取本插件帮助
 {default_start}help list  # 展示已加载插件列表
 {default_start}help <plugin_name>  # 调取目标插件帮助信息
-'''))
+''', at_sender=True)
 
 
 @helper.got("content")
 async def get_result(event: Event, content: Message = Arg()):
-    at = MessageSegment.at(event.get_user_id())
     arg = content.extract_plain_text().strip()
     if arg.lower() == "list":
         plugin_set = nonebot.plugin.get_loaded_plugins()
         plugin_names = []
         for plugin in plugin_set:
             # plugin.name, then metadata name or legacy help name
             name = f'{plugin.name} | '
@@ -105,9 +107,8 @@
                 results.extend(["", "序号. 命令名: 命令用途"])
                 results.extend(
                     [f'{key}: {value}' for key, value in infos.items()
                      if key and value]
                 )
             results = list(filter(None, results))
             result = '\n'.join(results)
-    await helper.finish(Message().append(at).append(
-        MessageSegment.text(result)))
+    await helper.finish(result, at_sender=True)
```

### Comparing `nonebot-plugin-help-0.3.1/pyproject.toml` & `nonebot_plugin_help-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-help"
-version = "0.3.1"
+version = "0.4.0"
 description = "A general help lister for nonebot2 plugins"
 authors = ["XZhouQD <X.Zhou.QD@hotmail.com>"]
 license = "AGPL v3"
 readme = "README.md"
 homepage = "https://github.com/XZhouQD/nonebot-plugin-help"
 repository = "https://github.com/XZhouQD/nonebot-plugin-help"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.3"
+python = "^3.8.0"
 nonebot2 = "^2.0.0-beta.4"
-nonebot-adapter-onebot = "^2.0.0-beta.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot-plugin-help-0.3.1/README.md` & `nonebot_plugin_help-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,31 +8,30 @@
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-help">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-help?color=green&style=for-the-badge" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-help">
     <img src="https://img.shields.io/pypi/dm/nonebot-plugin-help?style=for-the-badge" alt="pypi download">
 </a>
-<img src="https://img.shields.io/badge/python-3.7.3+-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
 <br />
-<img src="https://img.shields.io/badge/tested_python-3.8.10-blue?style=for-the-badge" alt="python">
-<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0-rc1&color=blue&style=for-the-badge" alt="python">
-
-<br />
-<a href="https://github.com/botuniverse/onebot/blob/master/README.md">
-    <img src="https://img.shields.io/badge/Onebot-v11-brightgreen?style=for-the-badge" alt="onebot">
-</a>
-<a href="https://github.com/nonebot/nonebot2">
-    <img src="https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red&style=for-the-badge" alt="nonebot">
-</a>
-<a href="https://pypi.org/project/nonebot-adapter-cqhttp/">
-    <img src="https://img.shields.io/static/v1?label=Nonebot-adapters-onebot&message=2.0.0%2Dbeta.1&color=red&style=for-the-badge" alt="nonebot-adapters-cqhttp">
-</a>
+<img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
 </div>
 
+## 配置help插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+
+用户可在.env配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将help命令配置为`priority=100, block=True`
+```
+help_block = true
+help_priority = 100
+```
+
 ## 开发者接入此插件列表方法
 您可以直接参考本插件的接入方式，阅读源代码即可！
 ### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)
 使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含Matcher级别接入）
 ```python
 # New way of self registering (use PluginMetadata)
 __plugin_meta__ = nonebot.plugin.PluginMetadata(
```

#### html2text {}

```diff
@@ -1,12 +1,17 @@
 # nonebot-plugin-help ### Nonebot2 è½»éçº§å¸®å©æä»¶ [license] [pypi] [pypi
                               download] [python]
-                              [python] [python]
-                 [onebot] [nonebot] [nonebot-adapters-cqhttp]
-## å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³
+                          [python] [python] [nonebot]
+## éç½®helpæä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https:
+//img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
+block=False`
+ç¨æ·å¯å¨.envéç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°helpå½ä»¤éç½®ä¸º`priority=100,
+block=True` ``` help_block = true help_priority = 100 ``` ##
+å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³
 æ¨å¯ä»¥ç´æ¥åèæ¬æä»¶çæ¥å¥æ¹å¼ï¼éè¯»æºä»£ç å³å¯ï¼ ###
 æä»¶çº§å«åæ°æ®æ¥å¥ ![nonebot2](https://img.shields.io/static/
 v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ä½¿ç¨èª **Nonebot 2.0.0-
 beta.4**
 çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«Matcherçº§å«æ¥å¥ï¼
 ```python # New way of self registering (use PluginMetadata) __plugin_meta__ =
 nonebot.plugin.PluginMetadata( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-
```

### Comparing `nonebot-plugin-help-0.3.1/setup.py` & `nonebot_plugin_help-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,168 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-help
+Version: 0.4.0
+Summary: A general help lister for nonebot2 plugins
+Home-page: https://github.com/XZhouQD/nonebot-plugin-help
+License: AGPL v3
+Author: XZhouQD
+Author-email: X.Zhou.QD@hotmail.com
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot2 (>=2.0.0-beta.4,<3.0.0)
+Project-URL: Repository, https://github.com/XZhouQD/nonebot-plugin-help
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# nonebot-plugin-help
+### Nonebot2 轻量级帮助插件
+
+<a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-help/main/LICENSE">
+    <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-help">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-help?color=green&style=for-the-badge" alt="pypi">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-help">
+    <img src="https://img.shields.io/pypi/dm/nonebot-plugin-help?style=for-the-badge" alt="pypi download">
+</a>
+<img src="https://img.shields.io/badge/require_python-3.8+-blue?style=for-the-badge" alt="python">
+<br />
+<img src="https://img.shields.io/badge/tested_python-3.10.6-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/badge/tested_env-go_cqhttp_1.0.0-blue?style=for-the-badge" alt="python">
+<img src="https://img.shields.io/badge/tested_Nonebot-2.0.0_rc4-red?style=for-the-badge" alt="nonebot">
+</div>
+
+## 配置help插件优先级与阻塞（可选） ![nonebot-plugin-help](https://img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0版本起，新增插件优先级与阻塞设置（可选），默认为`priority=1, block=False`
+
+用户可在.env配置文件内通过配置项`help_block`与`help_priority`进行配置，例如，以下配置可将help命令配置为`priority=100, block=True`
+```
+help_block = true
+help_priority = 100
+```
+
+## 开发者接入此插件列表方法
+您可以直接参考本插件的接入方式，阅读源代码即可！
+### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)
+使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含Matcher级别接入）
+```python
+# New way of self registering (use PluginMetadata)
+__plugin_meta__ = nonebot.plugin.PluginMetadata(
+    name='您的插件名称（有别于nonebot-plugin-xxx的包名）',
+    description='您的简单插件描述',
+    usage='''您想在使用命令/help <your plugin package name>时提供的帮助文本''',
+    extra={'version': '0.3.1'}
+)
+```
+### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
+使用python包形态的插件（已发布/自行开发皆可），并在插件包的__init__.py文件内增加如下代码：
+```python
+# 您的插件版本号，将在/help list中显示
+# Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
+__help_version__ = '0.3.1'
+# 此名称有助于美化您的插件在/help list中的显示
+# 但使用/help xxx查询插件用途时仍必须使用包名
+# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
+__help_plugin_name__ = "您的插件名称（有别于nonebot-plugin-xxx的包名）"
+# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage
+# 若此文本不存在，将显示包的__doc__
+__usage__ = '您想在使用命令/help <your plugin package name>时提供的帮助文本'
+```
+### Matcher级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
+Matcher级别帮助请为Matcher添加如下代码：
+```python
+default_start = list(nonebot.get_driver().config.command_start)[0]
+helper = on_command("help", priority=1, aliases={"帮助"})
+helper.__help_name__ = '您的命令触发指令名'
+helper.__help_info__ = '您为此命令提供的帮助文本'
+helper.__doc__ = '您为此命令提供的帮助文本, 当您不希望使用__help_info__提供时，可以使用__doc__提供'
+```
+请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此Matcher不会列入Matcher级别帮助！
+
+## 实际使用
+此部分介绍以使用'/'作为command_start为例。
+### 获取本插件帮助
+指令： /help
+
+返回示例：
+```
+@<user_who_send_command> 欢迎使用Nonebot2 Help Menu
+支持使用的前缀：/
+/help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <plugin_name>  # 调取目标插件帮助信息
+```
+### 查看已加载插件列表
+指令：/help list
+
+返回示例：
+```
+@<user_who_send_command> 已加载插件：
+nonebot_plugin_cloverdata | 四叶草魔物娘属性计算插件 | 0.1.0
+nonebot_plugin_guild_patch 
+nonebot_plugin_help | Nonebot2 Help Menu | 0.3.1
+```
+
+### 查看已加载某一插件用途
+指令：/help <plugin_package_name | plugin_help_name>
+示例：
+```
+/help nonebot_plugin_help
+
+@<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
+欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
+本插件提供公共帮助菜单能力
+此Bot配置的命令前缀：/
+
+/help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <插件名>  # 调取目标插件帮助信息
+
+
+序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
+1. help: /help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <plugin_name>  # 调取目标插件帮助信息
+```
+或使用提供的插件美化名示例：
+```
+/help Nonebot2 Help Menu
+
+@<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件
+欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助
+本插件提供公共帮助菜单能力
+此Bot配置的命令前缀：/
+
+/help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <插件名>  # 调取目标插件帮助信息
+
+
+序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助
+1. help: /help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <plugin_name>  # 调取目标插件帮助信息
+```
+
+若插件未提供__usage__，则会显示__doc__，示例：
+```
+/help nonebot_plugin_help
+
+@<user_who_send_command>
+Nonebot 2 Help Menu
+Author: XZhouQD
+Since: 16 May 2021
+
+
+序号. 命令名: 命令用途
+1. help: /help  # 获取本插件帮助
+/help list  # 展示已加载插件列表
+/help <plugin_name>  # 调取目标插件帮助信息
+```
 
-packages = \
-['nonebot_plugin_help']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0', 'nonebot2>=2.0.0-beta.4,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-help',
-    'version': '0.3.1',
-    'description': 'A general help lister for nonebot2 plugins',
-    'long_description': '<div align="center">\n\n# nonebot-plugin-help\n### Nonebot2 轻量级帮助插件\n\n<a href="https://raw.githubusercontent.com/xzhouqd/nonebot-plugin-help/main/LICENSE">\n    <img src="https://img.shields.io/github/license/xzhouqd/nonebot-plugin-help?style=for-the-badge" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-help">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-help?color=green&style=for-the-badge" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-help">\n    <img src="https://img.shields.io/pypi/dm/nonebot-plugin-help?style=for-the-badge" alt="pypi download">\n</a>\n<img src="https://img.shields.io/badge/python-3.7.3+-blue?style=for-the-badge" alt="python">\n<br />\n<img src="https://img.shields.io/badge/tested_python-3.8.10-blue?style=for-the-badge" alt="python">\n<img src="https://img.shields.io/static/v1?label=tested+env&message=go-cqhttp+1.0.0-rc1&color=blue&style=for-the-badge" alt="python">\n\n<br />\n<a href="https://github.com/botuniverse/onebot/blob/master/README.md">\n    <img src="https://img.shields.io/badge/Onebot-v11-brightgreen?style=for-the-badge" alt="onebot">\n</a>\n<a href="https://github.com/nonebot/nonebot2">\n    <img src="https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red&style=for-the-badge" alt="nonebot">\n</a>\n<a href="https://pypi.org/project/nonebot-adapter-cqhttp/">\n    <img src="https://img.shields.io/static/v1?label=Nonebot-adapters-onebot&message=2.0.0%2Dbeta.1&color=red&style=for-the-badge" alt="nonebot-adapters-cqhttp">\n</a>\n</div>\n\n## 开发者接入此插件列表方法\n您可以直接参考本插件的接入方式，阅读源代码即可！\n### 插件级别元数据接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)\n使用自 **Nonebot 2.0.0-beta.4** 版本起新增的插件元数据进行插件级统一接入（不包含Matcher级别接入）\n```python\n# New way of self registering (use PluginMetadata)\n__plugin_meta__ = nonebot.plugin.PluginMetadata(\n    name=\'您的插件名称（有别于nonebot-plugin-xxx的包名）\',\n    description=\'您的简单插件描述\',\n    usage=\'\'\'您想在使用命令/help <your plugin package name>时提供的帮助文本\'\'\',\n    extra={\'version\': \'0.3.1\'}\n)\n```\n### 插件级别传统接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)\n使用python包形态的插件（已发布/自行开发皆可），并在插件包的__init__.py文件内增加如下代码：\n```python\n# 您的插件版本号，将在/help list中显示\n# Deprecated for nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra[\'version\']\n__help_version__ = \'0.3.1\'\n# 此名称有助于美化您的插件在/help list中的显示\n# 但使用/help xxx查询插件用途时仍必须使用包名\n# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name\n__help_plugin_name__ = "您的插件名称（有别于nonebot-plugin-xxx的包名）"\n# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage\n# 若此文本不存在，将显示包的__doc__\n__usage__ = \'您想在使用命令/help <your plugin package name>时提供的帮助文本\'\n```\n### Matcher级别接入 ![nonebot2](https://img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)\nMatcher级别帮助请为Matcher添加如下代码：\n```python\ndefault_start = list(nonebot.get_driver().config.command_start)[0]\nhelper = on_command("help", priority=1, aliases={"帮助"})\nhelper.__help_name__ = \'您的命令触发指令名\'\nhelper.__help_info__ = \'您为此命令提供的帮助文本\'\nhelper.__doc__ = \'您为此命令提供的帮助文本, 当您不希望使用__help_info__提供时，可以使用__doc__提供\'\n```\n请注意：当您未提供`__help_name__`或`__help_info__`与`__doc__`中的一个时，此Matcher不会列入Matcher级别帮助！\n\n## 实际使用\n此部分介绍以使用\'/\'作为command_start为例。\n### 获取本插件帮助\n指令： /help\n\n返回示例：\n```\n@<user_who_send_command> 欢迎使用Nonebot2 Help Menu\n支持使用的前缀：/\n/help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <plugin_name>  # 调取目标插件帮助信息\n```\n### 查看已加载插件列表\n指令：/help list\n\n返回示例：\n```\n@<user_who_send_command> 已加载插件：\nnonebot_plugin_cloverdata | 四叶草魔物娘属性计算插件 | 0.1.0\nnonebot_plugin_guild_patch \nnonebot_plugin_help | Nonebot2 Help Menu | 0.3.1\n```\n\n### 查看已加载某一插件用途\n指令：/help <plugin_package_name | plugin_help_name>\n示例：\n```\n/help nonebot_plugin_help\n\n@<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件\n欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助\n本插件提供公共帮助菜单能力\n此Bot配置的命令前缀：/\n\n/help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <插件名>  # 调取目标插件帮助信息\n\n\n序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助\n1. help: /help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <plugin_name>  # 调取目标插件帮助信息\n```\n或使用提供的插件美化名示例：\n```\n/help Nonebot2 Help Menu\n\n@<user_who_send_command> Nonebot2 Help Menu: Nonebot2轻量级帮助插件\n欢迎使用Nonebot2 Help Menu                       // 这里是插件元数据提供的帮助\n本插件提供公共帮助菜单能力\n此Bot配置的命令前缀：/\n\n/help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <插件名>  # 调取目标插件帮助信息\n\n\n序号. 命令名: 命令用途                             // 这里是Matcher级别接入提供的帮助\n1. help: /help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <plugin_name>  # 调取目标插件帮助信息\n```\n\n若插件未提供__usage__，则会显示__doc__，示例：\n```\n/help nonebot_plugin_help\n\n@<user_who_send_command>\nNonebot 2 Help Menu\nAuthor: XZhouQD\nSince: 16 May 2021\n\n\n序号. 命令名: 命令用途\n1. help: /help  # 获取本插件帮助\n/help list  # 展示已加载插件列表\n/help <plugin_name>  # 调取目标插件帮助信息\n```\n',
-    'author': 'XZhouQD',
-    'author_email': 'X.Zhou.QD@hotmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/XZhouQD/nonebot-plugin-help',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.3,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,77 +1,83 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_help'] package_data = \ {'': ['*']} install_requires = \
-['nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0', 'nonebot2>=2.0.0-
-beta.4,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-help', 'version':
-'0.3.1', 'description': 'A general help lister for nonebot2 plugins',
-'long_description': '
-     \n\n# nonebot-plugin-help\n### Nonebot2 è½»éçº§å¸®å©æä»¶\n\n\n_
-          [license]\n\n\n_[pypi]\n\n\n_[pypi_download]\n\n[python]\n
-                           \n[python]\n[python]\n\n
-       \n\n_[onebot]\n\n\n_[nonebot]\n\n\n_[nonebot-adapters-cqhttp]\n\n
-\n\n##
-å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³\næ¨å¯ä»¥ç´æ¥åèæ¬æä»¶çæ¥å¥æ¹å¼ï¼éè¯»æºä»£ç å³å¯ï¼\n###
+Metadata-Version: 2.1 Name: nonebot-plugin-help Version: 0.4.0 Summary: A
+general help lister for nonebot2 plugins Home-page: https://github.com/XZhouQD/
+nonebot-plugin-help License: AGPL v3 Author: XZhouQD Author-email:
+X.Zhou.QD@hotmail.com Requires-Python: >=3.8.0,<4.0.0 Classifier: License ::
+Other/Proprietary License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
+(>=2.0.0-beta.4,<3.0.0) Project-URL: Repository, https://github.com/XZhouQD/
+nonebot-plugin-help Description-Content-Type: text/markdown
+# nonebot-plugin-help ### Nonebot2 è½»éçº§å¸®å©æä»¶ [license] [pypi] [pypi
+                              download] [python]
+                          [python] [python] [nonebot]
+## éç½®helpæä»¶ä¼åçº§ä¸é»å¡ï¼å¯éï¼ ![nonebot-plugin-help](https:
+//img.shields.io/static/v1?label=nonebot-plugin-help&message=0.4.0&color=red)
+0.4.0çæ¬èµ·ï¼æ°å¢æä»¶ä¼åçº§ä¸é»å¡è®¾ç½®ï¼å¯éï¼ï¼é»è®¤ä¸º`priority=1,
+block=False`
+ç¨æ·å¯å¨.envéç½®æä»¶åéè¿éç½®é¡¹`help_block`ä¸`help_priority`è¿è¡éç½®ï¼ä¾å¦ï¼ä»¥ä¸éç½®å¯å°helpå½ä»¤éç½®ä¸º`priority=100,
+block=True` ``` help_block = true help_priority = 100 ``` ##
+å¼åèæ¥å¥æ­¤æä»¶åè¡¨æ¹æ³
+æ¨å¯ä»¥ç´æ¥åèæ¬æä»¶çæ¥å¥æ¹å¼ï¼éè¯»æºä»£ç å³å¯ï¼ ###
 æä»¶çº§å«åæ°æ®æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red)\nä½¿ç¨èª **Nonebot 2.0.0-
+v1?label=Nonebot&message=2.0.0%2Dbeta.4&color=red) ä½¿ç¨èª **Nonebot 2.0.0-
 beta.4**
-çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«Matcherçº§å«æ¥å¥ï¼\n```python\n#
-New way of self registering (use PluginMetadata)\n__plugin_meta__ =
-nonebot.plugin.PluginMetadata(\n name=\'æ¨çæä»¶åç§°ï¼æå«äºnonebot-
-plugin-xxxçååï¼\',\n description=\'æ¨çç®åæä»¶æè¿°\',\n
-usage=\'\'\'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬\'\'\',\n extra=
-{\'version\': \'0.3.1\'}\n)\n```\n### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2]
-(https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)\nä½¿ç¨pythonåå½¢æçæä»¶ï¼å·²åå¸/
-èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç__init__.pyæä»¶åå¢å å¦ä¸ä»£ç ï¼\n```python\n#
-æ¨çæä»¶çæ¬å·ï¼å°å¨/help listä¸­æ¾ç¤º\n# Deprecated for nonebot-
-plugin-help 0.3.1+, prefer PluginMetadata.extra[\'version\']\n__help_version__
-= \'0.3.1\'\n# æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help listä¸­çæ¾ç¤º\n#
-ä½ä½¿ç¨/help xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå\n# Deprecated for
-nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name\n__help_plugin_name__ =
-"æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-xxxçååï¼"\n# Deprecated
-for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.usage\n#
-è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__\n__usage__ =
-\'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬\'\n```\n###
+çæ¬èµ·æ°å¢çæä»¶åæ°æ®è¿è¡æä»¶çº§ç»ä¸æ¥å¥ï¼ä¸åå«Matcherçº§å«æ¥å¥ï¼
+```python # New way of self registering (use PluginMetadata) __plugin_meta__ =
+nonebot.plugin.PluginMetadata( name='æ¨çæä»¶åç§°ï¼æå«äºnonebot-
+plugin-xxxçååï¼', description='æ¨çç®åæä»¶æè¿°',
+usage='''æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬''', extra=
+{'version': '0.3.1'} ) ``` ### æä»¶çº§å«ä¼ ç»æ¥å¥ ![nonebot2](https://
+img.shields.io/static/v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
+ä½¿ç¨pythonåå½¢æçæä»¶ï¼å·²åå¸/
+èªè¡å¼åçå¯ï¼ï¼å¹¶å¨æä»¶åç__init__.pyæä»¶åå¢å å¦ä¸ä»£ç ï¼
+```python # æ¨çæä»¶çæ¬å·ï¼å°å¨/help listä¸­æ¾ç¤º # Deprecated for
+nonebot-plugin-help 0.3.1+, prefer PluginMetadata.extra['version']
+__help_version__ = '0.3.1' # æ­¤åç§°æå©äºç¾åæ¨çæä»¶å¨/help
+listä¸­çæ¾ç¤º # ä½ä½¿ç¨/help xxxæ¥è¯¢æä»¶ç¨éæ¶ä»å¿é¡»ä½¿ç¨åå
+# Deprecated for nonebot-plugin-help 0.3.0+, prefer PluginMetadata.name
+__help_plugin_name__ = "æ¨çæä»¶åç§°ï¼æå«äºnonebot-plugin-
+xxxçååï¼" # Deprecated for nonebot-plugin-help 0.3.0+, prefer
+PluginMetadata.usage # è¥æ­¤ææ¬ä¸å­å¨ï¼å°æ¾ç¤ºåç__doc__ __usage__
+= 'æ¨æ³å¨ä½¿ç¨å½ä»¤/help æ¶æä¾çå¸®å©ææ¬' ``` ###
 Matcherçº§å«æ¥å¥ ![nonebot2](https://img.shields.io/static/
-v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)\nMatcherçº§å«å¸®å©è¯·ä¸ºMatcheræ·»å å¦ä¸ä»£ç ï¼\n```python\ndefault_start
-= list(nonebot.get_driver().config.command_start)[0]\nhelper = on_command
-("help", priority=1, aliases={"å¸®å©"})\nhelper.__help_name__ =
-\'æ¨çå½ä»¤è§¦åæä»¤å\'\nhelper.__help_info__ =
-\'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬\'\nhelper.__doc__ =
-\'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬,
-å½æ¨ä¸å¸æä½¿ç¨__help_info__æä¾æ¶ï¼å¯ä»¥ä½¿ç¨__doc__æä¾\'\n```\nè¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤Matcherä¸ä¼åå¥Matcherçº§å«å¸®å©ï¼\n\n##
-å®éä½¿ç¨\næ­¤é¨åä»ç»ä»¥ä½¿ç¨\'/\'ä½ä¸ºcommand_startä¸ºä¾ã\n###
-è·åæ¬æä»¶å¸®å©\næä»¤ï¼ /help\n\nè¿åç¤ºä¾ï¼\n```\n@
-æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu\næ¯æä½¿ç¨çåç¼ï¼/\n/help #
-è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/help  #
-è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n```\n###
-æ¥çå·²å è½½æä»¶åè¡¨\næä»¤ï¼/help list\n\nè¿åç¤ºä¾ï¼\n```\n@
-å·²å è½½æä»¶ï¼\nnonebot_plugin_cloverdata |
-åå¶èé­ç©å¨å±æ§è®¡ç®æä»¶ | 0.1.0\nnonebot_plugin_guild_patch
-\nnonebot_plugin_help | Nonebot2 Help Menu | 0.3.1\n```\n\n###
-æ¥çå·²å è½½æä¸æä»¶ç¨é\næä»¤ï¼/help
- plugin_help_name>\nç¤ºä¾ï¼\n```\n/help nonebot_plugin_help\n\n@ Nonebot2
-Help Menu: Nonebot2è½»éçº§å¸®å©æä»¶\næ¬¢è¿ä½¿ç¨Nonebot2 Help Menu /
-/
-è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©\næ¬æä»¶æä¾å¬å±å¸®å©èåè½å\næ­¤Botéç½®çå½ä»¤åç¼ï¼/
-\n\n/help # è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/
-help <æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n\n\nåºå·. å½ä»¤å:
-å½ä»¤ç¨é // è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å©\n1. help: /help #
-è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/help  #
-è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n```\næä½¿ç¨æä¾çæä»¶ç¾ååç¤ºä¾ï¼\n```\n/
-help Nonebot2 Help Menu\n\n@ Nonebot2 Help Menu:
-Nonebot2è½»éçº§å¸®å©æä»¶\næ¬¢è¿ä½¿ç¨Nonebot2 Help Menu /
-/
-è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©\næ¬æä»¶æä¾å¬å±å¸®å©èåè½å\næ­¤Botéç½®çå½ä»¤åç¼ï¼/
-\n\n/help # è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/
-help <æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n\n\nåºå·. å½ä»¤å:
-å½ä»¤ç¨é // è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å©\n1. help: /help #
-è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/help  #
-è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n```\n\nè¥æä»¶æªæä¾__usage__ï¼åä¼æ¾ç¤º__doc__ï¼ç¤ºä¾ï¼\n```\n/
-help nonebot_plugin_help\n\n@\nNonebot 2 Help Menu\nAuthor: XZhouQD\nSince: 16
-May 2021\n\n\nåºå·. å½ä»¤å: å½ä»¤ç¨é\n1. help: /help #
-è·åæ¬æä»¶å¸®å©\n/help list # å±ç¤ºå·²å è½½æä»¶åè¡¨\n/help  #
-è°åç®æ æä»¶å¸®å©ä¿¡æ¯\n```\n', 'author': 'XZhouQD', 'author_email':
-'X.Zhou.QD@hotmail.com', 'maintainer': None, 'maintainer_email': None, 'url':
-'https://github.com/XZhouQD/nonebot-plugin-help', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.7.3,<4.0.0', } setup(**setup_kwargs)
+v1?label=Nonebot&message=2.0.0%2Dbeta.1&color=red)
+Matcherçº§å«å¸®å©è¯·ä¸ºMatcheræ·»å å¦ä¸ä»£ç ï¼ ```python default_start =
+list(nonebot.get_driver().config.command_start)[0] helper = on_command("help",
+priority=1, aliases={"å¸®å©"}) helper.__help_name__ =
+'æ¨çå½ä»¤è§¦åæä»¤å' helper.__help_info__ =
+'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬' helper.__doc__ =
+'æ¨ä¸ºæ­¤å½ä»¤æä¾çå¸®å©ææ¬,
+å½æ¨ä¸å¸æä½¿ç¨__help_info__æä¾æ¶ï¼å¯ä»¥ä½¿ç¨__doc__æä¾' ```
+è¯·æ³¨æï¼å½æ¨æªæä¾`__help_name__`æ`__help_info__`ä¸`__doc__`ä¸­çä¸ä¸ªæ¶ï¼æ­¤Matcherä¸ä¼åå¥Matcherçº§å«å¸®å©ï¼
+## å®éä½¿ç¨ æ­¤é¨åä»ç»ä»¥ä½¿ç¨'/'ä½ä¸ºcommand_startä¸ºä¾ã ###
+è·åæ¬æä»¶å¸®å© æä»¤ï¼ /help è¿åç¤ºä¾ï¼ ``` @
+æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu æ¯æä½¿ç¨çåç¼ï¼/ /help #
+è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
+è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ``` ### æ¥çå·²å è½½æä»¶åè¡¨ æä»¤ï¼/
+help list è¿åç¤ºä¾ï¼ ``` @ å·²å è½½æä»¶ï¼ nonebot_plugin_cloverdata |
+åå¶èé­ç©å¨å±æ§è®¡ç®æä»¶ | 0.1.0 nonebot_plugin_guild_patch
+nonebot_plugin_help | Nonebot2 Help Menu | 0.3.1 ``` ###
+æ¥çå·²å è½½æä¸æä»¶ç¨é æä»¤ï¼/help
+ plugin_help_name> ç¤ºä¾ï¼ ``` /help nonebot_plugin_help @ Nonebot2 Help
+Menu: Nonebot2è½»éçº§å¸®å©æä»¶ æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu /
+/ è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©
+æ¬æä»¶æä¾å¬å±å¸®å©èåè½å æ­¤Botéç½®çå½ä»¤åç¼ï¼/ /help #
+è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help
+<æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ åºå·. å½ä»¤å: å½ä»¤ç¨é /
+/ è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å© 1. help: /help #
+è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
+è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ``` æä½¿ç¨æä¾çæä»¶ç¾ååç¤ºä¾ï¼
+``` /help Nonebot2 Help Menu @ Nonebot2 Help Menu:
+Nonebot2è½»éçº§å¸®å©æä»¶ æ¬¢è¿ä½¿ç¨Nonebot2 Help Menu /
+/ è¿éæ¯æä»¶åæ°æ®æä¾çå¸®å©
+æ¬æä»¶æä¾å¬å±å¸®å©èåè½å æ­¤Botéç½®çå½ä»¤åç¼ï¼/ /help #
+è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help
+<æä»¶å> # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ åºå·. å½ä»¤å: å½ä»¤ç¨é /
+/ è¿éæ¯Matcherçº§å«æ¥å¥æä¾çå¸®å© 1. help: /help #
+è·åæ¬æä»¶å¸®å© /help list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  #
+è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
+è¥æä»¶æªæä¾__usage__ï¼åä¼æ¾ç¤º__doc__ï¼ç¤ºä¾ï¼ ``` /help
+nonebot_plugin_help @ Nonebot 2 Help Menu Author: XZhouQD Since: 16 May 2021
+åºå·. å½ä»¤å: å½ä»¤ç¨é 1. help: /help # è·åæ¬æä»¶å¸®å© /help
+list # å±ç¤ºå·²å è½½æä»¶åè¡¨ /help  # è°åç®æ æä»¶å¸®å©ä¿¡æ¯ ```
```

