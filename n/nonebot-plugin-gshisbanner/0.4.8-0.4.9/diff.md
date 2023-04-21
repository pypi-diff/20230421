# Comparing `tmp/nonebot_plugin_gshisbanner-0.4.8.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.9.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.4.8.tar` & `nonebot_plugin_gshisbanner-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/LICENSE
--rw-r--r--   0        0        0     4443 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/README.md
--rw-r--r--   0        0        0      389 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      406 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      292 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3663 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1182 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4509 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2654 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      576 2023-04-15 09:47:53.664856 nonebot_plugin_gshisbanner-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     5136 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/LICENSE
+-rw-r--r--   0        0        0     4580 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/README.md
+-rw-r--r--   0        0        0      389 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      406 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      292 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3663 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1182 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     4637 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2654 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      576 2023-04-21 15:30:20.920371 nonebot_plugin_gshisbanner-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     5273 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.9/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.4.8/LICENSE` & `nonebot_plugin_gshisbanner-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.8/README.md` & `nonebot_plugin_gshisbanner-0.4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,20 +48,25 @@
 # 单次合并转发消息长度（int）,默认为10
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
-·· 1."banners.52v6.com/data" #默认
-·· 2."genshin-gacha-banners.vercel.app/data" #vercel代理，国内可能无法直连
-·· 3."genshin-gacha-banners.52v6.com/data" #cloudfare代理，可能会被墙
+·· 1."banners.52v6.com/data" 
+     #默认
+·· 2."genshin-gacha-banners.vercel.app/data" 
+     #vercel代理，国内可能无法直连
+·· 3."genshin-gacha-banners.52v6.com/data" 
+     #cloudfare代理，可能会被墙
 ·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
+·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
+     ##jsdelivr代理的文件，大多数情况可用
 ```
 
 ## 🎉 使用
 ### 指令表
 |        指令         |    权限    | 需要@ | 范围 |                             说明                             |
 | :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
 | [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
```

#### html2text {}

```diff
@@ -17,18 +17,19 @@
 1."banners.52v6.com/data" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app/
 data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
 banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/
 https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha"
 ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
-(éè¦æ¯æhttps) ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | | :-----------------: | :--------: | :---: | :--: |
-:----------------------------------------------------------: | |
-[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+(éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
+gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ ``` ## ð ä½¿ç¨ ###
+æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-----------------:
+| :--------: | :---: | :--: | :------------------------------------------------
+----------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

### Comparing `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/deal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     event: MessageEvent,
     regex_dict: dict = RegexDict(),
 ):
     type_name = regex_dict["name"]
     types = ["character", "weapon"]
     if type_name == "历史卡池":
         for i in types:
-            url = f"https://{config.gshisbanner_json_url}/data/{i}.json"
+            url = f"https://{config.gshisbanner_json_url}/{i}.json"
             path = gacha_info_path / f"{i}.json"
             result = await load_json_from_url(url, path, True)
             if not result:
                 await refresh.finish(f"刷新{type_name}失败,可能是网络问题或api失效")
             save_json(result, path)
             logger.info(f"{i}.json文件保存成功")
     elif type_name == "别名":
@@ -114,14 +114,16 @@
 async def init_group_card():
     if not gacha_info_path.exists():
         gacha_info_path.mkdir(parents=True)
     url = (
         "https://ghproxy.com/https://raw.githubusercontent.com/forchannot/nonebot-plugin-gshisbanner/main/data"
         "/genshin_history/alias.json"
     )
+    # url = "https://fastly.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json"
+    # 备用
     try:
         resp = await get(url)
     except Exception as e:
         logger.warning(f"alias.json文件下载失败,错误信息:{e}")
         return False
     if resp.status_code != 200:
         logger.warning("alias.json文件下载失败")
```

### Comparing `nonebot_plugin_gshisbanner-0.4.8/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.4.9/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.8/pyproject.toml` & `nonebot_plugin_gshisbanner-0.4.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "0.4.8"
+version = "0.4.9"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_gshisbanner-0.4.8/PKG-INFO` & `nonebot_plugin_gshisbanner-0.4.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.4.8
+Version: 0.4.9
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -67,20 +67,25 @@
 # 单次合并转发消息长度（int）,默认为10
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
-·· 1."banners.52v6.com/data" #默认
-·· 2."genshin-gacha-banners.vercel.app/data" #vercel代理，国内可能无法直连
-·· 3."genshin-gacha-banners.52v6.com/data" #cloudfare代理，可能会被墙
+·· 1."banners.52v6.com/data" 
+     #默认
+·· 2."genshin-gacha-banners.vercel.app/data" 
+     #vercel代理，国内可能无法直连
+·· 3."genshin-gacha-banners.52v6.com/data" 
+     #cloudfare代理，可能会被墙
 ·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
      ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
+·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
+     ##jsdelivr代理的文件，大多数情况可用
 ```
 
 ## 🎉 使用
 ### 指令表
 |        指令         |    权限    | 需要@ | 范围 |                             说明                             |
 | :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
 | [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.9 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
@@ -27,18 +27,19 @@
 1."banners.52v6.com/data" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app/
 data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
 banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/
 https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha"
 ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
-(éè¦æ¯æhttps) ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
-éè¦@ | èå´ | è¯´æ | | :-----------------: | :--------: | :---: | :--: |
-:----------------------------------------------------------: | |
-[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+(éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
+gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ ``` ## ð ä½¿ç¨ ###
+æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-----------------:
+| :--------: | :---: | :--: | :------------------------------------------------
+----------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

