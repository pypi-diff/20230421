# Comparing `tmp/nonebot_plugin_bilichat-1.4.1.tar.gz` & `tmp/nonebot_plugin_bilichat-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.4.1.tar", last modified: Thu Apr 20 03:15:16 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.5.0.tar", last modified: Fri Apr 21 16:46:38 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.4.1.tar` & `nonebot_plugin_bilichat-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    34523 2023-04-20 03:15:06.033037 nonebot_plugin_bilichat-1.4.1/LICENSE
--rw-r--r--   0        0        0    10989 2023-04-20 03:15:06.033037 nonebot_plugin_bilichat-1.4.1/README.md
--rw-r--r--   0        0        0     7289 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4611 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4592 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4657 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2854 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      893 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-20 03:15:06.041037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5573 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4388 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2342 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-20 03:15:06.045037 nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-04-20 03:15:16.561197 nonebot_plugin_bilichat-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    12278 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-21 16:46:25.797468 nonebot_plugin_bilichat-1.5.0/LICENSE
+-rw-r--r--   0        0        0    11167 2023-04-21 16:46:25.797468 nonebot_plugin_bilichat-1.5.0/README.md
+-rw-r--r--   0        0        0     7289 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4809 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4657 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      893 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5681 2023-04-21 16:46:25.805468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4856 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2359 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1764 2023-04-21 16:46:25.809468 nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-04-21 16:46:38.373550 nonebot_plugin_bilichat-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    12456 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.4.1/LICENSE` & `nonebot_plugin_bilichat-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/README.md` & `nonebot_plugin_bilichat-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,19 @@
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-bilichat[all]
+    nb plugin install nonebot-plugin-bilichat
+
+注: 由于 nb-cli 不支持依赖组，因此需要启用词云和AI总结的用户要通过其他的包管理器安装额外的依赖
+
+    pip install nonebot-plugin-bilichat[all]
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
```

#### html2text {}

```diff
@@ -16,29 +16,32 @@
 è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
 å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
 é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
 - ð¹ï¸ 7+
 Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
 ```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-bilichat[all]   pdm
-pdm add nonebot-plugin-bilichat[all]   poetry poetry add nonebot-plugin-
-bilichat[all]   conda conda install nonebot-plugin-bilichat[all]  æå¼
-nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®,
-éç½®åä¸º**éå¿é¡»é¡¹** ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bilichat_block | bool |
-False | æ¯å¦æ¦æªäºä»¶(é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | |
-bilichat_enable_private | bool | True | æ¯å¦åè®¸ååºç§è | |
-bilichat_enable_self | bool | False | æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | |
-bilichat_enable_v12_channel | bool | True | ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯
-(ob12ä¸å±)~~(ææªå®ç°) | | bilichat_enable_unkown_src | bool | False |
+install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
+pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
+nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
+poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
+plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
+æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
+### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
+|:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+(é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
+æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_v12_channel | bool | True
+| ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±)~~(ææªå®ç°) | |
+bilichat_enable_unkown_src | bool | False |
 æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
 | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,42 +86,48 @@
 
     @validator("bilichat_openai_token", always=True)
     def check_pypackage_openai(cls, v):
         if (importlib.util.find_spec("tiktoken_async") and importlib.util.find_spec("minidynamicrender")) or not v:
             return v
         else:
             raise RuntimeError(
-                "Package(s) of fuction openai summary not installed, use **nb plugin install nonebot-plugin-bilichat[openai]** to install required dependencies"
+                "Package(s) of fuction openai summary not installed, use **pip install nonebot-plugin-bilichat[openai]** to install required dependencies"
             )
 
     @validator("bilichat_newbing_cookie", always=True)
     def check_pypackage_newbing_and_cookie(cls, v):
         if not v:
             return v
         if not importlib.util.find_spec("EdgeGPT") or not importlib.util.find_spec("minidynamicrender"):
             raise RuntimeError(
-                "Package(s) of fuction newbing summary not installed, use **nb plugin install nonebot-plugin-bilichat[newbing]** to install required dependencies"
+                "Package(s) of fuction newbing summary not installed, use **pip install nonebot-plugin-bilichat[newbing]** to install required dependencies"
             )
 
         # verify cookie file
-        try:
-            if Path(v).is_file():
+        if Path(v).is_file():
+            try:
                 json.loads(Path(v).read_text("utf-8"))
-        except Exception as e:
-            raise ValueError("Config bilichat_newbing_cookie got a problem occurred") from e
+            except Exception as e:
+                raise ValueError("Config bilichat_newbing_cookie got a problem occurred") from e
+
+        elif Path(v).is_dir():
+            raise ValueError(f"Config bilichat_newbing_cookie requires a file, but {v} is a folder")
+
+        else:
+            raise ValueError(f"Path {v} is not recognized")
 
         return v
 
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
         if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
-                "Package(s) of fuction wordcloud not installed, use **nb plugin install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
+                "Package(s) of fuction wordcloud not installed, use **pip install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
             )
 
     def verify_permission(self, uid: Union[str, int]):
         if self.bilichat_whitelist:
             return str(uid) in self.bilichat_whitelist
         elif self.bilichat_blacklist:
             return str(uid) not in self.bilichat_blacklist
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,22 @@
 from bilireq.grpc.protos.bilibili.community.service.dm.v1.dm_pb2_grpc import DMStub
 from bilireq.grpc.utils import grpc_request
 from bilireq.utils import get, post
 from loguru import logger
 
 from bilireq.auth import Auth
 
-hc = httpx.AsyncClient()
+hc = httpx.AsyncClient(
+    headers={
+        "User-Agent": (
+            "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
+            "(KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.39"
+        )
+    }
+)
 Bili_Auth = Auth()
 
 
 async def relation_modify(uid: Union[str, int], act: int):
     """
     修改关系
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import random
 import re
 import string
-import random
 
 
 def num_fmt(num: int):
     if num < 10000:
         return str(num)
     elif num < 100000000:
         return ("%.2f" % (num / 10000)) + "万"
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,26 @@
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
 
 cookies = json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 logger.info("Try init bing chatbot")
+init = False
 for count in range(5):
     try:
         bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
         logger.success("Bing chatbot init success")
+        init = True
         break
-    except Exception:
-        logger.error(f"Bing chatbot init failed, retrying {count+1}/5")
+    except Exception as e:
+        logger.error(f"Bing chatbot init failed, retrying {count+1}/5: {e}")
+
+if not init:
+    raise RuntimeError("Bing chatbot init failed")
 
 
 def get_small_size_transcripts(title: str, text_data: List[str]):
     prompt = (
         "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”：\
         ## 概述\
         {内容，尽可能精简总结内容不要太详细}\
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,38 +4,37 @@
 from typing import Dict, List, Optional
 
 import httpx
 import tiktoken_async
 from loguru import logger
 
 from ..config import plugin_config
-from ..model.openai import AISummary
+from ..model.openai import OpenAI, TokenUsage
 
 if plugin_config.bilichat_openai_token:
     logger.info("Loading OpenAI Token enc model")
     tiktoken_enc = asyncio.run(tiktoken_async.encoding_for_model(plugin_config.bilichat_openai_model))
     logger.success(f"Enc model {tiktoken_enc.name} load successfully")
 
 
-def get_user_prompt(title: str, transcript: str) -> List[Dict[str, str]]:
+def get_summarise_prompt(title: str, transcript: str) -> List[Dict[str, str]]:
     title = title.replace("\n", " ").strip() if title else ""
     transcript = transcript.replace("\n", " ").strip() if transcript else ""
-    language = "Chinese"
-    sys_prompt = (
-        "Your output should use the following template:\n## 总结\n## 要点\n"
-        "- [Emoji] Bulletpoint\n\n"
-        "Your task is to summarise the video I have given you in up to 2 to 6 concise bullet points, "
-        "starting with a short highlight, each bullet point is at least 15 words. "
-        "Choose an appropriate emoji for each bullet point. "
-        "Use the video above: {{Title}} {{Transcript}}."
-        "If you think that the content in the transcript is meaningless, "
-        "Or if there is very little content that cannot be well summarized, "
-        "then you can simply output the two words 'no meaning'. Remember, not to output anything else."
+    return get_full_prompt(
+        prompt=(
+            "使用以下Markdown模板为我总结视频字幕数据，除非字幕中的内容无意义，或者内容较少无法总结，或者未提供字幕数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
+            "\n## 概述"
+            "\n{内容，尽可能精简总结内容不要太详细}"
+            "\n## 要点"
+            "\n- {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}"
+            "\n不要随意翻译任何内容。仅使用中文总结。"
+            "\n不说与总结无关的其他内容，你的回复仅限固定格式提供的“概述”和“要点”两项。"
+            f"\n视频标题名称为“{title}”，视频字幕数据如下，立刻开始总结：“{transcript}”"
+        )
     )
-    return get_full_prompt(f'Title: "{title}"\nTranscript: "{transcript}"', sys_prompt, language)
 
 
 def count_tokens(prompts: List[Dict[str, str]]):
     """根据内容计算 token 数"""
 
     if plugin_config.bilichat_openai_model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4
@@ -55,56 +54,67 @@
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
 def get_small_size_transcripts(text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit):
     unique_texts = list(OrderedDict.fromkeys(text_data))
-    while count_tokens(get_user_prompt("", " ".join(unique_texts))) > token_limit:
+    while count_tokens(get_summarise_prompt("", " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
-def get_full_prompt(prompt: str, system: Optional[str] = None, language: Optional[str] = None):
+def get_full_prompt(prompt: Optional[str] = None, system: Optional[str] = None, language: Optional[str] = None):
     plist: List[Dict[str, str]] = []
     if system:
         plist.append({"role": "system", "content": system})
-    plist.append({"role": "user", "content": prompt})
+    if prompt:
+        plist.append({"role": "user", "content": prompt})
     if language:
         plist.extend(
             (
                 {
                     "role": "assistant",
                     "content": "What language do you want to output?",
                 },
                 {"role": "user", "content": language},
             )
         )
+    if not plist:
+        raise ValueError("No prompt provided")
     return plist
 
 
 async def openai_req(
     prompt_message: List[Dict[str, str]],
     token: Optional[str] = plugin_config.bilichat_openai_token,
     model: str = plugin_config.bilichat_openai_model,
-) -> AISummary:
+    temperature: Optional[float] = None,
+):
+    if not token:
+        return OpenAI(error=True, message="未配置 OpenAI API Token")
     async with httpx.AsyncClient(
-        proxies=plugin_config.bilichat_openai_proxy,  # type: ignore
+        proxies=plugin_config.bilichat_openai_proxy,
         headers={
             "Authorization": f"Bearer {token}",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)"
             " Chrome/110.0.0.0 Safari/537.36 Edg/110.0.1587.69",
         },
         timeout=100,
     ) as client:
-        req = await client.post(
-            "https://api.openai.com/v1/chat/completions",
-            json={
-                "model": model,
-                "messages": prompt_message,
-            },
-        )
+        data = {
+            "model": model,
+            "messages": prompt_message,
+        }
+        if temperature:
+            data["temperature"] = temperature
+        req = await client.post("https://api.openai.com/v1/chat/completions", json=data)
         if req.status_code != 200:
-            return AISummary(error=True, message=req.text, raw=req.json())
+            return OpenAI(error=True, message=req.text, raw=req.json())
         logger.info(f"[OpenAI] Response:\n{req.json()['choices'][0]['message']['content']}")
-        logger.info(f"[OpenAI] Response token usage: {req.json()['usage']}")
-        return AISummary(summary=req.json()["choices"][0]["message"]["content"], raw=req.json())
+        usage = req.json()["usage"]
+        logger.info(f"[OpenAI] Response 实际 token 消耗: {usage}")
+        return OpenAI(
+            response=req.json()["choices"][0]["message"]["content"],
+            raw=req.json(),
+            token_usage=TokenUsage(**usage),
+        )
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import re
 from typing import List
 
 from loguru import logger
 
-from .openai import get_small_size_transcripts, get_user_prompt, openai_req
-from .text_to_image import rich_text2image
+from ..config import plugin_config
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
-from ..config import plugin_config
+from .openai import get_small_size_transcripts, get_summarise_prompt, openai_req
+from .text_to_image import rich_text2image
 
 
 async def subtitle_summarise(title: str, sub: List[str]):
     small_size_transcripts = get_small_size_transcripts(sub)
-    prompt = get_user_prompt(title, small_size_transcripts)
+    prompt = get_summarise_prompt(title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
 async def column_summarise(cv_title: str, cv_text: str):
     sentences = re.split(r"[，。；,.;\n]+", cv_text)
     small_size_transcripts = get_small_size_transcripts(sentences)
-    prompt = get_user_prompt(cv_title, small_size_transcripts)
+    prompt = get_summarise_prompt(cv_title, small_size_transcripts)
     logger.debug(prompt)
     return await openai_req(prompt)
 
 
 async def openai_summarization(cache: Cache, cid: str = "0"):
     try:
         if not cache.episodes[cid].openai:
             if cache.id[:2].lower() in ["bv", "av"]:
                 ai_summary = await subtitle_summarise(cache.title, cache.episodes[cid].content)
             elif cache.id[:2].lower() == "cv":
                 ai_summary = await column_summarise(cache.title, cache.episodes[cid].content[0])
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
-            if ai_summary.summary:
-                cache.episodes[cid].openai = ai_summary.summary
+            if ai_summary.response:
+                cache.episodes[cid].openai = ai_summary.response
                 cache.save()
             else:
                 logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
                 return f"视频(专栏) {cache.id} 总结失败: {ai_summary.raw}"
         if img := await rich_text2image(cache.episodes[cid].openai or "视频无法总结", plugin_config.bilichat_openai_model):
             return img
         else:
```

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.4.1/pyproject.toml` & `nonebot_plugin_bilichat-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.4.1"
+version = "1.5.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.4.1/PKG-INFO` & `nonebot_plugin_bilichat-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.4.1
+Version: 1.5.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -123,15 +123,19 @@
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
-    nb plugin install nonebot-plugin-bilichat[all]
+    nb plugin install nonebot-plugin-bilichat
+
+注: 由于 nb-cli 不支持依赖组，因此需要启用词云和AI总结的用户要通过其他的包管理器安装额外的依赖
+
+    pip install nonebot-plugin-bilichat[all]
 
 </details>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.4.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.5.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -34,29 +34,32 @@
 è½ææ²çº¿ç¨éäº8+ï¼ä½ä¸­ä½é¢æ®µè½ææ°´å¹³ç¸åã - ð°
 å¦æç»ç«¯æºä»·æ ¼åå°1500-2000åï¼ç«äºåè¿æ¯å¾è¶³çã - ð§ª
 é«éèªå·±ä¹æè¯å°éªé¾7ç³»åçç«äºåé®é¢ï¼è¿ä¹ä½¿å¶æäºå¿é¡»è¦è§£å³çä¸ä¸ªé®é¢ã
 - ð¹ï¸ 7+
 Gen2å°±æ¯8+çCPUï¼æè°è§æ ¼ä¸æ¾ï¼æå¤§çåçèæ¯å¤§åæ¸¸æã
 ```  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install nonebot-plugin-bilichat[all]   pdm
-pdm add nonebot-plugin-bilichat[all]   poetry poetry add nonebot-plugin-
-bilichat[all]   conda conda install nonebot-plugin-bilichat[all]  æå¼
-nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®,
-éç½®åä¸º**éå¿é¡»é¡¹** ### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | bilichat_block | bool |
-False | æ¯å¦æ¦æªäºä»¶(é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | |
-bilichat_enable_private | bool | True | æ¯å¦åè®¸ååºç§è | |
-bilichat_enable_self | bool | False | æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | |
-bilichat_enable_v12_channel | bool | True | ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯
-(ob12ä¸å±)~~(ææªå®ç°) | | bilichat_enable_unkown_src | bool | False |
+install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
+pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
+nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
+poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
+plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
+æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_bilichat"]  ## âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®, éç½®åä¸º**éå¿é¡»é¡¹**
+### éç¨éç½®é¡¹ | éç½®é¡¹ | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:
+|:----:|:----:| | bilichat_block | bool | False | æ¯å¦æ¦æªäºä»¶
+(é²æ­¢å¶ä»æä»¶äºæ¬¡è§£æ) | | bilichat_enable_private | bool | True |
+æ¯å¦åè®¸ååºç§è | | bilichat_enable_self | bool | False |
+æ¯å¦åè®¸ååºèªèº«çæ¶æ¯ | | bilichat_enable_v12_channel | bool | True
+| ~~æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±)~~(ææªå®ç°) | |
+bilichat_enable_unkown_src | bool | False |
 æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist | list[str] | []
 | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | | bilichat_blacklist
 | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
 (é²æ­¢å·å±) | | bilichat_neterror_retry | int | 3 |
 å¯¹é¨åç½ç»è¯·æ±éè¯¯çå°è¯æ¬¡æ° | | bilichat_use_bcut_asr | bool |
```

