# Comparing `tmp/nonebot_poe_chat-0.0.2.tar.gz` & `tmp/nonebot_poe_chat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_poe_chat-0.0.2.tar", last modified: Fri Apr 21 13:13:45 2023, max compression
+gzip compressed data, was "nonebot_poe_chat-0.0.3.tar", last modified: Fri Apr 21 14:57:51 2023, max compression
```

## Comparing `nonebot_poe_chat-0.0.2.tar` & `nonebot_poe_chat-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 13:13:45.609683 nonebot_poe_chat-0.0.2/
--rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      534 2023-04-21 13:13:45.608674 nonebot_poe_chat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-04-21 12:16:18.000000 nonebot_poe_chat-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 13:13:45.601162 nonebot_poe_chat-0.0.2/nonebot_poe_chat/
--rw-rw-rw-   0        0        0    21624 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-04-21 13:10:05.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/config.py
--rw-rw-rw-   0        0        0     4596 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_chat.py
--rw-rw-rw-   0        0        0     1440 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_clear.py
--rw-rw-rw-   0        0        0     2898 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_create.py
--rw-rw-rw-   0        0        0     2445 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_login.py
-drwxrwxrwx   0        0        0        0 2023-04-21 13:13:45.607674 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/
--rw-rw-rw-   0        0        0      534 2023-04-21 13:13:45.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-21 13:13:45.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 13:13:45.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-04-21 13:13:45.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 13:13:45.000000 nonebot_poe_chat-0.0.2/nonebot_poe_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 13:13:45.609683 nonebot_poe_chat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-21 13:13:17.000000 nonebot_poe_chat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/
+-rw-rw-rw-   0        0        0    12533 2023-04-02 14:35:33.000000 nonebot_poe_chat-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2942 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2447 2023-04-21 14:42:40.000000 nonebot_poe_chat-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.247945 nonebot_poe_chat-0.0.3/nonebot_poe_chat/
+-rw-rw-rw-   0        0        0    21868 2023-04-21 14:42:29.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/__init__.py
+-rw-rw-rw-   0        0        0     3026 2023-04-21 13:10:05.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/config.py
+-rw-rw-rw-   0        0        0     4308 2023-04-21 14:52:49.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_chat.py
+-rw-rw-rw-   0        0        0     1440 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_clear.py
+-rw-rw-rw-   0        0        0     2898 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_create.py
+-rw-rw-rw-   0        0        0     2445 2023-04-21 12:50:52.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_login.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:57:51.252945 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 14:57:51.000000 nonebot_poe_chat-0.0.3/nonebot_poe_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:57:51.253945 nonebot_poe_chat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-21 14:57:12.000000 nonebot_poe_chat-0.0.3/setup.py
```

### Comparing `nonebot_poe_chat-0.0.2/LICENSE.txt` & `nonebot_poe_chat-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/__init__.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import re, json, uuid, asyncio
+import re, json, uuid, asyncio,string,random
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from nonebot.plugin import on_command, on
 from nonebot.params import ArgStr, CommandArg
 from nonebot.typing import T_State
 from nonebot.matcher import Matcher
 from nonebot.adapters.onebot.v11 import Message, Event, Bot, MessageEvent,MessageSegment
 from nonebot.internal.rule import Rule
@@ -103,14 +103,19 @@
             with open(user_path, 'w') as f:
                 json.dump(user_dict, f)
             await matcher.finish(reply_out(event, "创建成功并切换到新建bot"))
         else:
             await matcher.finish(reply_out(event, "出错了，多次出错请联系机器人管理员"))
 
 ######################################################    
+def generate_random_string(length=8):
+    """生成指定长度的随机字符串"""
+    letters = string.ascii_letters + string.digits
+    return ''.join(random.choice(letters) for _ in range(length))
+
 #保留上一个回答的chatsuggest
 chat_lock = asyncio.Semaphore(3)
 chat_suggest = {}
 waitque = []
 poe_chat_ = on_command(
     "poetalk",
     aliases={
@@ -122,27 +127,28 @@
 @poe_chat_.handle()
 async def __chat_bot__(matcher:Matcher,event: Event, args: Message = CommandArg()):
     global chat_lock,chat_suggest
     userid = str(event.user_id)
     if not is_cookie_exists:
         await matcher.finish(reply_out(event, "管理员还没填写可用的poe_cookie或登陆"))
     if userid not in user_dict:
-        truename = str(generate_uuid(str(userid + "default")))
+        random = generate_random_string()
+        truename = str(generate_uuid(str(userid + random)))
         is_created = await poe_create(cookie_path,truename,1,"一个智能助理")
         if is_created:
             user_dict[userid] = {}        
             user_dict[userid]['all'] = {}
             user_dict[userid]['all']["default"] = truename
             user_dict[userid]['now'] = {}
             user_dict[userid]['now']["default"] = truename
             with open(user_path, 'w') as f:
                 json.dump(user_dict, f)
-            await matcher.send(reply_out(event, "自动创建default gpt3.5成功"))
+            await matcher.send(reply_out(event, "自动创建gpt3.5成功"))
         else:
-            await matcher.send(reply_out(event, "自动创建default gpt3.5失败，多次失败请联系机器人管理员"))
+            await matcher.send(reply_out(event, "自动创建gpt3.5失败，多次失败请联系机器人管理员"))
     if userid in chat_suggest and len(str(args[0])) == 1 and str(args[0]) in ['1','2','3','4']:
         text = chat_suggest[userid][int(str(args[0]))-1]
     else:
         text = str(args[0])
     botname = str(list(user_dict[userid]["now"].values())[0])
     if userid in waitque:
         await matcher.finish(reply_out(event, "你已经有一个对话进行中了，请等结束后再发送"))
@@ -274,22 +280,22 @@
     bots = list(user_dict[userid]["all"].keys())
     bot_str = '\n'.join(str(bot) for bot in bots)
     # bot_truname = str(list(user_dict[userid]["now"].values())[0])
     nickname = str(list(user_dict[userid]["now"].keys())[0])
     if len(bots)==1:
         await matcher.finish(reply_out(event, f"当前只有一个bot:{nickname}"))
     msg = "你已经创建的的bot有：\n" + bot_str +f"\n当前使用的bot是{nickname}"
-    await matcher.finish(reply_out(event, msg))
+    await matcher.send(reply_out(event, msg))
 
 @poe_switch.got('nickname',prompt='请输入要切换的机器人名称')
 async def __poe_switch____(matcher:Matcher,event: Event, infos: str = ArgStr("nickname")):
     userid = str(event.user_id)
     bots = list(user_dict[userid]["all"].keys())
     if infos in ["取消", "算了"]:
-        await matcher.finish(reply_out(event, "终止切换"))
+        await matcher.finish(reply_out(event, "中断切换"))
     infos = infos.split(" ")
     nickname = infos[0]
     if not (nickname in bots):
         await matcher.reject(reply_out(event, "输入信息有误，请检查后重新输入"))
     to_truename = user_dict[userid]["all"][nickname]
     del user_dict[userid]["now"]
     user_dict[userid]["now"] = {}
```

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/config.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_chat.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,21 @@
             # 找到发送按钮元素并点击
             await page.wait_for_selector('button.Button_primary__pIDjn')
             send_button = await page.wait_for_selector('button.Button_primary__pIDjn')
             # await asyncio.sleep(0.5)
             await send_button.click()
             # 发送成功后退出循环
             break
-        except (TimeoutError, SyncTimeoutError) as ex:
+        except:
             # 如果出现超时异常，打印错误信息并稍等一段时间后重试
-            print(f"发送失败，错误信息：{ex}")
             error_count += 1
             if error_count >= 1:
                 await asyncio.sleep(retry_interval)
             current_retry += 1
             continue
-        except Exception as ex:
-            # 如果出现其他异常，打印错误信息并抛出异常
-            print(f"发送失败，错误信息：{ex}")
-            raise ex
-
     if current_retry == retry_count:
         return False
 
 async def get_message_async(page,botname, sleep):
     consecutive_errors = 0  # initialize a counter for consecutive errors
     while True:
         await asyncio.sleep(sleep)
```

#### html2text {}

```diff
@@ -10,27 +10,23 @@
 bot has been deleted for violating our" content = await page.content() if text
 in content: return "banned" # æ¾å°è¾å¥æ¡åç´  input_box = await
 page.wait_for_selector('.ChatMessageInputView_textInput__Aervw') #
 å°å­ç¬¦ä¸²åéå°è¾å¥æ¡ä¸­ await input_box.fill(input_str) #
 æ¾å°åéæé®åç´ å¹¶ç¹å» await page.wait_for_selector
 ('button.Button_primary__pIDjn') send_button = await page.wait_for_selector
 ('button.Button_primary__pIDjn') # await asyncio.sleep(0.5) await
-send_button.click() # åéæååéåºå¾ªç¯ break except (TimeoutError,
-SyncTimeoutError) as ex: #
+send_button.click() # åéæååéåºå¾ªç¯ break except: #
 å¦æåºç°è¶æ¶å¼å¸¸ï¼æå°éè¯¯ä¿¡æ¯å¹¶ç¨ç­ä¸æ®µæ¶é´åéè¯
-print(f"åéå¤±è´¥ï¼éè¯¯ä¿¡æ¯ï¼{ex}") error_count += 1 if error_count >=
-1: await asyncio.sleep(retry_interval) current_retry += 1 continue except
-Exception as ex: # å¦æåºç°å¶ä»å¼å¸¸ï¼æå°éè¯¯ä¿¡æ¯å¹¶æåºå¼å¸¸
-print(f"åéå¤±è´¥ï¼éè¯¯ä¿¡æ¯ï¼{ex}") raise ex if current_retry ==
-retry_count: return False async def get_message_async(page,botname, sleep):
-consecutive_errors = 0 # initialize a counter for consecutive errors while
-True: await asyncio.sleep(sleep) try: await page.goto(f'https://poe.com/
-{botname}') response = await page.content() text = "This bot has been deleted
-for violating our" if text in response: return "banned" match_text = re.search
-(r'
+error_count += 1 if error_count >= 1: await asyncio.sleep(retry_interval)
+current_retry += 1 continue if current_retry == retry_count: return False async
+def get_message_async(page,botname, sleep): consecutive_errors = 0 # initialize
+a counter for consecutive errors while True: await asyncio.sleep(sleep) try:
+await page.goto(f'https://poe.com/{botname}') response = await page.content()
+text = "This bot has been deleted for violating our" if text in response:
+return "banned" match_text = re.search(r'
 ', response, re.DOTALL) json_data_text = match_text.group(1) json_obj_text =
 json.loads(json_data_text) chat_list_raw = json_obj_text["props"]["pageProps"]
 ["payload"]["chatOfBotDisplayName"]["messagesConnection"]["edges"]
 chat_list_raw = [a["node"] for a in chat_list_raw] chat_list_text = [a["text"]
 for a in chat_list_raw] if chat_list_text[-1]: match_suggest = re.search(r'*
 (.*?)', response, re.DOTALL) string_list = re.findall(r'>\s*([^<>\n]+)\s*<',
 match_suggest.group(1)) if len(string_list) == 4: return chat_list_text,
```

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_clear.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_clear.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_create.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_create.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.2/nonebot_poe_chat/poe_login.py` & `nonebot_poe_chat-0.0.3/nonebot_poe_chat/poe_login.py`

 * *Files identical despite different names*

### Comparing `nonebot_poe_chat-0.0.2/setup.py` & `nonebot_poe_chat-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot_poe_chat",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.2",  # 程序版本
+    version="0.0.3",  # 程序版本
     author="canxin",  # 项目作者
     author_email="1969730106@qq.com",  # 作者邮件
     description="nonebot_poe_chat",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/canxin121/nonebot_poe_chat",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

