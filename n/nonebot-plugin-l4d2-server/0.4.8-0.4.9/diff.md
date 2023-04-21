# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.8.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.9.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.8.tar` & `nonebot_plugin_l4d2_server-0.4.9.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.8/LICENSE
--rw-r--r--   0        0        0    17164 2023-04-15 17:43:59.561254 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8619 2023-04-15 17:41:38.056669 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     5046 2023-04-13 15:39:47.743742 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1748 2023-04-13 15:08:36.760710 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      788 2023-04-13 15:01:07.140804 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10949 2023-04-13 15:16:25.729675 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1505 2023-04-15 17:44:06.669779 nonebot_plugin_l4d2_server-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    11585 2023-04-15 17:43:01.023713 nonebot_plugin_l4d2_server-0.4.8/README.md
--rw-r--r--   0        0        0    13394 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.8/setup.py
--rw-r--r--   0        0        0    13236 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.9/LICENSE
+-rw-r--r--   0        0        0    17186 2023-04-21 12:53:33.326433 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8646 2023-04-19 12:28:03.179586 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     8731 2023-04-21 12:49:18.045680 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1748 2023-04-13 15:08:36.760710 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-21 12:49:18.045680 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2947 2023-04-21 12:49:18.074588 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      788 2023-04-13 15:01:07.140804 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10949 2023-04-13 15:16:25.729675 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0        6 2023-04-21 12:49:18.115451 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/config.py
+-rw-r--r--   0        0        0     6644 2023-04-21 12:49:18.181231 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    11923 2023-04-21 12:49:18.234054 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1522 2023-04-21 12:53:38.686262 nonebot_plugin_l4d2_server-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    11652 2023-04-21 12:53:13.473228 nonebot_plugin_l4d2_server-0.4.9/README.md
+-rw-r--r--   0        0        0    13485 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.9/setup.py
+-rw-r--r--   0        0        0    13339 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.9/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/LICENSE` & `nonebot_plugin_l4d2_server-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     from .l4d2_web import web,webUI
 else:
     pass
 
 driver = get_driver()
 
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
@@ -360,25 +360,25 @@
             file_name = data_one['名字']+ '.vpk'
             await upload_file(bot, event, data_file, file_name)
     else:
         await matcher.finish('已取消上传')
     
 
 
-@updata.handle()
-async def _(matcher:Matcher,args:Message = CommandArg()):
-    """更新"""
-    msg = args.extract_plain_text()
-    if not msg:
-        load_josn()
-        reload_ip()
-        await matcher.finish('已更新缓存数据')
-    else:
-        message = await write_json(msg)
-        await matcher.finish(message)
+# @updata.handle()
+# async def _(matcher:Matcher,args:Message = CommandArg()):
+#     """更新"""
+#     msg = args.extract_plain_text()
+#     if not msg:
+#         load_josn()
+#         reload_ip()
+#         await matcher.finish('已更新缓存数据')
+#     else:
+#         message = await write_json(msg)
+#         await matcher.finish(message)
   
 
             
 @vtf_make.handle()
 async def _(matcher:Matcher,state:T_State,args:Message = CommandArg()):
     msg:str = args.extract_plain_text()
     if msg not in ['拉伸','填充','覆盖','']:
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # anne
 anne_player = on_command('Ranne',aliases={"求生anne"},priority=25,block=True)
 anne_bind = on_command('Rbind',aliases={'steam绑定','求生绑定','anne绑定'},priority=20,block=True)
 del_bind = on_command('del_bind',aliases={'steam解绑','求生解绑','anne解绑'},priority=20,block=True)
 prison = on_command('zl',aliases={'坐牢'},priority=20,block=True)
 open_prison = on_command('kl',aliases={'开牢'},priority=20,block=True)
 
-updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
+# updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
 tan_jian = on_command('tj',aliases={'探监'},priority=20,block=True)
 
 # 查询
 queries = on_command('queries',aliases={'求生ip','求生IP'},priority=20,block=True)
 add_queries = on_command('addq',aliases={"求生添加订阅"},priority=20,block=True,permission= Master)
 del_queries = on_command('delq',aliases={"求生取消订阅"},priority=20,block=True,permission= Master)
 show_queries = on_command('showq',aliases={"求生订阅"},priority=20,block=True)
@@ -148,14 +148,15 @@
         except KeyError:
             pass
     
     
     get_ip = on_command('anne',aliases=server_key(),priority=80,block=True)
     @get_ip.handle()
     async def _(matcher:Matcher,start:str = CommandStart(),command: str = RawCommand(),args:Message = CommandArg()):
+        global matchers
         if get_ip.plugin_name not in matchers:
             matchers[get_ip.plugin_name] = []
         matchers[get_ip.plugin_name].append(get_ip)
         if start:
             command = command.replace(start,'')
         if command == 'anne':
             command = '云'
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from fastapi import Header, HTTPException, Depends
 from fastapi.responses import JSONResponse, HTMLResponse, RedirectResponse
 from jose import jwt
 from nonebot import get_bot, get_app
 
 from pathlib import Path
 
-
 from nonebot import get_driver, logger
-from .config import *
 from ..config import *
 from ..utils import split_maohao
 from ..l4d2_queries.qqgroup import qq_ip_querie
 CONFIG_PATH = Path() / 'data' / 'L4D2' / 'l4d2.yml'
 
 CONFIG_PATH.parent.mkdir(parents=True, exist_ok=True)
 
@@ -101,14 +99,23 @@
             }
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
             }
 
+    @app.post('/l4d2/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def post_chat_global_config(data: dict):
+        config_manager.config.update(**data)
+        config_manager.save()
+        return {
+            'status': 0,
+            'msg':    '保存成功'
+        }
+
     @app.get('/l4d2/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
     async def get_chat_global_config():
         try:
             bot = get_bot()
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from amis import LevelEnum, Select,  Alert, Tpl, Flex
 
 
 from ..config import NICKNAME
 
 logo = Html(html='''
 <p align="center">
-    <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server">
-        <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png"
+    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
+        <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
          width="256" height="256" alt="Learning-Chat">
     </a>
 </p>
 <h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
 <div align="center">
-    <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/" target="_blank">
+    <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
     Github仓库</a>
 </div>
 <br>
 <br>
 ''')
 login_api = AmisAPI(
     url='/l4d2/api/login',
@@ -67,14 +67,37 @@
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
     ],
     actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
              Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
+
+upload_map_form = Form(
+    title='全局配置',
+    name='global_config',
+    api='post:/l4d2/api/chat_map_config',
+    body=[
+        InputText(label='服务器host', name='web_username', value='${web_username}',
+                  labelRemark=Remark(shape='circle',
+                                     content='127.0.0.1')),
+        InputPassword(label='服务器', name='web_password', value='${web_password}',
+                      labelRemark=Remark(shape='circle',
+                                         content='登录本后台管理所需要的密码。')),
+        InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于本后台管理加密验证token的密钥。')),
+        InputText(label='查询key', name='l4_key', value='${l4_key}',
+                  labelRemark=Remark(shape='circle',
+                                     content='用于获取拓展功能的key。')),
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
+
 group_select = Select(label='分群配置', name='group_id', source='${group_list}',
                       placeholder='选择群')
 group_config_form = Form(
     title='分群配置（暂未完成）',
     visibleOn='group_id != null',
     initApi='/l4d2/api/chat_group_config?group_id=${group_id}',
     api='post:/l4d2/api/chat_group_config?group_id=${group_id}',
@@ -165,17 +188,17 @@
                            children=[message_page, context_page])
 config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
                          schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
                                      body=[global_config_form, group_select, group_config_form]))
 chat_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
 
 github_logo = Tpl(className='w-full',
-                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
+                  tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
 header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
 
 admin_app = App(brandName='L4d2-Server',
-                logo='https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png',
+                logo='https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png',
                 header=header,
                 pages=[{
                     'children': [config_page, database_page]
                 }],
-                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
+                footer='<div class="p-2 text-center bg-blue-100">Copyright © 2022 - 2023 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" class="link-secondary">AGNES_DIGIAL</a> X<a target="_blank" href="https://github.com/baidu/amis" class="link-secondary" rel="noopener"> amis v2.2.0</a></div>')
```

#### html2text {}

```diff
@@ -36,14 +36,27 @@
 (label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
 (shape='circle', content='ç¨äºè·åæå±åè½çkeyã')), InputTag
 (label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='${l4_master}',
 enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
 joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
 content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ], actions=[Action
 (label='ä¿å­', level=LevelEnum.success, type='submit'), Action
+(label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
+Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
+chat_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
+value='${web_username}', labelRemark=Remark(shape='circle',
+content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
+value='${web_password}', labelRemark=Remark(shape='circle',
+content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
+(label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
+{web_secret_key}', labelRemark=Remark(shape='circle',
+content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
+(label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
+(shape='circle', content='ç¨äºè·åæå±åè½çkeyã')), ], actions=
+[Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) group_select =
 Select(label='åç¾¤éç½®', name='group_id', source='${group_list}',
 placeholder='éæ©ç¾¤') group_config_form = Form
 ( title='åç¾¤éç½®ï¼ææªå®æï¼', visibleOn='group_id != null',
 initApi='/l4d2/api/chat_group_config?group_id=${group_id}', api='post:/l4d2/
 api/chat_group_config?group_id=${group_id}', body=[ Switch
 (label='åç¾¤å¼å³', name='enable', value='${enable}', onText='å¼å¯',
@@ -98,12 +111,12 @@
 icon='fa fa-wrench', label='éç½®', schema=Page(title='éç½®', initApi='/
 l4d2/api/get_group_list', body=[global_config_form, group_select,
 group_config_form])) chat_page = PageSchema(label='æ±çä¹è·¯', icon='fa fa-
 wechat (alias)', children=[config_page, database_page]) github_logo = Tpl
 (className='w-full', tpl='
 ') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
 items=[github_logo]) admin_app = App(brandName='L4d2-Server', logo='https://
-raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/
-main/image/logo.png', header=header, pages=[{ 'children': [config_page,
-database_page] }], footer='
+raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/
+logo.png', header=header, pages=[{ 'children': [config_page, database_page] }],
+footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
 ')
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.8/pyproject.toml` & `nonebot_plugin_l4d2_server-0.4.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.8"
+version = "0.4.9"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
@@ -41,11 +41,12 @@
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
 pandas = ">=1.5.2"
 python-jose = "^3.3.0"
+h11 = "^0.14.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/README.md` & `nonebot_plugin_l4d2_server-0.4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
+
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
@@ -26,58 +27,53 @@
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
-</div>
 
+</div>
 
 ## 快速使用（env示例）
+
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
     l4_master = ['1145149191']            # 允许上传地图的qq号
     l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
     l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
     l4_port = ['20715']                   # 服务器端口
     l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
     l4_font = 'simsun.ttc'                # 服务器字体
     l4_web = True                         # 网页控制台，默认是关闭
 
-
-
 ## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
-
 ## 如何获取key
 
 为了使得ip不被滥用，我采取这种方式管理。
 
 这并不影响正常使用，如果不需要可以忽略
 
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
         l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
         l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
-
-
 ## 提交自己的服务器？
 
-**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
-
-**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**
+__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__
 
+__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
 
         {
         "呆呆": [
                 {
                 "id": 1,
@@ -89,193 +85,199 @@
                 "version": "战役",
                 "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
 ## 🌐 默认服务器
-目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
+
+目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
 | 云 | anne电信服云服 | 东 | 27
-| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
-| 橘 | 橘希实香的小窝 | 橘希实香 | 14
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
+| 橘 | 橘希实香的小窝 | 橘希实香 | 21
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 
-
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.9--2022.4
+
+- 修复h11版本错误的bug
+- 重写了config，下个版本正式使用yaml替代env设置
+- 新增远程连接测试代码
+
 ### 0.4.8--2022.4.16
 
- - 新增重载ip
- - 修复了一些windows启动下奇奇怪怪的bug
+- 新增重载ip
+- 修复了一些windows启动下奇奇怪怪的bug
 
 ### 0.4.7--2022.4.13
 
- - 新增模式查询
- - 列表推导替换套娃循环
+- 新增模式查询
+- 列表推导替换套娃循环
 
 ### 0.4.6--2022.4.9
 
- - 显示无效服
- - 优化服务器排序算法（list.sort()天下第一）
- - 默认关闭web端
+- 显示无效服
+- 优化服务器排序算法（list.sort()天下第一）
+- 默认关闭web端
 
 ### 0.4.5--2022.4.9
 
 - 修bug（恼）
 
 ### 0.4.2--2022.4.9
 
- - 修复响应开头匹配出现的重大bug
- - 启用web端
- - web使用yaml管理，未来可能删除env配置
+- 修复响应开头匹配出现的重大bug
+- 启用web端
+- web使用yaml管理，未来可能删除env配置
 
 ### 0.4.1--2022.3
 
- - 修复rar压缩包命名错误
- - 更新了tag的参数读取方式
- - 确定了传文件私聊比群聊快速
- - 修复了电信服计算错误
+- 修复rar压缩包命名错误
+- 更新了tag的参数读取方式
+- 确定了传文件私聊比群聊快速
+- 修复了电信服计算错误
 
 ### 0.4.0--2022.3.27
 
- - 新增web控制台
- - 修复传图超时参数错误
- - 重写求生ip获取方法 ~ 数据库苦手 ~
- - 重写文档
- - 不再内置ip（毕竟ipv4都暴露太危险了）
+- 新增web控制台
+- 修复传图超时参数错误
+- 重写求生ip获取方法 ~ 数据库苦手 ~
+- 重写文档
+- 不再内置ip（毕竟ipv4都暴露太危险了）
 
 ### 0.3.7--2022.3
 
- - 新增三方下载网盘
- - 修复windows上传临时文件错误
- - 优化查服流程
- - 优化anne服随机功能
+- 新增三方下载网盘
+- 修复windows上传临时文件错误
+- 优化查服流程
+- 优化anne服随机功能
 
 ### 0.3.6--2022.3.10
 
- - 暂时关闭web端，后续修改
- - 优化图片显示
- - 修复了海量bug
- - 新增三方图查询
+- 暂时关闭web端，后续修改
+- 优化图片显示
+- 修复了海量bug
+- 新增三方图查询
 
 ### 0.3.5--2022.3.6
 
- - 新增ping查询（在ip里包括）
- - 新增api查询（未完成）
- - 修复了电信服查询绑定名字无法查询的错误
- - 新增了救援率的显示
- - 新增web端（未完成）
+- 新增ping查询（在ip里包括）
+- 新增api查询（未完成）
+- 修复了电信服查询绑定名字无法查询的错误
+- 新增了救援率的显示
+- 新增web端（未完成）
 
 ### 0.3.4--2022.3.1
 
- - 新增本地插件smx查询
- - 增加了三个内置群服
- - 修改了图片的UI,变好看了
- - 删减了部分图片和字体，使得轻量化
- - 修复了海量bug
- - 修复了python3.8中typing错误
+- 新增本地插件smx查询
+- 增加了三个内置群服
+- 修改了图片的UI,变好看了
+- 删减了部分图片和字体，使得轻量化
+- 修复了海量bug
+- 修复了python3.8中typing错误
 
 ### 0.3.3--2022.2.26
 
- - 重写协议，使用a2s库，同时解决win端不同报错无法输出
- - 重~抄~写服务器查询UI,解决了不好看的问题
- - 从win测试，解决了一些win特有的bug
- - 重写服务器查询~还得是json~
- - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
- - 新增批量查询服务器，不带参数则返回图片
+- 重写协议，使用a2s库，同时解决win端不同报错无法输出
+- 重~抄~写服务器查询UI,解决了不好看的问题
+- 从win测试，解决了一些win特有的bug
+- 重写服务器查询~还得是json~
+- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
+- 新增批量查询服务器，不带参数则返回图片
 
 ### 0.3.1--2022.2.22
 
- - 修复了路径识别为str对象的错误
- - 修复了初始化找不到文件的错误
- - 修复了路径拼接错误
- - 在win端成功测试，修复压缩包bug
- - 新增开关协程异步env设置
- - 测试rcon建立通讯
- - 实现切换路径查看地图和使用rcon指令
+- 修复了路径识别为str对象的错误
+- 修复了初始化找不到文件的错误
+- 修复了路径拼接错误
+- 在win端成功测试，修复压缩包bug
+- 新增开关协程异步env设置
+- 测试rcon建立通讯
+- 实现切换路径查看地图和使用rcon指令
 
 ### 0.3.0--2022.2.18
 
- - 修改了新的env配置，使得支持本地多服务器操作
- - 彻底解决了压缩包解压linux端的问题
- - 解决了win端默认gbk解码的错误
- - 解决rcon指令字体报错
+- 修改了新的env配置，使得支持本地多服务器操作
+- 彻底解决了压缩包解压linux端的问题
+- 解决了win端默认gbk解码的错误
+- 解决rcon指令字体报错
 
 ### 0.2.5--2022.2.10
 
- - 修复了依赖不足的bug
- - 更新了电信服战绩个人图片UI
- - 更新了批量服务器查看的UI
- - 修改了传文件为协程异步
- - 优化了部分rcon指令
- - ~tnd7z怎么不去死啊~使用pyunpack库解压7z
+- 修复了依赖不足的bug
+- 更新了电信服战绩个人图片UI
+- 更新了批量服务器查看的UI
+- 修改了传文件为协程异步
+- 优化了部分rcon指令
+- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
 
 ### 0.2.4--2022.2.8
 
- - 使用poetry修复了pip安装文件缺失的bug
+- 使用poetry修复了pip安装文件缺失的bug
 
 ### 0.2.3--2022.2.7
 
- - 新增坐牢和开牢
- - 修改了获取资源为异步协程却阻碍其他指令的bug
- - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
- - 喷剂制作开摆了，推测需要c/c++环境
- - 修改抽取文案
- - 新增查询服务器状态时返回connect ip
- - 修复了服务器查询无响应的时候，因为报错无回复信息的bug
- - 个人信息重置测试代码，下个版本更新
- - 新增求生更新添加和删除
+- 新增坐牢和开牢
+- 修改了获取资源为异步协程却阻碍其他指令的bug
+- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
+- 喷剂制作开摆了，推测需要c/c++环境
+- 修改抽取文案
+- 新增查询服务器状态时返回connect ip
+- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
+- 个人信息重置测试代码，下个版本更新
+- 新增求生更新添加和删除
 
 ### 0.2.2--2022.2.1
 
- - 新增探监
- - 新增喷漆制作
- - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
- - 修改了部分对话响应
+- 新增探监
+- 新增喷漆制作
+- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
+- 修改了部分对话响应
 
 ### 0.2.1--2022.1.25
 
- - 新增电信服获取（东哥的肯定）
- - 优化图片UI 
- - 新增云服快捷查询
- - 修复了因为没用玩家，导致的服务器状态查询错误
- - 新增电信服ip爬取（仅仅作为单次更新ip列表）
+- 新增电信服获取（东哥的肯定）
+- 优化图片UI
+- 新增云服快捷查询
+- 修复了因为没用玩家，导致的服务器状态查询错误
+- 新增电信服ip爬取（仅仅作为单次更新ip列表）
 
 ### 0.2.0--2022.1.21
 
- - 新增创意工坊查询
- - 优化查询图片UI
- - 新增创意工坊文件下载
- - 修复了因为电信服官网前端修改导致查询失败的BUG
+- 新增创意工坊查询
+- 优化查询图片UI
+- 新增创意工坊文件下载
+- 修复了因为电信服官网前端修改导致查询失败的BUG
 
 ### 0.1.7--2022.1.19
 
- - 新增群ip订阅，批量查询
- - 新增图片显示ip状态
- - 修复了因为玩家名字特殊字符导致的utf-8解码错误
- - 更新自己的第三方库VSQ==0.0.6
+- 新增群ip订阅，批量查询
+- 新增图片显示ip状态
+- 修复了因为玩家名字特殊字符导致的utf-8解码错误
+- 更新自己的第三方库VSQ==0.0.6
 
 ### 0.1.6--2022.1.15
 
- - 新增ip查询服务器提供玩家数量和名字
- - 增加协程函数修复因为加载顺序导致的错误
- - 更新自己的第三方库VSQ==0.0.4
+- 新增ip查询服务器提供玩家数量和名字
+- 增加协程函数修复因为加载顺序导致的错误
+- 更新自己的第三方库VSQ==0.0.4
 
 ### 0.1.5--2022.1.15
 
 - 新增服务器控制台指令，新增依赖rcon
 - 重新了数据库，不再使用json而是使用sql3
 - 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
 
@@ -325,23 +327,23 @@
 
 - 插件初次发布，可私聊添加地图
 
 </details>
 
 ## 🙈 其他
 
-+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
-+ 如果本插件对你有帮助，不要忘了点个Star~
-+ 本项目仅供学习使用，请勿用于商业用途
-+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
-        
+- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
+- 如果本插件对你有帮助，不要忘了点个Star~
+- 本项目仅供学习使用，请勿用于商业用途
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
-- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架
-- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
-- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
-- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
-  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
-- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
-- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
-- 呆呆 - 提供三方地图的详细数据
+- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
+- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
+- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
+- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
+  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
+- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
+- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
+- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
+- 呆呆- 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -24,30 +24,32 @@
 è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
 (https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
 l4_key = 'qwertyuiopasdfg' #
 è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
 æäº¤èªå·±çæå¡å¨ï¼
-**æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
-**é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
+__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__
+__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
 { "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
-é»è®¤æå¡å¨ ç®å **å·²ææ**
+é»è®¤æå¡å¨ ç®å __å·²ææ__
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
-27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
-3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
+ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ |
+27 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
+21 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³
+| 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
-0.4.8--2022.4.16 - æ°å¢éè½½ip -
+0.4.9--2022.4 - ä¿®å¤h11çæ¬éè¯¯çbug -
+éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
+æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
 ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
 æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
 æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
 é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
 ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
@@ -120,23 +122,23 @@
 - æ°å¢æ¯æå¾çè¾åº - æ°å¢æ¥è¯¢anneææ°æ® ### 0.1.1--2022.1.5 -
 æ°å¢å é¤å°å¾ - æ°å¢å°å¾æ¹å - æ°å¢æ¯æå¾çè¾åº ### 0.1.0--
 2022.1.4 - éä¸­ä¿®å¤äºBug ### 0.0.9--2022.1.4 -
 æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­ -
 ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
-æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
+æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» -
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
+& Pr - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
 [@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
-github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:
-//github.com/s52047qwas/nonebot_plugin_xiuxian) -
-æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
+github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:/
+/github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè - ~~
+[èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
+(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
-MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
-github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
-webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
-GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
-æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
+MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
+CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
+[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
+(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/setup.py` & `nonebot_plugin_l4d2_server-0.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
                                 'data/L4D2/image/template/*']}
 
 install_requires = \
 ['aiohttp>=3.8.3,<4.0.0',
  'amis-python>=1.0.6,<2.0.0',
  'asyncio>=3.4.3',
  'beautifulsoup4>=4.8.0',
+ 'h11>=0.14.0,<0.15.0',
  'httpx>=0.23.3,<0.24.0',
  'jieba>=0.42.1,<0.43.0',
  'jinja2>=3.0.0',
  'nonebot-adapter-onebot>=2.1.5',
  'nonebot2>=2.0.0rc4,<3.0.0',
  'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
  'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0',
@@ -39,17 +40,17 @@
  'rarfile>=4.0,<5.0',
  'rcon>=2.1.0,<3.0.0',
  'ruamel.yaml>=0.17.21,<0.18.0',
  'srctools>=2.3.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n    l4_web = True                         # 网页控制台，默认是关闭\n\n\n\n## 主要功能\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n## 如何获取key\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                },\n                {\n                "id": 2,\n                "version": "战役",\n                "ip": "43.248.188.17:27032"\n                }\n        ]\n        }\n\n## 🌐 默认服务器\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14\n| 橘 | 橘希实香的小窝 | 橘希实香 | 14\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.8--2022.4.16\n\n - 新增重载ip\n - 修复了一些windows启动下奇奇怪怪的bug\n\n### 0.4.7--2022.4.13\n\n - 新增模式查询\n - 列表推导替换套娃循环\n\n### 0.4.6--2022.4.9\n\n - 显示无效服\n - 优化服务器排序算法（list.sort()天下第一）\n - 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n\n</div>\n\n## 快速使用（env示例）\n\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n    l4_web = True                         # 网页控制台，默认是关闭\n\n## 主要功能\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n## 如何获取key\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n## 提交自己的服务器？\n\n__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__\n\n__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                },\n                {\n                "id": 2,\n                "version": "战役",\n                "ip": "43.248.188.17:27032"\n                }\n        ]\n        }\n\n## 🌐 默认服务器\n\n目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 21\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.9--2022.4\n\n- 修复h11版本错误的bug\n- 重写了config，下个版本正式使用yaml替代env设置\n- 新增远程连接测试代码\n\n### 0.4.8--2022.4.16\n\n- 新增重载ip\n- 修复了一些windows启动下奇奇怪怪的bug\n\n### 0.4.7--2022.4.13\n\n- 新增模式查询\n- 列表推导替换套娃循环\n\n### 0.4.6--2022.4.9\n\n- 显示无效服\n- 优化服务器排序算法（list.sort()天下第一）\n- 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n- 修复响应开头匹配出现的重大bug\n- 启用web端\n- web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n- 修复rar压缩包命名错误\n- 更新了tag的参数读取方式\n- 确定了传文件私聊比群聊快速\n- 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n- 新增web控制台\n- 修复传图超时参数错误\n- 重写求生ip获取方法 ~ 数据库苦手 ~\n- 重写文档\n- 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n- 新增三方下载网盘\n- 修复windows上传临时文件错误\n- 优化查服流程\n- 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n- 暂时关闭web端，后续修改\n- 优化图片显示\n- 修复了海量bug\n- 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n- 新增ping查询（在ip里包括）\n- 新增api查询（未完成）\n- 修复了电信服查询绑定名字无法查询的错误\n- 新增了救援率的显示\n- 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n- 新增本地插件smx查询\n- 增加了三个内置群服\n- 修改了图片的UI,变好看了\n- 删减了部分图片和字体，使得轻量化\n- 修复了海量bug\n- 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n- 重写协议，使用a2s库，同时解决win端不同报错无法输出\n- 重~抄~写服务器查询UI,解决了不好看的问题\n- 从win测试，解决了一些win特有的bug\n- 重写服务器查询~还得是json~\n- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n- 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n- 修复了路径识别为str对象的错误\n- 修复了初始化找不到文件的错误\n- 修复了路径拼接错误\n- 在win端成功测试，修复压缩包bug\n- 新增开关协程异步env设置\n- 测试rcon建立通讯\n- 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n- 修改了新的env配置，使得支持本地多服务器操作\n- 彻底解决了压缩包解压linux端的问题\n- 解决了win端默认gbk解码的错误\n- 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n- 修复了依赖不足的bug\n- 更新了电信服战绩个人图片UI\n- 更新了批量服务器查看的UI\n- 修改了传文件为协程异步\n- 优化了部分rcon指令\n- ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n- 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n- 新增坐牢和开牢\n- 修改了获取资源为异步协程却阻碍其他指令的bug\n- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n- 喷剂制作开摆了，推测需要c/c++环境\n- 修改抽取文案\n- 新增查询服务器状态时返回connect ip\n- 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n- 个人信息重置测试代码，下个版本更新\n- 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n- 新增探监\n- 新增喷漆制作\n- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n- 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n- 新增电信服获取（东哥的肯定）\n- 优化图片UI\n- 新增云服快捷查询\n- 修复了因为没用玩家，导致的服务器状态查询错误\n- 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n- 新增创意工坊查询\n- 优化查询图片UI\n- 新增创意工坊文件下载\n- 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n- 新增群ip订阅，批量查询\n- 新增图片显示ip状态\n- 修复了因为玩家名字特殊字符导致的utf-8解码错误\n- 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n- 新增ip查询服务器提供玩家数量和名字\n- 增加协程函数修复因为加载顺序导致的错误\n- 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n- 如果本插件对你有帮助，不要忘了点个Star~\n- 本项目仅供学习使用，请勿用于商业用途\n- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n\n## 🌐 感谢\n\n- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考\n- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)\n- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考\n- [日向麻麻](https://github.com/Special-Week)- 代码优化参考\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考\n- 呆呆- 提供三方地图的详细数据\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -4,139 +4,141 @@
 'nonebot_plugin_l4d2_server.l4d2_image',
 'nonebot_plugin_l4d2_server.l4d2_queries',
 'nonebot_plugin_l4d2_server.l4d2_server',
 'nonebot_plugin_l4d2_server.l4d2_web'] package_data = \ {'': ['*'],
 'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*', 'data/L4D2/image/
 header/*', 'data/L4D2/image/template/*']} install_requires = \
 ['aiohttp>=3.8.3,<4.0.0', 'amis-python>=1.0.6,<2.0.0', 'asyncio>=3.4.3',
-'beautifulsoup4>=4.8.0', 'httpx>=0.23.3,<0.24.0', 'jieba>=0.42.1,<0.43.0',
-'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
-'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
+'beautifulsoup4>=4.8.0', 'h11>=0.14.0,<0.15.0', 'httpx>=0.23.3,<0.24.0',
+'jieba>=0.42.1,<0.43.0', 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5',
+'nonebot2>=2.0.0rc4,<3.0.0', 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
 'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
 a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
 'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
 'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
-server', 'version': '0.4.8', 'description': 'L4D2 server related operations
+server', 'version': '0.4.9', 'description': 'L4D2 server related operations
 plugin for NoneBot2', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
-         \n\n# nonebot_plugin_l4d2_server\n_â¨Nonebot & Left 4 Dead 2
+        \n\n# nonebot_plugin_l4d2_server\n\n_â¨Nonebot & Left 4 Dead 2
                               serveræä½â¨_\n
             \n ææ¡£   Â·  \n æä»¤åè¡¨   Â·  \n å¸¸è§é®é¢\n
 
     \n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_
-            [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n
-\n\n\n## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼\n #
+           [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n\n
+\n\n## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼\n\n #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®\n
 # ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\'] #
 åè®¸ä¸ä¼ å°å¾çqqå·\n l4_file = [\'/home/ubuntu/l4d2/coop\'] #
 æ¬å°æå¡å¨è·¯å¾\n l4_host = [\'127.0.0.1\'] #
 æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼\n l4_port = [\'20715\'] #
 æå¡å¨ç«¯å£\n l4_rcon = [\'1145149191810\'] #
 æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´ \n l4_font =
 \'simsun.ttc\' # æå¡å¨å­ä½\n l4_web = True #
-ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­\n\n\n\n## ä¸»è¦åè½\n\n- æ±çæå¡å¨-
+ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­\n\n## ä¸»è¦åè½\n\n- æ±çæå¡å¨-
 æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
 åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)\n\n\n##
+ranking/index.php)\n\n##
 å¦ä½è·åkey\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n\nè¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥\n\n
 [ç¹å»è¿éå ç¾¤](https://jq.qq.com/
 ?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ\nå¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼\n\n
 l4_tag = [\'åå\',\'æ©\'] #
 è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡\n l4_key = \'qwertyuiopasdfg\' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n\n\n##
-æäº¤èªå·±çæå¡å¨ï¼\n\n**æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**\n\n**é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**\n\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n\n
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n##
+æäº¤èªå·±çæå¡å¨ï¼\n\n__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__\n\n__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n\n
 {\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
 27031"\n },\n {\n "id": 2,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27032"\n }\n ]\n }\n\n## ð é»è®¤æå¡å¨\nç®å **å·²ææ**
+27032"\n }\n ]\n }\n\n## ð é»è®¤æå¡å¨\n\nç®å __å·²ææ__
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸»\n\n|
 æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3\n| äº | anneçµä¿¡æäºæ | ä¸
-| 27\n| åå | ååçå°çª | æè«å¤§é­ç | 14\n| æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
-| 6\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
+ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4\n| äº | anneçµä¿¡æäºæ | ä¸
+| 27\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
+| 21\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
 æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
-15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.4.8--2022.4.16\n\n - æ°å¢éè½½ip\n -
-ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug\n\n### 0.4.7--2022.4.13\n\n -
-æ°å¢æ¨¡å¼æ¥è¯¢\n - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯\n\n### 0.4.6--
-2022.4.9\n\n - æ¾ç¤ºæ ææ\n - ä¼åæå¡å¨æåºç®æ³ï¼list.sort
-()å¤©ä¸ç¬¬ä¸ï¼\n - é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n-
-ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n -
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
-webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n -
-ä¿®å¤raråç¼©åå½åéè¯¯\n - æ´æ°äºtagçåæ°è¯»åæ¹å¼\n -
-ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n -
-ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n -
-æ°å¢webæ§å¶å°\n - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n -
-éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n - éåææ¡£\n -
-ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n -
-æ°å¢ä¸æ¹ä¸è½½ç½ç\n - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯\n -
-ä¼åæ¥ææµç¨\n - ä¼åanneæéæºåè½\n\n### 0.3.6--2022.3.10\n\n -
-ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹\n - ä¼åå¾çæ¾ç¤º\n -
-ä¿®å¤äºæµ·ébug\n - æ°å¢ä¸æ¹å¾æ¥è¯¢\n\n### 0.3.5--2022.3.6\n\n -
-æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼\n - æ°å¢apiæ¥è¯¢ï¼æªå®æï¼\n -
-ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯\n -
-æ°å¢äºææ´ççæ¾ç¤º\n - æ°å¢webç«¯ï¼æªå®æï¼\n\n### 0.3.4--
-2022.3.1\n\n - æ°å¢æ¬å°æä»¶smxæ¥è¯¢\n - å¢å äºä¸ä¸ªåç½®ç¾¤æ\n -
-ä¿®æ¹äºå¾ççUI,åå¥½çäº\n -
-å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå\n - ä¿®å¤äºæµ·ébug\n -
-ä¿®å¤äºpython3.8ä¸­typingéè¯¯\n\n### 0.3.3--2022.2.26\n\n -
-éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº\n -
-é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢\n -
-ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug\n -
-éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~\n -
+15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
+æ¶èµ·\n\n### 0.4.9--2022.4\n\n- ä¿®å¤h11çæ¬éè¯¯çbug\n-
+éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½®\n-
+æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç \n\n### 0.4.8--2022.4.16\n\n- æ°å¢éè½½ip\n-
+ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug\n\n### 0.4.7--2022.4.13\n\n-
+æ°å¢æ¨¡å¼æ¥è¯¢\n- åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯\n\n### 0.4.6--
+2022.4.9\n\n- æ¾ç¤ºæ ææ\n- ä¼åæå¡å¨æåºç®æ³ï¼list.sort
+()å¤©ä¸ç¬¬ä¸ï¼\n- é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n-
+ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n-
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n- å¯ç¨webç«¯\n-
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n-
+ä¿®å¤raråç¼©åå½åéè¯¯\n- æ´æ°äºtagçåæ°è¯»åæ¹å¼\n-
+ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n-
+ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n-
+æ°å¢webæ§å¶å°\n- ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n-
+éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n- éåææ¡£\n-
+ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n-
+æ°å¢ä¸æ¹ä¸è½½ç½ç\n- ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯\n-
+ä¼åæ¥ææµç¨\n- ä¼åanneæéæºåè½\n\n### 0.3.6--2022.3.10\n\n-
+ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹\n- ä¼åå¾çæ¾ç¤º\n-
+ä¿®å¤äºæµ·ébug\n- æ°å¢ä¸æ¹å¾æ¥è¯¢\n\n### 0.3.5--2022.3.6\n\n-
+æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼\n- æ°å¢apiæ¥è¯¢ï¼æªå®æï¼\n-
+ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯\n-
+æ°å¢äºææ´ççæ¾ç¤º\n- æ°å¢webç«¯ï¼æªå®æï¼\n\n### 0.3.4--
+2022.3.1\n\n- æ°å¢æ¬å°æä»¶smxæ¥è¯¢\n- å¢å äºä¸ä¸ªåç½®ç¾¤æ\n-
+ä¿®æ¹äºå¾ççUI,åå¥½çäº\n-
+å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå\n- ä¿®å¤äºæµ·ébug\n-
+ä¿®å¤äºpython3.8ä¸­typingéè¯¯\n\n### 0.3.3--2022.2.26\n\n-
+éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº\n-
+é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢\n-
+ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug\n-
+éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~\n-
 åç½®æå¡å¨æ¥è¯¢ç³»ç»ï¼å¯ä»¥éè¿[æå¡å¨ç®ç§°]+[number]/
-[æ¨¡å¼]æ¥è®¿é®\n -
+[æ¨¡å¼]æ¥è®¿é®\n-
 æ°å¢æ¹éæ¥è¯¢æå¡å¨ï¼ä¸å¸¦åæ°åè¿åå¾ç\n\n### 0.3.1--
-2022.2.22\n\n - ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯\n -
-ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯\n - ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯\n -
-å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug\n -
-æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®\n - æµè¯rconå»ºç«éè®¯\n -
-å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤\n\n### 0.3.0--2022.2.18\n\n -
-ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½\n -
-å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢\n -
-è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯\n - è§£å³rconæä»¤å­ä½æ¥é\n\n###
-0.2.5--2022.2.10\n\n - ä¿®å¤äºä¾èµä¸è¶³çbug\n -
-æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI\n -
-æ´æ°äºæ¹éæå¡å¨æ¥ççUI\n - ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥\n -
-ä¼åäºé¨årconæä»¤\n -
-~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z\n\n### 0.2.4--2022.2.8\n\n -
-ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug\n\n### 0.2.3--2022.2.7\n\n -
-æ°å¢åç¢åå¼ç¢\n -
-ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug\n -
-æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼\n
-- å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢\n - ä¿®æ¹æ½åææ¡\n -
-æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip\n -
-ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug\n
-- ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ°\n -
-æ°å¢æ±çæ´æ°æ·»å åå é¤\n\n### 0.2.2--2022.2.1\n\n - æ°å¢æ¢ç\n -
-æ°å¢å·æ¼å¶ä½\n -
-ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼\n -
-ä¿®æ¹äºé¨åå¯¹è¯ååº\n\n### 0.2.1--2022.1.25\n\n -
-æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼\n - ä¼åå¾çUI \n -
-æ°å¢äºæå¿«æ·æ¥è¯¢\n -
-ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯\n -
+2022.2.22\n\n- ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯\n-
+ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯\n- ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯\n-
+å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug\n-
+æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®\n- æµè¯rconå»ºç«éè®¯\n-
+å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤\n\n### 0.3.0--2022.2.18\n\n-
+ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½\n-
+å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢\n-
+è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯\n- è§£å³rconæä»¤å­ä½æ¥é\n\n###
+0.2.5--2022.2.10\n\n- ä¿®å¤äºä¾èµä¸è¶³çbug\n-
+æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI\n-
+æ´æ°äºæ¹éæå¡å¨æ¥ççUI\n- ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥\n-
+ä¼åäºé¨årconæä»¤\n-
+~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z\n\n### 0.2.4--2022.2.8\n\n-
+ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug\n\n### 0.2.3--2022.2.7\n\n-
+æ°å¢åç¢åå¼ç¢\n-
+ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug\n-
+æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼\n-
+å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢\n- ä¿®æ¹æ½åææ¡\n-
+æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip\n-
+ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug\n-
+ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ°\n-
+æ°å¢æ±çæ´æ°æ·»å åå é¤\n\n### 0.2.2--2022.2.1\n\n- æ°å¢æ¢ç\n-
+æ°å¢å·æ¼å¶ä½\n-
+ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼\n-
+ä¿®æ¹äºé¨åå¯¹è¯ååº\n\n### 0.2.1--2022.1.25\n\n-
+æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼\n- ä¼åå¾çUI\n-
+æ°å¢äºæå¿«æ·æ¥è¯¢\n-
+ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯\n-
 æ°å¢çµä¿¡æipç¬åï¼ä»ä»ä½ä¸ºåæ¬¡æ´æ°ipåè¡¨ï¼\n\n### 0.2.0--
-2022.1.21\n\n - æ°å¢åæå·¥åæ¥è¯¢\n - ä¼åæ¥è¯¢å¾çUI\n -
-æ°å¢åæå·¥åæä»¶ä¸è½½\n -
+2022.1.21\n\n- æ°å¢åæå·¥åæ¥è¯¢\n- ä¼åæ¥è¯¢å¾çUI\n-
+æ°å¢åæå·¥åæä»¶ä¸è½½\n-
 ä¿®å¤äºå ä¸ºçµä¿¡æå®ç½åç«¯ä¿®æ¹å¯¼è´æ¥è¯¢å¤±è´¥çBUG\n\n###
-0.1.7--2022.1.19\n\n - æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢\n -
-æ°å¢å¾çæ¾ç¤ºipç¶æ\n -
-ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯\n -
-æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n -
-æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­\n -
-å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯\n -
+0.1.7--2022.1.19\n\n- æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢\n-
+æ°å¢å¾çæ¾ç¤ºipç¶æ\n-
+ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯\n-
+æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n-
+æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­\n-
+å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯\n-
 æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n-
 æ°å¢æå¡å¨æ§å¶å°æä»¤ï¼æ°å¢ä¾èµrcon\n-
 éæ°äºæ°æ®åºï¼ä¸åä½¿ç¨jsonèæ¯ä½¿ç¨sql3\n-
 æ¹åäºæ±çanneä¿¡æ¯æ¾ç¤ºæ¹å¼ï¼å¦æåä¸ªæ°æ®ä»¥å¾çæ¾ç¤ºï¼å¦æå¤ä¸ªæ°æ®ä»¥æå­æ¾ç¤º\n\n###
 0.1.4--2022.1.9\n\n- æ°å¢æ±çanneè¯¦æï¼çæåï¼\n-
 ææçè¯·æ±æ¹ä¸ºhttpx\n- æ´æ°äºanneä¿¡æ¯å¾ç\n-
 å¯éä½¿ç¨æ¨¡æè°·æ­æµè§å¨æ¥è·åanneæ´å¤æ°æ®ï¼~æç¹å±äºï¼å¸æå¤§ä½¬ææ~)\n\n###
@@ -147,27 +149,27 @@
 æ°å¢æ¯æå¾çè¾åº\n\n### 0.1.0--2022.1.4\n\n- éä¸­ä¿®å¤äºBug\n\n###
 0.0.9--2022.1.4\n\n-
 æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­\n-
 ä¿®å¤ä¸­æåä¹±ç é®é¢\n\n### 0.0.8--2022.1.4\n\n-
 æ¯ævpkæ ¼å¼å°å¾\n- æ¯ææ¥çæævpkæ ¼å¼æä»¶\n\n### 0.0.6--
 2022.1.3\n\n- ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç \n\n### 0.0.1--
 2022.1.3\n\n- æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾\n\n\n\n## ð
-å¶ä»\n\n+
+å¶ä»\n\n-
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr\n+ å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [GPL-3.0 License]
+& Pr\n- å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n-
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n- [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)\n \n\n## ð æè°¢\n\n- [nonebot2]
-(https://github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶\n-
-[ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
-æ°æ®åºçåæ³æ¥èªäºä»\n- [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Agnes4m/VSQ)(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq) -
+[@Agnes4m](https://github.com/Agnes4m)\n\n## ð æè°¢\n\n- [nonebot2](https:
+//github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶\n- [ä¿®ä»]
+(https://github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè\n- ~~
+[èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
+(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq)-
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q](https://github.com/
-MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å©\n- [ç¾¤èå­¦ä¹ ](https:/
-/github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
-webæ§å¶å°çåæ³æ¥èªäºä»\n- [gsuid](https://github.com/KimigaiiWuyi/
-GenshinUID) - readmeåwikiçæ ¼å¼åè\n- åå -
-æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n', 'author': 'Agnes_Digital',
+MeetWq/mybot)- æå¡å¨å¾çåè\n- [ç¾¤èå­¦ä¹ ](https://github.com/
+CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè\n-
+[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè\n- [gsuid]
+(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè\n-
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n', 'author': 'Agnes_Digital',
 'author_email': 'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
 'packages': packages, 'package_data': package_data, 'install_requires':
 install_requires, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.8/PKG-INFO` & `nonebot_plugin_l4d2_server-0.4.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.4.8
+Version: 0.4.9
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
+Requires-Dist: h11 (>=0.14.0,<0.15.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
@@ -50,14 +51,15 @@
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
+
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
         <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
         <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
 </div><br>
 <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
@@ -73,58 +75,53 @@
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
     <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
 </a>
     <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
-</div>
 
+</div>
 
 ## 快速使用（env示例）
+
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
     l4_master = ['1145149191']            # 允许上传地图的qq号
     l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
     l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
     l4_port = ['20715']                   # 服务器端口
     l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
     l4_font = 'simsun.ttc'                # 服务器字体
     l4_web = True                         # 网页控制台，默认是关闭
 
-
-
 ## 主要功能
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
 
-
 ## 如何获取key
 
 为了使得ip不被滥用，我采取这种方式管理。
 
 这并不影响正常使用，如果不需要可以忽略
 
 [点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
 如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
 
         l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
         l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
 
-
-
 ## 提交自己的服务器？
 
-**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**
-
-**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**
+__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__
 
+__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__
 
 新增一个json文件，格式如下,文件名与需要响应的指令一致
 
         {
         "呆呆": [
                 {
                 "id": 1,
@@ -136,193 +133,199 @@
                 "version": "战役",
                 "ip": "43.248.188.17:27032"
                 }
         ]
         }
 
 ## 🌐 默认服务器
-目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
+
+目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
-| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
 | 云 | anne电信服云服 | 东 | 27
-| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
-| 橘 | 橘希实香的小窝 | 橘希实香 | 14
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
+| 橘 | 橘希实香的小窝 | 橘希实香 | 21
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
 | 3ks | 为人民服务 | DK | 14
 
-
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.9--2022.4
+
+- 修复h11版本错误的bug
+- 重写了config，下个版本正式使用yaml替代env设置
+- 新增远程连接测试代码
+
 ### 0.4.8--2022.4.16
 
- - 新增重载ip
- - 修复了一些windows启动下奇奇怪怪的bug
+- 新增重载ip
+- 修复了一些windows启动下奇奇怪怪的bug
 
 ### 0.4.7--2022.4.13
 
- - 新增模式查询
- - 列表推导替换套娃循环
+- 新增模式查询
+- 列表推导替换套娃循环
 
 ### 0.4.6--2022.4.9
 
- - 显示无效服
- - 优化服务器排序算法（list.sort()天下第一）
- - 默认关闭web端
+- 显示无效服
+- 优化服务器排序算法（list.sort()天下第一）
+- 默认关闭web端
 
 ### 0.4.5--2022.4.9
 
 - 修bug（恼）
 
 ### 0.4.2--2022.4.9
 
- - 修复响应开头匹配出现的重大bug
- - 启用web端
- - web使用yaml管理，未来可能删除env配置
+- 修复响应开头匹配出现的重大bug
+- 启用web端
+- web使用yaml管理，未来可能删除env配置
 
 ### 0.4.1--2022.3
 
- - 修复rar压缩包命名错误
- - 更新了tag的参数读取方式
- - 确定了传文件私聊比群聊快速
- - 修复了电信服计算错误
+- 修复rar压缩包命名错误
+- 更新了tag的参数读取方式
+- 确定了传文件私聊比群聊快速
+- 修复了电信服计算错误
 
 ### 0.4.0--2022.3.27
 
- - 新增web控制台
- - 修复传图超时参数错误
- - 重写求生ip获取方法 ~ 数据库苦手 ~
- - 重写文档
- - 不再内置ip（毕竟ipv4都暴露太危险了）
+- 新增web控制台
+- 修复传图超时参数错误
+- 重写求生ip获取方法 ~ 数据库苦手 ~
+- 重写文档
+- 不再内置ip（毕竟ipv4都暴露太危险了）
 
 ### 0.3.7--2022.3
 
- - 新增三方下载网盘
- - 修复windows上传临时文件错误
- - 优化查服流程
- - 优化anne服随机功能
+- 新增三方下载网盘
+- 修复windows上传临时文件错误
+- 优化查服流程
+- 优化anne服随机功能
 
 ### 0.3.6--2022.3.10
 
- - 暂时关闭web端，后续修改
- - 优化图片显示
- - 修复了海量bug
- - 新增三方图查询
+- 暂时关闭web端，后续修改
+- 优化图片显示
+- 修复了海量bug
+- 新增三方图查询
 
 ### 0.3.5--2022.3.6
 
- - 新增ping查询（在ip里包括）
- - 新增api查询（未完成）
- - 修复了电信服查询绑定名字无法查询的错误
- - 新增了救援率的显示
- - 新增web端（未完成）
+- 新增ping查询（在ip里包括）
+- 新增api查询（未完成）
+- 修复了电信服查询绑定名字无法查询的错误
+- 新增了救援率的显示
+- 新增web端（未完成）
 
 ### 0.3.4--2022.3.1
 
- - 新增本地插件smx查询
- - 增加了三个内置群服
- - 修改了图片的UI,变好看了
- - 删减了部分图片和字体，使得轻量化
- - 修复了海量bug
- - 修复了python3.8中typing错误
+- 新增本地插件smx查询
+- 增加了三个内置群服
+- 修改了图片的UI,变好看了
+- 删减了部分图片和字体，使得轻量化
+- 修复了海量bug
+- 修复了python3.8中typing错误
 
 ### 0.3.3--2022.2.26
 
- - 重写协议，使用a2s库，同时解决win端不同报错无法输出
- - 重~抄~写服务器查询UI,解决了不好看的问题
- - 从win测试，解决了一些win特有的bug
- - 重写服务器查询~还得是json~
- - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
- - 新增批量查询服务器，不带参数则返回图片
+- 重写协议，使用a2s库，同时解决win端不同报错无法输出
+- 重~抄~写服务器查询UI,解决了不好看的问题
+- 从win测试，解决了一些win特有的bug
+- 重写服务器查询~还得是json~
+- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
+- 新增批量查询服务器，不带参数则返回图片
 
 ### 0.3.1--2022.2.22
 
- - 修复了路径识别为str对象的错误
- - 修复了初始化找不到文件的错误
- - 修复了路径拼接错误
- - 在win端成功测试，修复压缩包bug
- - 新增开关协程异步env设置
- - 测试rcon建立通讯
- - 实现切换路径查看地图和使用rcon指令
+- 修复了路径识别为str对象的错误
+- 修复了初始化找不到文件的错误
+- 修复了路径拼接错误
+- 在win端成功测试，修复压缩包bug
+- 新增开关协程异步env设置
+- 测试rcon建立通讯
+- 实现切换路径查看地图和使用rcon指令
 
 ### 0.3.0--2022.2.18
 
- - 修改了新的env配置，使得支持本地多服务器操作
- - 彻底解决了压缩包解压linux端的问题
- - 解决了win端默认gbk解码的错误
- - 解决rcon指令字体报错
+- 修改了新的env配置，使得支持本地多服务器操作
+- 彻底解决了压缩包解压linux端的问题
+- 解决了win端默认gbk解码的错误
+- 解决rcon指令字体报错
 
 ### 0.2.5--2022.2.10
 
- - 修复了依赖不足的bug
- - 更新了电信服战绩个人图片UI
- - 更新了批量服务器查看的UI
- - 修改了传文件为协程异步
- - 优化了部分rcon指令
- - ~tnd7z怎么不去死啊~使用pyunpack库解压7z
+- 修复了依赖不足的bug
+- 更新了电信服战绩个人图片UI
+- 更新了批量服务器查看的UI
+- 修改了传文件为协程异步
+- 优化了部分rcon指令
+- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
 
 ### 0.2.4--2022.2.8
 
- - 使用poetry修复了pip安装文件缺失的bug
+- 使用poetry修复了pip安装文件缺失的bug
 
 ### 0.2.3--2022.2.7
 
- - 新增坐牢和开牢
- - 修改了获取资源为异步协程却阻碍其他指令的bug
- - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
- - 喷剂制作开摆了，推测需要c/c++环境
- - 修改抽取文案
- - 新增查询服务器状态时返回connect ip
- - 修复了服务器查询无响应的时候，因为报错无回复信息的bug
- - 个人信息重置测试代码，下个版本更新
- - 新增求生更新添加和删除
+- 新增坐牢和开牢
+- 修改了获取资源为异步协程却阻碍其他指令的bug
+- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
+- 喷剂制作开摆了，推测需要c/c++环境
+- 修改抽取文案
+- 新增查询服务器状态时返回connect ip
+- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
+- 个人信息重置测试代码，下个版本更新
+- 新增求生更新添加和删除
 
 ### 0.2.2--2022.2.1
 
- - 新增探监
- - 新增喷漆制作
- - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
- - 修改了部分对话响应
+- 新增探监
+- 新增喷漆制作
+- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
+- 修改了部分对话响应
 
 ### 0.2.1--2022.1.25
 
- - 新增电信服获取（东哥的肯定）
- - 优化图片UI 
- - 新增云服快捷查询
- - 修复了因为没用玩家，导致的服务器状态查询错误
- - 新增电信服ip爬取（仅仅作为单次更新ip列表）
+- 新增电信服获取（东哥的肯定）
+- 优化图片UI
+- 新增云服快捷查询
+- 修复了因为没用玩家，导致的服务器状态查询错误
+- 新增电信服ip爬取（仅仅作为单次更新ip列表）
 
 ### 0.2.0--2022.1.21
 
- - 新增创意工坊查询
- - 优化查询图片UI
- - 新增创意工坊文件下载
- - 修复了因为电信服官网前端修改导致查询失败的BUG
+- 新增创意工坊查询
+- 优化查询图片UI
+- 新增创意工坊文件下载
+- 修复了因为电信服官网前端修改导致查询失败的BUG
 
 ### 0.1.7--2022.1.19
 
- - 新增群ip订阅，批量查询
- - 新增图片显示ip状态
- - 修复了因为玩家名字特殊字符导致的utf-8解码错误
- - 更新自己的第三方库VSQ==0.0.6
+- 新增群ip订阅，批量查询
+- 新增图片显示ip状态
+- 修复了因为玩家名字特殊字符导致的utf-8解码错误
+- 更新自己的第三方库VSQ==0.0.6
 
 ### 0.1.6--2022.1.15
 
- - 新增ip查询服务器提供玩家数量和名字
- - 增加协程函数修复因为加载顺序导致的错误
- - 更新自己的第三方库VSQ==0.0.4
+- 新增ip查询服务器提供玩家数量和名字
+- 增加协程函数修复因为加载顺序导致的错误
+- 更新自己的第三方库VSQ==0.0.4
 
 ### 0.1.5--2022.1.15
 
 - 新增服务器控制台指令，新增依赖rcon
 - 重新了数据库，不再使用json而是使用sql3
 - 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
 
@@ -372,24 +375,24 @@
 
 - 插件初次发布，可私聊添加地图
 
 </details>
 
 ## 🙈 其他
 
-+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
-+ 如果本插件对你有帮助，不要忘了点个Star~
-+ 本项目仅供学习使用，请勿用于商业用途
-+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
-        
+- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
+- 如果本插件对你有帮助，不要忘了点个Star~
+- 本项目仅供学习使用，请勿用于商业用途
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
 
 ## 🌐 感谢
 
-- [nonebot2](https://github.com/nonebot/nonebot2) - 聊天机器人的基础框架
-- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
-- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
-- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
-  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
-- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
-- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
-- 呆呆 - 提供三方地图的详细数据
+- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
+- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
+- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
+- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
+  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
+- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
+- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
+- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
+- 呆呆- 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.9 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
 (>=3.8.3,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
-asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: httpx
-(>=0.23.3,<0.24.0) Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist:
-jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist:
-nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler
-(>=0.2.0,<0.3.0) Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
-Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
-Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
-Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose
-(>=3.3.0,<4.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist:
-rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
-ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
-Description-Content-Type: text/markdown
+asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: h11
+(>=0.14.0,<0.15.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: jieba
+(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-
+Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
+nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
+patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
+python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
+(>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
+Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
@@ -51,30 +52,32 @@
 è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
 (https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
 å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
 l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
 l4_key = 'qwertyuiopasdfg' #
 è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
 æäº¤èªå·±çæå¡å¨ï¼
-**æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip**
-**é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip**
+__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__
+__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
 { "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
-é»è®¤æå¡å¨ ç®å **å·²ææ**
+é»è®¤æå¡å¨ ç®å __å·²ææ__
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
-27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
-3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
+ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ |
+27 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
+21 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³
+| 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
 | 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
-0.4.8--2022.4.16 - æ°å¢éè½½ip -
+0.4.9--2022.4 - ä¿®å¤h11çæ¬éè¯¯çbug -
+éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
+æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
 ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
 æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
 æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
 é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
 ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
@@ -147,23 +150,23 @@
 - æ°å¢æ¯æå¾çè¾åº - æ°å¢æ¥è¯¢anneææ°æ® ### 0.1.1--2022.1.5 -
 æ°å¢å é¤å°å¾ - æ°å¢å°å¾æ¹å - æ°å¢æ¯æå¾çè¾åº ### 0.1.0--
 2022.1.4 - éä¸­ä¿®å¤äºBug ### 0.0.9--2022.1.4 -
 æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­ -
 ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
-æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
+æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» -
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
+& Pr - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
 [@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
-github.com/nonebot/nonebot2) - èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:
-//github.com/s52047qwas/nonebot_plugin_xiuxian) -
-æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
+github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:/
+/github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè - ~~
+[èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
+(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
 éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
-MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
-github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
-webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
-GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
-æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
+MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
+CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
+[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
+(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
```

