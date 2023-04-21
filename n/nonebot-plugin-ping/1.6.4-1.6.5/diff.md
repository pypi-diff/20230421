# Comparing `tmp/nonebot_plugin_ping-1.6.4.tar.gz` & `tmp/nonebot_plugin_ping-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ping-1.6.4.tar", last modified: Thu Apr 20 00:01:38 2023, max compression
+gzip compressed data, was "nonebot_plugin_ping-1.6.5.tar", last modified: Fri Apr 21 00:56:32 2023, max compression
```

## Comparing `nonebot_plugin_ping-1.6.4.tar` & `nonebot_plugin_ping-1.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.354305 nonebot_plugin_ping-1.6.4/
--rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.4/LICENSE
--rw-rw-rw-   0        0        0     1659 2023-04-20 00:01:38.349371 nonebot_plugin_ping-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.339242 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/
--rw-rw-rw-   0        0        0     4392 2023-04-19 23:48:09.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:01:38.349371 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/
--rw-rw-rw-   0        0        0     1659 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-20 00:01:38.000000 nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 00:01:38.354305 nonebot_plugin_ping-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     3944 2023-04-19 23:59:42.000000 nonebot_plugin_ping-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/
+-rw-rw-rw-   0        0        0     1088 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0     1659 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-02-03 08:23:04.000000 nonebot_plugin_ping-1.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.350281 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/
+-rw-rw-rw-   0        0        0     3674 2023-04-21 00:55:53.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:56:32.354335 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/
+-rw-rw-rw-   0        0        0     1659 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-21 00:56:32.000000 nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 00:56:32.357589 nonebot_plugin_ping-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     3944 2023-04-21 00:56:03.000000 nonebot_plugin_ping-1.6.5/setup.py
```

### Comparing `nonebot_plugin_ping-1.6.4/LICENSE` & `nonebot_plugin_ping-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.4/PKG-INFO` & `nonebot_plugin_ping-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_ping
-Version: 1.6.4
+Version: 1.6.5
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.4/README.md` & `nonebot_plugin_ping-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ping-1.6.4/nonebot_plugin_ping/__init__.py` & `nonebot_plugin_ping-1.6.5/nonebot_plugin_ping/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import platform
 
 try:
     model: int = nonebot.get_driver().config.ping
 except:
     model: int = 1
 
-from .httpcat import httpcat_msgs
-
 
 
 """PING网址"""
 ping = on_command('ping', aliases={'Ping'}, priority=60, block=True)
 @ping.handle()
 async def _(msg: Message = CommandArg()):
     url = msg.extract_plain_text().strip()
@@ -100,25 +98,8 @@
             email = (res["data"]["owner_email"])
             regtime = (res["data"]["create_date"])
             exptime = (res["data"]["expire_date"])
             dnsserver = (res["data"]["nameserver"])
             status = (res["data"]["status"])
             updatetime = (res["data"]["update_date"])
             res = f"请求域名: {url}\n注册商: {reg}\n邮箱: {email}\n注册时间: {regtime}\n过期时间: {exptime}\nDNS服务器: {dnsserver}\n域名状态: {status}\n更新时间: {updatetime}"
-            return res
-
-
-
-http_cat = on_command('http_cat', aliases={'httpcat','http猫'}, priority=5, block=True)
-@http_cat.handle()
-async def _handle(code: Message = CommandArg()):
-    url = "https://httpcats.com/{}.jpg".format(code)
-    msgs = await httpcat_msgs('http://www.httpstatus.cn/{}'.format(code))  
-    await http_cat.finish(msgs + MessageSegment.image(file=url, cache=False), at_sender=True)
-#httpx异步 await httpcat_msg(code)
-async def httpcat_msg(code):
-    msgs = await httpcat_msgs('http://www.httpstatus.cn/{}'.format(code))
-    return msgs
-#url同步 httpcat_pic(code)
-def httpcat_pic(code):
-    url = "https://httpcats.com/{}.jpg".format(code)
-    return str(url)
+            return res
```

### Comparing `nonebot_plugin_ping-1.6.4/nonebot_plugin_ping.egg-info/PKG-INFO` & `nonebot_plugin_ping-1.6.5/nonebot_plugin_ping.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ping
-Version: 1.6.4
+Version: 1.6.5
 Summary: ping
 Home-page: https://github.com/zhulinyv/nonebot_plugin_ping
 Author: (๑•小丫头片子•๑)
 Author-email: zhulinyv2005@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_ping-1.6.4/setup.py` & `nonebot_plugin_ping-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_ping'
 DESCRIPTION = 'ping'
 URL = 'https://github.com/zhulinyv/nonebot_plugin_ping'
 EMAIL = 'zhulinyv2005@outlook.com'
 AUTHOR = '(๑•小丫头片子•๑)'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.6.4'
+VERSION = '1.6.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'nonebot2', 'nonebot-adapter-onebot', 'httpx',
 ]
 
 # What packages are optional?
```

