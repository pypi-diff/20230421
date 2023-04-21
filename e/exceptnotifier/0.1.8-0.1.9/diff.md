# Comparing `tmp/exceptnotifier-0.1.8.tar.gz` & `tmp/exceptnotifier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptnotifier-0.1.8.tar", last modified: Wed Apr 19 18:24:09 2023, max compression
+gzip compressed data, was "exceptnotifier-0.1.9.tar", last modified: Wed Apr 19 19:09:49 2023, max compression
```

## Comparing `exceptnotifier-0.1.8.tar` & `exceptnotifier-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.306756 exceptnotifier-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.237726 exceptnotifier-0.1.8/ExceptNotifier/
--rw-rw-rw-   0        0        0     2714 2023-04-19 17:36:16.000000 exceptnotifier-0.1.8/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.296358 exceptnotifier-0.1.8/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1232 2023-04-19 18:19:59.000000 exceptnotifier-0.1.8/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 exceptnotifier-0.1.8/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 exceptnotifier-0.1.8/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      583 2023-04-19 12:04:52.000000 exceptnotifier-0.1.8/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0      975 2023-04-19 12:04:07.000000 exceptnotifier-0.1.8/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 exceptnotifier-0.1.8/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 exceptnotifier-0.1.8/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 exceptnotifier-0.1.8/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 exceptnotifier-0.1.8/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      680 2023-04-19 12:02:25.000000 exceptnotifier-0.1.8/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1364 2023-04-19 12:03:24.000000 exceptnotifier-0.1.8/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 exceptnotifier-0.1.8/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      908 2023-04-19 14:11:30.000000 exceptnotifier-0.1.8/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      548 2023-04-19 17:11:23.000000 exceptnotifier-0.1.8/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 exceptnotifier-0.1.8/ExceptNotifier/base/whatsapp_sender.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 exceptnotifier-0.1.8/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6393 2023-04-19 13:25:44.000000 exceptnotifier-0.1.8/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5769 2023-04-19 15:47:40.000000 exceptnotifier-0.1.8/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     6479 2023-04-19 13:24:37.000000 exceptnotifier-0.1.8/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     6563 2023-04-19 13:24:31.000000 exceptnotifier-0.1.8/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     6033 2023-04-19 13:24:27.000000 exceptnotifier-0.1.8/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     7746 2023-04-19 13:24:20.000000 exceptnotifier-0.1.8/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     6094 2023-04-19 13:24:12.000000 exceptnotifier-0.1.8/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     6085 2023-04-19 15:32:02.000000 exceptnotifier-0.1.8/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     6020 2023-04-19 14:03:49.000000 exceptnotifier-0.1.8/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     6275 2023-04-19 14:10:48.000000 exceptnotifier-0.1.8/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.300359 exceptnotifier-0.1.8/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      263 2023-04-19 15:56:09.000000 exceptnotifier-0.1.8/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 exceptnotifier-0.1.8/ExceptNotifier/utils/kakao_token.py
--rw-rw-rw-   0        0        0     6148 2023-04-19 17:33:09.000000 exceptnotifier-0.1.8/ExceptNotifier/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.263963 exceptnotifier-0.1.8/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    23587 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1526 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    23587 2023-04-19 18:24:09.305750 exceptnotifier-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    22539 2023-04-19 18:15:27.000000 exceptnotifier-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 18:24:09.306756 exceptnotifier-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1926 2023-04-19 18:23:49.000000 exceptnotifier-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:09:49.681512 exceptnotifier-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-04-19 19:09:49.601980 exceptnotifier-0.1.9/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2877 2023-04-19 19:08:28.000000 exceptnotifier-0.1.9/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:09:49.671514 exceptnotifier-0.1.9/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1283 2023-04-19 19:07:20.000000 exceptnotifier-0.1.9/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      536 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0     1001 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1307 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      858 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1839 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0      940 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      676 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1391 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      637 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      924 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      558 2023-04-19 19:05:47.000000 exceptnotifier-0.1.9/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1470 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1817 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6710 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     6083 2023-04-19 19:06:28.000000 exceptnotifier-0.1.9/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     6799 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     6843 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6333 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     8326 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     6390 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     6735 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     6313 2023-04-19 19:06:19.000000 exceptnotifier-0.1.9/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     6616 2023-04-19 19:06:22.000000 exceptnotifier-0.1.9/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:09:49.675514 exceptnotifier-0.1.9/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      267 2023-04-19 19:08:17.000000 exceptnotifier-0.1.9/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-04-19 19:04:19.000000 exceptnotifier-0.1.9/ExceptNotifier/utils/kakao_token.py
+-rw-rw-rw-   0        0        0     6395 2023-04-19 19:06:25.000000 exceptnotifier-0.1.9/ExceptNotifier/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:09:49.632964 exceptnotifier-0.1.9/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    24974 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 19:09:49.000000 exceptnotifier-0.1.9/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    24974 2023-04-19 19:09:49.680513 exceptnotifier-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    23926 2023-04-19 19:02:23.000000 exceptnotifier-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 19:09:49.681512 exceptnotifier-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1928 2023-04-19 19:07:35.000000 exceptnotifier-0.1.9/setup.py
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.mail_sender import send_gmail_msg
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.chime_sender import send_chime_msg
@@ -12,13 +12,26 @@
 from ExceptNotifier.base.whatsapp_sender import send_whatsapp_msg
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.beep_sender import beep
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 
 
-__all__ = ['send_kakao_msg', 'send_gmail_msg', 'send_slack_msg', 'send_telegram_msg', 'send_chime_msg', 'send_discord_msg',
-           'send_line_msg', 'send_wechat_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
-           ]
+__all__ = [
+    "send_kakao_msg",
+    "send_gmail_msg",
+    "send_slack_msg",
+    "send_telegram_msg",
+    "send_chime_msg",
+    "send_discord_msg",
+    "send_line_msg",
+    "send_wechat_msg",
+    "send_line_msg",
+    "send_teams_msg",
+    "send_whatsapp_msg",
+    "send_sms_msg",
+    "beep",
+    "receive_openai_advice",
+]
 
-__version__ = "0.1.8"
-__author__ = "daniel park <parkminwoo1991@gmail.com>"
+__version__ = "0.1.9"
+__author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/beep_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import os
 import platform
 import winsound
 
+
 def beep(sec=1, freq=1000) -> None:
     """Make beep sound
 
     :param sec: beep duration, defaults to 1
     :type sec: int, optional
     :param freq: beep fequency, defaults to 1000
     :type freq: int, optional
     """
 
     sys = platform.system()
 
     if sys == "Windows":
-        winsound.Beep(int(1000*sec), freq)
+        winsound.Beep(int(1000 * sec), freq)
     else:
-        os.system('play -nq -t alsa synth {} sine {}'.format(sec, freq))
+        os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/chime_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 import urllib3
 import json
 
 http = urllib3.PoolManager()
 
+
 def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
     """Send message to chat room through chime app's webhook url.
 
     :param _CHIME_WEBHOOK_URL: Webhook url from chime app
     :type _CHIME_WEBHOOK_URL: str
     :param msg: Message text
     :type msg: str
@@ -23,9 +24,9 @@
     resp = http.request("POST", url, body=encoded_msg)
 
     return resp
 
 
 if __name__ == "__main__":
     _CHIME_WEBHOOK_URL = "xxxxx"
-    
-    send_chime_msg(_CHIME_WEBHOOK_URL, "Test")
+
+    send_chime_msg(_CHIME_WEBHOOK_URL, "Test")
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/desktop_sender.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import time
 from plyer import notification
 
 
 def send_desktop_msg(title_msg: str, body_msg: str, DISP_TIME=5) -> None:
     """Sending notification to desktop
@@ -10,12 +10,8 @@
     :param title_msg: Title of message
     :type title_msg: str
     :param body_msg: Body of message
     :type body_msg: str
     :param DISP_TIME: Time duration, defaults to 5
     :type DISP_TIME: int, optional
     """
-    notification.notify(
-            title = title_msg[:20],
-            message=body_msg[:200] ,
-            timeout=DISP_TIME)
-    
+    notification.notify(title=title_msg[:20], message=body_msg[:200], timeout=DISP_TIME)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/discord_sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 
 def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
     """Send message to chat room through discord app's webhook url.
 
     :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
     :type _DISCORD_WEBHOOK_URL: str
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
-    try: 
+    try:
         from discord import Webhook, RequestsWebhookAdapter
-        webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
+
+        webhook = Webhook.from_url(
+            _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
+        )
         resp = webhook.send(msg[:150])
     except:
         from discord import SyncWebhook
-        webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL) # Initializing webhook
-        webhook.send(content=msg[:150]) 
-    return resp
 
+        webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
+        webhook.send(content=msg[:150])
+    return resp
 
 
-if __name__ =="__main__":
+if __name__ == "__main__":
     _DISCORD_WEBHOOK_URL = "xxxxx"
     msg = "Sending Test"
 
     send_discord_msg(_DISCORD_WEBHOOK_URL, msg)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/line_sender.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
-import requests   
+import requests
+
 
 def send_line_msg(_LINE_NOTIFY_API_TOKEN: str, msg: str) -> dict:
     """Send message to chat room through Line app's REST API.
 
     :param _LINE_NOTIFY_API_TOKEN: Line notify API token
     :type _LINE_NOTIFY_API_TOKEN: str
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
 
     api_url = "https://notify-api.line.me/api/notify"
-    headers = {'Authorization':'Bearer '+ _LINE_NOTIFY_API_TOKEN}
-    message = {
-        "message" : msg
-    }
-    resp = requests.post(api_url, headers= headers , data = message)
+    headers = {"Authorization": "Bearer " + _LINE_NOTIFY_API_TOKEN}
+    message = {"message": msg}
+    resp = requests.post(api_url, headers=headers, data=message)
     return resp
 
 
-
-if __name__ == "__main__": 
+if __name__ == "__main__":
     global _LINE_NOTIFY_API_TOKEN
     _LINE_NOTIFY_API_TOKEN = "XXXXXXXXX"
     msg = "Test Message"
     send_line_msg(_LINE_NOTIFY_API_TOKEN, msg)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/mail_sender.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import smtplib
 from email.message import EmailMessage
 
-def send_gmail_msg(_GMAIL_SENDER_ADDR: str, _GAMIL_RECIPIENT_ADDR: str, _GMAIL_APP_PASSWORD_OF_SENDER: str, subject_msg: str, body_msg: str) -> dict:
+
+def send_gmail_msg(
+    _GMAIL_SENDER_ADDR: str,
+    _GAMIL_RECIPIENT_ADDR: str,
+    _GMAIL_APP_PASSWORD_OF_SENDER: str,
+    subject_msg: str,
+    body_msg: str,
+) -> dict:
     """Send mail through gmail smtp server
 
     :param _GMAIL_SENDER_ADDR: Gmail address who send message
     :type _GMAIL_SENDER_ADDR: str
     :param _GAMIL_RECIPIENT_ADDR: Gmail address who receive message
     :type _GAMIL_RECIPIENT_ADDR: str
     :param _GMAIL_APP_PASSWORD_OF_SENDER: Google app password
@@ -15,16 +22,16 @@
     :param subject_msg: Mail title
     :type subject_msg: str
     :param body_msg: Mail body
     :type body_msg: str
     :return: Response according to sending request
     :rtype: dict
     """
-    
-    SMTP_SERVER = 'smtp.gmail.com'
+
+    SMTP_SERVER = "smtp.gmail.com"
     SMTP_PORT = 465
     smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
     EMAIL_ADDR = _GMAIL_SENDER_ADDR
     EMAIL_PASSWORD = _GMAIL_APP_PASSWORD_OF_SENDER
     smtp.login(EMAIL_ADDR, EMAIL_PASSWORD)
     message = EmailMessage()
     message.set_content(body_msg)
@@ -33,15 +40,21 @@
     message["To"] = _GAMIL_RECIPIENT_ADDR
     resp = smtp.send_message(message)
     smtp.quit()
 
     return resp
 
 
-if __name__ == "__main__": #No-QA
-    _GMAIL_SENDER_ADDR = 'xxxxx@gmail.com'
-    _GMAIL_APP_PASSWORD_OF_SENDER = 'yyyyy'
-    _GAMIL_RECIPIENT_ADDR = 'zzzzz@gmail.com'
+if __name__ == "__main__":  # No-QA
+    _GMAIL_SENDER_ADDR = "xxxxx@gmail.com"
+    _GMAIL_APP_PASSWORD_OF_SENDER = "yyyyy"
+    _GAMIL_RECIPIENT_ADDR = "zzzzz@gmail.com"
     subject_msg = "Python Code Alarm: Process End."
     body_msg = "Python Code Notice: \nA notification has arrived from your code."
-    
-    send_gmail_msg(_GMAIL_SENDER_ADDR, _GAMIL_RECIPIENT_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER, subject_msg, body_msg)
+
+    send_gmail_msg(
+        _GMAIL_SENDER_ADDR,
+        _GAMIL_RECIPIENT_ADDR,
+        _GMAIL_APP_PASSWORD_OF_SENDER,
+        subject_msg,
+        body_msg,
+    )
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/openai_receiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import openai
 
+
 def receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message):
     openai.api_key = _OPEN_AI_API
     model_engine = _OPEN_AI_MODEL
 
     input_text = f"How can I fix this error? Give me short infomation about next error. Let me know which code line and which code is incorrect. and try to make it fix or fix exampel. error== {error_message}"
     response = openai.ChatCompletion.create(
-                                            model=model_engine,
-                                            messages=[{"role": "user", "content": input_text }]
-                                            )
-    advice_msg = response['choices'][0]['message']['content']
+        model=model_engine, messages=[{"role": "user", "content": input_text}]
+    )
+    advice_msg = response["choices"][0]["message"]["content"]
     return advice_msg
 
 
 if __name__ == "__main__":
     _OPEN_AI_API = "sk-xxxxx"
     _OPEN_AI_MODEL = "gpt-3.5-turbo"
-    error_message = ' Cell 3 in ()----> 1 1/0 ZeroDivisionError: division by zero'
+    error_message = " Cell 3 in ()----> 1 1/0 ZeroDivisionError: division by zero"
     advice_msg = receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message)
-    print(advice_msg)
+    print(advice_msg)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/slack_sender.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 import requests
 
 
 def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
     """Send message to chat room through slack app's api.
@@ -10,17 +10,17 @@
     :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
     :type _SLACK_WEBHOOK_URL: str
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
-    
-    data = {'text':msg}
+
+    data = {"text": msg}
     resp = requests.post(url=_SLACK_WEBHOOK_URL, json=data)
     return resp
 
 
-if __name__ == "__main__": 
+if __name__ == "__main__":
     _SLACK_WEBHOOK_URL = "xxxxx"
     msg = "Test Message"
     send_slack_msg(_SLACK_WEBHOOK_URL, msg)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/sms_sender.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 from twilio.rest import Client
 
-def send_sms_msg(_TWILIO_SID: str, _TWILIO_TOKEN: str, _SENDER_PHONE_NUMBER: str, _RECIPIENT_PHONE_NUMBER: str, msg: str)->dict:
+
+def send_sms_msg(
+    _TWILIO_SID: str,
+    _TWILIO_TOKEN: str,
+    _SENDER_PHONE_NUMBER: str,
+    _RECIPIENT_PHONE_NUMBER: str,
+    msg: str,
+) -> dict:
     """Send SMS through twilio platform.
     https://www.twilio.com/en-us
 
     :param _TWILIO_SID: Twilio personal _TWILIO_SID
     :type _TWILIO_SID: str
     :param _TWILIO_TOKEN: Twilio personal _TWILIO_TOKEN
     :type _TWILIO_TOKEN: str
@@ -16,28 +23,28 @@
     :param _RECIPIENT_PHONE_NUMBER: Recipient phone number
     :type _RECIPIENT_PHONE_NUMBER: str
     :param msg: SMS content
     :type msg: str
     :return: Response dict
     :rtype: dict
     """
-    
+
     client = Client(_TWILIO_SID, _TWILIO_TOKEN)
     resp = client.messages.create(
-        to=_RECIPIENT_PHONE_NUMBER,
-        from_=_SENDER_PHONE_NUMBER,  
-        body=msg[:1500]
+        to=_RECIPIENT_PHONE_NUMBER, from_=_SENDER_PHONE_NUMBER, body=msg[:1500]
     )
     return resp
 
 
 if __name__ == "__main__":
     """https://www.twilio.com/en-us"""
 
-    _TWILIO_SID = 'xxxxx'
-    _TWILIO_TOKEN = 'yyyyy'
+    _TWILIO_SID = "xxxxx"
+    _TWILIO_TOKEN = "yyyyy"
     client = Client(_TWILIO_SID, _TWILIO_TOKEN)
     _SENDER_PHONE_NUMBER = "+aaaaa"
     _RECIPIENT_PHONE_NUMBER = "+bbbbb"
-    msg="ExceptNotifier Test"
+    msg = "ExceptNotifier Test"
 
-    send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg)
+    send_sms_msg(
+        _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg
+    )
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/telegram_sender.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 
 import requests
 
 
 def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
     """Send message via telegram bot.
@@ -13,19 +13,21 @@
     :type msg: str
     :return: Response dict
     :rtype: dict
     """
     url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/getUpdates"
     req_dict = requests.get(url).json()
     print(req_dict)
-    bot_id = dict(dict(dict(list(dict(req_dict).values())[1][0])['message'])['from'])['id']
+    bot_id = dict(dict(dict(list(dict(req_dict).values())[1][0])["message"])["from"])[
+        "id"
+    ]
     bot_url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/sendMessage?chat_id={bot_id}&text={msg}"
     resp = requests.get(bot_url).json()
 
     return resp
 
 
 if __name__ == "__main__":
 
-    _TELEGRAM_TOKEN = 'xxxxxxxxxx'
+    _TELEGRAM_TOKEN = "xxxxxxxxxx"
     msg = "Test Message"
     send_telegram_msg(_TELEGRAM_TOKEN, msg)
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.1.9/ExceptNotifier/base/whatsapp_sender.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import logging
 import requests
 
 
 def send_whatsapp_msg(
-    msg: str, sender_phone_number_id: str, TOKEN: str, receiver_number: str, recipient_type:str="individual"
+    msg: str,
+    sender_phone_number_id: str,
+    TOKEN: str,
+    receiver_number: str,
+    recipient_type: str = "individual",
 ) -> dict:
     """Send me a message via whatsapp.
     However, from v16 api, it seems to have been changed so that templates that have passed deliberation can be sent. 
     Therefore, it is *NOT used* by ExceptNotifier.
 
     :param msg: Message content (Cannot be used as it is not a template)
     :type msg: str
@@ -21,24 +25,21 @@
     :type receiver_number: str
     :param recipient_type: Type of recipient, defaults to "individual"
     :type recipient_type: str, optional
     :return: _description_
     :rtype: dict
     """
 
-    url =  f"https://graph.facebook.com/v16.0/{sender_phone_number_id}/messages"
-    
-    data = { "messaging_product": "whatsapp", 
-            "to": receiver_number, 
-            "type": "template", 
-            "template": 
-                        { "name": "hello_world", 
-                          "language": 
-                                    { "code": "en_US" }
-                        } 
-            }
+    url = f"https://graph.facebook.com/v16.0/{sender_phone_number_id}/messages"
+
+    data = {
+        "messaging_product": "whatsapp",
+        "to": receiver_number,
+        "type": "template",
+        "template": {"name": "hello_world", "language": {"code": "en_US"}},
+    }
     headers = {
-            "Content-Type": "application/json",
-            "Authorization": "Bearer {}".format(TOKEN),
-        }
+        "Content-Type": "application/json",
+        "Authorization": "Bearer {}".format(TOKEN),
+    }
     resp = requests.post(f"{url}", headers=headers, json=data)
-    return resp
+    return resp
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/beep_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/beep_notifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import sys
 import os
 import platform
 import winsound
-from ExceptNotifier import beep 
+from ExceptNotifier import beep
 
 
 class ExceptBeep(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
@@ -17,66 +17,61 @@
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        
+
         beep(BEEP_TIME)
         beep(BEEP_TIME)
         beep(BEEP_TIME)
         beep(BEEP_TIME)
         beep(BEEP_TIME)
 
-
     @staticmethod
     def beep(sec=1, freq=1000) -> None:
         """Make beep sound
 
         :param sec: beep duration, defaults to 1
         :type sec: int, optional
         :param freq: beep fequency, defaults to 1000
         :type freq: int, optional
         """
 
         sys = platform.system()
 
         if sys == "Windows":
-            winsound.Beep(int(1000*sec), freq)
+            winsound.Beep(int(1000 * sec), freq)
         else:
-            os.system('play -nq -t alsa synth {} sine {}'.format(sec, freq))
-
-
+            os.system("play -nq -t alsa synth {} sine {}".format(sec, freq))
 
 
 class SuccessBeep:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         beep(BEEP_TIME)
         beep(BEEP_TIME)
 
 
-
 class SendBeep:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         beep(BEEP_TIME)
 
 
-
 if __name__ == "__main__":
     BEEP_TIME = 1
     sys.excepthook = ExceptBeep.__call__
 
     try:
-        print(1/20)  
-        SuccessBeep().__call__() #1 success beep-beep          
+        print(1 / 20)
+        SuccessBeep().__call__()  # 1 success beep-beep
 
-    except ExceptBeep as e:      #2 except beep-beep                
+    except ExceptBeep as e:  # 2 except beep-beep
         sys.exit()
 
-    SendBeep().__call__()        #3 customized beep-beep              
+    SendBeep().__call__()  # 3 customized beep-beep
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/chime_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/teams_notifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,155 +1,167 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
+import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-import urllib3
 import json
-from ExceptNotifier.base.chime_sender import send_chime_msg
-from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier import send_teams_msg, receive_openai_advice
 
-
-
-http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
-class ExceptChime(BaseException):
+
+class ExceptTeams(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to AWS Chime.
+        """Override excepthook to send error message to Microsoft Teams.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] :warning: Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        print(exceptNotifier['BODY'])
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
-        send_chime_msg(_CHIME_WEBHOOK_URL, data['text'])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_teams_msg(_TEAMS_WEBHOOK_URL, data["text"])
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_chime_msg(_CHIME_WEBHOOK_URL, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_teams_msg(_TEAMS_WEBHOOK_URL, advice_msg)
         except Exception as e:
             print(e)
             pass
 
-
     @staticmethod
-    def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
-        """Send message to chat room through chime app's webhook url.
+    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
+        """Send message to chat room through microsoft teams app's webhook url.
 
-        :param _CHIME_WEBHOOK_URL: Webhook url from chime app
-        :type _CHIME_WEBHOOK_URL: str
+        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
+        :type _TEAMS_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
 
-        url = _CHIME_WEBHOOK_URL
-        message = {"Content": msg}
-        encoded_msg = json.dumps(message).encode("utf-8")
-        resp = http.request("POST", url, body=encoded_msg)
+        payload = {"text": msg}
+        headers = {"Content-Type": "application/json"}
+        resp = requests.post(
+            _TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload)
+        )
 
         return resp
 
 
-
-class SuccessChime:
+class SuccessTeams:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] :tada: Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        send_chime_msg(_CHIME_WEBHOOK_URL, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_teams_msg(_TEAMS_WEBHOOK_URL, data["text"])
 
-class SendChime:
+
+class SendTeams:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_chime_msg(_CHIME_WEBHOOK_URL, data['text'])
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_teams_msg(_TEAMS_WEBHOOK_URL, data["text"])
 
 
+if __name__ == "__main__":
 
+    """Follow next page"""
 
+    global _TEAMS_WEBHOOK_URL
+    _TEAMS_WEBHOOK_URL = "microsoft webhook _TEAMS_WEBHOOK_URL"
 
-if __name__ == "__main__":
-    
-    # Get your slcak bot and enter _CHIME_WEBHOOK_URL
-    """Get your Webhook _CHIME_WEBHOOK_URL from your chatroom. 
-    https://docs.aws.amazon.com/chime/latest/ag/webhooks.html"""
-
-    global _CHIME_WEBHOOK_URL 
-    _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx"
-    _OPEN_AI_API = "xxxxxxxxxxxxx"
-    _OPEN_AI_MODEL = "gpt-3.5-turbo"
-    sys.excepthook = ExceptChime.__call__
+    sys.excepthook = ExceptTeams.__call__
 
     try:
-        print(1/0)  
-        SuccessChime().__call__() #1 success sender          
+        print(1 / 20)
+        SuccessTeams().__call__()  # 1 success sender
 
-    except ExceptChime as e:      #2 except sender            
+    except ExceptTeams as e:  # 2 except sender
         sys.exit()
 
-    SendChime().__call__()        #3 customized sender          
+    SendTeams().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/desktop_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/desktop_notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright 2023 parkminwoo Authors.
-
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import re
 import sys
 import datetime
 import traceback
 from plyer import notification
 from email.message import EmailMessage
 from ExceptNotifier import send_desktop_msg, receive_openai_advice
@@ -21,110 +21,134 @@
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ⚠️ Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        exceptNotifier['BODY'] += '\nLocal by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        
-        print(exceptNotifier['BODY'])
-                    
-        send_desktop_msg(title = exceptNotifier['SUBJECT'], message=exceptNotifier['BODY'])
+        print(exceptNotifier["BODY"])
+
+        send_desktop_msg(
+            title=exceptNotifier["SUBJECT"], message=exceptNotifier["BODY"]
+        )
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_desktop_msg(title = "chatGPT: How to Debug your code.", message=advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_desktop_msg(
+                title="chatGPT: How to Debug your code.", message=advice_msg
+            )
         except Exception as e:
             print(e)
             pass
-        
-        
-
 
     @staticmethod
     def send_desktop_msg(title_msg: str, body_msg: str, DISP_TIME=5) -> None:
         """Sending notification to desktop
 
         :param title_msg: Title of message
         :type title_msg: str
         :param body_msg: Body of message
         :type body_msg: str
         :param DISP_TIME: Time duration, defaults to 5
         :type DISP_TIME: int, optional
         """
-        notification.notify(
-                title = title_msg,
-                message=body_msg ,
-                timeout=DISP_TIME)
+        notification.notify(title=title_msg, message=body_msg, timeout=DISP_TIME)
 
 
 class SuccessDesktop:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] 🎉 Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         send_desktop_msg(
-            title = exceptNotifier['SUBJECT'][:20],
-            message=exceptNotifier['BODY'][:200])
+            title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
+        )
 
 
 class SendDesktop:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
         send_desktop_msg(
-            title = exceptNotifier['SUBJECT'][:20],
-            message=exceptNotifier['BODY'][:200])
-
-
+            title=exceptNotifier["SUBJECT"][:20], message=exceptNotifier["BODY"][:200]
+        )
 
 
 if __name__ == "__main__":
     sys.excepthook = ExceptDesktop.__call__
     try:
-        print(1/0)  
-        SuccessDesktop().__call__() #1 success sender          
-    except ExceptDesktop as e:      #2 except sender            
+        print(1 / 0)
+        SuccessDesktop().__call__()  # 1 success sender
+    except ExceptDesktop as e:  # 2 except sender
         sys.exit()
-    SendDesktop().__call__()        #3 customized sender          
+    SendDesktop().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/discord_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/discord_notifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,154 +1,171 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 from ExceptNotifier import send_discord_msg, receive_openai_advice
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
+
 class ExceptDiscord(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         """Override excepthook to send error message to Discord.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] :warning: Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        print(exceptNotifier['BODY'])
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
-        send_discord_msg(_DISCORD_WEBHOOK_URL, data['text'])
-        
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        print(exceptNotifier["BODY"])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_discord_msg(_DISCORD_WEBHOOK_URL, data["text"])
+
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
             send_discord_msg(_DISCORD_WEBHOOK_URL, advice_msg)
         except Exception as e:
             print(e)
             pass
 
-
     @staticmethod
     def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through discord app's webhook url.
 
         :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
         :type _DISCORD_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
-        try: 
+        try:
             from discord import Webhook, RequestsWebhookAdapter
-            webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
+
+            webhook = Webhook.from_url(
+                _DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter()
+            )
             resp = webhook.send(msg)
         except:
             from discord import SyncWebhook
-            webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL) # Initializing webhook
-            webhook.send(content=msg) 
-        return resp
-
 
+            webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL)  # Initializing webhook
+            webhook.send(content=msg)
+        return resp
 
 
 class SuccessDiscord:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] :tada: Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        send_discord_msg(_DISCORD_WEBHOOK_URL, data['text'][:2000])
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_discord_msg(_DISCORD_WEBHOOK_URL, data["text"][:2000])
 
 
 class SendDiscord:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_discord_msg(_DISCORD_WEBHOOK_URL, data['text'][:2000])
-
-
-
-
-
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_discord_msg(_DISCORD_WEBHOOK_URL, data["text"][:2000])
 
 
 if __name__ == "__main__":
-    
+
     # Get your slcak bot and enter _DISCORD_WEBHOOK_URL
     """Get your _DISCORD_WEBHOOK_URL from HERE. 
     https://discord.com/developers/docs/resources/webhook"""
 
-    global _DISCORD_WEBHOOK_URL 
+    global _DISCORD_WEBHOOK_URL
     _DISCORD_WEBHOOK_URL = "xxxxxxxxxxxxxxxxx"
-    
+
     sys.excepthook = ExceptDiscord.__call__
 
     try:
-        print(1/20)  
-        SuccessDiscord().__call__() #1 success sender          
+        print(1 / 20)
+        SuccessDiscord().__call__()  # 1 success sender
 
-    except ExceptDiscord as e:      #2 except sender            
+    except ExceptDiscord as e:  # 2 except sender
         sys.exit()
 
-    SendDiscord().__call__()        #3 customized sender          
+    SendDiscord().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/kakao_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/line_notifier.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,165 @@
-#-*- coding: utf-8 -*- 
-# Copyright 2023 parkminwoo
+# Copyright 2023 parkminwoo Authors.
+
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-import json
-from ExceptNotifier import send_kakao_msg, receive_openai_advice
+from ExceptNotifier import send_line_msg
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptKakao(BaseException):
+class ExceptLine(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Kakaotalk.
+        """Override excepthook to send error message to Line.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ** Error! ** Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - Code Status: Fail. \n - Detail: Python Code Ran Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocal by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        print(exceptNotifier['BODY'])
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
-        
-        send_kakao_msg(_KAKAO_TOKEN_PATH, data['text'])
-        
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        print(exceptNotifier["BODY"])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_line_msg(_LINE_NOTIFY_API_TOKEN, data["text"])
+
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_kakao_msg(_KAKAO_TOKEN_PATH, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_line_msg(_LINE_NOTIFY_API_TOKEN, advice_msg)
         except Exception as e:
-            print(e)
             pass
 
-
     @staticmethod
-    def send_kakao_msg(_KAKAO_TOKEN_PATH: str, msg: str) -> dict:
-        """Send message to chat room through kakaotalk app's REST API.
+    def send_line_msg(_LINE_NOTIFY_API_TOKEN: str, msg: str) -> dict:
+        """Send message to chat room through Line app's REST API.
 
-        :param _KAKAO_TOKEN_PATH: Kakaotalk token path
-        :type _KAKAO_TOKEN_PATH: str
+        :param _LINE_NOTIFY_API_TOKEN: Line notify API token
+        :type _LINE_NOTIFY_API_TOKEN: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
 
-        with open(_KAKAO_TOKEN_PATH,"r") as kakao:
-            tokens = json.load(kakao)
-
-        url="https://kapi.kakao.com/v2/api/talk/memo/default/send"
-        headers={
-            "Authorization" : "Bearer " + tokens["access_token"]
-        }
-        data = {
-            'object_type': 'text',
-            'text': msg,
-            'link': {
-                'web_url': 'https://developers.kakao.com',
-                'mobile_web_url': 'https://developers.kakao.com'
-            }
-        }
-        
-        data = {'template_object': json.dumps(data)}
-        resp = requests.post(url, headers=headers, data=data)
-
+        api_url = "https://notify-api.line.me/api/notify"
+        headers = {"Authorization": "Bearer " + _LINE_NOTIFY_API_TOKEN}
+        message = {"message": msg}
+        resp = requests.post(api_url, headers=headers, data=message)
         return resp
 
 
-
-class SuccessKakao:
+class SuccessLine:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] ** Success! ** Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_kakao_msg(_KAKAO_TOKEN_PATH, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-class SendKakao:
+        send_line_msg(_LINE_NOTIFY_API_TOKEN, data["text"])
+
+
+class SendLine:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        with open(_KAKAO_TOKEN_PATH,"r") as kakao:
-            tokens = json.load(kakao)
-
-        send_kakao_msg(_KAKAO_TOKEN_PATH, data['text'])
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_line_msg(_LINE_NOTIFY_API_TOKEN, data["text"])
 
 
+if __name__ == "__main__":
 
+    """Get your URL from HERE. 
+    https://notify-bot.line.me/my/"""
 
-if __name__ == "__main__":
-    
-    """Follow next notebooks"""
+    global _LINE_NOTIFY_API_TOKEN
+    _LINE_NOTIFY_API_TOKEN = "xxxxxxxxxxx"
 
-    global _KAKAO_TOKEN_PATH 
-    _KAKAO_TOKEN_PATH = r'C:\Users\parkm\Desktop\git\ExceptionNotifier\tutorials\token.json'
-    
-    sys.excepthook = ExceptKakao.__call__
+    sys.excepthook = ExceptLine.__call__
 
     try:
-        print(1/0)  
-        SuccessKakao().__call__() #1 success sender          
+        print(1 / 20)
+        SuccessLine().__call__()  # 1 success sender
 
-    except ExceptKakao as e:      #2 except sender            
+    except ExceptLine as e:  # 2 except sender
         sys.exit()
 
-    SendKakao().__call__()        #3 customized sender          
+    SendLine().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/line_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/chime_notifier.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,145 +1,172 @@
-# Copyright 2023 parkminwoo Authors.
-
-import requests
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-from ExceptNotifier import send_line_msg
+import urllib3
+import json
+from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
+
+http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptLine(BaseException):
+class ExceptChime(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Line.
+        """Override excepthook to send error message to AWS Chime.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ⚠️ Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :x: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        exceptNotifier['BODY'] += '\nLocal by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        print(exceptNotifier['BODY'])
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        send_line_msg(_LINE_NOTIFY_API_TOKEN, data['text'])
+        print(exceptNotifier["BODY"])
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_chime_msg(_CHIME_WEBHOOK_URL, data["text"])
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_line_msg(_LINE_NOTIFY_API_TOKEN, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_chime_msg(_CHIME_WEBHOOK_URL, advice_msg)
         except Exception as e:
+            print(e)
             pass
 
     @staticmethod
-    def send_line_msg(_LINE_NOTIFY_API_TOKEN: str, msg: str) -> dict:
-        """Send message to chat room through Line app's REST API.
+    def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
+        """Send message to chat room through chime app's webhook url.
 
-        :param _LINE_NOTIFY_API_TOKEN: Line notify API token
-        :type _LINE_NOTIFY_API_TOKEN: str
+        :param _CHIME_WEBHOOK_URL: Webhook url from chime app
+        :type _CHIME_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
 
-        api_url = "https://notify-api.line.me/api/notify"
-        headers = {'Authorization':'Bearer '+ _LINE_NOTIFY_API_TOKEN}
-        message = {
-            "message" : msg
-        }
-        resp = requests.post(api_url, headers= headers , data = message)
-        return resp
-
+        url = _CHIME_WEBHOOK_URL
+        message = {"Content": msg}
+        encoded_msg = json.dumps(message).encode("utf-8")
+        resp = http.request("POST", url, body=encoded_msg)
 
+        return resp
 
 
-class SuccessLine:
+class SuccessChime:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] 🎉 Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
-        send_line_msg(_LINE_NOTIFY_API_TOKEN, data['text'])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_chime_msg(_CHIME_WEBHOOK_URL, data["text"])
 
 
-class SendLine:
+class SendChime:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-
-        send_line_msg(_LINE_NOTIFY_API_TOKEN, data['text'])
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_chime_msg(_CHIME_WEBHOOK_URL, data["text"])
 
 
 if __name__ == "__main__":
-    
-    """Get your URL from HERE. 
-    https://notify-bot.line.me/my/"""
-
-    global _LINE_NOTIFY_API_TOKEN 
-    _LINE_NOTIFY_API_TOKEN = 'xxxxxxxxxxx'
-    
-    sys.excepthook = ExceptLine.__call__
+
+    # Get your slcak bot and enter _CHIME_WEBHOOK_URL
+    """Get your Webhook _CHIME_WEBHOOK_URL from your chatroom. 
+    https://docs.aws.amazon.com/chime/latest/ag/webhooks.html"""
+
+    global _CHIME_WEBHOOK_URL
+    _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx"
+    _OPEN_AI_API = "xxxxxxxxxxxxx"
+    _OPEN_AI_MODEL = "gpt-3.5-turbo"
+    sys.excepthook = ExceptChime.__call__
 
     try:
-        print(1/20)  
-        SuccessLine().__call__() #1 success sender          
+        print(1 / 0)
+        SuccessChime().__call__()  # 1 success sender
 
-    except ExceptLine as e:      #2 except sender            
+    except ExceptChime as e:  # 2 except sender
         sys.exit()
 
-    SendLine().__call__()        #3 customized sender          
+    SendChime().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/mail_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/mail_notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import sys
 import traceback
 import re
 import smtplib
 import datetime
 from email.message import EmailMessage
 from ExceptNotifier import send_gmail_msg, receive_openai_advice
-DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
+DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptMail(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
@@ -21,60 +21,104 @@
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
-        exceptNotifier = {'TO':_GAMIL_RECIPIENT_ADDR, 'FROM':_GMAIL_SENDER_ADDR, 'SUBJECT':'[Except Notifier] Error! Python Code Exception Detected', 'BODY':f'IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier.\n\n{excType}: %{etype.__doc__}\n\n {value} \n\n'}
-        SMTP_SERVER = 'smtp.gmail.com'
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
+        exceptNotifier = {
+            "TO": _GAMIL_RECIPIENT_ADDR,
+            "FROM": _GMAIL_SENDER_ADDR,
+            "SUBJECT": "[Except Notifier] Error! Python Code Exception Detected",
+            "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier.\n\n{excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
+        SMTP_SERVER = "smtp.gmail.com"
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier['BODY'] += f'\nTime Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += f"\nTime Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-        
-        print(exceptNotifier['BODY'])            
-        exceptNotifier['ALL'] = 'From: %s\nTo: %s\nSubject: %s\n\n%s' % (exceptNotifier['FROM'], exceptNotifier['TO'], exceptNotifier['SUBJECT'], exceptNotifier['BODY'])
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        print(exceptNotifier["BODY"])
+        exceptNotifier["ALL"] = "From: %s\nTo: %s\nSubject: %s\n\n%s" % (
+            exceptNotifier["FROM"],
+            exceptNotifier["TO"],
+            exceptNotifier["SUBJECT"],
+            exceptNotifier["BODY"],
+        )
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, 465)
         smtp.login(_GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER)
-        smtp.sendmail(exceptNotifier['FROM'], exceptNotifier['TO'], exceptNotifier['ALL'])
+        smtp.sendmail(
+            exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
+        )
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message[:150]) #NO-QA
-            exceptNotifier = {'TO':_GAMIL_RECIPIENT_ADDR, 'FROM':_GMAIL_SENDER_ADDR, 'SUBJECT':'[Except AI Debugging] Error! chatGPT Debugging guide.', 'BODY':f'IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}'}
-            smtp.sendmail(exceptNotifier['FROM'], exceptNotifier['TO'], exceptNotifier['ALL'])
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message[:150]
+            )  # NO-QA
+            exceptNotifier = {
+                "TO": _GAMIL_RECIPIENT_ADDR,
+                "FROM": _GMAIL_SENDER_ADDR,
+                "SUBJECT": "[Except AI Debugging] Error! chatGPT Debugging guide.",
+                "BODY": f"IMPORTANT WARNING: \nPython Exception Detected in Your Code. \n\nHi there, \nThis is advice from OpenAI ChatGPT \n\n {advice_msg}",
+            }
+            smtp.sendmail(
+                exceptNotifier["FROM"], exceptNotifier["TO"], exceptNotifier["ALL"]
+            )
         except Exception as e:
             pass
-        
+
         smtp.quit()
 
     @staticmethod
-    def send_gmail_msg(from_email_addr: str, to_email_addr: str, from_email_app_password: str, subject_msg: str, body_msg: str) -> dict:
+    def send_gmail_msg(
+        from_email_addr: str,
+        to_email_addr: str,
+        from_email_app_password: str,
+        subject_msg: str,
+        body_msg: str,
+    ) -> dict:
         """Send mail through gmail smtp server
 
         :param from_email_addr: Gmail address who send message
         :type from_email_addr: str
         :param to_email_addr: Gmail address who receive message
         :type to_email_addr: str
         :param from_email_app_password: Google app password
@@ -82,16 +126,16 @@
         :param subject_msg: Mail title
         :type subject_msg: str
         :param body_msg: Mail body
         :type body_msg: str
         :return: Response according to sending request
         :rtype: dict
         """
-        
-        SMTP_SERVER = 'smtp.gmail.com'
+
+        SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
         EMAIL_ADDR = from_email_addr
         EMAIL_PASSWORD = from_email_app_password
         smtp.login(EMAIL_ADDR, EMAIL_PASSWORD)
         message = EmailMessage()
         message.set_content(body_msg)
@@ -100,90 +144,75 @@
         message["To"] = to_email_addr
         resp = smtp.send_message(message)
         smtp.quit()
 
         return resp
 
 
-
 class SuccessMail:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
-        SMTP_SERVER = 'smtp.gmail.com'
+        SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
         smtp.login(_GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER)
         message = EmailMessage()
         start_time = datetime.datetime.now()
-        
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        message.set_content(f"Hi there, \nThis is a success notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)} \n - Code Status: Done. \n - Detail: Python Code Ran Without Exceptions. \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier")
-        message["Subject"] = "[Success Notifier] Success! Python Code Executed Successfully"
+
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        message.set_content(
+            f"Hi there, \nThis is a success notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)} \n - Code Status: Done. \n - Detail: Python Code Ran Without Exceptions. \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        )
+        message[
+            "Subject"
+        ] = "[Success Notifier] Success! Python Code Executed Successfully"
         message["From"] = _GMAIL_SENDER_ADDR
         message["To"] = _GAMIL_RECIPIENT_ADDR
-        
+
         smtp.send_message(message)
         smtp.quit()
 
 
 class SendMail:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
-        SMTP_SERVER = 'smtp.gmail.com'
+        SMTP_SERVER = "smtp.gmail.com"
         SMTP_PORT = 465
         smtp = smtplib.SMTP_SSL(SMTP_SERVER, SMTP_PORT)
         smtp.login(_GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER)
         message = EmailMessage()
         start_time = datetime.datetime.now()
-        
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        message.set_content(f"Hi there, \nThis is a customized notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)}\n - Code Status: Done. \n - Detail: Code Execution Reached Specified Line. \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier")
-        message["Subject"] = "[Codeline Notifier] Notice! Code Execution Reached Specified Line"
+
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        message.set_content(
+            f"Hi there, \nThis is a customized notifier.\n\n - Time: {start_time.strftime(DATE_FORMAT)}\n - Code Status: Done. \n - Detail: Code Execution Reached Specified Line. \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+        )
+        message[
+            "Subject"
+        ] = "[Codeline Notifier] Notice! Code Execution Reached Specified Line"
         message["From"] = _GMAIL_SENDER_ADDR
         message["To"] = _GAMIL_RECIPIENT_ADDR
         smtp.send_message(message)
         smtp.quit()
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     # Set global variables
     global _GAMIL_RECIPIENT_ADDR, _GMAIL_SENDER_ADDR, _GMAIL_APP_PASSWORD_OF_SENDER
-    _GAMIL_RECIPIENT_ADDR = 'parkminwoo1991@gmail.com'
-    _GMAIL_SENDER_ADDR = 'heydudenotice@gmail.com'
-    _GMAIL_APP_PASSWORD_OF_SENDER = 'xxxxxxxxxxx'
+    _GAMIL_RECIPIENT_ADDR = "parkminwoo1991@gmail.com"
+    _GMAIL_SENDER_ADDR = "heydudenotice@gmail.com"
+    _GMAIL_APP_PASSWORD_OF_SENDER = "xxxxxxxxxxx"
     sys.excepthook = ExceptMail.__call__
 
     try:
-        print(1/0)      
-        SuccessMail().__call__() #1 success sender
-
+        print(1 / 0)
+        SuccessMail().__call__()  # 1 success sender
 
-    except ExceptMail as e:      #2 except sender            
+    except ExceptMail as e:  # 2 except sender
         sys.exit()
 
-
-    SendMail().__call__()        #3 Any line sender
-
+    SendMail().__call__()  # 3 Any line sender
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/slack_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/slack_notifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,88 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 from ExceptNotifier import send_slack_msg, receive_openai_advice
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
+
 class ExceptSlack(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
         """Override excepthook to send error message to Slack.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] :warning: Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :large_red_square: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] :warning: Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - :x: Code Status: Fail. \n - :large_red_square: Detail: Python Code Ran Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(_SLACK_WEBHOOK_URL, data)
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
             send_slack_msg(_SLACK_WEBHOOK_URL, advice_msg)
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
     def send_slack_msg(_SLACK_WEBHOOK_URL: str, msg: str) -> dict:
@@ -69,74 +91,70 @@
         :param _SLACK_WEBHOOK_URL: _SLACK_WEBHOOK_URL from slack app
         :type _SLACK_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
-        
-        data = {'text':msg}
+
+        data = {"text": msg}
         resp = requests.post(url=_SLACK_WEBHOOK_URL, json=data)
         return resp
 
 
-
-
 class SuccessSlcak:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] :tada: Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] :tada: Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - :white_check_mark: Code Status: Success. \n - :white_check_mark: Detail: Python Code Ran Without Exceptions. \n - :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
         send_slack_msg(_SLACK_WEBHOOK_URL, data)
 
 
 class SendSlack:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        send_slack_msg(_SLACK_WEBHOOK_URL, data)
-
-
-
-
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] :clap: Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- :white_check_mark: Code Status: Done. \n- :white_check_mark: Detail: Code Execution Reached Specified Line.  \n- :clock2: Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_slack_msg(_SLACK_WEBHOOK_URL, data)
 
 
 if __name__ == "__main__":
-    
+
     # Get your slcak bot and enter _SLACK_WEBHOOK_URL
     """Get your _SLACK_WEBHOOK_URL from HERE. 
     https://api.slack.com/messaging/webhooks#create_a_webhook"""
 
-    global _SLACK_WEBHOOK_URL 
-    _SLACK_WEBHOOK_URL = 'https://hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx'
-    
+    global _SLACK_WEBHOOK_URL
+    _SLACK_WEBHOOK_URL = "https://hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx"
+
     sys.excepthook = ExceptSlack.__call__
 
     try:
-        print(1/0)  
-        SuccessSlcak().__call__() #1 success sender          
+        print(1 / 0)
+        SuccessSlcak().__call__()  # 1 success sender
 
-    except ExceptSlack as e:      #2 except sender            
+    except ExceptSlack as e:  # 2 except sender
         sys.exit()
 
-    SendSlack().__call__()        #3 customized sender          
+    SendSlack().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/sms_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/sms_notifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-#-*- coding: utf-8 -*- 
+# -*- coding: utf-8 -*-
 # Copyright 2023 parkminwoo
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 import pickle
 from twilio.rest import Client
 from ExceptNotifier import send_sms_msg, receive_openai_advice
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptSMS(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
@@ -21,112 +22,165 @@
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ** Error! ** Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - Code Status: Fail. \n - Detail: Python Code Ran Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ** Error! ** Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - Code Status: Fail. \n - Detail: Python Code Ran Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, data['text'])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_sms_msg(
+            _TWILIO_SID,
+            _TWILIO_TOKEN,
+            _SENDER_PHONE_NUMBER,
+            _RECIPIENT_PHONE_NUMBER,
+            data["text"],
+        )
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_sms_msg(
+                _TWILIO_SID,
+                _TWILIO_TOKEN,
+                _SENDER_PHONE_NUMBER,
+                _RECIPIENT_PHONE_NUMBER,
+                advice_msg,
+            )
         except Exception as e:
             print(e)
             pass
 
     @staticmethod
-    def send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg):
+    def send_sms_msg(
+        _TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, msg
+    ):
         client = Client(_TWILIO_SID, _TWILIO_TOKEN)
         client.messages.create(
-            to=_RECIPIENT_PHONE_NUMBER,
-            from_=_SENDER_PHONE_NUMBER,  
-        body=msg
-    )
-
+            to=_RECIPIENT_PHONE_NUMBER, from_=_SENDER_PHONE_NUMBER, body=msg
+        )
 
 
 class SuccessSMS:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] ** Success! ** Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] ** Success! ** Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_sms_msg(
+            _TWILIO_SID,
+            _TWILIO_TOKEN,
+            _SENDER_PHONE_NUMBER,
+            _RECIPIENT_PHONE_NUMBER,
+            data["text"],
+        )
+
 
 class SendSMS:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_sms_msg(_TWILIO_SID, _TWILIO_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_sms_msg(
+            _TWILIO_SID,
+            _TWILIO_TOKEN,
+            _SENDER_PHONE_NUMBER,
+            _RECIPIENT_PHONE_NUMBER,
+            data["text"],
+        )
+
 
 if __name__ == "__main__":
-    
+
     """https://www.twilio.com/en-us"""
 
     global _TWILIO_SID, TWILIO_AUTH_TOKEN, _SENDER_PHONE_NUMBER, _RECIPIENT_PHONE_NUMBER
-    _TWILIO_SID = 'xxxx'
-    _TWILIO_TOKEN = 'yyyyyy'
-    _RECIPIENT_PHONE_NUMBER="+aaaaaa",
-    _SENDER_PHONE_NUMBER="+bbbbbb",  
-    
+    _TWILIO_SID = "xxxx"
+    _TWILIO_TOKEN = "yyyyyy"
+    _RECIPIENT_PHONE_NUMBER = ("+aaaaaa",)
+    _SENDER_PHONE_NUMBER = ("+bbbbbb",)
+
     sys.excepthook = ExceptSMS.__call__
 
     try:
-        print(1/10)  
-        SuccessSMS().__call__() #1 success sender          
+        print(1 / 10)
+        SuccessSMS().__call__()  # 1 success sender
 
-    except ExceptSMS as e:      #2 except sender    
+    except ExceptSMS as e:  # 2 except sender
         with open("exceptError.pickle", "wb") as f:
             pickle.dump(e, f)
         raise pickle.load(f)
         sys.exit()
-    
-    SendSMS().__call__()        #3 customized sender          
+
+    SendSMS().__call__()  # 3 customized sender
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/teams_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/telegram_notifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,170 @@
-# Copyright 2023 parkminwoo Authors.
-
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-import json
-from ExceptNotifier import send_teams_msg, receive_openai_advice
+from ExceptNotifier import send_telegram_msg, receive_openai_advice
 
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptTeams(BaseException):
+class ExceptTelegram(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Microsoft Teams.
+        """Override excepthook to send error message to Telegram.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ⚠️ Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        
-        exceptNotifier['BODY'] += '\nLocal by frame, innermost last::::'
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
 
-        send_teams_msg(_TEAMS_WEBHOOK_URL, data['text'])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_telegram_msg(_TELEGRAM_TOKEN, data["text"])
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_teams_msg(_TEAMS_WEBHOOK_URL, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_telegram_msg(_TELEGRAM_TOKEN, advice_msg)
         except Exception as e:
             print(e)
             pass
 
-
-
     @staticmethod
-    def send_teams_msg(_TEAMS_WEBHOOK_URL, msg):
-        """Send message to chat room through microsoft teams app's webhook url.
+    def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
+        """Send message via telegram bot.
 
-        :param _TEAMS_WEBHOOK_URL: _TEAMS_WEBHOOK_URL from teams app
-        :type _TEAMS_WEBHOOK_URL: str
-        :param msg: Message text
+        :param _TELEGRAM_TOKEN: Telegram secure bot Token
+        :type _TELEGRAM_TOKEN: str
+        :param msg: Message content
         :type msg: str
-        :return: Response according to REST API request
+        :return: Response dict
         :rtype: dict
         """
-        
-        payload = {
-            "text": msg
-        }
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        resp = requests.post(_TEAMS_WEBHOOK_URL, headers=headers, data=json.dumps(payload))
+        url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/getUpdates"
+        req_dict = requests.get(url).json()
+        bot_id = dict(
+            dict(dict(list(dict(req_dict).values())[1][0])["message"])["from"]
+        )["id"]
+        bot_url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/sendMessage?chat_id={bot_id}&text={msg}"
+        resp = requests.get(bot_url).json()
 
         return resp
 
 
-
-class SuccessTeams:
+class SuccessTelegram:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] 🎉 Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
-        send_teams_msg(_TEAMS_WEBHOOK_URL, data['text'])
+        send_telegram_msg(_TELEGRAM_TOKEN, data["text"])
 
 
-class SendTeams:
+class SendTelegram:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-
-        send_teams_msg(_TEAMS_WEBHOOK_URL, data['text'])
-
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_telegram_msg(_TELEGRAM_TOKEN, data["text"])
 
 
 if __name__ == "__main__":
-    
-    """Follow next page"""
 
-    global _TEAMS_WEBHOOK_URL 
-    _TEAMS_WEBHOOK_URL = 'microsoft webhook _TEAMS_WEBHOOK_URL'
-    
-    sys.excepthook = ExceptTeams.__call__
+    """Get your bot from botfather. 
+    https://core.telegram.org/bots/tutorial"""
+
+    global _TELEGRAM_TOKEN
+    _TELEGRAM_TOKEN = "xxxxxxxxxxx"
+    _OPEN_AI_MODEL = "gpt-3.5-turbo"
+    _OPEN_AI_API = "sk-xxxxxxxxx"
+    sys.excepthook = ExceptTelegram.__call__
 
     try:
-        print(1/20)  
-        SuccessTeams().__call__() #1 success sender          
+        print(1 / 0)
+        SuccessTelegram().__call__()  # 1 success sender
 
-    except ExceptTeams as e:      #2 except sender            
+    except ExceptTelegram as e:  # 2 except sender
         sys.exit()
 
-    SendTeams().__call__()        #3 customized sender          
+    SendTelegram().__call__()  # 3 customized sender
+
+    send = SendTelegram()  # You can use it like this, too.
+    send()
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/telegram_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/kakao_notifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,184 @@
-# Copyright 2023 parkminwoo Authors.
-
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-from ExceptNotifier import send_telegram_msg, receive_openai_advice
+import json
+from ExceptNotifier import send_kakao_msg, receive_openai_advice
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
-class ExceptTelegram(BaseException):
+class ExceptKakao(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
-        """Override excepthook to send error message to Telegram.
+        """Override excepthook to send error message to Kakaotalk.
 
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ⚠️ Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ** Error! ** Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - Code Status: Fail. \n - Detail: Python Code Ran Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\n :no_entry: {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
-        send_telegram_msg(_TELEGRAM_TOKEN, data['text'])
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        print(exceptNotifier["BODY"])
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_kakao_msg(_KAKAO_TOKEN_PATH, data["text"])
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
-            send_telegram_msg(_TELEGRAM_TOKEN, advice_msg)
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
+            send_kakao_msg(_KAKAO_TOKEN_PATH, advice_msg)
         except Exception as e:
             print(e)
             pass
 
-
     @staticmethod
-    def send_telegram_msg(_TELEGRAM_TOKEN: str, msg: str) -> dict:
-        """Send message via telegram bot.
+    def send_kakao_msg(_KAKAO_TOKEN_PATH: str, msg: str) -> dict:
+        """Send message to chat room through kakaotalk app's REST API.
 
-        :param _TELEGRAM_TOKEN: Telegram secure bot Token
-        :type _TELEGRAM_TOKEN: str
-        :param msg: Message content
+        :param _KAKAO_TOKEN_PATH: Kakaotalk token path
+        :type _KAKAO_TOKEN_PATH: str
+        :param msg: Message text
         :type msg: str
-        :return: Response dict
+        :return: Response according to REST API request
         :rtype: dict
         """
-        url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/getUpdates"
-        req_dict = requests.get(url).json()
-        bot_id = dict(dict(dict(list(dict(req_dict).values())[1][0])['message'])['from'])['id']
-        bot_url = f"https://api.telegram.org/bot{_TELEGRAM_TOKEN}/sendMessage?chat_id={bot_id}&text={msg}"
-        resp = requests.get(bot_url).json()
 
-        return resp
+        with open(_KAKAO_TOKEN_PATH, "r") as kakao:
+            tokens = json.load(kakao)
+
+        url = "https://kapi.kakao.com/v2/api/talk/memo/default/send"
+        headers = {"Authorization": "Bearer " + tokens["access_token"]}
+        data = {
+            "object_type": "text",
+            "text": msg,
+            "link": {
+                "web_url": "https://developers.kakao.com",
+                "mobile_web_url": "https://developers.kakao.com",
+            },
+        }
+
+        data = {"template_object": json.dumps(data)}
+        resp = requests.post(url, headers=headers, data=data)
 
+        return resp
 
 
-class SuccessTelegram:
+class SuccessKakao:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] 🎉 Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_telegram_msg(_TELEGRAM_TOKEN, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] ** Success! ** Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - Code Status: Success. \n - Detail: Python Code Ran Without Exceptions. \n - Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_kakao_msg(_KAKAO_TOKEN_PATH, data["text"])
 
-class SendTelegram:
+
+class SendKakao:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_telegram_msg(_TELEGRAM_TOKEN, data['text'])
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] ** Notice! ** Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- Code Status: Done. \n- Detail: Code Execution Reached Specified Line.  \n- Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        with open(_KAKAO_TOKEN_PATH, "r") as kakao:
+            tokens = json.load(kakao)
 
+        send_kakao_msg(_KAKAO_TOKEN_PATH, data["text"])
 
 
+if __name__ == "__main__":
 
+    """Follow next notebooks"""
 
+    global _KAKAO_TOKEN_PATH
+    _KAKAO_TOKEN_PATH = (
+        r"C:\Users\parkm\Desktop\git\ExceptionNotifier\tutorials\token.json"
+    )
 
-if __name__ == "__main__":
-    
-    """Get your bot from botfather. 
-    https://core.telegram.org/bots/tutorial"""
-
-    global _TELEGRAM_TOKEN 
-    _TELEGRAM_TOKEN = "xxxxxxxxxxx"
-    _OPEN_AI_MODEL="gpt-3.5-turbo"
-    _OPEN_AI_API="sk-xxxxxxxxx"
-    sys.excepthook = ExceptTelegram.__call__
+    sys.excepthook = ExceptKakao.__call__
 
     try:
-        print(1/0)  
-        SuccessTelegram().__call__() #1 success sender          
+        print(1 / 0)
+        SuccessKakao().__call__()  # 1 success sender
 
-    except ExceptTelegram as e:      #2 except sender            
+    except ExceptKakao as e:  # 2 except sender
         sys.exit()
 
-    SendTelegram().__call__()        #3 customized sender          
-
-
-
-
-
-
-
-    send = SendTelegram()            # You can use it like this, too.
-    send()
+    SendKakao().__call__()  # 3 customized sender
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.1.9/ExceptNotifier/utils/kakao_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import requests
 import json
 
+
 def get_authorize_code(rest_api_key: str) -> None:
     """Get authorize code link by using KAKAO REST API KEY
 
     :param rest_api_key: REST API KEY
     :type rest_api_key: str
     """
-    redirect_uri = 'https://example.com/oauth'
+    redirect_uri = "https://example.com/oauth"
     print()
-    print(f'\n\nhttps://kauth.kakao.com/oauth/authorize?client_id={rest_api_key}&redirect_uri={redirect_uri}&response_type=code')
-    
+    print(
+        f"\n\nhttps://kauth.kakao.com/oauth/authorize?client_id={rest_api_key}&redirect_uri={redirect_uri}&response_type=code"
+    )
+
 
 def save_token(rest_api_key: str, authorize_code: str, token_path: str) -> dict:
     """Receive authorized token and save it in json format.
 
     :param rest_api_key: REST API KEY
     :type rest_api_key: str
     :param authorize_code: The code that comes out when you click the link that comes as the return value of the get_authorize_code function.
     :type authorize_code: str
     :param token_path: Path to store token
     :type token_path: str
     :return: Generated tokens
     :rtype: dict
     """
 
-    redirect_uri = 'https://example.com/oauth'
-    url_token = 'https://kauth.kakao.com/oauth/token'
+    redirect_uri = "https://example.com/oauth"
+    url_token = "https://kauth.kakao.com/oauth/token"
     data = {
-        'grant_type':'authorization_code',
-        'client_id':rest_api_key,
-        'redirect_uri':redirect_uri,
-        'code': authorize_code,
+        "grant_type": "authorization_code",
+        "client_id": rest_api_key,
+        "redirect_uri": redirect_uri,
+        "code": authorize_code,
     }
     response = requests.post(url_token, data=data)
     tokens = response.json()
-    with open(token_path,"w") as f:
+    with open(token_path, "w") as f:
         json.dump(tokens, f)
-    
-    return tokens
 
+    return tokens
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier/wechat_notifier.py` & `exceptnotifier-0.1.9/ExceptNotifier/wechat_notifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Copyright 2023 parkminwoo Authors.
-
+# -*- coding: utf-8 -*-
+# Copyright 2023 parkminwoo
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 from ExceptNotifier import send_wechat_msg, receive_openai_advice
+
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptWechat(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
@@ -20,133 +21,142 @@
         :param etype: Error Type
         :type etype: _type_
         :param value: Error Value
         :type value: _type_
         :param tb: Traceback Information
         :type tb: _type_
         """
-        excType = re.sub('(<(type|class \')|\'exceptions.|\'>|__main__.)', '', str(etype)).strip()
+        excType = re.sub(
+            "(<(type|class ')|'exceptions.|'>|__main__.)", "", str(etype)
+        ).strip()
         start_time = datetime.datetime.now()
-        
-        exceptNotifier = {'SUBJECT':'[Except Notifier] ⚠️ Error! Python Code Exception Detected', 'BODY':f'\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n'}
+
+        exceptNotifier = {
+            "SUBJECT": "[Except Notifier] ⚠️ Error! Python Code Exception Detected",
+            "BODY": f"\n\nIMPORTANT WARNING \nPython Exception Detected in Your Code. \n\nHi there, \nThis is an exception catch notifier. \n\n - ☑️ Code Status: Fail.🛠 \n - ☑️ Detail: Python Code Ran Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\n ⛔️ {excType}: %{etype.__doc__}\n\n {value} \n\n",
+        }
         for line in traceback.extract_tb(tb):
-            exceptNotifier['BODY'] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            exceptNotifier["BODY"] += '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
         while 1:
-            if not tb.tb_next: break
+            if not tb.tb_next:
+                break
             tb = tb.tb_next
         stack = []
         f = tb.tb_frame
         while f:
             stack.append(f)
             f = f.f_back
         stack.reverse()
-        exceptNotifier['BODY'] += '\nLocals by frame, innermost last::::'
+        exceptNotifier["BODY"] += "\nLocals by frame, innermost last::::"
         for frame in stack:
-            exceptNotifier['BODY'] += '\nFrame %s in %s at line %s' % (frame.f_code.co_name, frame.f_code.co_filename, frame.f_lineno)
+            exceptNotifier["BODY"] += "\nFrame %s in %s at line %s" % (
+                frame.f_code.co_name,
+                frame.f_code.co_filename,
+                frame.f_lineno,
+            )
             for key, val in frame.f_locals.items():
-                exceptNotifier['BODY'] += '\n\t%20s = ' % key
+                exceptNotifier["BODY"] += "\n\t%20s = " % key
                 try:
-                    exceptNotifier['BODY'] += str(val)
+                    exceptNotifier["BODY"] += str(val)
                 except:
-                    exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
-                    
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
-        send_wechat_msg(_WECHAT_WEBHOOK_URL, data['text'])
+                    exceptNotifier["BODY"] += "<ERROR WHILE PRINTING VALUE>"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+        send_wechat_msg(_WECHAT_WEBHOOK_URL, data["text"])
 
         try:
-            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
-            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
-            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message) #NO-QA
+            error_message = f"error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}"
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (
+                line[0],
+                line[2],
+                line[1],
+                line[3],
+            )
+            advice_msg += receive_openai_advice(
+                _OPEN_AI_MODEL, _OPEN_AI_API, error_message
+            )  # NO-QA
             send_wechat_msg(_WECHAT_WEBHOOK_URL, advice_msg)
         except Exception as e:
             print(e)
             pass
 
-
     @staticmethod
     def send_wechat_msg(_WECHAT_WEBHOOK_URL: str, msg: str) -> None:
         """Send message to wechat.
 
         :param _WECHAT_WEBHOOK_URL: Wechat Webhook URL https://work.weixin.qq.com/api/doc/90000/90136/91770
         :type _WECHAT_WEBHOOK_URL: str
         :param msg: Message to send
         :type msg: str
         """
-        msg_template = {
-            "msgtype": "text", 
-            "text": {
-                "content": ""
-            }
-        }
-        msg_template['text']['content'] = '\n'.join(msg)
+        msg_template = {"msgtype": "text", "text": {"content": ""}}
+        msg_template["text"]["content"] = "\n".join(msg)
         requests.post(_WECHAT_WEBHOOK_URL, json=msg_template)
 
 
-
 class SuccessWechat:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Success Notifier] 🎉 Success! Python Code Executed Successfully"}
-        exceptNotifier["BODY"]=f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_wechat_msg(_WECHAT_WEBHOOK_URL, data['text'])
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Success Notifier] 🎉 Success! Python Code Executed Successfully"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a success notifier.\n\n - ✅ Code Status: Success. \n - ✅ Detail: Python Code Ran Without Exceptions. \n - 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nI just wanted to let you know that your Python code has run successfully without any exceptions. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
+
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
+
+        send_wechat_msg(_WECHAT_WEBHOOK_URL, data["text"])
 
 
 class SendWechat:
     def __init__(self) -> None:
         pass
-        
+
     def __call__(self, *args, **kwds) -> None:
         exceptNotifier = EmailMessage()
         start_time = datetime.datetime.now()
-        f'Time Stamp: {start_time.strftime(DATE_FORMAT)}'
-        exceptNotifier = {"SUBJECT":"[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"}
-        exceptNotifier["BODY"] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
-        
-        data = {'text':exceptNotifier['SUBJECT']+exceptNotifier["BODY"]}
-        
-        send_wechat_msg(_WECHAT_WEBHOOK_URL, data['text'])
-
-
-
-
-
-
+        f"Time Stamp: {start_time.strftime(DATE_FORMAT)}"
+        exceptNotifier = {
+            "SUBJECT": "[Codeline Notifier] 👏 Notice! Code Execution Reached Specified Line"
+        }
+        exceptNotifier[
+            "BODY"
+        ] = f"\n\nHi there, \nThis is a customized notifier.\n\n- ✅ Code Status: Done. \n- ✅ Detail: Code Execution Reached Specified Line.  \n- 🕐 Time: {start_time.strftime(DATE_FORMAT)} \n\nThe code has reached the line where you requested an email to be sent. As per your instruction, we are sending this email. \n\nAll the best, \nExcept Notifier https://github.com/dsdanielpark/ExceptNotifier"
 
+        data = {"text": exceptNotifier["SUBJECT"] + exceptNotifier["BODY"]}
 
+        send_wechat_msg(_WECHAT_WEBHOOK_URL, data["text"])
 
 
 if __name__ == "__main__":
-    
+
     """Get your wechat webhook URL. 
     https://work.weixin.qq.com/api/doc/90000/90136/91770"""
 
-    global _WECHAT_WEBHOOK_URL 
+    global _WECHAT_WEBHOOK_URL
     _WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
-    _OPEN_AI_MODEL="gpt-3.5-turbo"
-    _OPEN_AI_API="sk-xxxxxxxxx"
+    _OPEN_AI_MODEL = "gpt-3.5-turbo"
+    _OPEN_AI_API = "sk-xxxxxxxxx"
     sys.excepthook = ExceptWechat.__call__
 
     try:
-        print(1/0)  
-        SuccessWechat().__call__() #1 success sender          
+        print(1 / 0)
+        SuccessWechat().__call__()  # 1 success sender
 
-    except ExceptWechat as e:      #2 except sender            
+    except ExceptWechat as e:  # 2 except sender
         sys.exit()
 
-    SendWechat().__call__()        #3 customized sender          
-
-
-
-
-
-
+    SendWechat().__call__()  # 3 customized sender
 
-    send = SendWechat()            # You can use it like this, too.
-    send()
+    send = SendWechat()  # You can use it like this, too.
+    send()
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,25 @@
-Metadata-Version: 2.1
-Name: exceptnotifier
-Version: 0.1.8
-Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
-Home-page: https://github.com/dsdanielpark/ExceptNotifier
-Author: daniel park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ExceptNotifier_logo.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/logo2.png)
 
-<h3 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h3>
+<h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
-<a href="https://anaconda.org/conda-forge/exceptnotifier/"><img alt="conda-forge" src="https://img.shields.io/conda/dn/conda-forge/exceptnotifier.svg?label=conda-forge"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main3.png)
+##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
-##### Provides a notification from the application shown in the captured screen.
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 <Br>
 
 #### Could you kindly add this badge to your repository?
@@ -50,15 +27,57 @@
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 
 <br><br>
 
-### Supporting Applications
+
+
+
+# Contents
+
+- [OPEN AI API](https://platform.openai.com/docs/introduction)
+- [Python Package: ExceptNotifier](#python-package--exceptnotifier)
+- [Supporting Applications](#supporting-applications)
+  * [AI Debugging using OpenAI API](#ai-debugging-using-openai-api)
+- [Quick Start](#quick-start)
+- [App Setup Overview](#app-setup-overview)
+- [1. Key Features](#1-key-features)
+  * [1-1. Except`[appName]`](#1-1-except--appname--)
+  * [1-2. AI Debbugging Infomation Notification](#1-2-ai-debbugging-infomation-notification)
+  * [1-3. Success`[appName]`](#1-3-success--appname--)
+  * [1-4. Send`[appName]`](#1-4-send--appname--)
+<details>
+<summary> See more...</summary>
+- [Feature](#feature)
+  * [2. Notifier](#2-notifier)
+    + [2-1. *Telegram Notifier*](#2-1--telegram-notifier-)
+      - [a. Without OpenAI API](#a-without-openai-api)
+      - [b. With OpenAI API](#b-with-openai-api)
+    + [2-2. *Mail Notifier*](#2-2--mail-notifier-)
+    + [2-3. *Discord Notifier*](#2-3--discord-notifier-)
+    + [2-4. *Chime Notifier*](#2-4--chime-notifier-)
+    + [2-5. *Slack Notifier*](#2-5--slack-notifier-)
+    + [2-6. *Line Notifier*](#2-6--line-notifier-)
+    + [2-7. *SMS Notifier*](#2-7--sms-notifier-)
+    + [2-8. *Teams Notifier*](#2-8--teams-notifier-)
+    + [2-9. *Kakaotalk Notifier*](#2-9--kakaotalk-notifier-)
+    + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-)
+    + [2-11. *Beep Notifier*](#2-11--beep-notifier-)
+    + [2-12. *Desktop Notifier*](#2-12--desktop-notifier-)
+  * [3. Sender](#3-sender)
+- [License](#license)
+- [Code of Conduct](#code-of-conduct)
+
+</details>
+
+<br><br>
+
+# Supporting Applications
 
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
@@ -69,26 +88,22 @@
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
 If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-- [OPEN AI API](https://platform.openai.com/docs/introduction)
+-  [Opea AI API](https://openai.com/blog/openai-api)
 
 
-<br><br>
+<br>
 
 # Quick Start
 ```bash
-pip install ExceptNotifier
-pip install exceptnotifier
-
-conda install ExceptNotifier
-conda install exceptnotifier
+$ pip install ExceptNotifier    #pip install exceptnotifier
 ```
 
 <br>
 
 
 # App Setup Overview
 
@@ -117,14 +132,16 @@
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](https://github.com/dsdanielpark/ExceptNotifier/blob/main/documents/APIOpenAI/GUIDE.md)|
 
 
 <br><br>
 
+
+
 # 1. Key Features
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 ## 1-1. Except`[appName]`
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
@@ -205,17 +222,18 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# Feature
 
-## Notifier
+# Features
+
+## 2. Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
 ### 2-1. *Telegram Notifier*
 
@@ -618,15 +636,15 @@
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
-## Sender
+## 3. Sender
 
 
 
 <Br><br><br>
 
 # License
 MIT
```

#### html2text {}

```diff
@@ -1,59 +1,65 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.8 Summary: With
-Python's try-except to receive notifications about Errors or Successes in your
-code through messenger app or email. Home-page: https://github.com/
-dsdanielpark/ExceptNotifier Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
-Alarm,Error notifications,Customizable notifications,Traceback
-management,Single line alarm Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 3 - Alpha
+Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-ExceptNotifier_logo.png)
-  **** Integrates AI-assisted debugging notifications into Python try-except
-              statements for various messaging applications. ****
-              [PyPI] [Downloads] [conda-forge] [Code_style:_black]
+logo2.png)
+   ** Integrates AI-assisted debugging notifications into Python try-except
+               statements for various messaging applications. **
+                     [PyPI] [Downloads] [Code_style:_black]
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-main2.png) # Python Package: ExceptNotifier ##### Provides a notification from
-the application shown in the captured screen. The `ExceptNotifier` Python
+main3.png) ##### Provides a notification from the application shown in the
+captured screen. # Python Package: ExceptNotifier The `ExceptNotifier` Python
 package offers a flexible approach to receiving notifications by enhancing
 Python's try-except statement. This package enables you to receive alerts
 through various messaging applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process.
 #### Could you kindly add this badge to your repository? ``` ![Except-Notifier]
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
-### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
+# Contents - [OPEN AI API](https://platform.openai.com/docs/introduction) -
+[Python Package: ExceptNotifier](#python-package--exceptnotifier) - [Supporting
+Applications](#supporting-applications) * [AI Debugging using OpenAI API](#ai-
+debugging-using-openai-api) - [Quick Start](#quick-start) - [App Setup
+Overview](#app-setup-overview) - [1. Key Features](#1-key-features) * [1-1.
+Except`[appName]`](#1-1-except--appname--) * [1-2. AI Debbugging Infomation
+Notification](#1-2-ai-debbugging-infomation-notification) * [1-3. Success`
+[appName]`](#1-3-success--appname--) * [1-4. Send`[appName]`](#1-4-send--
+appname--)   See more... - [Feature](#feature) * [2. Notifier](#2-notifier) +
+[2-1. *Telegram Notifier*](#2-1--telegram-notifier-) - [a. Without OpenAI API]
+(#a-without-openai-api) - [b. With OpenAI API](#b-with-openai-api) + [2-2.
+*Mail Notifier*](#2-2--mail-notifier-) + [2-3. *Discord Notifier*](#2-3--
+discord-notifier-) + [2-4. *Chime Notifier*](#2-4--chime-notifier-) + [2-5.
+*Slack Notifier*](#2-5--slack-notifier-) + [2-6. *Line Notifier*](#2-6--line-
+notifier-) + [2-7. *SMS Notifier*](#2-7--sms-notifier-) + [2-8. *Teams
+Notifier*](#2-8--teams-notifier-) + [2-9. *Kakaotalk Notifier*](#2-9--
+kakaotalk-notifier-) + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-) + [2-
+11. *Beep Notifier*](#2-11--beep-notifier-) + [2-12. *Desktop Notifier*](#2-12-
+-desktop-notifier-) * [3. Sender](#3-sender) - [License](#license) - [Code of
+Conduct](#code-of-conduct)
+
+# Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
 www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
 www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
 Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
 from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
-[OPEN AI API](https://platform.openai.com/docs/introduction)
-
-# Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
-conda install ExceptNotifier conda install exceptnotifier ```
+[Opea AI API](https://openai.com/blog/openai-api)
+# Quick Start ```bash $ pip install ExceptNotifier #pip install exceptnotifier
+```
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - If you are using Telegram, an example is attached as an
 image. - As you already know, API Keys or security tokens must be secured. Note
 that the key values which exposured in github will be expired after insecured.
 | App | Required Variables | Free or Paid | Ease of Setup | Time Required for
 Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |Beep|N/A|Free|N/A|0
@@ -123,20 +129,20 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# Feature ## Notifier You can receive debugging information from ChatGPT via
-OpenAI's API when using the Except statement. The syntax remains the same, but
-you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
-### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
-BotFather. (A built-in Telegram bot that helps users create custom Telegram
-bots)
+# Features ## 2. Notifier You can receive debugging information from ChatGPT
+via OpenAI's API when using the Except statement. The syntax remains the same,
+but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ### 2-1. *Telegram Notifier* - a. Open your
+telegram app and search for BotFather. (A built-in Telegram bot that helps
+users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
 #### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
@@ -285,15 +291,15 @@
 ### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
-## Sender
+## 3. Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `exceptnotifier-0.1.8/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.1.9/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.1.8/LICENSE` & `exceptnotifier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptnotifier-0.1.8/PKG-INFO` & `exceptnotifier-0.1.9/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exceptnotifier
-Version: 0.1.8
+Version: 0.1.9
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -19,30 +19,29 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ExceptNotifier_logo.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/logo2.png)
 
-<h3 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h3>
+<h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
-<a href="https://anaconda.org/conda-forge/exceptnotifier/"><img alt="conda-forge" src="https://img.shields.io/conda/dn/conda-forge/exceptnotifier.svg?label=conda-forge"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main3.png)
+##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
-##### Provides a notification from the application shown in the captured screen.
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 <Br>
 
 #### Could you kindly add this badge to your repository?
@@ -50,15 +49,57 @@
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 
 <br><br>
 
-### Supporting Applications
+
+
+
+# Contents
+
+- [OPEN AI API](https://platform.openai.com/docs/introduction)
+- [Python Package: ExceptNotifier](#python-package--exceptnotifier)
+- [Supporting Applications](#supporting-applications)
+  * [AI Debugging using OpenAI API](#ai-debugging-using-openai-api)
+- [Quick Start](#quick-start)
+- [App Setup Overview](#app-setup-overview)
+- [1. Key Features](#1-key-features)
+  * [1-1. Except`[appName]`](#1-1-except--appname--)
+  * [1-2. AI Debbugging Infomation Notification](#1-2-ai-debbugging-infomation-notification)
+  * [1-3. Success`[appName]`](#1-3-success--appname--)
+  * [1-4. Send`[appName]`](#1-4-send--appname--)
+<details>
+<summary> See more...</summary>
+- [Feature](#feature)
+  * [2. Notifier](#2-notifier)
+    + [2-1. *Telegram Notifier*](#2-1--telegram-notifier-)
+      - [a. Without OpenAI API](#a-without-openai-api)
+      - [b. With OpenAI API](#b-with-openai-api)
+    + [2-2. *Mail Notifier*](#2-2--mail-notifier-)
+    + [2-3. *Discord Notifier*](#2-3--discord-notifier-)
+    + [2-4. *Chime Notifier*](#2-4--chime-notifier-)
+    + [2-5. *Slack Notifier*](#2-5--slack-notifier-)
+    + [2-6. *Line Notifier*](#2-6--line-notifier-)
+    + [2-7. *SMS Notifier*](#2-7--sms-notifier-)
+    + [2-8. *Teams Notifier*](#2-8--teams-notifier-)
+    + [2-9. *Kakaotalk Notifier*](#2-9--kakaotalk-notifier-)
+    + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-)
+    + [2-11. *Beep Notifier*](#2-11--beep-notifier-)
+    + [2-12. *Desktop Notifier*](#2-12--desktop-notifier-)
+  * [3. Sender](#3-sender)
+- [License](#license)
+- [Code of Conduct](#code-of-conduct)
+
+</details>
+
+<br><br>
+
+# Supporting Applications
 
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
@@ -69,26 +110,22 @@
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
 If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-- [OPEN AI API](https://platform.openai.com/docs/introduction)
+-  [Opea AI API](https://openai.com/blog/openai-api)
 
 
-<br><br>
+<br>
 
 # Quick Start
 ```bash
-pip install ExceptNotifier
-pip install exceptnotifier
-
-conda install ExceptNotifier
-conda install exceptnotifier
+$ pip install ExceptNotifier    #pip install exceptnotifier
 ```
 
 <br>
 
 
 # App Setup Overview
 
@@ -117,14 +154,16 @@
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](https://github.com/dsdanielpark/ExceptNotifier/blob/main/documents/APIOpenAI/GUIDE.md)|
 
 
 <br><br>
 
+
+
 # 1. Key Features
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 ## 1-1. Except`[appName]`
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
@@ -205,17 +244,18 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# Feature
 
-## Notifier
+# Features
+
+## 2. Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
 ### 2-1. *Telegram Notifier*
 
@@ -618,15 +658,15 @@
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
-## Sender
+## 3. Sender
 
 
 
 <Br><br><br>
 
 # License
 MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.8 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.9 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -11,49 +11,69 @@
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-ExceptNotifier_logo.png)
-  **** Integrates AI-assisted debugging notifications into Python try-except
-              statements for various messaging applications. ****
-              [PyPI] [Downloads] [conda-forge] [Code_style:_black]
+logo2.png)
+   ** Integrates AI-assisted debugging notifications into Python try-except
+               statements for various messaging applications. **
+                     [PyPI] [Downloads] [Code_style:_black]
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-main2.png) # Python Package: ExceptNotifier ##### Provides a notification from
-the application shown in the captured screen. The `ExceptNotifier` Python
+main3.png) ##### Provides a notification from the application shown in the
+captured screen. # Python Package: ExceptNotifier The `ExceptNotifier` Python
 package offers a flexible approach to receiving notifications by enhancing
 Python's try-except statement. This package enables you to receive alerts
 through various messaging applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process.
 #### Could you kindly add this badge to your repository? ``` ![Except-Notifier]
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
-### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
+# Contents - [OPEN AI API](https://platform.openai.com/docs/introduction) -
+[Python Package: ExceptNotifier](#python-package--exceptnotifier) - [Supporting
+Applications](#supporting-applications) * [AI Debugging using OpenAI API](#ai-
+debugging-using-openai-api) - [Quick Start](#quick-start) - [App Setup
+Overview](#app-setup-overview) - [1. Key Features](#1-key-features) * [1-1.
+Except`[appName]`](#1-1-except--appname--) * [1-2. AI Debbugging Infomation
+Notification](#1-2-ai-debbugging-infomation-notification) * [1-3. Success`
+[appName]`](#1-3-success--appname--) * [1-4. Send`[appName]`](#1-4-send--
+appname--)   See more... - [Feature](#feature) * [2. Notifier](#2-notifier) +
+[2-1. *Telegram Notifier*](#2-1--telegram-notifier-) - [a. Without OpenAI API]
+(#a-without-openai-api) - [b. With OpenAI API](#b-with-openai-api) + [2-2.
+*Mail Notifier*](#2-2--mail-notifier-) + [2-3. *Discord Notifier*](#2-3--
+discord-notifier-) + [2-4. *Chime Notifier*](#2-4--chime-notifier-) + [2-5.
+*Slack Notifier*](#2-5--slack-notifier-) + [2-6. *Line Notifier*](#2-6--line-
+notifier-) + [2-7. *SMS Notifier*](#2-7--sms-notifier-) + [2-8. *Teams
+Notifier*](#2-8--teams-notifier-) + [2-9. *Kakaotalk Notifier*](#2-9--
+kakaotalk-notifier-) + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-) + [2-
+11. *Beep Notifier*](#2-11--beep-notifier-) + [2-12. *Desktop Notifier*](#2-12-
+-desktop-notifier-) * [3. Sender](#3-sender) - [License](#license) - [Code of
+Conduct](#code-of-conduct)
+
+# Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
 www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
 www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
 Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
 from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
-[OPEN AI API](https://platform.openai.com/docs/introduction)
-
-# Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
-conda install ExceptNotifier conda install exceptnotifier ```
+[Opea AI API](https://openai.com/blog/openai-api)
+# Quick Start ```bash $ pip install ExceptNotifier #pip install exceptnotifier
+```
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - If you are using Telegram, an example is attached as an
 image. - As you already know, API Keys or security tokens must be secured. Note
 that the key values which exposured in github will be expired after insecured.
 | App | Required Variables | Free or Paid | Ease of Setup | Time Required for
 Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |Beep|N/A|Free|N/A|0
@@ -123,20 +143,20 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# Feature ## Notifier You can receive debugging information from ChatGPT via
-OpenAI's API when using the Except statement. The syntax remains the same, but
-you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
-### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
-BotFather. (A built-in Telegram bot that helps users create custom Telegram
-bots)
+# Features ## 2. Notifier You can receive debugging information from ChatGPT
+via OpenAI's API when using the Except statement. The syntax remains the same,
+but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ### 2-1. *Telegram Notifier* - a. Open your
+telegram app and search for BotFather. (A built-in Telegram bot that helps
+users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
 #### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
@@ -285,15 +305,15 @@
 ### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
-## Sender
+## 3. Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `exceptnotifier-0.1.8/README.md` & `exceptnotifier-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,47 @@
+Metadata-Version: 2.1
+Name: exceptnotifier
+Version: 0.1.9
+Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
+Home-page: https://github.com/dsdanielpark/ExceptNotifier
+Author: daniel park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ExceptNotifier_logo.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/logo2.png)
 
-<h3 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h3>
+<h5 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h5>
 
 <p align="center">
 <a href="(https://img.shields.io/badge/pypi-ExceptNotifier-orange"></a>
 <a href="https://pypi.org/project/exceptnotifier/"><img alt="PyPI" src="https://img.shields.io/pypi/v/exceptnotifier"></a>
 <a href="https://pepy.tech/project/exceptnotifier"><img alt="Downloads" src="https://pepy.tech/badge/exceptnotifier"></a>
-<a href="https://anaconda.org/conda-forge/exceptnotifier/"><img alt="conda-forge" src="https://img.shields.io/conda/dn/conda-forge/exceptnotifier.svg?label=conda-forge"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
-![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
+![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main3.png)
+##### Provides a notification from the application shown in the captured screen.
 
 # Python Package: ExceptNotifier
-##### Provides a notification from the application shown in the captured screen.
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
 
 <Br>
 
 #### Could you kindly add this badge to your repository?
@@ -28,15 +49,57 @@
 ```
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ```
 
 
 <br><br>
 
-### Supporting Applications
+
+
+
+# Contents
+
+- [OPEN AI API](https://platform.openai.com/docs/introduction)
+- [Python Package: ExceptNotifier](#python-package--exceptnotifier)
+- [Supporting Applications](#supporting-applications)
+  * [AI Debugging using OpenAI API](#ai-debugging-using-openai-api)
+- [Quick Start](#quick-start)
+- [App Setup Overview](#app-setup-overview)
+- [1. Key Features](#1-key-features)
+  * [1-1. Except`[appName]`](#1-1-except--appname--)
+  * [1-2. AI Debbugging Infomation Notification](#1-2-ai-debbugging-infomation-notification)
+  * [1-3. Success`[appName]`](#1-3-success--appname--)
+  * [1-4. Send`[appName]`](#1-4-send--appname--)
+<details>
+<summary> See more...</summary>
+- [Feature](#feature)
+  * [2. Notifier](#2-notifier)
+    + [2-1. *Telegram Notifier*](#2-1--telegram-notifier-)
+      - [a. Without OpenAI API](#a-without-openai-api)
+      - [b. With OpenAI API](#b-with-openai-api)
+    + [2-2. *Mail Notifier*](#2-2--mail-notifier-)
+    + [2-3. *Discord Notifier*](#2-3--discord-notifier-)
+    + [2-4. *Chime Notifier*](#2-4--chime-notifier-)
+    + [2-5. *Slack Notifier*](#2-5--slack-notifier-)
+    + [2-6. *Line Notifier*](#2-6--line-notifier-)
+    + [2-7. *SMS Notifier*](#2-7--sms-notifier-)
+    + [2-8. *Teams Notifier*](#2-8--teams-notifier-)
+    + [2-9. *Kakaotalk Notifier*](#2-9--kakaotalk-notifier-)
+    + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-)
+    + [2-11. *Beep Notifier*](#2-11--beep-notifier-)
+    + [2-12. *Desktop Notifier*](#2-12--desktop-notifier-)
+  * [3. Sender](#3-sender)
+- [License](#license)
+- [Code of Conduct](#code-of-conduct)
+
+</details>
+
+<br><br>
+
+# Supporting Applications
 
 - [Telegram](https://telegram.org/)
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
@@ -47,26 +110,22 @@
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
 If you have OpenAI API Key and model name, you can get information and code examples for debugging in any application.
-- [OPEN AI API](https://platform.openai.com/docs/introduction)
+-  [Opea AI API](https://openai.com/blog/openai-api)
 
 
-<br><br>
+<br>
 
 # Quick Start
 ```bash
-pip install ExceptNotifier
-pip install exceptnotifier
-
-conda install ExceptNotifier
-conda install exceptnotifier
+$ pip install ExceptNotifier    #pip install exceptnotifier
 ```
 
 <br>
 
 
 # App Setup Overview
 
@@ -95,14 +154,16 @@
 | API | Required Variables | Free or Paid | Ease of Setup | Time Required for Setup|Guide Tutorial Link|
 |:--:|:--|:--:|:--:|:--:|:---:|
 | OpenAI API |`Required variables for each application`+ `_OPEN_AI_MODEL`,`_OPEN_AI_API`|Not free|Easy|2min|[APIOpenAI](https://github.com/dsdanielpark/ExceptNotifier/blob/main/documents/APIOpenAI/GUIDE.md)|
 
 
 <br><br>
 
+
+
 # 1. Key Features
 To use the desired application, you must define the necessary variables. Ensure that the variable names remain unchanged, and you can use either local or global variables. If you are using `Telegram`, an example is attached as an image.
 
 ## 1-1. Except`[appName]`
 If you use Python's try except statement as it is, but change except as follows, you can receive notifications through your application.
 ```
 ExceptChime, ExceptTelegram, ExceptDiscord, ExceptSMS, ExceptMail, ExceptKakao, ExceptLine, ExceptSlack, ExceptTeams, ExceptDesktope, ExceptBeep
@@ -183,17 +244,18 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# Feature
 
-## Notifier
+# Features
+
+## 2. Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
 ### 2-1. *Telegram Notifier*
 
@@ -596,15 +658,15 @@
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
 <br>
 
-## Sender
+## 3. Sender
 
 
 
 <Br><br><br>
 
 # License
 MIT
```

#### html2text {}

```diff
@@ -1,45 +1,79 @@
-Development Status :: 3 - Alpha
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.9 Summary: With
+Python's try-except to receive notifications about Errors or Successes in your
+code through messenger app or email. Home-page: https://github.com/
+dsdanielpark/ExceptNotifier Author: daniel park Author-email:
+parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
+Alarm,Error notifications,Customizable notifications,Traceback
+management,Single line alarm Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research Classifier: Natural Language
+:: English Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-ExceptNotifier_logo.png)
-  **** Integrates AI-assisted debugging notifications into Python try-except
-              statements for various messaging applications. ****
-              [PyPI] [Downloads] [conda-forge] [Code_style:_black]
+logo2.png)
+   ** Integrates AI-assisted debugging notifications into Python try-except
+               statements for various messaging applications. **
+                     [PyPI] [Downloads] [Code_style:_black]
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-main2.png) # Python Package: ExceptNotifier ##### Provides a notification from
-the application shown in the captured screen. The `ExceptNotifier` Python
+main3.png) ##### Provides a notification from the application shown in the
+captured screen. # Python Package: ExceptNotifier The `ExceptNotifier` Python
 package offers a flexible approach to receiving notifications by enhancing
 Python's try-except statement. This package enables you to receive alerts
 through various messaging applications or emails.
 
 With `ExceptNotifier`, you can obtain detailed compilation errors, including
 debug information, sent directly to your preferred messaging platform or email.
 By integrating OpenAI's ChatGPT, you can receive additional error code
 information as long as you provide the required API model name and key. This
 feature ensures that error handling and notifications are more informative and
 accessible, streamlining your debugging process.
 #### Could you kindly add this badge to your repository? ``` ![Except-Notifier]
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
-### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
+# Contents - [OPEN AI API](https://platform.openai.com/docs/introduction) -
+[Python Package: ExceptNotifier](#python-package--exceptnotifier) - [Supporting
+Applications](#supporting-applications) * [AI Debugging using OpenAI API](#ai-
+debugging-using-openai-api) - [Quick Start](#quick-start) - [App Setup
+Overview](#app-setup-overview) - [1. Key Features](#1-key-features) * [1-1.
+Except`[appName]`](#1-1-except--appname--) * [1-2. AI Debbugging Infomation
+Notification](#1-2-ai-debbugging-infomation-notification) * [1-3. Success`
+[appName]`](#1-3-success--appname--) * [1-4. Send`[appName]`](#1-4-send--
+appname--)   See more... - [Feature](#feature) * [2. Notifier](#2-notifier) +
+[2-1. *Telegram Notifier*](#2-1--telegram-notifier-) - [a. Without OpenAI API]
+(#a-without-openai-api) - [b. With OpenAI API](#b-with-openai-api) + [2-2.
+*Mail Notifier*](#2-2--mail-notifier-) + [2-3. *Discord Notifier*](#2-3--
+discord-notifier-) + [2-4. *Chime Notifier*](#2-4--chime-notifier-) + [2-5.
+*Slack Notifier*](#2-5--slack-notifier-) + [2-6. *Line Notifier*](#2-6--line-
+notifier-) + [2-7. *SMS Notifier*](#2-7--sms-notifier-) + [2-8. *Teams
+Notifier*](#2-8--teams-notifier-) + [2-9. *Kakaotalk Notifier*](#2-9--
+kakaotalk-notifier-) + [2-10. *Wechat Notifier*](#2-10--wechat-notifier-) + [2-
+11. *Beep Notifier*](#2-11--beep-notifier-) + [2-12. *Desktop Notifier*](#2-12-
+-desktop-notifier-) * [3. Sender](#3-sender) - [License](#license) - [Code of
+Conduct](#code-of-conduct)
+
+# Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
 www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
 www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
 Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
 from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
-[OPEN AI API](https://platform.openai.com/docs/introduction)
-
-# Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
-conda install ExceptNotifier conda install exceptnotifier ```
+[Opea AI API](https://openai.com/blog/openai-api)
+# Quick Start ```bash $ pip install ExceptNotifier #pip install exceptnotifier
+```
 # App Setup Overview - The variables in the following table must not be
 contaminated. - Depending on the situation, consider designating them as global
 variables for use. - If you are using Telegram, an example is attached as an
 image. - As you already know, API Keys or security tokens must be secured. Note
 that the key values which exposured in github will be expired after insecured.
 | App | Required Variables | Free or Paid | Ease of Setup | Time Required for
 Setup|Guide Tutorial Link| |:--:|:--|:--:|:--:|:--:|:---:| |Beep|N/A|Free|N/A|0
@@ -109,20 +143,20 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# Feature ## Notifier You can receive debugging information from ChatGPT via
-OpenAI's API when using the Except statement. The syntax remains the same, but
-you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
-### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
-BotFather. (A built-in Telegram bot that helps users create custom Telegram
-bots)
+# Features ## 2. Notifier You can receive debugging information from ChatGPT
+via OpenAI's API when using the Except statement. The syntax remains the same,
+but you'll need to configure these two variables:
+`_OPEN_AI_MODEL`,`_OPEN_AI_API` ### 2-1. *Telegram Notifier* - a. Open your
+telegram app and search for BotFather. (A built-in Telegram bot that helps
+users create custom Telegram bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
 #### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
@@ -271,15 +305,15 @@
 ### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
-## Sender
+## 3. Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `exceptnotifier-0.1.8/setup.py` & `exceptnotifier-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,42 @@
     if not match:
         raise RuntimeError("{} doesn't contain __version__".format(filename))
     version = match.groups()[0]
     return version
 
 
 def get_long_description():
-    with open("README.md", encoding='UTF-8') as f:
+    with open("README.md", encoding="UTF-8") as f:
         long_description = f.read()
         return long_description
 
 
 version = get_version()
 
 
 setup(
     name="exceptnotifier",
-    version="0.1.8",
+    version="0.1.9",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=['twilio', 'plyer', 'openai', 'discord'],
+    install_requires=["twilio", "plyer", "openai", "discord"],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     entry_points={"console_scripts": ["ExceptNotifier=ExceptNotifier.cli:main"]},
-)
+)
```

