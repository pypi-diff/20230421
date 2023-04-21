# Comparing `tmp/nonebot_plugin_rename-1.0.3.tar.gz` & `tmp/nonebot_plugin_rename-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_rename-1.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_rename-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_rename-1.0.3.tar` & `nonebot_plugin_rename-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1066 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/LICENSE
--rw-r--r--   0        0        0     4789 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/README.md
--rw-r--r--   0        0        0      363 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/__init__.py
--rw-r--r--   0        0        0      244 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/__init__.py
--rw-r--r--   0        0        0      789 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/gaokao_time.py
--rw-r--r--   0        0        0      885 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/genshin_time.py
--rw-r--r--   0        0        0      689 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/get_times.py
--rw-r--r--   0        0        0      925 2023-04-20 17:50:09.853582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/hot_search.py
--rw-r--r--   0        0        0      408 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/message.py
--rw-r--r--   0        0        0      466 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/one_word.py
--rw-r--r--   0        0        0      603 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/status.py
--rw-r--r--   0        0        0      252 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/config.py
--rw-r--r--   0        0        0     7117 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/main.py
--rw-r--r--   0        0        0      151 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/__init__.py
--rw-r--r--   0        0        0      478 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/card_choice.py
--rw-r--r--   0        0        0      867 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/card_name.py
--rw-r--r--   0        0        0     1407 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/draw.py
--rw-r--r--   0        0        0      423 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/my_yaml.py
--rw-r--r--   0        0        0      644 2023-04-20 17:50:09.857582 nonebot_plugin_rename-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5654 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-21 04:43:58.135962 nonebot_plugin_rename-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4789 2023-04-21 04:43:58.135962 nonebot_plugin_rename-1.1.0/README.md
+-rw-r--r--   0        0        0      363 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/__init__.py
+-rw-r--r--   0        0        0      789 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/gaokao_time.py
+-rw-r--r--   0        0        0      885 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/genshin_time.py
+-rw-r--r--   0        0        0      689 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/get_times.py
+-rw-r--r--   0        0        0      925 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/hot_search.py
+-rw-r--r--   0        0        0      408 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/message.py
+-rw-r--r--   0        0        0      466 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/one_word.py
+-rw-r--r--   0        0        0      603 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/status.py
+-rw-r--r--   0        0        0      252 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/config.py
+-rw-r--r--   0        0        0     7444 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/main.py
+-rw-r--r--   0        0        0      186 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/card_choice.py
+-rw-r--r--   0        0        0      867 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/card_name.py
+-rw-r--r--   0        0        0      507 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/download.py
+-rw-r--r--   0        0        0     1535 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/draw.py
+-rw-r--r--   0        0        0      423 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/my_yaml.py
+-rw-r--r--   0        0        0      663 2023-04-21 04:43:58.167962 nonebot_plugin_rename-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 nonebot_plugin_rename-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_rename-1.0.3/LICENSE` & `nonebot_plugin_rename-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/README.md` & `nonebot_plugin_rename-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/gaokao_time.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/gaokao_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/genshin_time.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/genshin_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/get_times.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/get_times.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/hot_search.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/hot_search.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/card/status.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/card/status.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/main.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,35 @@
     ActionFailed,
 )
 from nonebot.drivers import Driver
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 
 from .config import Config
-from .utils import choice_card, generate_card_image, card_list, read_yaml, write_yaml
+from .utils import (
+    choice_card,
+    generate_card_image,
+    card_list,
+    read_yaml,
+    write_yaml,
+    download_file,
+)
 
 require("nonebot_plugin_apscheduler")
 from nonebot_plugin_apscheduler import scheduler
 
 driver: Driver = get_driver()
 env_config = Config.parse_obj(get_driver().config.dict())
 hour, minute = env_config.set_group_card_hour, env_config.set_group_card_minute
 if driver.config.nickname:
-    NICKNAME = env_config.self_name if env_config.self_name else list(driver.config.nickname)[0]
+    NICKNAME = (
+        env_config.self_name
+        if env_config.self_name
+        else list(driver.config.nickname)[0]
+    )
 else:
     NICKNAME = env_config.self_name if env_config.self_name else "bot"
 yml_file = Path.cwd() / "data" / "group_card"
 permissions = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 
 group_card = on_command(
     "设置群名片",
@@ -184,13 +195,17 @@
     logger.info("开始为列表中的群更改bot群名片")
     await set_group_card()
 
 
 # bot启动时执行
 @driver.on_startup
 async def init_group_card():
-    if not yml_file.exists():
-        yml_file.mkdir(parents=True)
-        logger.info("创建group_card文件夹成功")
     if not (yml_file / "group_card.yaml").exists():
+        yml_file.mkdir(parents=True, exist_ok=True)
         (yml_file / "group_card.yaml").touch()
         logger.info("创建group_card.yaml文件成功")
+    if not (yml_file / "fonts" / "draw.ttf").exists():
+        (yml_file / "fonts").mkdir(parents=True, exist_ok=True)
+        await download_file(
+            url="https://fastly.jsdelivr.net/gh/forchannot/nonebot_plugin_rename@main/data/fonts/draw.ttf",
+            file_path=yml_file / "fonts" / "draw.ttf",
+        )
```

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/card_name.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/card_name.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_rename-1.0.3/nonebot_plugin_rename/utils/draw.py` & `nonebot_plugin_rename-1.1.0/nonebot_plugin_rename/utils/draw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from io import BytesIO
 
 from PIL import Image, ImageDraw, ImageFont
+from pathlib import Path
 
 from .card_name import card_list
 
 
+font_path = Path.cwd() / "data" / "group_card" / "fonts" / "draw.ttf"
+
+
 def generate_card_image(
-    font_path: str = "simhei.ttf",
+    font: Path = font_path,
     font_size: int = 20,
     title_left: str = "群名片序号",
     title_right: str = "群名片描述",
 ):
     # 创建一个空白的图片
     img = Image.new("RGB", (800, len(card_list) * 50 + 50), color="white")
     # 设置字体和字号
-    font = ImageFont.truetype(font_path, size=font_size)
+    font = ImageFont.truetype(font.as_posix(), size=font_size)
     # 创建一个绘制对象
     draw = ImageDraw.Draw(img)
     # 绘制标题和分割线
     draw.text((50, 10), title_left, font=font, fill="black")
     draw.line((200, 0, 200, len(card_list) * 50 + 50), fill="black")
     draw.text((220, 10), title_right, font=font, fill="black")
     draw.line((0, 50, 800, 50), fill="black")
     # 遍历列表，获取内容并绘制到图片上
     for i in range(len(card_list)):
         if card_list[str(i + 1)][0]:
-            draw.text((95, i * 50 + 65), str(i+1), font=font, fill="black")
+            draw.text((95, i * 50 + 65), str(i + 1), font=font, fill="black")
             draw.line((200, i * 50 + 50, 200, (i + 1) * 50 + 50), fill="black")
-            draw.text((220, i * 50 + 65), card_list[str(i + 1)][0], font=font, fill="black")
+            draw.text(
+                (220, i * 50 + 65), card_list[str(i + 1)][0], font=font, fill="black"
+            )
             draw.line((0, (i + 1) * 50 + 50, 800, (i + 1) * 50 + 50), fill="black")
     # 返回base64编码后的图片字符串
     img_buffer = BytesIO()
     img.save(img_buffer, format="PNG")
     return img_buffer.getvalue()
```

### Comparing `nonebot_plugin_rename-1.0.3/pyproject.toml` & `nonebot_plugin_rename-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-rename"
-version = "1.0.3"
+version = "1.1.0"
 description = "更改qq机器人的群名片，内置多种有趣名片"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_rename"}]
 
 [[tool.poetry.source]]
@@ -16,12 +16,13 @@
 python = "^3.8"
 httpx = "^0.23.3"
 nonebot-adapter-onebot = "^2.2.2"
 nonebot-plugin-apscheduler = "^0.2.0"
 psutil = "^5.9.5"
 pyyaml = "^6.0"
 pillow = "^9.5.0"
+aiohttp = "^3.8.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_rename-1.0.3/PKG-INFO` & `nonebot_plugin_rename-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-rename
-Version: 1.0.3
+Version: 1.1.0
 Summary: 更改qq机器人的群名片，内置多种有趣名片
 License: GPL-3.0
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-rename Version: 1.1.0 Summary:
 æ´æ¹qqæºå¨äººçç¾¤åçï¼åç½®å¤ç§æè¶£åç License: GPL-3.0
 Author: forchannot Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-
-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-
-Dist: psutil (>=5.9.5,<6.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Description-
-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-
+Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0) Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                          # nonebot-plugin-rename _â¨
 éè¿å®æ¶ä»»å¡æ´æ¹botæå¨ç¾¤èªå·±çç¾¤åç,åç½®äºå ç§å¸¸è§çç¾¤åçå¹¶ä¸åæ­¥æ¯æäºå¤bot,æ¬¢è¿**pr**æ°çç¾¤åç!
                         â¨_ [license] [pypi] [python]
  * [nonebot-plugin-rename](#nonebot-plugin-rename) * [ðç®ä»](#ç®ä») *
 [ðè®¸å¯](#è®¸å¯) * [ð¿ å®è£æ¹æ³](#-å®è£æ¹æ³) *
```

