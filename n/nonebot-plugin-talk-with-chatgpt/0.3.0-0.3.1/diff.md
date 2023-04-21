# Comparing `tmp/nonebot_plugin_talk_with_chatgpt-0.3.0.tar.gz` & `tmp/nonebot_plugin_talk_with_chatgpt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_chatgpt-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0.tar` & `nonebot_plugin_talk_with_chatgpt-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8970 2023-04-21 07:17:21.517655 nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/__init__.py
--rw-r--r--   0        0        0    13442 2023-04-21 07:36:47.249360 nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/config.py
--rw-r--r--   0        0        0     4946 2023-04-21 07:14:40.011533 nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/data_handle.py
--rw-r--r--   0        0        0      974 2023-04-21 07:24:15.055493 nonebot_plugin_talk_with_chatgpt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4605 2023-04-21 07:40:03.876185 nonebot_plugin_talk_with_chatgpt-0.3.0/README.md
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     8970 2023-04-21 07:17:21.517655 nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/__init__.py
+-rw-r--r--   0        0        0    13442 2023-04-21 07:36:47.249360 nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/config.py
+-rw-r--r--   0        0        0     4946 2023-04-21 07:14:40.011533 nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/data_handle.py
+-rw-r--r--   0        0        0      974 2023-04-21 07:40:45.667009 nonebot_plugin_talk_with_chatgpt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4605 2023-04-21 07:40:42.743256 nonebot_plugin_talk_with_chatgpt-0.3.1/README.md
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_chatgpt-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/__init__.py` & `nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/config.py` & `nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/nonebot_plugin_talk_with_chatgpt/data_handle.py` & `nonebot_plugin_talk_with_chatgpt-0.3.1/nonebot_plugin_talk_with_chatgpt/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/pyproject.toml` & `nonebot_plugin_talk_with_chatgpt-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_chatgpt"
-version = "0.3.0"
+version = "0.3.1"
 description = "Nonebot2 基于accessToken登录的ChatGPT聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_chatgpt"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt"
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/README.md` & `nonebot_plugin_talk_with_chatgpt-0.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/21 \[v0.3.0]
+### 2023/4/21 \[v0.3.1]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
 
 ### 2023/4/11 \[v0.2.3]
```

#### html2text {}

```diff
@@ -48,12 +48,12 @@
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/21 \[v0.3.0] *
+4/21 \[v0.3.1] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

### Comparing `nonebot_plugin_talk_with_chatgpt-0.3.0/PKG-INFO` & `nonebot_plugin_talk_with_chatgpt-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-chatgpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: Nonebot2 基于accessToken登录的ChatGPT聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_chatgpt
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -119,15 +119,15 @@
 |:-----:|:----:|
 | /talk | 开始对话，群里@机器人也可以 |
 | /hi | 沉浸式对话（仅限私聊） |
 | /clear | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 
 ## 更新日志
-### 2023/4/21 \[v0.3.0]
+### 2023/4/21 \[v0.3.1]
 
 * 更换了默认API，暂时能用，建议还是自己搭建API
 * 新增多预设功能，内置三个预设：猫娘、魅魔、开发者模式
 * 增加私聊沉浸式对话
 * 优化大量细节
 
 ### 2023/4/11 \[v0.2.3]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.3.0
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-chatgpt Version: 0.3.1
 Summary: Nonebot2 åºäºaccessTokenç»å½çChatGPTèå¤©æä»¶ Home-page:
 https://github.com/nikissXI/nonebot_plugins/tree/main/
 nonebot_plugin_talk_with_chatgpt License: MIT Author: nikissXI Author-email:
 1299577815@qq.com Requires-Python: >=3.8 Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -63,12 +63,12 @@
 æä»¶æ°æ®æä»¶åï¼é»è®¤./data/talk_with_chatgpt.json
 talk_with_chatgpt_data = talk_with_chatgpt.json ``` ##
 æä»¶å½ä»¤ï¼åå¯ä¿®æ¹ï¼ï¼ | æä»¤ | è¯´æ | |:-----:|:----:| | /talk
 | å¼å§å¯¹è¯ï¼ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /clear |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | ## æ´æ°æ¥å¿ ### 2023/
-4/21 \[v0.3.0] *
+4/21 \[v0.3.1] *
 æ´æ¢äºé»è®¤APIï¼ææ¶è½ç¨ï¼å»ºè®®è¿æ¯èªå·±æ­å»ºAPI *
 æ°å¢å¤é¢è®¾åè½ï¼åç½®ä¸ä¸ªé¢è®¾ï¼ç«å¨ãé­é­ãå¼åèæ¨¡å¼
 * å¢å ç§èæ²æµ¸å¼å¯¹è¯ * ä¼åå¤§éç»è ### 2023/4/11 \[v0.2.3] *
 åå¸ç¬¬ä¸çè¾ç®éçæä»¶ï¼å¹¶ä¿®å¤äºäºå°é®é¢ï¼ç»èå¾éè¦
```

