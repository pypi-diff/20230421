# Comparing `tmp/nonebot_plugin_autoreply-0.2.3.tar.gz` & `tmp/nonebot_plugin_autoreply-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_autoreply-0.2.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_autoreply-0.2.4.tar", last modified: Fri Apr 21 14:05:04 2023, max compression
```

## Comparing `nonebot_plugin_autoreply-0.2.3.tar` & `nonebot_plugin_autoreply-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/LICENSE
--rw-r--r--   0        0        0     8285 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/README.md
--rw-r--r--   0        0        0      251 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/nonebot_plugin_autoreply/__init__.py
--rw-r--r--   0        0        0     4849 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/nonebot_plugin_autoreply/__main__.py
--rw-r--r--   0        0        0     1695 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/nonebot_plugin_autoreply/config.py
--rw-r--r--   0        0        0      424 2023-02-22 09:31:15.427090 nonebot_plugin_autoreply-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     9319 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.3/setup.py
--rw-r--r--   0        0        0     8990 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/LICENSE
+-rw-r--r--   0        0        0     8689 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/README.md
+-rw-r--r--   0        0        0      303 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__init__.py
+-rw-r--r--   0        0        0     5086 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__main__.py
+-rw-r--r--   0        0        0     1788 2023-04-21 14:04:54.385930 nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/config.py
+-rw-r--r--   0        0        0      610 2023-04-21 14:05:04.605983 nonebot_plugin_autoreply-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     9230 1970-01-01 00:00:00.000000 nonebot_plugin_autoreply-0.2.4/PKG-INFO
```

### Comparing `nonebot_plugin_autoreply-0.2.3/LICENSE` & `nonebot_plugin_autoreply-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_autoreply-0.2.3/README.md` & `nonebot_plugin_autoreply-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -127,15 +127,18 @@
         // 是否去掉消息前后的空格再匹配
         // 可以不填，默认为 `true`
         "strip": true,
 
         // 当带 cq 码的消息匹配失败时，是否使用去掉 cq 码的消息再匹配一遍
         // 可以不填，默认为 `true`
         "allow_plaintext": true
-      }
+      },
+
+      // 如果规则为一个字符串，则会转换为一个属性全部默认的 `match` 来匹配
+      "测试2"
 
       // 更多匹配规则...
     ],
 
     // 匹配成功后，回复的消息
     // 如果有多个，将随机抽取一个回复
     "replies": [
@@ -150,14 +153,17 @@
 
       // type=plain 时，message 需要为字符串，但是 message 中的 CQ 码不会被解析
       {
         "type": "plain",
         "message": "这条消息后面的CQ码会以原样发送[CQ:at,qq=3076823485]"
       },
 
+      // 直接写 @ 开头的字符串也能表示 type=plain
+      "@这条消息后面的CQ码也会以原样发送[CQ:at,qq=3076823485]",
+
       // type=array 时，message 中需要填 CQ 码的 json 格式
       {
         "type": "array",
         "message": [
           {
             "type": "text",
             "data": {
@@ -276,14 +282,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.4
+
+- 让字符串可以作为默认属性的 `match` 使用
+- 让 `@` 开头的字符串 `reply` 解析为 `plain` 形式的回复
+
 ### 0.2.3
 
 - 修复一处 py 3.8 无法使用的类型注解
 
 ### 0.2.2
 
 - 修复群聊和用户过滤器无法正常使用的问题
```

#### html2text {}

```diff
@@ -32,25 +32,29 @@
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
 æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `false` "to_me": false, // æ¯å¦å¿½ç¥å¤§å°å /
 / å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "ignore_case": true, /
 / æ¯å¦å»ææ¶æ¯ååçç©ºæ ¼åå¹é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
 "strip": true, // å½å¸¦ cq ç çæ¶æ¯å¹éå¤±è´¥æ¶ï¼æ¯å¦ä½¿ç¨å»æ cq
 ç çæ¶æ¯åå¹éä¸é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
-"allow_plaintext": true } // æ´å¤å¹éè§å... ], /
+"allow_plaintext": true }, /
+/ å¦æè§åä¸ºä¸ä¸ªå­ç¬¦ä¸²ï¼åä¼è½¬æ¢ä¸ºä¸ä¸ªå±æ§å¨é¨é»è®¤ç
+`match` æ¥å¹é "æµè¯2" // æ´å¤å¹éè§å... ], /
 / å¹éæååï¼åå¤çæ¶æ¯ /
 / å¦ææå¤ä¸ªï¼å°éæºæ½åä¸ä¸ªåå¤ "replies": [ // type=normal
 æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä¼è§£æ message ä¸­ç CQ ç å¹¶åé
 { "type": "normal", "message": "è¿æ¯ä¸æ¡æ¶æ¯ï¼å¯ä»¥ä½¿ç¨CQç [CQ:
 image,file=https://pixiv.re/103981177.png]" }, /
 / ç´æ¥åå­ç¬¦ä¸²ä¹è½è¡¨ç¤º type=normal
 "è¿æ¯ä¸æ¡æ¶æ¯ï¼å¯ä»¥ä½¿ç¨CQç [CQ:image,file=https://pixiv.re/
 103981177.png]", // type=plain æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä½æ¯
 message ä¸­ç CQ ç ä¸ä¼è¢«è§£æ { "type": "plain", "message":
 "è¿æ¡æ¶æ¯åé¢çCQç ä¼ä»¥åæ ·åé[CQ:at,qq=3076823485]" }, /
+/ ç´æ¥å @ å¼å¤´çå­ç¬¦ä¸²ä¹è½è¡¨ç¤º type=plain
+"@è¿æ¡æ¶æ¯åé¢çCQç ä¹ä¼ä»¥åæ ·åé[CQ:at,qq=3076823485]", /
 / type=array æ¶ï¼message ä¸­éè¦å¡« CQ ç ç json æ ¼å¼ { "type":
 "array", "message": [ { "type": "text", "data": { "text":
 "æåé¢å¸¦äºä¸å¼ å¾çå¦" } }, { "type": "image", "data": { "file":
 "https://pixiv.re/103981177.png" } } ] }, // ç´æ¥åæ°ç»ä¹è½ä»£è¡¨
 type=array [ { "type": "text", "data": { "text": "æå¯ä»¥æ­£å¸¸åéå¦" } }
 ], // type=multi æ¶ï¼message éè¦ä¸ºä¸é¢æå°çæ¶æ¯ç±»åçæ°ç» /
 / ä¼æé¡ºåºåé message ä¸­çææåå®¹ // message
@@ -76,14 +80,16 @@
 æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.3 - ä¿®å¤ä¸å¤ py 3.8
-æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 -
+è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
+å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
 ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
 `match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
 å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
 æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
 `.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

### Comparing `nonebot_plugin_autoreply-0.2.3/nonebot_plugin_autoreply/__main__.py` & `nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from nonebot.permission import SUPERUSER
 from nonebot.typing import T_State
 from typing_extensions import TypeVarTuple, Unpack
 
 from .config import (
     FilterModel,
     MatchModel,
+    MatchType,
     MessageSegmentModel,
     ReplyModel,
     ReplyType,
     config,
     reload_replies,
     replies,
 )
@@ -38,23 +39,26 @@
     is_any: bool = False,
 ) -> bool:
     # 感谢 nb2 群内 Bryan不可思议 佬的帮助！！
     iterator = starmap(function, will_check)
     return any(iterator) if is_any else all(iterator)
 
 
-def check_filter(filter: FilterModel[T], val: Optional[T]) -> bool:
+def check_filter(will_check: FilterModel[T], val: Optional[T]) -> bool:
     # 判断黑名单 值不在列表中ok
-    ok = val not in filter.values
-    if filter.type == "white":  # 白名单则反过来
+    ok = val not in will_check.values
+    if will_check.type == "white":  # 白名单则反过来
         ok = not ok
     return ok
 
 
-def check_match(match: MatchModel, event: MessageEvent) -> bool:
+def check_match(match: MatchType, event: MessageEvent) -> bool:
+    if isinstance(match, str):
+        match = MatchModel(match=match)
+
     if match.to_me and (not event.is_tome()):
         return False
 
     msg_str = str(event.message)
     msg_plaintext = event.message.extract_plain_text()
     match_template = match.match
 
@@ -66,15 +70,15 @@
         flag = re.I if match.ignore_case else 0
         return bool(
             (re.search(match_template, msg_str, flag))
             or (
                 re.search(match_template, msg_plaintext, flag)
                 if match.allow_plaintext
                 else False
-            )
+            ),
         )
 
     if match.ignore_case:
         # regex 匹配已经处理过了，这边不需要管
         msg_str = msg_str.lower()
         match_template = match_template.lower()
 
@@ -107,18 +111,24 @@
         state["reply"] = random.choice(reply.replies)
         return True
 
     return False
 
 
 def get_reply_msgs(
-    reply: ReplyType, refuse_multi: bool = False
+    reply: ReplyType,
+    refuse_multi: bool = False,
 ) -> Tuple[List[Message], Optional[Tuple[int, int]]]:
     if isinstance(reply, str):
-        reply = ReplyModel(type="normal", message=reply)
+        str_is_plain = reply.startswith("@")
+        if str_is_plain:
+            reply = reply[1:]
+
+        reply = ReplyModel(type="plain" if str_is_plain else "normal", message=reply)
+
     elif isinstance(reply, list):
         reply = ReplyModel(type="array", message=reply)
 
     rt = reply.type
     msg = reply.message
 
     if rt == "plain":
@@ -126,16 +136,16 @@
 
     if rt == "array":
         return [
             Message(
                 [
                     MessageSegment(type=x.type, data=x.data)
                     for x in cast(List[MessageSegmentModel], msg)
-                ]
-            )
+                ],
+            ),
         ], None
 
     if rt == "multi":
         if refuse_multi:
             raise ValueError("Nested `multi` is not allowed")
         return [
             get_reply_msgs(x, True)[0][0] for x in cast(List[ReplyModel], msg)
```

### Comparing `nonebot_plugin_autoreply-0.2.3/nonebot_plugin_autoreply/config.py` & `nonebot_plugin_autoreply-0.2.4/nonebot_plugin_autoreply/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,45 @@
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
 REPLY_JSON_PATH = DATA_PATH / "replies.json"
 if not REPLY_JSON_PATH.exists():
     REPLY_JSON_PATH.write_text("[]", encoding="u8")
 
+MatchType = Union[str, "MatchModel"]
 ReplyType = Union[str, List["MessageSegmentModel"], "ReplyModel"]
 
 
 class MatchModel(BaseModel):
     match: str
-    type: Literal["full", "fuzzy", "regex"] = "fuzzy"
+    type: Literal["full", "fuzzy", "regex"] = "fuzzy"  # noqa: A003
     to_me: bool = False
     ignore_case: bool = True
     strip: bool = True
     allow_plaintext: bool = True
 
 
 class MessageSegmentModel(BaseModel):
-    type: str
+    type: str  # noqa: A003
     data: Dict[str, Any]
 
 
 class ReplyModel(BaseModel):
-    type: Literal["normal", "plain", "array", "multi"]
+    type: Literal["normal", "plain", "array", "multi"]  # noqa: A003
     message: Union[str, List[MessageSegmentModel], List[ReplyType]]
     delay: Tuple[int, int] = (0, 0)
 
 
 class FilterModel(BaseModel, Generic[T]):
-    type: Literal["black", "white"] = "black"
+    type: Literal["black", "white"] = "black"  # noqa: A003
     values: List[T]
 
 
 class ReplyEntryModel(BaseModel):
-    matches: List[MatchModel]
+    matches: List[MatchType]
     replies: List[ReplyType]
     groups: FilterModel[int] = FilterModel(values=[])
     users: FilterModel[int] = FilterModel(values=[])
 
 
 class ConfigModel(BaseModel):
     autoreply_block: bool = False
@@ -61,12 +62,12 @@
 
 def reload_replies():
     replies.clear()
     replies.extend(
         [
             ReplyEntryModel(**x)
             for x in json.loads(REPLY_JSON_PATH.read_text(encoding="u8"))
-        ]
+        ],
     )
 
 
 reload_replies()
```

### Comparing `nonebot_plugin_autoreply-0.2.3/setup.py` & `nonebot_plugin_autoreply-0.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,326 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-autoreply
+Version: 0.2.4
+Summary: A powerful auto reply plugin for NoneBot2
+Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
+Author-Email: student_2333 <lgc2333@126.com>
+License: MIT
+Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-autoreply
+Requires-Python: <4.0,>=3.8
+Requires-Dist: nonebot2>=2.0.0rc1
+Requires-Dist: pydantic>=1.10.4
+Requires-Dist: nonebot-adapter-onebot>=2.1.0
+Requires-Dist: typing-extensions>=4.4.0
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_autoreply']
+<!-- markdownlint-disable MD033 MD036 MD041 -->
 
-package_data = \
-{'': ['*']}
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
 
-install_requires = \
-['nonebot-adapter-onebot>=2.1.0',
- 'nonebot2>=2.0.0rc1',
- 'pydantic>=1.10.4,<2.0.0',
- 'typing-extensions>=4.4.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-autoreply',
-    'version': '0.2.3',
-    'description': 'As the name suggests',
-    'long_description': '<!-- markdownlint-disable MD033 MD036 MD041 -->\n\n<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# NoneBot-Plugin-AutoReply\n\n_✨ 自动回复 ✨_\n\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-autoreply.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot-plugin-autoreply">\n    <img src="https://img.shields.io/pypi/v/nonebot-plugin-autoreply.svg" alt="pypi">\n</a>\n<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n<a href="https://pypi.python.org/pypi/nonebot-plugin-autoreply">\n    <img src="https://img.shields.io/pypi/dm/nonebot-plugin-autoreply" alt="pypi download">\n</a>\n<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/3eb869b8-2edf-46dd-b325-916d9f8a4888">\n  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/3eb869b8-2edf-46dd-b325-916d9f8a4888.svg" alt="wakatime">\n</a>\n</div>\n\n## 📖 介绍\n\n一个简单的关键词自动回复插件，支持 模糊匹配、完全匹配 与 正则匹配，配置文件高度自定义  \n因为商店里没有我想要的那种关键词回复，所以我就自己写了一个  \n这个插件是从 [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/main/src/plugins/shigure_bot/plugins/keyword_reply) 那边拆出来的，我重写了一下做成了单品插件\n\n插件并没有经过深度测试，如果在使用中遇到任何问题请一定一定要过来发 issue 向我汇报，我会尽快解决  \n如果有功能请求也可以直接发 issue 来 dd 我\n\n## 💿 安装\n\n<details open>\n<summary>[推荐] 使用 nb-cli 安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n\n```bash\nnb plugin install nonebot-plugin-autoreply\n```\n\n</details>\n\n<details>\n<summary>使用包管理器安装</summary>\n在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令\n\n<details>\n<summary>pip</summary>\n\n```bash\npip install nonebot-plugin-autoreply\n```\n\n</details>\n<details>\n<summary>pdm</summary>\n\n```bash\npdm add nonebot-plugin-autoreply\n```\n\n</details>\n<details>\n<summary>poetry</summary>\n\n```bash\npoetry add nonebot-plugin-autoreply\n```\n\n</details>\n<details>\n<summary>conda</summary>\n\n```bash\nconda install nonebot-plugin-autoreply\n```\n\n</details>\n\n打开 nonebot2 项目的 `bot.py` 文件, 在其中写入\n\n```py\nnonebot.load_plugin(\'nonebot_plugin_autoreply\')\n```\n\n</details>\n\n## ⚙️ 配置\n\n### 回复配置\n\n插件的配置文件位于 `data/autoreply/replies.json` 下  \n因为把这种东西写在 env 里会太紧凑不易读，所以我单独弄出来了\n\n请根据下面的注释来编辑配置文件，实际配置文件内不要有注释\n\n```jsonc\n[\n  {\n    // 消息的匹配规则，可以放置多个\n    "matches": [\n      {\n        // 用于匹配消息的文本\n        "match": "测试",\n\n        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)\n        // 在正则匹配下，请使用 `\\\\` 在 json 里的正则表达式里表示 `\\`，因为 json 解析时本身就会将 `\\` 作为转义字符\n        // 可以不填，默认为 `fuzzy`\n        "type": "fuzzy",\n\n        // 是否需要 at 机器人才能触发（叫机器人昵称也可以）\n        // 可以不填，默认为 `false`\n        "to_me": false,\n\n        // 是否忽略大小写\n        // 可以不填，默认为 `true`\n        "ignore_case": true,\n\n        // 是否去掉消息前后的空格再匹配\n        // 可以不填，默认为 `true`\n        "strip": true,\n\n        // 当带 cq 码的消息匹配失败时，是否使用去掉 cq 码的消息再匹配一遍\n        // 可以不填，默认为 `true`\n        "allow_plaintext": true\n      }\n\n      // 更多匹配规则...\n    ],\n\n    // 匹配成功后，回复的消息\n    // 如果有多个，将随机抽取一个回复\n    "replies": [\n      // type=normal 时，message 需要为字符串，会解析 message 中的 CQ 码并发送\n      {\n        "type": "normal",\n        "message": "这是一条消息，可以使用CQ码[CQ:image,file=https://pixiv.re/103981177.png]"\n      },\n\n      // 直接写字符串也能表示 type=normal\n      "这是一条消息，可以使用CQ码[CQ:image,file=https://pixiv.re/103981177.png]",\n\n      // type=plain 时，message 需要为字符串，但是 message 中的 CQ 码不会被解析\n      {\n        "type": "plain",\n        "message": "这条消息后面的CQ码会以原样发送[CQ:at,qq=3076823485]"\n      },\n\n      // type=array 时，message 中需要填 CQ 码的 json 格式\n      {\n        "type": "array",\n        "message": [\n          {\n            "type": "text",\n            "data": {\n              "text": "我后面带了一张图片哦"\n            }\n          },\n          {\n            "type": "image",\n            "data": {\n              "file": "https://pixiv.re/103981177.png"\n            }\n          }\n        ]\n      },\n\n      // 直接写数组也能代表 type=array\n      [\n        {\n          "type": "text",\n          "data": {\n            "text": "我可以正常发送哦"\n          }\n        }\n      ],\n\n      // type=multi 时，message 需要为上面提到的消息类型的数组\n      // 会按顺序发送 message 中的所有内容\n      // message 中不允许嵌套其他的 type=multi 类型的回复\n      {\n        "type": "multi",\n        // delay 是每条消息发送成功后的延时，格式为 [最低延时, 最高延时]\n        // 单位为毫秒（1000 毫秒 = 1 秒），可以不填，默认为 [0, 0]\n        "delay": [1000, 1000],\n        "message": [\n          "hello! 一会给你发张图哦~",\n          "[CQ:image,file=https://pixiv.re/103981177.png]一会给你分享首歌哦awa~",\n          [\n            {\n              "type": "music",\n              "data": {\n                "type": "163",\n                "id": "2008994667"\n              }\n            }\n          ]\n        ]\n      }\n\n      // 更多消息...\n    ],\n\n    // 过滤指定群聊\n    // 可以不填，默认为空的黑名单\n    "groups": {\n      // 黑名单类型，可选 `black`(黑名单)、`white`(白名单)\n      "type": "black",\n\n      // 要过滤的群号\n      "values": [\n        123456789, 987654321\n        // 更多群号...\n      ]\n    },\n\n    // 过滤指定用户\n    // 可以不填，默认为空的黑名单\n    "users": {\n      // 黑名单类型，可选 `black`(黑名单)、`white`(白名单)\n      "type": "black",\n\n      // 要过滤的QQ号\n      "values": [\n        1145141919, 9191415411\n        // 更多QQ号...\n      ]\n    }\n  }\n\n  // ...\n]\n```\n\n### 常规配置\n\n下方的配置皆为可选，如果不需要可以忽略不配置  \n配置项请参考下面的文本\n\n```ini\n# matcher 是否阻断消息，默认 False\nAUTOREPLY_BLOCK=False\n\n# matcher 优先级\nAUTOREPLY_PRIORITY=99\n```\n\n## 💬 指令\n\n### `重载自动回复`\n\n此命令用于重载自动回复配置，仅 `SUPERUSER` 可以执行\n\n## 📞 联系\n\nQQ：3076823485  \nTelegram：[@lgc2333](https://t.me/lgc2333)  \n吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  \n邮箱：<lgc2333@126.com>\n\n## 💰 赞助\n\n感谢大家的赞助！你们的赞助将是我继续创作的动力！\n\n- [爱发电](https://afdian.net/@lgc2333)\n- <details>\n    <summary>赞助二维码（点击展开）</summary>\n\n  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)\n\n  </details>\n\n## 📝 更新日志\n\n### 0.2.3\n\n- 修复一处 py 3.8 无法使用的类型注解\n\n### 0.2.2\n\n- 修复群聊和用户过滤器无法正常使用的问题\n\n### 0.2.1\n\n- 修复多 `match` 无法使用的问题\n\n### 0.2.0\n\n- 使用 `rule` 匹配消息，避免日志刷屏\n- 支持一次回复多条消息，调整配置文件结构\n- 增加了两个 `.env` 配置项\n- 增加热重载配置文件的指令\n',
-    'author': 'lgc2333',
-    'author_email': 'lgc2333@126.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+<div align="center">
 
+# NoneBot-Plugin-AutoReply
 
-setup(**setup_kwargs)
+_✨ 自动回复 ✨_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/lgc2333/nonebot-plugin-autoreply.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-autoreply">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-autoreply.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+<a href="https://pypi.python.org/pypi/nonebot-plugin-autoreply">
+    <img src="https://img.shields.io/pypi/dm/nonebot-plugin-autoreply" alt="pypi download">
+</a>
+<a href="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/3eb869b8-2edf-46dd-b325-916d9f8a4888">
+  <img src="https://wakatime.com/badge/user/b61b0f9a-f40b-4c82-bc51-0a75c67bfccf/project/3eb869b8-2edf-46dd-b325-916d9f8a4888.svg" alt="wakatime">
+</a>
+</div>
+
+## 📖 介绍
+
+一个简单的关键词自动回复插件，支持 模糊匹配、完全匹配 与 正则匹配，配置文件高度自定义  
+因为商店里没有我想要的那种关键词回复，所以我就自己写了一个  
+这个插件是从 [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/main/src/plugins/shigure_bot/plugins/keyword_reply) 那边拆出来的，我重写了一下做成了单品插件
+
+插件并没有经过深度测试，如果在使用中遇到任何问题请一定一定要过来发 issue 向我汇报，我会尽快解决  
+如果有功能请求也可以直接发 issue 来 dd 我
+
+## 💿 安装
+
+<details open>
+<summary>[推荐] 使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+```bash
+nb plugin install nonebot-plugin-autoreply
+```
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+```bash
+pip install nonebot-plugin-autoreply
+```
+
+</details>
+<details>
+<summary>pdm</summary>
+
+```bash
+pdm add nonebot-plugin-autoreply
+```
+
+</details>
+<details>
+<summary>poetry</summary>
+
+```bash
+poetry add nonebot-plugin-autoreply
+```
+
+</details>
+<details>
+<summary>conda</summary>
+
+```bash
+conda install nonebot-plugin-autoreply
+```
+
+</details>
+
+打开 nonebot2 项目的 `bot.py` 文件, 在其中写入
+
+```py
+nonebot.load_plugin('nonebot_plugin_autoreply')
+```
+
+</details>
+
+## ⚙️ 配置
+
+### 回复配置
+
+插件的配置文件位于 `data/autoreply/replies.json` 下  
+因为把这种东西写在 env 里会太紧凑不易读，所以我单独弄出来了
+
+请根据下面的注释来编辑配置文件，实际配置文件内不要有注释
+
+```jsonc
+[
+  {
+    // 消息的匹配规则，可以放置多个
+    "matches": [
+      {
+        // 用于匹配消息的文本
+        "match": "测试",
+
+        // 匹配模式，可选 `full`(完全匹配)、`fuzzy`(模糊匹配)、`regex`(正则匹配)
+        // 在正则匹配下，请使用 `\\` 在 json 里的正则表达式里表示 `\`，因为 json 解析时本身就会将 `\` 作为转义字符
+        // 可以不填，默认为 `fuzzy`
+        "type": "fuzzy",
+
+        // 是否需要 at 机器人才能触发（叫机器人昵称也可以）
+        // 可以不填，默认为 `false`
+        "to_me": false,
+
+        // 是否忽略大小写
+        // 可以不填，默认为 `true`
+        "ignore_case": true,
+
+        // 是否去掉消息前后的空格再匹配
+        // 可以不填，默认为 `true`
+        "strip": true,
+
+        // 当带 cq 码的消息匹配失败时，是否使用去掉 cq 码的消息再匹配一遍
+        // 可以不填，默认为 `true`
+        "allow_plaintext": true
+      },
+
+      // 如果规则为一个字符串，则会转换为一个属性全部默认的 `match` 来匹配
+      "测试2"
+
+      // 更多匹配规则...
+    ],
+
+    // 匹配成功后，回复的消息
+    // 如果有多个，将随机抽取一个回复
+    "replies": [
+      // type=normal 时，message 需要为字符串，会解析 message 中的 CQ 码并发送
+      {
+        "type": "normal",
+        "message": "这是一条消息，可以使用CQ码[CQ:image,file=https://pixiv.re/103981177.png]"
+      },
+
+      // 直接写字符串也能表示 type=normal
+      "这是一条消息，可以使用CQ码[CQ:image,file=https://pixiv.re/103981177.png]",
+
+      // type=plain 时，message 需要为字符串，但是 message 中的 CQ 码不会被解析
+      {
+        "type": "plain",
+        "message": "这条消息后面的CQ码会以原样发送[CQ:at,qq=3076823485]"
+      },
+
+      // 直接写 @ 开头的字符串也能表示 type=plain
+      "@这条消息后面的CQ码也会以原样发送[CQ:at,qq=3076823485]",
+
+      // type=array 时，message 中需要填 CQ 码的 json 格式
+      {
+        "type": "array",
+        "message": [
+          {
+            "type": "text",
+            "data": {
+              "text": "我后面带了一张图片哦"
+            }
+          },
+          {
+            "type": "image",
+            "data": {
+              "file": "https://pixiv.re/103981177.png"
+            }
+          }
+        ]
+      },
+
+      // 直接写数组也能代表 type=array
+      [
+        {
+          "type": "text",
+          "data": {
+            "text": "我可以正常发送哦"
+          }
+        }
+      ],
+
+      // type=multi 时，message 需要为上面提到的消息类型的数组
+      // 会按顺序发送 message 中的所有内容
+      // message 中不允许嵌套其他的 type=multi 类型的回复
+      {
+        "type": "multi",
+        // delay 是每条消息发送成功后的延时，格式为 [最低延时, 最高延时]
+        // 单位为毫秒（1000 毫秒 = 1 秒），可以不填，默认为 [0, 0]
+        "delay": [1000, 1000],
+        "message": [
+          "hello! 一会给你发张图哦~",
+          "[CQ:image,file=https://pixiv.re/103981177.png]一会给你分享首歌哦awa~",
+          [
+            {
+              "type": "music",
+              "data": {
+                "type": "163",
+                "id": "2008994667"
+              }
+            }
+          ]
+        ]
+      }
+
+      // 更多消息...
+    ],
+
+    // 过滤指定群聊
+    // 可以不填，默认为空的黑名单
+    "groups": {
+      // 黑名单类型，可选 `black`(黑名单)、`white`(白名单)
+      "type": "black",
+
+      // 要过滤的群号
+      "values": [
+        123456789, 987654321
+        // 更多群号...
+      ]
+    },
+
+    // 过滤指定用户
+    // 可以不填，默认为空的黑名单
+    "users": {
+      // 黑名单类型，可选 `black`(黑名单)、`white`(白名单)
+      "type": "black",
+
+      // 要过滤的QQ号
+      "values": [
+        1145141919, 9191415411
+        // 更多QQ号...
+      ]
+    }
+  }
+
+  // ...
+]
+```
+
+### 常规配置
+
+下方的配置皆为可选，如果不需要可以忽略不配置  
+配置项请参考下面的文本
+
+```ini
+# matcher 是否阻断消息，默认 False
+AUTOREPLY_BLOCK=False
+
+# matcher 优先级
+AUTOREPLY_PRIORITY=99
+```
+
+## 💬 指令
+
+### `重载自动回复`
+
+此命令用于重载自动回复配置，仅 `SUPERUSER` 可以执行
+
+## 📞 联系
+
+QQ：3076823485  
+Telegram：[@lgc2333](https://t.me/lgc2333)  
+吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
+邮箱：<lgc2333@126.com>
+
+## 💰 赞助
+
+感谢大家的赞助！你们的赞助将是我继续创作的动力！
+
+- [爱发电](https://afdian.net/@lgc2333)
+- <details>
+    <summary>赞助二维码（点击展开）</summary>
+
+  ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
+
+  </details>
+
+## 📝 更新日志
+
+### 0.2.4
+
+- 让字符串可以作为默认属性的 `match` 使用
+- 让 `@` 开头的字符串 `reply` 解析为 `plain` 形式的回复
+
+### 0.2.3
+
+- 修复一处 py 3.8 无法使用的类型注解
+
+### 0.2.2
+
+- 修复群聊和用户过滤器无法正常使用的问题
+
+### 0.2.1
+
+- 修复多 `match` 无法使用的问题
+
+### 0.2.0
+
+- 使用 `rule` 匹配消息，避免日志刷屏
+- 支持一次回复多条消息，调整配置文件结构
+- 增加了两个 `.env` 配置项
+- 增加热重载配置文件的指令
```

#### html2text {}

```diff
@@ -1,108 +1,103 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_autoreply'] package_data = \ {'': ['*']} install_requires = \
-['nonebot-adapter-onebot>=2.1.0', 'nonebot2>=2.0.0rc1',
-'pydantic>=1.10.4,<2.0.0', 'typing-extensions>=4.4.0,<5.0.0'] setup_kwargs =
-{ 'name': 'nonebot-plugin-autoreply', 'version': '0.2.3', 'description': 'As
-the name suggests', 'long_description': '\n\n
-                           \n [NoneBotPluginLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-autoreply Version: 0.2.4 Summary: A
+powerful auto reply plugin for NoneBot2 Home-page: https://github.com/lgc-
+NB2Dev/nonebot-plugin-autoreply Author-Email: student_2333
+126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
+nonebot-plugin-autoreply Requires-Python: <4.0,>=3.8 Requires-Dist:
+nonebot2>=2.0.0rc1 Requires-Dist: pydantic>=1.10.4 Requires-Dist: nonebot-
+adapter-onebot>=2.1.0 Requires-Dist: typing-extensions>=4.4.0 Description-
+Content-Type: text/markdown
+                             [NoneBotPluginLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-\n\n# NoneBot-Plugin-AutoReply\n\n_â¨ èªå¨åå¤ â¨_\n\n\n_[license]\n\n\n_
-          [pypi]\n\n[python]\n\n_[pypi_download]\n\n\n_[wakatime]\n\n
-\n\n## ð ä»ç»\n\nä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
+ # NoneBot-Plugin-AutoReply _â¨ èªå¨åå¤ â¨_ [license] [pypi] [python]
+                          [pypi_download] [wakatime]
+## ð ä»ç» ä¸ä¸ªç®åçå³é®è¯èªå¨åå¤æä»¶ï¼æ¯æ
 æ¨¡ç³å¹éãå®å¨å¹é ä¸ æ­£åå¹éï¼éç½®æä»¶é«åº¦èªå®ä¹
-\nå ä¸ºååºéæ²¡æææ³è¦çé£ç§å³é®è¯åå¤ï¼æä»¥æå°±èªå·±åäºä¸ä¸ª
-\nè¿ä¸ªæä»¶æ¯ä» [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/
+å ä¸ºååºéæ²¡æææ³è¦çé£ç§å³é®è¯åå¤ï¼æä»¥æå°±èªå·±åäºä¸ä¸ª
+è¿ä¸ªæä»¶æ¯ä» [ShigureBot](https://github.com/lgc2333/ShigureBot/tree/
 main/src/plugins/shigure_bot/plugins/keyword_reply)
-é£è¾¹æåºæ¥çï¼æéåäºä¸ä¸åæäºååæä»¶\n\næä»¶å¹¶æ²¡æç»è¿æ·±åº¦æµè¯ï¼å¦æå¨ä½¿ç¨ä¸­éå°ä»»ä½é®é¢è¯·ä¸å®ä¸å®è¦è¿æ¥å
-issue åææ±æ¥ï¼æä¼å°½å¿«è§£å³
-\nå¦ææåè½è¯·æ±ä¹å¯ä»¥ç´æ¥å issue æ¥ dd æ\n\n## ð¿
-å®è£\n\n\n[æ¨è] ä½¿ç¨ nb-cli å®è£\nå¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£\n\n```bash\nnb plugin install nonebot-plugin-
-autoreply\n```\n\n\n\n\nä½¿ç¨åç®¡çå¨å®è£\nå¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤\n\n\npip\n\n```bash\npip install nonebot-plugin-
-autoreply\n```\n\n\n\npdm\n\n```bash\npdm add nonebot-plugin-
-autoreply\n```\n\n\n\npoetry\n\n```bash\npoetry add nonebot-plugin-
-autoreply\n```\n\n\n\nconda\n\n```bash\nconda install nonebot-plugin-
-autoreply\n```\n\n\n\næå¼ nonebot2 é¡¹ç®ç `bot.py` æä»¶,
-å¨å¶ä¸­åå¥\n\n```py\nnonebot.load_plugin
-(\'nonebot_plugin_autoreply\')\n```\n\n\n\n## âï¸ éç½®\n\n###
-åå¤éç½®\n\næä»¶çéç½®æä»¶ä½äº `data/autoreply/replies.json` ä¸
-\nå ä¸ºæè¿ç§ä¸è¥¿åå¨ env
-éä¼å¤ªç´§åä¸æè¯»ï¼æä»¥æåç¬å¼åºæ¥äº\n\nè¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é\n\n```jsonc\n
-[\n {\n // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª\n "matches": [\n {\n /
-/ ç¨äºå¹éæ¶æ¯çææ¬\n "match": "æµè¯",\n\n // å¹éæ¨¡å¼ï¼å¯é
-`full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é)\n /
-/ å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
-`\\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\\` ä½ä¸ºè½¬ä¹å­ç¬¦\n /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy`\n "type": "fuzzy",\n\n // æ¯å¦éè¦ at
-æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼\n /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `false`\n "to_me": false,\n\n /
-/ æ¯å¦å¿½ç¥å¤§å°å\n // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`\n "ignore_case":
-true,\n\n // æ¯å¦å»ææ¶æ¯ååçç©ºæ ¼åå¹é\n /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`\n "strip": true,\n\n // å½å¸¦ cq
-ç çæ¶æ¯å¹éå¤±è´¥æ¶ï¼æ¯å¦ä½¿ç¨å»æ cq
-ç çæ¶æ¯åå¹éä¸é\n // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`\n
-"allow_plaintext": true\n }\n\n // æ´å¤å¹éè§å...\n ],\n\n /
-/ å¹éæååï¼åå¤çæ¶æ¯\n /
-/ å¦ææå¤ä¸ªï¼å°éæºæ½åä¸ä¸ªåå¤\n "replies": [\n // type=normal
-æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä¼è§£æ message ä¸­ç CQ ç å¹¶åé\n
-{\n "type": "normal",\n "message": "è¿æ¯ä¸æ¡æ¶æ¯ï¼å¯ä»¥ä½¿ç¨CQç [CQ:
-image,file=https://pixiv.re/103981177.png]"\n },\n\n /
-/ ç´æ¥åå­ç¬¦ä¸²ä¹è½è¡¨ç¤º type=normal\n
+é£è¾¹æåºæ¥çï¼æéåäºä¸ä¸åæäºååæä»¶
+æä»¶å¹¶æ²¡æç»è¿æ·±åº¦æµè¯ï¼å¦æå¨ä½¿ç¨ä¸­éå°ä»»ä½é®é¢è¯·ä¸å®ä¸å®è¦è¿æ¥å
+issue åææ±æ¥ï¼æä¼å°½å¿«è§£å³ å¦ææåè½è¯·æ±ä¹å¯ä»¥ç´æ¥å
+issue æ¥ dd æ ## ð¿ å®è£  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
+plugin install nonebot-plugin-autoreply ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
+install nonebot-plugin-autoreply ```   pdm ```bash pdm add nonebot-plugin-
+autoreply ```   poetry ```bash poetry add nonebot-plugin-autoreply ```   conda
+```bash conda install nonebot-plugin-autoreply ```  æå¼ nonebot2 é¡¹ç®ç
+`bot.py` æä»¶, å¨å¶ä¸­åå¥ ```py nonebot.load_plugin
+('nonebot_plugin_autoreply') ```  ## âï¸ éç½® ### åå¤éç½®
+æä»¶çéç½®æä»¶ä½äº `data/autoreply/replies.json` ä¸
+å ä¸ºæè¿ç§ä¸è¥¿åå¨ env
+éä¼å¤ªç´§åä¸æè¯»ï¼æä»¥æåç¬å¼åºæ¥äº
+è¯·æ ¹æ®ä¸é¢çæ³¨éæ¥ç¼è¾éç½®æä»¶ï¼å®ééç½®æä»¶åä¸è¦ææ³¨é
+```jsonc [ { // æ¶æ¯çå¹éè§åï¼å¯ä»¥æ¾ç½®å¤ä¸ª "matches": [ { /
+/ ç¨äºå¹éæ¶æ¯çææ¬ "match": "æµè¯", // å¹éæ¨¡å¼ï¼å¯é
+`full`(å®å¨å¹é)ã`fuzzy`(æ¨¡ç³å¹é)ã`regex`(æ­£åå¹é) /
+/ å¨æ­£åå¹éä¸ï¼è¯·ä½¿ç¨ `\\` å¨ json éçæ­£åè¡¨è¾¾å¼éè¡¨ç¤º
+`\`ï¼å ä¸º json è§£ææ¶æ¬èº«å°±ä¼å° `\` ä½ä¸ºè½¬ä¹å­ç¬¦ /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `fuzzy` "type": "fuzzy", // æ¯å¦éè¦ at
+æºå¨äººæè½è§¦åï¼å«æºå¨äººæµç§°ä¹å¯ä»¥ï¼ /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `false` "to_me": false, // æ¯å¦å¿½ç¥å¤§å°å /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true` "ignore_case": true, /
+/ æ¯å¦å»ææ¶æ¯ååçç©ºæ ¼åå¹é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
+"strip": true, // å½å¸¦ cq ç çæ¶æ¯å¹éå¤±è´¥æ¶ï¼æ¯å¦ä½¿ç¨å»æ cq
+ç çæ¶æ¯åå¹éä¸é // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º `true`
+"allow_plaintext": true }, /
+/ å¦æè§åä¸ºä¸ä¸ªå­ç¬¦ä¸²ï¼åä¼è½¬æ¢ä¸ºä¸ä¸ªå±æ§å¨é¨é»è®¤ç
+`match` æ¥å¹é "æµè¯2" // æ´å¤å¹éè§å... ], /
+/ å¹éæååï¼åå¤çæ¶æ¯ /
+/ å¦ææå¤ä¸ªï¼å°éæºæ½åä¸ä¸ªåå¤ "replies": [ // type=normal
+æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä¼è§£æ message ä¸­ç CQ ç å¹¶åé
+{ "type": "normal", "message": "è¿æ¯ä¸æ¡æ¶æ¯ï¼å¯ä»¥ä½¿ç¨CQç [CQ:
+image,file=https://pixiv.re/103981177.png]" }, /
+/ ç´æ¥åå­ç¬¦ä¸²ä¹è½è¡¨ç¤º type=normal
 "è¿æ¯ä¸æ¡æ¶æ¯ï¼å¯ä»¥ä½¿ç¨CQç [CQ:image,file=https://pixiv.re/
-103981177.png]",\n\n // type=plain æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä½æ¯
-message ä¸­ç CQ ç ä¸ä¼è¢«è§£æ\n {\n "type": "plain",\n "message":
-"è¿æ¡æ¶æ¯åé¢çCQç ä¼ä»¥åæ ·åé[CQ:at,qq=3076823485]"\n },\n\n /
-/ type=array æ¶ï¼message ä¸­éè¦å¡« CQ ç ç json æ ¼å¼\n {\n "type":
-"array",\n "message": [\n {\n "type": "text",\n "data": {\n "text":
-"æåé¢å¸¦äºä¸å¼ å¾çå¦"\n }\n },\n {\n "type": "image",\n "data": {\n
-"file": "https://pixiv.re/103981177.png"\n }\n }\n ]\n },\n\n /
-/ ç´æ¥åæ°ç»ä¹è½ä»£è¡¨ type=array\n [\n {\n "type": "text",\n "data":
-{\n "text": "æå¯ä»¥æ­£å¸¸åéå¦"\n }\n }\n ],\n\n // type=multi
-æ¶ï¼message éè¦ä¸ºä¸é¢æå°çæ¶æ¯ç±»åçæ°ç»\n /
-/ ä¼æé¡ºåºåé message ä¸­çææåå®¹\n // message
-ä¸­ä¸åè®¸åµå¥å¶ä»ç type=multi ç±»åçåå¤\n {\n "type": "multi",\n
-// delay æ¯æ¯æ¡æ¶æ¯åéæååçå»¶æ¶ï¼æ ¼å¼ä¸º [æä½å»¶æ¶,
-æé«å»¶æ¶]\n // åä½ä¸ºæ¯«ç§ï¼1000 æ¯«ç§ = 1
-ç§ï¼ï¼å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º [0, 0]\n "delay": [1000, 1000],\n "message":
-[\n "hello! ä¸ä¼ç»ä½ åå¼ å¾å¦~",\n "[CQ:image,file=https://pixiv.re/
-103981177.png]ä¸ä¼ç»ä½ åäº«é¦æ­å¦awa~",\n [\n {\n "type": "music",\n
-"data": {\n "type": "163",\n "id": "2008994667"\n }\n }\n ]\n ]\n }\n\n /
-/ æ´å¤æ¶æ¯...\n ],\n\n // è¿æ»¤æå®ç¾¤è\n /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå\n "groups": {\n /
-/ é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå)\n "type":
-"black",\n\n // è¦è¿æ»¤çç¾¤å·\n "values": [\n 123456789, 987654321\n /
-/ æ´å¤ç¾¤å·...\n ]\n },\n\n // è¿æ»¤æå®ç¨æ·\n /
-/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå\n "users": {\n /
-/ é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå)\n "type":
-"black",\n\n // è¦è¿æ»¤çQQå·\n "values": [\n 1145141919, 9191415411\n /
-/ æ´å¤QQå·...\n ]\n }\n }\n\n // ...\n]\n```\n\n###
-å¸¸è§éç½®\n\nä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
-\néç½®é¡¹è¯·åèä¸é¢çææ¬\n\n```ini\n# matcher
-æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤ False\nAUTOREPLY_BLOCK=False\n\n# matcher
-ä¼åçº§\nAUTOREPLY_PRIORITY=99\n```\n\n## ð¬ æä»¤\n\n###
-`éè½½èªå¨åå¤`\n\næ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä»
-`SUPERUSER` å¯ä»¥æ§è¡\n\n## ð èç³»\n\nQQï¼3076823485 \nTelegramï¼
-[@lgc2333](https://t.me/lgc2333) \nå¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
-?_wv=1027&k=Z3n1MpEp) \né®ç®±ï¼
-126.com>\n\n## ð°
-èµå©\n\næè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼\n\n-
-[ç±åçµ](https://afdian.net/@lgc2333)\n- \n
-èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼\n\n ![è®¨é¥­](https://
-raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/
-sponsor.png)\n\n \n\n## ð æ´æ°æ¥å¿\n\n### 0.2.3\n\n- ä¿®å¤ä¸å¤ py 3.8
-æ æ³ä½¿ç¨çç±»åæ³¨è§£\n\n### 0.2.2\n\n-
-ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢\n\n### 0.2.1\n\n-
-ä¿®å¤å¤ `match` æ æ³ä½¿ç¨çé®é¢\n\n### 0.2.0\n\n- ä½¿ç¨ `rule`
-å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å±\n-
-æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ\n- å¢å äºä¸¤ä¸ª
-`.env` éç½®é¡¹\n- å¢å ç­éè½½éç½®æä»¶çæä»¤\n', 'author':
-'lgc2333', 'author_email': 'lgc2333@126.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+103981177.png]", // type=plain æ¶ï¼message éè¦ä¸ºå­ç¬¦ä¸²ï¼ä½æ¯
+message ä¸­ç CQ ç ä¸ä¼è¢«è§£æ { "type": "plain", "message":
+"è¿æ¡æ¶æ¯åé¢çCQç ä¼ä»¥åæ ·åé[CQ:at,qq=3076823485]" }, /
+/ ç´æ¥å @ å¼å¤´çå­ç¬¦ä¸²ä¹è½è¡¨ç¤º type=plain
+"@è¿æ¡æ¶æ¯åé¢çCQç ä¹ä¼ä»¥åæ ·åé[CQ:at,qq=3076823485]", /
+/ type=array æ¶ï¼message ä¸­éè¦å¡« CQ ç ç json æ ¼å¼ { "type":
+"array", "message": [ { "type": "text", "data": { "text":
+"æåé¢å¸¦äºä¸å¼ å¾çå¦" } }, { "type": "image", "data": { "file":
+"https://pixiv.re/103981177.png" } } ] }, // ç´æ¥åæ°ç»ä¹è½ä»£è¡¨
+type=array [ { "type": "text", "data": { "text": "æå¯ä»¥æ­£å¸¸åéå¦" } }
+], // type=multi æ¶ï¼message éè¦ä¸ºä¸é¢æå°çæ¶æ¯ç±»åçæ°ç» /
+/ ä¼æé¡ºåºåé message ä¸­çææåå®¹ // message
+ä¸­ä¸åè®¸åµå¥å¶ä»ç type=multi ç±»åçåå¤ { "type": "multi", /
+/ delay æ¯æ¯æ¡æ¶æ¯åéæååçå»¶æ¶ï¼æ ¼å¼ä¸º [æä½å»¶æ¶,
+æé«å»¶æ¶] // åä½ä¸ºæ¯«ç§ï¼1000 æ¯«ç§ = 1
+ç§ï¼ï¼å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸º [0, 0] "delay": [1000, 1000], "message":
+[ "hello! ä¸ä¼ç»ä½ åå¼ å¾å¦~", "[CQ:image,file=https://pixiv.re/
+103981177.png]ä¸ä¼ç»ä½ åäº«é¦æ­å¦awa~", [ { "type": "music", "data":
+{ "type": "163", "id": "2008994667" } } ] ] } // æ´å¤æ¶æ¯... ], /
+/ è¿æ»¤æå®ç¾¤è // å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå "groups": { /
+/ é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå) "type":
+"black", // è¦è¿æ»¤çç¾¤å· "values": [ 123456789, 987654321 /
+/ æ´å¤ç¾¤å·... ] }, // è¿æ»¤æå®ç¨æ· /
+/ å¯ä»¥ä¸å¡«ï¼é»è®¤ä¸ºç©ºçé»åå "users": { /
+/ é»ååç±»åï¼å¯é `black`(é»åå)ã`white`(ç½åå) "type":
+"black", // è¦è¿æ»¤çQQå· "values": [ 1145141919, 9191415411 /
+/ æ´å¤QQå·... ] } } // ... ] ``` ### å¸¸è§éç½®
+ä¸æ¹çéç½®çä¸ºå¯éï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ä¸éç½®
+éç½®é¡¹è¯·åèä¸é¢çææ¬ ```ini # matcher æ¯å¦é»æ­æ¶æ¯ï¼é»è®¤
+False AUTOREPLY_BLOCK=False # matcher ä¼åçº§ AUTOREPLY_PRIORITY=99 ``` ##
+ð¬ æä»¤ ### `éè½½èªå¨åå¤`
+æ­¤å½ä»¤ç¨äºéè½½èªå¨åå¤éç½®ï¼ä» `SUPERUSER` å¯ä»¥æ§è¡ ## ð
+èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
+[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+126.com> ## ð° èµå©
+æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
+[ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
+[è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.4 -
+è®©å­ç¬¦ä¸²å¯ä»¥ä½ä¸ºé»è®¤å±æ§ç `match` ä½¿ç¨ - è®© `@`
+å¼å¤´çå­ç¬¦ä¸² `reply` è§£æä¸º `plain` å½¢å¼çåå¤ ### 0.2.3 -
+ä¿®å¤ä¸å¤ py 3.8 æ æ³ä½¿ç¨çç±»åæ³¨è§£ ### 0.2.2 -
+ä¿®å¤ç¾¤èåç¨æ·è¿æ»¤å¨æ æ³æ­£å¸¸ä½¿ç¨çé®é¢ ### 0.2.1 - ä¿®å¤å¤
+`match` æ æ³ä½¿ç¨çé®é¢ ### 0.2.0 - ä½¿ç¨ `rule`
+å¹éæ¶æ¯ï¼é¿åæ¥å¿å·å± -
+æ¯æä¸æ¬¡åå¤å¤æ¡æ¶æ¯ï¼è°æ´éç½®æä»¶ç»æ - å¢å äºä¸¤ä¸ª
+`.env` éç½®é¡¹ - å¢å ç­éè½½éç½®æä»¶çæä»¤
```

