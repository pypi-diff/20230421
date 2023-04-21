# Comparing `tmp/nonebot_api_paddle-1.0.2.tar.gz` & `tmp/nonebot_api_paddle-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_api_paddle-1.0.2.tar", last modified: Thu Apr  6 15:26:30 2023, max compression
+gzip compressed data, was "nonebot_api_paddle-1.0.3.tar", last modified: Fri Apr 21 15:52:16 2023, max compression
```

## Comparing `nonebot_api_paddle-1.0.2.tar` & `nonebot_api_paddle-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 15:26:30.081319 nonebot_api_paddle-1.0.2/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_api_paddle-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       18 2023-04-06 15:09:22.000000 nonebot_api_paddle-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      858 2023-04-06 15:26:30.080322 nonebot_api_paddle-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-06 14:52:18.000000 nonebot_api_paddle-1.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-06 15:26:30.072349 nonebot_api_paddle-1.0.2/nonebot_api_paddle/
--rw-rw-rw-   0        0        0     5430 2023-04-06 15:24:09.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-04-06 12:04:09.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_excel.py
--rw-rw-rw-   0        0        0     2410 2023-04-06 07:39:32.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_ocr.py
--rw-rw-rw-   0        0        0     2314 2023-04-06 15:21:19.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_voice.py
-drwxrwxrwx   0        0        0        0 2023-04-06 15:26:30.079325 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/
--rw-rw-rw-   0        0        0      858 2023-04-06 15:26:30.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-04-06 15:26:30.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 15:26:30.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-04-06 15:26:30.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-06 15:26:30.000000 nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 15:26:30.081319 nonebot_api_paddle-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1246 2023-04-06 15:26:16.000000 nonebot_api_paddle-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:52:16.369432 nonebot_api_paddle-1.0.3/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_api_paddle-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       18 2023-04-06 15:09:22.000000 nonebot_api_paddle-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      858 2023-04-21 15:52:16.368431 nonebot_api_paddle-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-04-06 14:52:18.000000 nonebot_api_paddle-1.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 15:52:16.362432 nonebot_api_paddle-1.0.3/nonebot_api_paddle/
+-rw-rw-rw-   0        0        0     5451 2023-04-21 15:44:47.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle/__init__.py
+-rw-rw-rw-   0        0        0     3280 2023-04-20 15:43:17.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_excel.py
+-rw-rw-rw-   0        0        0     2329 2023-04-20 15:24:32.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_ocr.py
+-rw-rw-rw-   0        0        0     2434 2023-04-20 15:26:30.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_voice.py
+drwxrwxrwx   0        0        0        0 2023-04-21 15:52:16.367432 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/
+-rw-rw-rw-   0        0        0      858 2023-04-21 15:52:16.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-04-21 15:52:16.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 15:52:16.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-04-21 15:52:16.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-21 15:52:16.000000 nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 15:52:16.369432 nonebot_api_paddle-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2023-04-21 15:51:19.000000 nonebot_api_paddle-1.0.3/setup.py
```

### Comparing `nonebot_api_paddle-1.0.2/LICENSE.txt` & `nonebot_api_paddle-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_api_paddle-1.0.2/PKG-INFO` & `nonebot_api_paddle-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_api_paddle
-Version: 1.0.2
+Version: 1.0.3
 Summary: nonbot_api_paddle
 Home-page: https://github.com/canxin121/nonebot_api_paddle
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot_api_paddle-1.0.2/nonebot_api_paddle/__init__.py` & `nonebot_api_paddle-1.0.3/nonebot_api_paddle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     getmsg = event.get_message()
     for segment in getmsg:
         if segment.type == 'image':
             await ocr_api.send("正在识别~~")
             url = segment.data['url']
             response = urllib.request.urlopen(url)
             img = io.BytesIO(response.read())
-            resulttext = api_paddle_ocr(img=img)
+            resulttext = await api_paddle_ocr(img=img)
             await ocr_api.reject(resulttext)
         elif segment.type == 'text':
             if getmsg[0].data['text'] == '/结束':
                 await ocr_api.finish("关闭ocr识别模式")
             else:
                 await ocr_api.send("请发送纯图片，如要结束，请发送/结束")
 
@@ -68,21 +68,21 @@
 voice_api = on_keyword({*voice_keyword_config_},rule=_tome_)
 
 
 @voice_api.handle()
 async def handlevoice(bot: Bot, event: Event, state: T_State):
     if bool(event.reply):
         text = event.reply.message[0].data['text']
-        url = getvoice(text)
+        url = await getvoice(text)
         record = MessageSegment.record(file=url)
         await voice_api.finish(record)
     else:
         text = event.get_plaintext()
         text = text.replace('/转语音', '').replace('/说', '')
-        url = getvoice(text)
+        url = await getvoice(text)
         record = MessageSegment.record(file=url)
         await voice_api.finish(record)
 
 
 
 ##############################
 try:
@@ -95,22 +95,22 @@
 
 excel_api = on(rule=(excel_command&_tome_))
 
 @excel_api.handle()
 async def handle_apiexcel(bot: Bot, event: Event, state: T_State):
     await excel_api.send("开始apiexcel识别模式")
 
-@excel_api.got("pic")
+@excel_api.got("")
 async def get_pic(bot: Bot, event: Event, state: T_State):
     getmsg = event.get_message()
     for segment in getmsg:
         if segment.type == 'image':
             await excel_api.send("正在识别~~")
             url = segment.data['url']
-            resulttext,filename= api_paddle_apiexcel(url)
+            resulttext,filename= await api_paddle_apiexcel(url)
             await excel_api.send(resulttext)
             filepath = os.path.dirname(os.path.realpath(__file__)) + r'\temp.xlsx'
             if isinstance(event, GroupMessageEvent) or isinstance(event, GroupUploadNoticeEvent):
                 await bot.call_api('upload_group_file', group_id= event.group_id, name=f'{filename}.xlsx', file=filepath)
                 await excel_api.reject()
             else:
                 await bot.call_api('upload_private_file', user_id= event.user_id, name=f'{filename}.xlsx', file=filepath)
```

### Comparing `nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_excel.py` & `nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_excel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import requests
-import json
+import aiohttp
+import asyncio
 import base64
-from PIL import Image
+import json
+import os
 from io import BytesIO
-from html.parser import HTMLParser
-import pandas as pd
-from io import StringIO
 from openpyxl import Workbook
-import os
-def html2excel(html):
+from PIL import Image
+from html.parser import HTMLParser
+
+
+async def html2excel(html):
     class MyHTMLParser(HTMLParser):
         def __init__(self):
             super().__init__()
             self.data = []
             self.row = []
-            self.in_td = False
 
         def handle_starttag(self, tag, attrs):
             if tag == 'td':
                 self.in_td = True
 
         def handle_endtag(self, tag):
             if tag == 'td':
@@ -26,67 +26,62 @@
             elif tag == 'tr':
                 self.data.append(self.row)
                 self.row = []
 
         def handle_data(self, data):
             if self.in_td:
                 self.row.append(data.strip())
+
     parser = MyHTMLParser()
     parser.feed(html)
     data = '\n'.join(['\t'.join(row) for row in parser.data])
     return data
 
-def api_paddle_apiexcel(image_url):
-    # Download and encode image
-    response = requests.get(image_url)
-    img = Image.open(BytesIO(response.content))
-    buffered = BytesIO()
-    img.save(buffered, format="JPEG")
-    img_str = base64.b64encode(buffered.getvalue()).decode('utf-8')
-
-    # Set request data
-    data = {
-        "session_hash": "75mq6m01qy4",
-        "fn_index": 0,
-        "data": [
-            f"data:image/jpeg;base64,{img_str}"
-        ]
-    }
-
-    # Set request headers
-    headers = {
-        'Content-Type': 'application/json',
-        'Origin': 'https://aistudio.baidu.com',
-        'Accept-Encoding': 'gzip, deflate, br',
-        'Cookie': '__bsi=10291592389384054246_00_34_N_R_16_0303_cca8_Y; IMG_WH=428_746; SE_LAUNCH=5%3A1680744441_31%3A28012407_49%3A28012719; PSCBD=31%3A1; BA_HECTOR=2kaha10la18l2104012l8h8v1i2s7vr1m; H_WISE_SIDS=219946_234020_131861_216852_213347_214806_219942_213035_230186_204906_',
-        'Connection': 'keep-alive',
-        'Accept': '*/*',
-        'User-Agent': 'Mozilla/5.0 (iPhone; CPU iPhone OS 16_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Mobile/15E148 Safari/604.1',
-        'Referer': 'https://aistudio.baidu.com/serving/app/23/?__theme=light',
-        'Content-Length': '195430',
-        'Accept-Language': 'zh-CN,zh-Hans;q=0.9'
-    }
-
-    # Set request URL
-    url = 'https://aistudio.baidu.com/serving/app/23/run/predict/'
-
-    # Make POST request
-    response = requests.post(url, headers=headers, data=json.dumps(data))
-    jsons = json.loads(response.text)
-    result = jsons["data"][0]
-    data_excel = html2excel(result)
-    # Return response text
-    
-    # 将字符串转换为列表
-    lines = data_excel.strip().split('\n')
-    lst = [line.split('\t') for line in lines]
-    # 创建一个新的工作簿和工作表
-    wb = Workbook()
-    ws = wb.active
-    # 写入每一行
-    for row in lst:
-        ws.append(row)
-    #filepath
-    filepath = os.path.dirname(os.path.realpath(__file__)) + r'\temp.xlsx'
-    # 保存文件
-    wb.save(filepath)
-    return data_excel,lst[0][0]
+
+async def api_paddle_apiexcel(image_url):
+    async with aiohttp.ClientSession() as session:
+        async with session.get(image_url) as response:
+            img = Image.open(BytesIO(await response.read()))
+            buffered = BytesIO()
+            img = img.convert('RGB')
+            img.save(buffered, format="JPEG")
+            img_str = base64.b64encode(buffered.getvalue()).decode('utf-8')
+
+            data = {
+                "session_hash": "75mq6m01qy4",
+                "fn_index": 0,
+                "data": [
+                    f"data:image/jpeg;base64,{img_str}"
+                ]
+            }
+
+            headers = {
+                'Content-Type': 'application/json',
+                'Origin': 'https://aistudio.baidu.com',
+                'Accept-Encoding': 'gzip, deflate, br',
+                'Cookie': '__bsi=10291592389384054246_00_34_N_R_16_0303_cca8_Y; IMG_WH=428_746; SE_LAUNCH=5%3A1680744441_31%3A28012407_49%3A28012719; PSCBD=31%3A1; BA_HECTOR=2kaha10la18l2104012l8h8v1i2s7vr1m; H_WISE_SIDS=219946_234020_131861_216852_213347_214806_219942_213035_230186_204906_',
+                'Connection': 'keep-alive',
+                'Accept': '*/*',
+                'User-Agent': 'Mozilla/5.0 (iPhone; CPU iPhone OS 16_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.2 Mobile/15E148 Safari/604.1',
+                'Referer': 'https://aistudio.baidu.com/serving/app/23/?__theme=light',
+                'Content-Length': '195430',
+                'Accept-Language': 'zh-CN,zh-Hans;q=0.9'
+            }
+
+            url = 'https://aistudio.baidu.com/serving/app/23/run/predict/'
+
+            async with session.post(url, headers=headers, data=json.dumps(data)) as response:
+                jsons = json.loads(await response.text())
+                result = jsons["data"][0]
+                data_excel = await html2excel(result)
+
+                lines = data_excel.strip().split('\n')
+                lst = [line.split('\t') for line in lines]
+                wb = Workbook()
+                ws = wb.active
+                for row in lst:
+                    ws.append(row)
+
+                filepath = os.path.dirname(os.path.realpath(__file__)) + r'\temp.xlsx'
+                wb.save(filepath)
+
+                return data_excel, lst[0][0]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_ocr.py` & `nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_ocr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-import requests
+import asyncio
+import aiohttp
 import base64
 import datetime
 
-def timestamp_to_utc(timestamp):
+async def timestamp_to_utc(timestamp):
     # 将时间戳转换为datetime对象
     dt = datetime.datetime.fromtimestamp(timestamp)
     # 将datetime对象转换为UTC时间
     utc = dt.astimezone(datetime.timezone.utc)
     # 将UTC时间格式化为字符串，注意要加上时区信息Z
     utc_str = utc.strftime("%a, %d %b %Y %H:%M:%S Z")
     return utc_str
-def api_paddle_ocr(img):
+
+async def api_paddle_ocr(img):
     # 定义请求的url和headers
     url = "https://www.paddlepaddle.org.cn/paddlehub-api/image_classification/chinese_ocr_db_crnn_mobile"
     headers = {
         "Content-Type": "application/json",
         "Origin": "https://www.paddlepaddle.org.cn",
         "Accept-Encoding": "gzip, deflate, br",
         #"Cookie": "Hm_lpvt_89be97848720f62fa00a07b1e0d83ae6=1680262774; Hm_lvt_89be97848720f62fa00a07b1e0d83ae6=1680262716",
         "Connection": "keep-alive",
         "Accept": "*/*",
         "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 16_2 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.0 Mobile/15E148 Safari/605.1.15",
         "Referer": "https://www.paddlepaddle.org.cn/hub/scene/ocr",
-        "Content-Length": "176200",
         "Accept-Language": "zh-CN,zh-Hans;q=0.9"
     }
     # 定义两个时间戳
     Hm_lpvt = 1680262774
     Hm_lvt = 1680262716
     # 调用函数，得到两个日期字符串
-    Hm_lpvt_utc = timestamp_to_utc(Hm_lpvt)
-    Hm_lvt_utc = timestamp_to_utc(Hm_lvt)
+    Hm_lpvt_utc = await timestamp_to_utc(Hm_lpvt)
+    Hm_lvt_utc = await timestamp_to_utc(Hm_lvt)
     # 将两个日期字符串拼接成Cookie的Expires属性，并添加到headers中
     headers["Cookie"] = f"Hm_lpvt_89be97848720f62fa00a07b1e0d83ae6={Hm_lpvt_utc}; Hm_lvt_89be97848720f62fa00a07b1e0d83ae6={Hm_lvt_utc}"
 
     # 将图片内容转换为base64编码
     pic_base64 = base64.b64encode(img.getvalue())
     # 定义请求的数据，使用base64编码的图片
     data = {
         "image": pic_base64.decode()
     }
 
     # 发送post请求，并获取响应
-    response = requests.post(url, headers=headers, json=data)
-    results = response.json()['result'][0]['data']
-    text = ''
-    for result in results:
-        result = result['text']
-        text += result + ' '
-
-    return text
+    async with aiohttp.ClientSession(headers=headers) as session:
+        async with session.post(url, json=data) as response:
+            results = (await response.json())['result'][0]['data']
+            text = ''
+            for result in results:
+                result = result['text']
+                text += result + ' '
 
-# with open(r"C:\Users\Administrator\PycharmProjects\paddle\ocr\ppocr_img\ch\ch.jpg", "rb") as pic:
-#     # 读取图片内容
-#     pic_data = pic.read()
-#     print(api_paddle_ocr(pic_data))
+    return text
```

### Comparing `nonebot_api_paddle-1.0.2/nonebot_api_paddle/api_voice.py` & `nonebot_api_paddle-1.0.3/nonebot_api_paddle/api_voice.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
-import requests
 import json
+import aiohttp
+import asyncio
+import os
 
-
-def getvoice(text) -> str:
+async def getvoice(text: str) -> str:
     url = 'https://aistudio.baidu.com/serving/app/10/run/predict/'
 
     headers = {
         'Content-Type': 'application/json',
         'Origin': 'https://aistudio.baidu.com',
         'Accept-Encoding': 'gzip, deflate, br',
         'Cookie': 'PSCBD=16%3A2_31%3A1; SE_LAUNCH=5%3A1680429424_16%3A28007298___31%3A28008975; __bsi=8248412395268301922_00_69_N_R_7_0303_cca8_Y; BA_HECTOR=ag808h2l8k048g80018halaj1i2lrmv1n; BAIDUID=E044455E10D5087EEC9D3C7B24F1A101:FG=1; H_WISE_SIDS=219946_234020_219563_216841_213348_214803_219943_213029_204916_230288_242157_110085_227870_236307_243890_244258_244715_240590_244955_245412_245701_246986_234207_248667_248725_243706_249910_249969_250145_247148_250738_251068_249344_247509_247461_251424_245919_251415_245217_252006_252221_247671_248079_250759_252562_249892_252577_252946_253044_252810_247585_252991_234296_253066_253463_253480_252354_253705_246823_250095_253516_253914_253427_229154_254217_254323_254458_254473_249983_254596_254261_254734_254683_248124_250226_251498_254749_254831_254890_249386_250390_251133_253900; H_WISE_SIDS_BFESS=219946_234020_114552_213347_214806_219943_213028_204904_230288_242157_242621_110085_227869_236307_243706_243887_244252_244722_240590_245412_246177_234208_247974_248725_249015_249633_247510_247148_250738_250889_251068_251127_245919_248239_247671_251415_251838_251884_252076_252262_250757_249893_247460_252580_252944_251150_253044_252811_247585_253170_234296_253064_248079_253480_252354_253704_246822_250091_251786_253976_253516_253914_253427_254143_229154_254296_254323_252306_254472_249981_179346_253900_254263_236539_254733_254683_248124_254687_254748_251132_244955_233835_8000072_8000124_8000137_8000149_8000161_8000163_8000166_8000171_8000193_8000204; BAIDUID_BFESS=72217B892980F06DF215AE904AC1B10F:FG=1; IMG_WH=428_804; PSTM=1679574152; BIDUPSID=135FA5FEB7755007A7A910CEA7AA5164'
@@ -15,12 +15,14 @@
 
     data = {
         "fn_index": 0,
         "data": [text],
         "session_hash": "playgnwv9r"
     }
 
-    response = requests.post(url, headers=headers, data=json.dumps(data))
-    json_data = json.loads(response.text)
-    file_name = str(json_data['data'][0]['name'])
-    url = 'https://aistudio.baidu.com/serving/app/10/file=' + file_name
-    return url
+    async with aiohttp.ClientSession(headers=headers) as session:
+        async with session.post(url, data=json.dumps(data)) as response:
+            json_data = await response.json()
+            file_name = str(json_data['data'][0]['name'])
+            url = 'https://aistudio.baidu.com/serving/app/10/file=' + file_name
+
+            return url
```

### Comparing `nonebot_api_paddle-1.0.2/nonebot_api_paddle.egg-info/PKG-INFO` & `nonebot_api_paddle-1.0.3/nonebot_api_paddle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-api-paddle
-Version: 1.0.2
+Version: 1.0.3
 Summary: nonbot_api_paddle
 Home-page: https://github.com/canxin121/nonebot_api_paddle
 Author: canxin
 Author-email: 1969730106@qq.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `nonebot_api_paddle-1.0.2/setup.py` & `nonebot_api_paddle-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_api_paddle",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.0.2",  # 程序版本
+    version="1.0.3",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonbot_api_paddle",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_api_paddle",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

