# Comparing `tmp/python-bale-bot-2.4.4.tar.gz` & `tmp/python-bale-bot-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bale-bot-2.4.4.tar", last modified: Thu Mar 23 20:54:47 2023, max compression
+gzip compressed data, was "python-bale-bot-2.4.5.tar", last modified: Fri Apr 21 07:00:33 2023, max compression
```

## Comparing `python-bale-bot-2.4.4.tar` & `python-bale-bot-2.4.5.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:47.193373 python-bale-bot-2.4.4/
--rw-rw-rw-   0        0        0     1091 2023-03-02 20:35:49.000000 python-bale-bot-2.4.4/LICENSE
--rw-rw-rw-   0        0        0     3052 2023-03-23 20:54:47.191437 python-bale-bot-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-03-21 11:29:38.000000 python-bale-bot-2.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:46.918434 python-bale-bot-2.4.4/bale/
--rw-rw-rw-   0        0        0     2782 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/__init__.py
--rw-rw-rw-   0        0        0      243 2022-10-25 17:23:48.000000 python-bale-bot-2.4.4/bale/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:47.025419 python-bale-bot-2.4.4/bale/attachments/
--rw-rw-rw-   0        0        0      240 2022-10-25 17:23:48.000000 python-bale-bot-2.4.4/bale/attachments/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/attachments/audio.py
--rw-rw-rw-   0        0        0     2060 2023-03-21 09:03:50.000000 python-bale-bot-2.4.4/bale/attachments/contact.py
--rw-rw-rw-   0        0        0     3366 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/attachments/document.py
--rw-rw-rw-   0        0        0     1987 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/attachments/location.py
--rw-rw-rw-   0        0        0     1995 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/attachments/photo.py
--rw-rw-rw-   0        0        0    32092 2023-03-21 11:19:04.000000 python-bale-bot-2.4.4/bale/bot.py
--rw-rw-rw-   0        0        0     3069 2023-03-02 20:35:49.000000 python-bale-bot-2.4.4/bale/callbackquery.py
--rw-rw-rw-   0        0        0    15583 2023-03-21 09:24:15.000000 python-bale-bot-2.4.4/bale/chat.py
--rw-rw-rw-   0        0        0     3128 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/chatmember.py
--rw-rw-rw-   0        0        0     6808 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/components.py
--rw-rw-rw-   0        0        0     3740 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/error.py
--rw-rw-rw-   0        0        0    15639 2023-03-21 09:04:39.000000 python-bale-bot-2.4.4/bale/message.py
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:47.081419 python-bale-bot-2.4.4/bale/payments/
--rw-rw-rw-   0        0        0      103 2022-10-25 17:23:48.000000 python-bale-bot-2.4.4/bale/payments/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/payments/invoice.py
--rw-rw-rw-   0        0        0     1733 2023-03-16 10:29:33.000000 python-bale-bot-2.4.4/bale/payments/price.py
--rw-rw-rw-   0        0        0     4402 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/permissions.py
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:47.144377 python-bale-bot-2.4.4/bale/request/
--rw-rw-rw-   0        0        0      201 2022-11-04 11:43:50.000000 python-bale-bot-2.4.4/bale/request/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-03-21 08:58:18.000000 python-bale-bot-2.4.4/bale/request/http.py
--rw-rw-rw-   0        0        0     1433 2022-12-20 11:44:01.000000 python-bale-bot-2.4.4/bale/request/parser.py
--rw-rw-rw-   0        0        0      123 2023-03-16 10:05:55.000000 python-bale-bot-2.4.4/bale/request/utils.py
--rw-rw-rw-   0        0        0     5610 2023-03-02 20:35:50.000000 python-bale-bot-2.4.4/bale/update.py
--rw-rw-rw-   0        0        0     4598 2023-03-23 10:31:08.000000 python-bale-bot-2.4.4/bale/updater.py
--rw-rw-rw-   0        0        0     9985 2023-03-21 09:24:14.000000 python-bale-bot-2.4.4/bale/user.py
--rw-rw-rw-   0        0        0      145 2023-03-23 10:08:50.000000 python-bale-bot-2.4.4/bale/version.py
-drwxrwxrwx   0        0        0        0 2023-03-23 20:54:47.188410 python-bale-bot-2.4.4/python_bale_bot.egg-info/
--rw-rw-rw-   0        0        0     3052 2023-03-23 20:54:45.000000 python-bale-bot-2.4.4/python_bale_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      781 2023-03-23 20:54:45.000000 python-bale-bot-2.4.4/python_bale_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 20:54:45.000000 python-bale-bot-2.4.4/python_bale_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-03-23 20:54:45.000000 python-bale-bot-2.4.4/python_bale_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-23 20:54:45.000000 python-bale-bot-2.4.4/python_bale_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 20:54:47.193373 python-bale-bot-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-03-23 10:08:50.000000 python-bale-bot-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.569614 python-bale-bot-2.4.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/LICENSE
+-rw-rw-rw-   0        0        0     3052 2023-04-21 07:00:33.566612 python-bale-bot-2.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.483621 python-bale-bot-2.4.5/bale/
+-rw-rw-rw-   0        0        0     1983 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.505619 python-bale-bot-2.4.5/bale/attachments/
+-rw-rw-rw-   0        0        0      179 2023-04-11 12:58:39.000000 python-bale-bot-2.4.5/bale/attachments/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/audio.py
+-rw-rw-rw-   0        0        0     1973 2023-04-11 13:00:45.000000 python-bale-bot-2.4.5/bale/attachments/contact.py
+-rw-rw-rw-   0        0        0     3366 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/document.py
+-rw-rw-rw-   0        0        0     1991 2023-04-11 13:00:45.000000 python-bale-bot-2.4.5/bale/attachments/location.py
+-rw-rw-rw-   0        0        0     1995 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/photo.py
+-rw-rw-rw-   0        0        0     2382 2023-04-11 12:52:46.000000 python-bale-bot-2.4.5/bale/attachments/video.py
+-rw-rw-rw-   0        0        0    40598 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/bot.py
+-rw-rw-rw-   0        0        0     3777 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/callbackquery.py
+-rw-rw-rw-   0        0        0    10832 2023-04-18 18:41:38.000000 python-bale-bot-2.4.5/bale/chat.py
+-rw-rw-rw-   0        0        0     3934 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/chatmember.py
+-rw-rw-rw-   0        0        0     7595 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/components.py
+-rw-rw-rw-   0        0        0     3740 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/error.py
+-rw-rw-rw-   0        0        0    14455 2023-04-13 11:01:04.000000 python-bale-bot-2.4.5/bale/message.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.514618 python-bale-bot-2.4.5/bale/payments/
+-rw-rw-rw-   0        0        0       56 2023-04-11 12:58:40.000000 python-bale-bot-2.4.5/bale/payments/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/payments/invoice.py
+-rw-rw-rw-   0        0        0     1733 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/payments/price.py
+-rw-rw-rw-   0        0        0     4402 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/permissions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.523617 python-bale-bot-2.4.5/bale/request/
+-rw-rw-rw-   0        0        0      201 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/request/__init__.py
+-rw-rw-rw-   0        0        0    12113 2023-04-11 12:44:43.000000 python-bale-bot-2.4.5/bale/request/http.py
+-rw-rw-rw-   0        0        0     1371 2023-04-11 12:44:43.000000 python-bale-bot-2.4.5/bale/request/parser.py
+-rw-rw-rw-   0        0        0      123 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/request/utils.py
+-rw-rw-rw-   0        0        0     6631 2023-04-11 17:56:28.000000 python-bale-bot-2.4.5/bale/update.py
+-rw-rw-rw-   0        0        0     5285 2023-04-13 11:33:59.000000 python-bale-bot-2.4.5/bale/updater.py
+-rw-rw-rw-   0        0        0     6176 2023-04-13 11:29:15.000000 python-bale-bot-2.4.5/bale/user.py
+-rw-rw-rw-   0        0        0      145 2023-04-21 06:51:10.000000 python-bale-bot-2.4.5/bale/version.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.564611 python-bale-bot-2.4.5/python_bale_bot.egg-info/
+-rw-rw-rw-   0        0        0     3052 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:00:33.569614 python-bale-bot-2.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2023-04-21 06:51:10.000000 python-bale-bot-2.4.5/setup.py
```

### Comparing `python-bale-bot-2.4.4/LICENSE` & `python-bale-bot-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/PKG-INFO` & `python-bale-bot-2.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.4
+Version: 2.4.5
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
 License: MIT License
-Project-URL: Documentation, https://python-bale-bot.rtfd.io/en/master/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
 Project-URL: Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.4 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.5 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
 bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
-Documentation, https://python-bale-bot.rtfd.io/en/master/ Project-URL:
+Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
 Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html Project-
 URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
 LICENSE # python-bale-bot
                            [python-bale-bot image]
```

### Comparing `python-bale-bot-2.4.4/README.md` & `python-bale-bot-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/attachments/audio.py` & `python-bale-bot-2.4.5/bale/attachments/audio.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/attachments/contact.py` & `python-bale-bot-2.4.5/bale/attachments/contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from bale import Bot, User
 
 
 class ContactMessage:
     """This object shows a Message Contact.
 
     Attributes
     ----------
```

### Comparing `python-bale-bot-2.4.4/bale/attachments/document.py` & `python-bale-bot-2.4.5/bale/attachments/document.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/attachments/location.py` & `python-bale-bot-2.4.5/bale/attachments/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
+
 class Location:
     """This object shows an end
 
     Attributes
     ----------
         longitude: int
             Location longitude
```

### Comparing `python-bale-bot-2.4.4/bale/attachments/photo.py` & `python-bale-bot-2.4.5/bale/attachments/photo.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/bot.py` & `python-bale-bot-2.4.5/bale/bot.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 """
 from __future__ import annotations
 import asyncio
 from typing import Callable, Dict, Tuple, List, Optional
 from builtins import enumerate, reversed
 from .error import NotFound, InvalidToken
 from bale import (Message, Update, User, Components, RemoveComponents, Chat, Price, ChatMember, HTTPClient, Updater,
-                  Photo, Document, Location, ContactMessage)
-
+                  Photo, Document, Location, ContactMessage, Video)
 
 __all__ = (
     "Bot"
 )
 
 
 class _Loop:
@@ -40,26 +39,25 @@
 
     def __getattr__(self, key):
         raise AttributeError((
             'loop attribute cannot be accessed in non-async contexts. '
             'Consider using either an asynchronous main function and passing it to asyncio.run or '
             'using asynchronous initialisation hooks such as Bot.setup_hook'
         ))
-    
 
 _loop = _Loop()
 
+
 class Bot:
     """This object represents a Bale Bot.
 
     Parameters
     ----------
         token: str 
             Bot Token
-
         updater: Optional[:class:`bale.Updater`]
         base_url: Optional[:class:`str`]
 
     .. note::
         When you create bot and run for first-step, use :meth:`bale.Bot.delete_webhook` method in `on_ready` event.
     """
     __slots__ = (
@@ -97,48 +95,48 @@
             raise TypeError(f"{function.__name__} is not a Coroutine Function")
 
         if not self.events.get(event):
             self.events[event] = list()
 
         self.events[event].append(function)
 
-    def remove_event(self, event: str, function = None):
+    def remove_event(self, event: str, function=None):
         """Register an Event with event name"""
         result = self.events.get(event)
         if not result:
             raise TypeError(f"{event} not in Events")
 
         if not function:
             del self.events[event]
             return
 
         if not function in result:
             raise TypeError(f"{function.__name__} not in Event Functions")
 
         del self.events[event][function]
 
-    def wait_for(self, event_name: str, *, check = None, timeout = None):
+    def wait_for(self, event_name: str, *, check=None, timeout=None):
         """Wait for an event"""
         self.loop: asyncio.AbstractEventLoop
         future = self.loop.create_future()
         event_name = event_name.lower()
         if not check:
             check = lambda *args: True
 
         listeners = self.listeners.get(event_name)
         if not listeners:
             listeners = []
             self.listeners[event_name] = listeners
 
         listeners.append((future, check))
-        return asyncio.wait_for(future, timeout = timeout)
+        return asyncio.wait_for(future, timeout=timeout)
 
     @property
-    def user(self) -> "User" or None:
-        """Represents the connected client. ``None`` if not logged in"""
+    def user(self) -> Optional["User"]:
+        """Optional[:class:`bale.User`]: Represents the connected client. ``None`` if not logged in"""
         return self._user
 
     async def setup_hook(self):
         loop = asyncio.get_running_loop()
         self.loop = loop
         self.http.loop = loop
         await self.http.start()
@@ -165,15 +163,15 @@
             await core(*args, **kwargs)
         except Exception as ext:
             await self.on_error(event_name, ext)
 
     def call_to_run_event(self, core, event_name, *args, **kwargs):
         task = self.run_event(core, event_name, *args, **kwargs)
         self.loop: asyncio.AbstractEventLoop
-        return self.loop.create_task(task, name = event_name)
+        return self.loop.create_task(task, name=event_name)
 
     def dispatch(self, event_name, /, *args, **kwargs):
         method = "on_" + event_name
         listeners = self.listeners.get(event_name)
         if listeners:
             removed = []
             for index, (future, check) in enumerate(listeners):
@@ -206,36 +204,31 @@
             for event_core in events_core:
                 self.call_to_run_event(event_core, method, *args, **kwargs)
 
     async def on_error(self, event_name, error):
         """a Event for get errors when exceptions"""
         print("error", event_name, error)
 
-
     async def get_bot(self) -> User:
-        """
-        |core|
-        Get bot information
+        """Get bot information
 
         Returns
         -------
             :class:`Bale.User` :
                 Bot User information.
         Raises
         ------
             APIError
                 Get bot Failed.
         """
         response = await self.http.get_bot()
         return User.from_dict(data=response.result, bot=self)
 
     async def delete_webhook(self) -> bool:
-        """
-        |core|
-        This service is used to remove the webhook set for the bot.
+        """This service is used to remove the webhook set for the bot.
 
         Returns
         -------
             bool:
                 ``True`` else ``False`` if not done
         Raises
         ------
@@ -243,82 +236,120 @@
                 You do not have permission to delete Webhook.
             APIError
                 Delete webhook Failed.
         """
         response = await self.http.delete_webhook()
         return response.result or False
 
-    async def send_message(self, chat: "Chat" | "User", text: str, *, components: Optional["Components" | "RemoveComponents"] = None,
-                    reply_to_message: Optional["Message"] = None) -> "Message":
-        """
-        |core|
-        This service is used to send text messages.
+    async def send_message(self, chat_id: str | int, text: str, *,
+                           components: Optional["Components" | "RemoveComponents"] = None,
+                           reply_to_message_id: Optional[str | int] = None) -> "Message":
+        """This service is used to send text messages.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat` | :class:`bale.User`
-                Chat
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             text: :class:`str`
-                Message Text
+                Text of the message to be sent. Max 4096 characters after entities parsing.
             components: Optional[:class:`bale.Components` | :class:`bale.RemoveComponents`]
                 Message Components
-            reply_to_message: Optional[:class:`bale.Message`]
-                Reply to a Message
+            reply_to_message_id: Optional[:class:`str` | :class:`int`]
+                Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
         Returns
         -------
             :class:`bale.Message`
                 The Message
         Raises
         ------
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to send Message to this chat.
             APIError
                 Send Message Failed.   
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of str or int"
             )
 
         if components:
             if not isinstance(components, (Components, RemoveComponents)):
                 raise TypeError(
                     "components param must be type of Components or RemoveComponents"
                 )
             components = components.to_dict()
 
+        if reply_to_message_id and not isinstance(reply_to_message_id, (int, str)):
+            raise TypeError(
+                "reply_to_message_id param must be type of Message"
+            )
 
-        if reply_to_message:
-            if not isinstance(reply_to_message, Message):
-                raise TypeError(
-                    "reply_to_message param must be type of Message"
-                )
-            reply_to_message = reply_to_message.message_id
-
-        response = await self.http.send_message(str(chat.chat_id), text, components=components, reply_to_message_id=reply_to_message)
+        response = await self.http.send_message(str(chat_id), text, components=components,
+                                                reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_document(self, chat: "Chat" | "User", document: bytes | str | "Document", *, caption: Optional[str] = None,
-                    reply_to_message: Optional["Message"] = None) -> "Message":
+    async def forward_message(self, chat_id: int | str, from_chat_id: int | str, message_id: int | str):
+        """This service is used to send text messages.
+
+        Parameters
+        ----------
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            from_chat_id: :class:`str` | :class:`int`
+                the chat where the original message was sent (or channel username in the format @channelusername).
+            message_id: :class:`int` | :class:`str`
+                Message in the chat specified in :param:`from_chat_id`.
+        Returns
+        -------
+            :class:`bale.Message`
+                The Message
+        Raises
+        ------
+            NotFound
+                Invalid Chat ID.
+            Forbidden
+                You do not have permission to send Message to this chat.
+            APIError
+                Forward Message Failed.
         """
-        |core|
-        This service is used to send document.
+        if not isinstance(chat_id, (str, int)):
+            raise TypeError(
+                "chat_id param must be type of str or int"
+            )
+
+        if not isinstance(from_chat_id, (Chat, User)):
+            raise TypeError(
+                "from_chat_id param must be type of str or int"
+            )
+
+        if not isinstance(message_id, Message):
+            raise TypeError(
+                "message_id param must be type of str or int"
+            )
+
+        response = await self.http.forward_message(str(chat_id), str(from_chat_id), str(message_id))
+        return Message.from_dict(data=response.result, bot=self)
+
+    async def send_document(self, chat_id: str | int, document: bytes | str | "Document", *,
+                            caption: Optional[str] = None,
+                            reply_to_message_id: Optional[str | int] = None) -> "Message":
+        """This service is used to send document.
 
         Parameters
         ----------
-        chat: :class:`bale.Chat` | :class:`bale.User`
-            Chat
+        chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         document: :class:`bytes` | :class:`str` | :class:`bale.Document`
-            Document
+            File to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
         caption: Optional[:class:`str`]
-            Message caption
-        reply_to_message: Optional[:class:`bale.Message`]
-            Reply to a Message
+            Document caption.
+        reply_to_message_id: Optional[:class:`str` | :class:`int`]
+                Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
                 
         Raises
@@ -326,53 +357,50 @@
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to send Document to this chat.
             APIError
                 Send Document Failed.        
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (Chat, User)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of Chat or User"
             )
 
         if not isinstance(document, (bytes, str, Document)):
             raise TypeError(
                 "document param must be type of bytes, str or Document"
             )
 
-        if reply_to_message:
-            if not isinstance(reply_to_message, Message):
-                raise TypeError(
-                    "reply_to_message param must be type of Message"
-                )
-            reply_to_message = reply_to_message.message_id
+        if reply_to_message_id and not isinstance(reply_to_message_id, Message):
+            raise TypeError(
+                "reply_to_message_id param must be type of Message"
+            )
 
         if isinstance(document, Document):
             document = document.file_id
 
-        response = await self.http.send_document(chat.chat_id, document, caption=caption, reply_to_message_id=reply_to_message)
+        response = await self.http.send_document(chat_id, document, caption=caption,
+                                                 reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_photo(self, chat: "Chat" | "User", photo: bytes | str | "Photo", *, caption: Optional[str] = None,
-                 reply_to_message: Optional["Message"] = None) -> "Message":
-        """
-        |core|
-        This service is used to send photo.
+    async def send_photo(self, chat_id: str | int, photo: bytes | str | "Photo", *, caption: Optional[str] = None,
+                         reply_to_message_id: Optional[str | int] = None) -> "Message":
+        """This service is used to send photo.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat` | :class:`bale.User`
-                Chat
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             photo: :class:`bytes` | :class:`str` | :class:`bale.Photo`
-                Photo
+                Photo to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
             caption: Optional[:class:`str`]
-                Message caption
-            reply_to_message: Optional[:class:`bale.Message`]
-                Reply to a Message
+                Photo caption.
+            reply_to_message_id: Optional[:class:`str` | :class:`int`]
+                Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
 
         Raises
@@ -380,53 +408,106 @@
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to Send Photo to chat.
             APIError
                 Send photo Failed.
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of str or int"
             )
 
         if not isinstance(photo, (bytes, str, Photo)):
             raise TypeError(
                 "photo param must be type of bytes, str or Photo"
             )
 
         if isinstance(photo, Photo):
             photo = photo.file_id
 
-        if reply_to_message:
-            if not isinstance(reply_to_message, Message):
-                raise TypeError(
-                    "reply_to_message param must be type of Message"
-                )
-            reply_to_message = reply_to_message.message_id
+        if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
+            raise TypeError(
+                "reply_to_message_id param must be type of str or int"
+            )
 
         if caption and not isinstance(caption, str):
             raise TypeError(
                 "caption param must be type of str"
             )
 
-        response = await self.http.send_photo(str(chat.chat_id), photo, caption=caption, reply_to_message_id=reply_to_message)
+        response = await self.http.send_photo(str(chat_id), photo, caption=caption,
+                                              reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_location(self, chat: "Chat" | "User", location: "Location") -> "Message":
+    async def send_video(self, chat_id: str | int, video: bytes | str | "Photo", *, caption: Optional[str] = None,
+                         reply_to_message_id: Optional[str | int] = None) -> "Message":
+        """This service is used to send Video.
+
+        Parameters
+        ----------
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            video: :class:`bytes` | :class:`str` | :class:`bale.Photo`
+                Video to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
+            caption: Optional[:class:`str`]
+                Video caption.
+            reply_to_message_id: Optional[:class:`str` | :class:`int`]
+                Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
+
+        Returns
+        --------
+            :class:`bale.Message`
+                The Message.
+
+        Raises
+        ------
+            NotFound
+                Invalid Chat ID.
+            Forbidden
+                You do not have permission to Send Video to chat.
+            APIError
+                Send Video Failed.
         """
-        |core|
-        This service is used to send location.
+        if not isinstance(chat_id, (str, int)):
+            raise TypeError(
+                "chat_id param must be type of str or int"
+            )
+
+        if not isinstance(video, (bytes, str, Video)):
+            raise TypeError(
+                "video param must be type of bytes, str or Video"
+            )
+
+        if isinstance(video, Video):
+            video = video.file_id
+
+        if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
+            raise TypeError(
+                "reply_to_message_id param must be type of str or int"
+            )
+
+        if caption and not isinstance(caption, str):
+            raise TypeError(
+                "caption param must be type of str"
+            )
+
+        response = await self.http.send_video(str(chat_id), video, caption=caption,
+                                              reply_to_message_id=reply_to_message_id)
+        return Message.from_dict(data=response.result, bot=self)
+
+    async def send_location(self, chat_id: str | int, location: "Location") -> "Message":
+        """Use this method to send point on the map.
 
         Parameters
         ----------
-        chat: :class:`bale.Chat` | :class:`bale.User`
-            Chat
+        chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         location: :class:`bale.Location`
-            Location
+            The Location.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
 
         Raises
@@ -434,38 +515,36 @@
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to send Location to this chat.
             APIError
                 Send Location Failed.
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of str or int"
             )
 
         if not isinstance(location, Location):
             raise TypeError(
                 "location param must be type of Location"
             )
 
-        response = await self.http.send_location(str(chat.chat_id), location.latitude, location.longitude)
+        response = await self.http.send_location(str(chat_id), location.latitude, location.longitude)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_contact(self, chat: "Chat" | "User", contact: "ContactMessage") -> "Message":
-        """
-        |core|
-        This service is used to send contact.
+    async def send_contact(self, chat_id: str | int, contact: "ContactMessage") -> "Message":
+        """This service is used to send contact.
 
         Parameters
         ----------
-        chat: :class:`bale.Chat` | :class:`bale.User`
-            Chat
+        chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         contact: :class:`bale.ContactMessage`
-            Contact Message
+            The Contact.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
 
         Raises
@@ -473,75 +552,77 @@
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to send Contact Message to this chat.
             APIError
                 Send Contact Message Failed.
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat param must be type of str or int"
             )
 
         if not isinstance(contact, ContactMessage):
             raise TypeError(
                 "contact param must be type of ContactMessage"
             )
 
-        response = await self.http.send_contact(str(chat.chat_id), contact.phone_number, contact.first_name, last_name=contact.last_name)
+        response = await self.http.send_contact(str(chat_id), contact.phone_number, contact.first_name,
+                                                last_name=contact.last_name)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_invoice(self, chat: "Chat" | "User", title: str, description: str, provider_token: str, prices: List["Price"], *,
-                   photo_url: Optional[str] = None, need_name: Optional[bool] = False, need_phone_number: Optional[bool] = False,
-                   need_email: Optional[bool] = False, need_shipping_address: Optional[bool] = False, is_flexible: Optional[bool] = True) -> Message:
-        """
-        |core|
-        You can use this service to send money request messages.
+    async def send_invoice(self, chat_id: str | int, title: str, description: str, provider_token: str,
+                           prices: List["Price"], *,
+                           photo_url: Optional[str] = None, need_name: Optional[bool] = False,
+                           need_phone_number: Optional[bool] = False,
+                           need_email: Optional[bool] = False, need_shipping_address: Optional[bool] = False,
+                           is_flexible: Optional[bool] = True) -> Message:
+        """You can use this service to send money request messages.
 
         Parameters
         ----------
-        chat: :class:`bale.Chat` | :class:`bale.User`
-            Chat
+        chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         title: str
-            Invoice Title
+            Product name. 1- 32 characters.
         description: str
-            Invoice Description
+            Product description. 1- 255 characters.
         provider_token: str
             You can use 3 methods to receive money: 1.Card number 2. Port number and acceptor number 3. Wallet number "Bale"
         prices: List[:class:`bale.Price`]
             A list of prices.
-        photo_url: str
-            Photo URL of Invoice. Defaults to None.
-        need_name: bool
-            Get a name from "User"?. Defaults to False.
-        need_phone_number: bool
-            Get a Phone number from "User"?. Defaults to False.
-        need_email: bool
-            Get an Email from "User"?. Defaults to False.
-        need_shipping_address: bool
-            Get a Shipping Address from "User"?. Defaults to False.
-        is_flexible: bool
-            Is the Invoice Photo Flexible to the Payment button?. Defaults to True.
+        photo_url: Optional[:class:`str`]
+            URL of the product photo for the invoice. Can be a photo of the goods or a marketing image for a service. People like it better when they see what they are paying for.
+        need_name: Optional[bool]
+            Pass True, if you require the user’s full name to complete the order.
+        need_phone_number: Optional[bool]
+            Pass True, if you require the user’s phone number to complete the order.
+        need_email: Optional[bool]
+            Pass True, if you require the user’s email to complete the order.
+        need_shipping_address: Optional[bool]
+            Pass True, if you require the user’s shipping address to complete the order.
+        is_flexible: Optional[bool]
+            Pass True, if the final price depends on the shipping method.
 
         Returns
         -------
             :class:`bale.Message`
             
         Raises
         ------
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to send Invoice to this chat.
             APIError
                 Send Invoice Failed.  
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat param must be type of str or int"
             )
 
         if not isinstance(photo_url, str):
             raise TypeError(
                 "photo_url param must be type of str"
             )
 
@@ -567,110 +648,107 @@
 
         if not isinstance(is_flexible, bool):
             raise TypeError(
                 "is_flexible param must be type of boolean"
             )
 
         prices = [price.to_dict() for price in prices if isinstance(price, Price)]
-        response = await self.http.send_invoice(str(chat.chat_id), title, description, provider_token, prices, photo_url, need_name,
-                    need_phone_number, need_email, need_shipping_address, is_flexible)
+        response = await self.http.send_invoice(str(chat_id), title, description, provider_token, prices, photo_url,
+                                                need_name,
+                                                need_phone_number, need_email, need_shipping_address, is_flexible)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def edit_message(self, chat: "Chat" | "User", message: "Message", text: str, *, components: "Components" | "RemoveComponents"=None) -> None:
-        """
-        |core|
-        You can use this service to edit text messages that you have already sent through the arm.
+    async def edit_message(self, chat_id: str | int, message_id: str | int, text: str, *,
+                           components: Optional["Components" | "RemoveComponents"] = None) -> "Message":
+        """You can use this service to edit text messages that you have already sent through the arm.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat`
-                chat
-            message: :class:`bale.Message`
-                message
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            message_id: :class:`str` | :class:`int`
+                Unique identifier for the message to edit.
             text: str
-                new content for message.
+                New text of the message, 1- 4096 characters after entities parsing.
             components: Optional[:class:`bale.Components` | :class:`bale.RemoveComponents`]
-                message components
+                An object for an inline keyboard.
         Raises
         ------
             NotFound
                 Invalid Message or Chat ID.
             Forbidden
                 You do not have permission to Edit Message.
             APIError
                 Edit Message Failed.
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of str or int"
             )
 
-        if not isinstance(message, Message):
+        if not isinstance(message_id, (str, int)):
             raise TypeError(
-                "message_id param must be type of Message or str"
+                "message_id param must be type of str or int"
             )
 
         if components and not isinstance(components, (Components, RemoveComponents)):
             raise TypeError(
                 "components param must be type of Components or RemoveComponents"
             )
 
         if components:
             components = components.to_dict()
 
-        await self.http.edit_message(chat.chat_id, message.message_id, text, components=components)
+        response = await self.http.edit_message(chat_id, message_id, text, components=components)
+        return response.result
 
-    async def delete_message(self, chat: "Chat" | "User", message: "Message") -> bool:
-        """
-        |core|
-        You can use this service to delete a message that you have already sent through the arm.
+    async def delete_message(self, chat_id: str | int, message_id: str | int) -> bool:
+        """You can use this service to delete a message that you have already sent through the arm.
 
         .. warning::
             In Channel or Group:
                 If it is a group or channel Manager, it can delete a message from (group or channel).
 
             In private message (PV):
                 If the message was sent by a bot, it can be deleted with this method
 
         Parameters
         ----------
-            chat: :class:`bale.Chat`
-                chat
-            message: :class:`bale.Message`
-                message
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            message_id: :class:`bale.Message`
+                Unique identifier for the message to delete.
         Raises
         ------
             NotFound
                 Invalid Message or Chat ID.
             Forbidden
                 You do not have permission to Delete Message.
             APIError
                 Delete Message Failed.
         """
-        if not isinstance(chat, (Chat, User)):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat or User"
+                "chat_id param must be type of str or int"
             )
 
-        if not isinstance(message, Message):
+        if not isinstance(message_id, (str, int)):
             raise TypeError(
-                "message param must be type of str or Message"
+                "message_id param must be type of str or int"
             )
-        response = await self.http.delete_message(str(chat.chat_id), message.message_id)
+        response = await self.http.delete_message(str(chat_id), message_id)
         return response.result or False
 
     async def get_chat(self, chat_id: int | str) -> Chat | None:
-        """
-        |core|
-        This service can be used to receive personal information that has previously interacted with the arm.
+        """Use this method to get up-to-date information about the chat (current name of the user for one-on-one conversations, current username of a user, group or channel, etc.).
 
         Parameters
         ----------
             chat_id: int | str
-                chat id
+                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         Returns
         -------
             Optional[:class:`bale.Chat`]
                 The chat or ``None`` if not found.
         Raises
         ------
             Forbidden
@@ -687,17 +765,15 @@
             response = await self.http.get_chat(str(chat_id))
         except NotFound:
             return None
         else:
             return Chat.from_dict(response.result, bot=self)
 
     async def get_user(self, user_id: int | str) -> "User" | None:
-        """
-        |core|
-        This Method almost like :class:`bale.Bot.get_chat` , but this a filter that only get user.
+        """This Method almost like :class:`bale.Bot.get_chat` , but this a filter that only get user.
 
         Parameters
         ----------
             user_id: int
                 user id
         Returns
         -------
@@ -717,128 +793,99 @@
 
         chat = await self.get_chat(user_id)
         if chat and chat.type.is_private_chat():
             return User.from_dict(chat.to_dict(), self)
 
         return None
 
-    async def get_chat_member(self, chat: "Chat", user: "User" = None, user_id: str | int = None) -> "ChatMember" | None:
-        """
+    async def get_chat_member(self, chat_id: str | int, user_id: str | int) -> "ChatMember" | None:
+        """Use this method to get information about a member of a chat. The method is only guaranteed to work for other users if the bot is an administrator in the chat.
+
         Parameters
         ----------
-            chat: :class:`bale.Chat`
-                chat
-            user: Optional[:class:`bale.User`]
-                user
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             user_id: Optional[:class:`int` | :class:`str`]
-                user id
+                Unique identifier of the target user.
 
         Returns
         -------
-            Optional[:class:`bale.ChatMember`]:
-                The chat member or ``None`` if not found.
+            Optional[:class:`bale.ChatMember`]
+                The chat member of ``None`` if not found.
 
         Raises
         ------
             NotFound
                 Invalid Chat or User ID.
             Forbidden
                 You do not have permission to get Chat Member.
             APIError
                 Get chat member Failed.
         """
-        if not isinstance(chat, Chat):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
                 "chat param must be type of Chat"
             )
 
-        if user is None and user_id is None:
-            raise TypeError(
-                "you must enter user or user_id"
-            )
-
-        if user and user_id:
-            raise TypeError(
-                "You can't use user & user_id together"
-            )
-
-        if user and not isinstance(user, User):
-            raise TypeError(
-                "user must be type of bale.User"
-            )
-
-        if user_id and not isinstance(user_id, (str, int)):
+        if not isinstance(user_id, (str, int)):
             raise TypeError(
                 "user_id must be type of str or int"
             )
 
         try:
-            response = await self.http.get_chat_member(chat_id=str(chat.chat_id), member_id=user.user_id if user else str(user_id))
+            response = await self.http.get_chat_member(chat_id=str(chat_id), member_id=str(user_id))
         except NotFound:
             return None
         else:
-            return ChatMember.from_dict(response.result)
+            return ChatMember.from_dict(chat_id, response.result, self)
 
-    async def invite_to_chat(self, chat: "Chat", user: "User"):
-        """Invite user to the chat
+    async def ban_chat_member(self, chat_id: str | int, user_id: str | int) -> "ChatMember":
+        """Use this method to ban a user from a group, supergroup or a channel. In the case of supergroups and channels, the user will not be able to return to the group on their own using invite links, etc., unless unbanned first.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat`
-                chat
-            user: :class:`bale.User`
-                user
-        
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            user_id: :class:`int` | :class:`str`
+                Unique identifier of the target user.
+
+        Returns
+        -------
+            :class:`bool`
+                On success, ``True`` is returned.
+
         Raises
         ------
             NotFound
                 Invalid Chat or User ID.
             Forbidden
-                You do not have permission to Add user to Chat.
+                You do not have permission to ban Chat Member.
             APIError
-                Invite user Failed.
+                ban chat member Failed.
         """
-        if not isinstance(chat, Chat):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat"
+                "chat_id param must be type of str or int"
             )
 
-        if not isinstance(user, User):
+        if not isinstance(user_id, (str, int)):
             raise TypeError(
-                "user param must be type of User"
+                "user_id must be type of str or int"
             )
 
-        await self.http.invite_to_chat(str(chat.chat_id), str(user.user_id))
+        response = await self.http.ban_chat_member(chat_id=str(chat_id), member_id=str(user_id))
+        return response.result
 
-    async def leave_chat(self, chat: "Chat"):
-        """Leave bot from a Chat
+    async def get_chat_members_count(self, chat_id: str | int) -> int:
+        """Use this method to get the number of members in a chat.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat`
-                chat
-        
-        Raises
-        ------
-            Forbidden
-                You do not have permission to Leave from chat.
-            APIError
-                Leave from chat Failed.
-        """
-        if not isinstance(chat, Chat):
-            raise TypeError(
-                "chat param must be type of Chat"
-            )
-        await self.http.leave_chat(str(chat.chat_id))
-
-    async def get_chat_members_count(self, chat: "Chat") -> int | None:
-        """
-        Parameters
-        ----------
-            chat: :class:`bale.Chat` 
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
 
         Raises
         ------
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to get Members count of the Chat.
@@ -846,65 +893,61 @@
                 get Members count of the Chat Failed.
 
         Returns
         --------
             :class:`int`:
                 The members count of the chat
         """
-        if not isinstance(chat, Chat):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat"
+                "chat_id param must be type of str or int"
             )
 
-        response = await self.http.get_chat_members_count(str(chat.chat_id))
+        response = await self.http.get_chat_members_count(str(chat_id))
         return response.result
 
-    async def get_chat_administrators(self, chat: "Chat") -> list["ChatMember"] | None:
-        """
-        |core|
-        This service can be used to display admins of a group or channel.
+    async def get_chat_administrators(self, chat_id: str | int) -> list["ChatMember"] | None:
+        """Use this method to get a list of administrators in a chat.
 
         Parameters
         ----------
-            chat: :class:`bale.Chat` 
-                Group id
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         Returns
         -------
-            Optional[List[:class:`bale.ChatMember`]]:
-                list of chat member or ``None`` if chat not found.
+            List[:class:`bale.ChatMember`]
+                list of chat member.
         Raises
         ------
             NotFound
                 Invalid Chat ID.
             Forbidden
                 You do not have permission to get Administrators of the Chat.
             APIError
                 get Administrators of the Chat from chat Failed.
         """
-        if not isinstance(chat, Chat):
+        if not isinstance(chat_id, (str, int)):
             raise TypeError(
-                "chat param must be type of Chat"
+                "chat_id param must be type of str or int"
             )
 
-        response = await self.http.get_chat_administrators(chat.chat_id)
-        return [ChatMember.from_dict(data=member_payload) for member_payload in response.result or list()]
+        response = await self.http.get_chat_administrators(chat_id)
+        return [ChatMember.from_dict(chat_id=chat_id, data=member_payload, bot=self) for member_payload in response.result or list()]
 
-    async def download_file(self, file_id: str):
-        """
-        .. warning::
-            You must be entered `chat` or `chat_id`
+    async def get_file(self, file_id: str):
+        """Use this method to get basic info about a file and prepare it for downloading. For the moment, bots can download files of up to ``20`` MB in size.
 
         Parameters
         ----------
             file_id: :class:`str`
-                    file id
+                Either the file identifier to get file information about.
 
         Returns
         -------
-            Optional[:class:`bytes`]:
+            :class:`bytes`
                 The content of the file
 
         Raises
         ------
             NotFound
                 Invalid file ID.
             Forbidden
@@ -915,15 +958,69 @@
         if not isinstance(file_id, str):
             raise TypeError(
                 "file_id must be type of str"
             )
 
         return await self.http.get_file(file_id)
 
-    async def get_updates(self, offset: int = None, limit: int = None) -> list["Update"] | None:
+    async def invite_user(self, chat_id: str | int, user_id: str | int) -> bool:
+        """Invite user to the chat
+
+        Parameters
+        ----------
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            user_id: :class:`str` | :class:`int`
+                Unique identifier for the target user.
+
+        Raises
+        ------
+            NotFound
+                Invalid Chat or User ID.
+            Forbidden
+                You do not have permission to Add user to Chat.
+            APIError
+                Invite user Failed.
+        """
+        if not isinstance(chat_id, (str, int)):
+            raise TypeError(
+                "chat_id param must be type of str or int"
+            )
+
+        if not isinstance(user_id, (str, int)):
+            raise TypeError(
+                "user_id param must be type of str or int"
+            )
+
+        response = await self.http.invite_to_chat(str(chat_id), str(user_id))
+        return response.result or False
+
+    async def leave_chat(self, chat_id: str | int) -> bool:
+        """Use this method for your bot to leave a group, channel.
+
+        Parameters
+        ----------
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+
+        Raises
+        ------
+            Forbidden
+                You do not have permission to Leave from chat.
+            APIError
+                Leave from chat Failed.
+        """
+        if not isinstance(chat_id, (str, int)):
+            raise TypeError(
+                "chat_id param must be type of str or int"
+            )
+        response = await self.http.leave_chat(str(chat_id))
+        return response.result or False
+
+    async def get_updates(self, offset: int = None, limit: int = None) -> list["Update"]:
         if offset and not isinstance(offset, int):
             raise TypeError(
                 "offset param must be int"
             )
 
         if limit and not isinstance(limit, int):
             raise TypeError(
@@ -932,18 +1029,20 @@
 
         response = await self.http.get_updates(offset, limit)
         return [Update.from_dict(data=update_payload, bot=self) for update_payload in response.result or list()
                 if not offset or (offset and update_payload.get("update_id") > offset)]
 
     async def connect(self, sleep_after_every_get_updates):
         self._user = await self.get_bot()
-        await self.updater.start(sleep_after_every_get_updates = sleep_after_every_get_updates)
+        await self.updater.start(sleep_after_every_get_updates=sleep_after_every_get_updates)
 
-    def run(self, sleep_after_every_get_updates = None):
+    def run(self, sleep_after_every_get_updates=None):
         """Run bot and https"""
+
         async def main():
             async with self:
-                await self.connect(sleep_after_every_get_updates = sleep_after_every_get_updates)
+                await self.connect(sleep_after_every_get_updates=sleep_after_every_get_updates)
+
         try:
             asyncio.run(main())
-        except KeyboardInterrupt: # Control-C
+        except KeyboardInterrupt:  # Control-C
             pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-bale-bot-2.4.4/bale/chat.py` & `python-bale-bot-2.4.5/bale/message.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,432 +18,256 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, List
+
+from datetime import datetime
+from typing import TYPE_CHECKING, List, Optional
+
 if TYPE_CHECKING:
-    from bale import Bot, Message, User, Photo, Document, Components, RemoveComponents, Price, Location, ContactMessage
+    from bale import Bot
 
+from bale import (Chat, User, Document, ContactMessage, Location, Photo, Invoice, Components, RemoveComponents, Price,
+                  Video)
 
-__all__ = (
-    "Chat",
-    "ChatType"
-)
-
-class ChatType:
-    """This object indicates a Chat Type.
-
-    .. container:: operations
-        .. describe:: x == y
-            Checks if two chat type are equal.
-        .. describe:: x != y
-            Checks if two chat type are not equal.
-    """
-    PRIVATE = "private"
-    GROUP = "group"
 
+class Message:
+    """This object shows a message.
+
+    Attributes
+    ----------
+        message_id: str
+            Unique message identifier inside this chat.
+        from_user: Optional[:class:`bale.User`]
+            Sender of the message; empty for messages sent to channels. For backward compatibility, this will contain a fake sender user in non-channel chats, if the message was sent on behalf of a chat.
+        chat: :class:`bale.Chat`
+            Conversation the message belongs to.
+        date: :class:`datetime.datetime`
+            Date the message was sent in Unix time.
+        text: Optional[:class:`str`]
+            Message Content
+        caption: Optional[:class:`str`]
+            Caption for the animation, audio, document, photo, video or voice.
+        forward_from: Optional[:class:`bale.User`]
+            For forwarded messages, sender of the original message.
+        forward_from_chat: Optional[:class:`bale.Chat`]
+            For messages forwarded from channels or from anonymous administrators, information about the original sender chat.
+        reply_to_message: Optional[:class:`bale.Message`]
+            For replies, the original message. Note that the Message object in this field will not contain further reply_to_message fields even if it itself is a reply.
+        contact: Optional[:class:`bale.ContactMessage`]
+            Message is a shared contact, information about the contact.
+        location: Optional[:class:`bale.Location`]
+            Message is a shared location, information about the location.
+        document: Optional[:class:`bale.Document`]
+            Message is a general file, information about the file.
+        new_chat_members: Optional[List[:class:`bale.User`]]
+            New members that were added to the group or supergroup and information about them (the bot itself may be one of these members). This list is empty if the message does not contain new chat members.
+        left_chat_member: Optional[:class:`bale.User`]
+            A member was removed from the group, information about them (this member may be the bot itself).
+        invoice: Optional[:class:`bale.Invoice`]
+            Message is an invoice for a payment, information about the invoice.
+    """
     __slots__ = (
-        "_type",
+        "text", "caption", "from_user", "_author", "contact", "location", "chat", "message_id", "forward_from",
+        "forward_from_chat", "forward_from_message_id", "date_code", "date",
+        "edit_date", "audio", "document", "photos", "voice", "location", "invoice", "new_chat_members",
+        "left_chat_member", "reply_to_message",
+        "invoice", "bot"
     )
 
-    def __init__(self, _type: str):
-        self._type = _type
+    def __init__(self, message_id: str, date: datetime, text: Optional[str] = None, caption: Optional[str] = None,
+                 forward_from: Optional["User"] = None, forward_from_chat: Optional["Chat"] = None,
+                 forward_from_message_id: Optional[str] = None, from_user: Optional["User"] = None,
+                 document: Optional["Document"] = None,
+                 contact: Optional["ContactMessage"] = None, location: Optional["Location"] = None,
+                 chat: Optional["Chat"] = None, photos: Optional[List["Photo"]] = None,
+                 reply_to_message: Optional["Message"] = None, invoice: Optional["Invoice"] = None,
+                 bot: 'Bot' = None, **options):
+        self.message_id: str = message_id if message_id is not None else None
+        self.date = date if date is not None else None
+
+        self.text: str | None = text if text is not None else None
+        self.chat: Chat | None = chat if chat is not None else None
+        self.reply_to_message: Message | None = reply_to_message if reply_to_message is not None else reply_to_message
+        self.from_user: User | None = from_user if from_user is not None else None
+        self.forward_from: User | None = forward_from if forward_from is not None else None
+        self.forward_from_message_id: str = forward_from_message_id if forward_from_message_id is not None else None
+        self.forward_from_chat: Chat | None = forward_from_chat if forward_from_chat is not None else None
+        self.caption: str | None = caption if caption is not None else None
+        self.document = document if document is not None else None
+        self.photos = photos if photos is not None else None
+        self.contact: ContactMessage | None = contact if contact is not None else None
+        self.location: Location | None = location if location is not None else None
+        self.new_chat_members: List[User] | None = options.get("new_chat_members")
+        self.left_chat_member: User | None = options.get("left_chat_member")
+        self.invoice = invoice
+        self.bot: Bot = bot if bot is not None else None
 
     @property
-    def type(self) -> str:
-        return self._type
+    def author(self):
+        """An alias for :attr:`from_user`"""
+        return self.from_user
 
-    def is_private_chat(self):
-        """bool:
-            Return ``True`` if Chat Type is Private"""
-        return self._type == self.PRIVATE
-
-    def is_group_chat(self):
-        """bool:
-            Return ``True`` if Chat Type is Group"""
-        return self._type == self.GROUP
+    @property
+    def content(self):
+        return self.caption or self.text
 
-    def __repr__(self):
-        return f"<ChatType type={self.type}>"
+    @content.setter
+    def content(self, _value):
+        if not isinstance(_value, str):
+            raise TypeError("content must be type of str")
+        if self.caption:
+            self.caption = _value
+        elif self.text:
+            self.text = _value
 
-    def __eq__(self, other):
-        return self._type == other
+    @property
+    def chat_id(self):
+        if self.chat:
+            return self.chat.chat_id
+        return None
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
+    @property
+    def reply_to_message_id(self):
+        if self.reply_to_message:
+            return self.reply_to_message.message_id
+        return None
+
+    @reply_to_message_id.setter
+    def reply_to_message_id(self, _value):
+        if not isinstance(_value, int):
+            raise TypeError("_value must be type of int")
 
-class Chat:
-    """This object indicates a chat.
+        if self.reply_to_message:
+            self.reply_to_message.message_id = _value
 
-    Attributes
-    ----------
-        chat_id: str
-            Chat ID.
-        _type: :class:`bale.ChatType`
-            Chat Type.
-        title: str
-            Chat Title.
-        username: str
-            Chat Username (for DM or PV).
-        first_name: str
-            First name Chat (for DM or PV).
-        last_name: str
-            Last name Chat (for DM or PV).
-        pinned_message: :class:`bale.Message`
-            Pinned messages in chat. Defaults to None.
-        all_members_are_administrators: bool
-            Does everyone have admin access?. Defaults to True. (for Group)
-        bot: :class:`bale.Bot`
-            Bot Object. Defaults to None.
-
-    .. container:: operations
-        .. describe:: x == y
-            Checks if two chat are equal.
-        .. describe:: x != y
-            Checks if two chat are not equal.
-    """
-    __slots__ = (
-        "chat_id",
-        "_type",
-        "title",
-        "username",
-        "first_name",
-        "last_name",
-        "pinned_message",
-        "all_members_are_administrators",
-        "bot"
-    )
+    @classmethod
+    def from_dict(cls, data: dict, bot):
+        options = {}
+        if data.get("new_chat_members"):
+            options["new_chat_members"] = [User.from_dict(bot=bot, data=i) for i in data.get("new_chat_members")]
+        if data.get("left_chat_member"):
+            options["left_chat_member"] = User.from_dict(bot=bot, data=data.get("left_chat_member"))
+
+        return cls(bot=bot, message_id=str(data.get("message_id")),
+                   chat=Chat.from_dict(bot=bot, data=data.get("chat")) if data.get("chat") else None,
+                   reply_to_message=Message.from_dict(bot=bot, data=data.get("reply_to_message")) if data.get(
+                       "reply_to_message") else None, date=datetime.fromtimestamp(int(data.get("date"))),
+                   text=data.get("text"),
+                   caption=data.get("caption"),
+                   from_user=User.from_dict(bot=bot, data=data.get("from")) if data.get("from") else None,
+                   forward_from=User.from_dict(bot=bot, data=data.get("forward_from")) if data.get(
+                       "forward_from") else None,
+                   forward_from_chat=Chat.from_dict(bot=bot, data=data.get("forward_from_chat")) if data.get(
+                       "forward_from_chat") else None,
+                   forward_from_message_id=str(data.get("forward_from_message_id")) if data.get(
+                       "forward_from_message_id") else None,
+                   document=Document.from_dict(bot=bot, data=data.get("document")) if data.get("document") else None,
+                   contact=ContactMessage.from_dict(data=data.get("contact")) if data.get("contact") else None,
+                   location=Location.from_dict(data=data.get("location")) if data.get("location") else None,
+                   photos=[Photo.from_dict(data=photo_payload) for photo_payload in data.get("photo")] if data.get(
+                       "photo") else None,
+                   invoice=Invoice.from_dict(data=data.get("invoice")) if data.get("invoice") else None, **options)
 
-    def __init__(self, chat_id: int | str, _type: "ChatType", title: str, username: str, first_name: str, last_name: str,
-                 pinned_message: Message | None = None, all_members_are_administrators: bool = True, bot: 'Bot' = None):
-        self.chat_id = chat_id
-        self._type = _type
-        self.title = title
-        self.username = username
-        self.first_name = first_name
-        self.last_name = last_name
-        self.pinned_message = pinned_message
-        self.all_members_are_administrators = all_members_are_administrators
-        self.bot = bot
+    def to_dict(self):
+        data = {"message_id": self.message_id, "date": self.date, "text": self.text}
 
-    @property
-    def type(self):
-        """Get chat type"""
-        return self._type
+        if self.chat:
+            data["chat"] = self.chat.to_dict()
+        if self.from_user:
+            data["from"] = self.from_user.to_dict()
+        if self.caption:
+            data["caption"] = self.caption
+        if self.document:
+            data["document"] = self.document.to_dict()
+        if self.photos:
+            data["photo"] = [photo.to_dict() for photo in self.photos]
+        if self.contact:
+            data["contact"] = self.contact.to_dict()
+        if self.location:
+            data["location"] = self.location.to_dict()
+        if self.new_chat_members:
+            data["new_chat_members"] = self.new_chat_members
+        if self.forward_from:
+            data["forward_from"] = self.forward_from.to_dict()
+        if self.forward_from_chat:
+            data["forward_from"] = self.forward_from_chat.to_dict()
+        if self.left_chat_member:
+            data["left_chat_member"] = self.left_chat_member.to_dict()
+        if self.reply_to_message_id:
+            data["reply_to_message_id"] = self.reply_to_message_id
 
-    @property
-    def mention(self) -> str | None:
-        """Optional[:class:`str`]"""
-        return ("@" + self.username) if self.username else None
+        return data
 
-    async def send(self, text: str, components: Optional["Components" | "RemoveComponents"] = None):
+    async def reply(self, text: str, *, components: Optional[Components | RemoveComponents] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
-
-        Parameters
-        -----------
-            text: str
-                Message content
-            components: Optional[:class:`bale.Components` | :class:`bale.RemoveComponents`]
-                Message components
-        Returns
-        --------
-            :class:`bale.Message`
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to send Message to this chat.
-            APIError
-                Send Message Failed.
         """
-        return await self.bot.send_message(self, text, components=components)
+        return await self.bot.send_message(self.chat_id, text, components=components,
+                                           reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def send_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
+    async def forward(self, chat_id: str | int):
         """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
+        For the documentation of the arguments, please see :meth:`bale.Bot.forward_message`.
+        """
+        return await self.bot.forward_message(chat_id, self.chat_id, self.message_id)
 
-        Parameters
-        ----------
-            document: :class:`bytes` | :class:`str` | :class:`bale.Document`
-                Document
-            caption: str
-                Message caption.
-        Returns
-        -------
-            Optional[:class:`bale.Message`]
-                On success, the sent Message is returned.
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to send Document to this chat.
-            APIError
-                Send Document Failed.  
+    async def reply_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
         """
-        return await self.bot.send_document(self, document, caption=caption)
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_document`.
+        """
+        return await self.bot.send_document(self.chat_id, document, caption=caption,
+                                            reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def send_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
+    async def reply_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
-
-        Parameters
-        ----------
-            photo: :class:`bytes` | :class:`str` | :class:`bale.Photo`
-                Photo
-            caption: Optional[:class:`str`]
-                Message caption
-        Returns
-        -------
-            Optional[:class:`bale.Message`]
-                On success, the sent Message is returned.
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to send Photo to chat.
-            APIError
-                Send Photo Failed.  
-        """
-        return await self.bot.send_photo(self, photo, caption=caption)
-
-    async def send_location(self, location: "Location"):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_location`.
-
-        Parameters
-        ----------
-            location: :class:`bale.Location`
-                Location
-        Returns
-        -------
-            Optional[:class:`bale.Message`]
-                On success, the sent Message is returned.
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to send Location to chat.
-            APIError
-                Send Location Failed.
-        """
-        return await self.bot.send_location(self, location)
-
-    async def send_contact(self, contact: "ContactMessage") -> "Message":
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_contact`.
-
-        Parameters
-        ----------
-            contact: :class:`bale.ContactMessage`
-                contact Message
-        Returns
-        -------
-            Optional[:class:`bale.Message`]
-                On success, the sent Message is returned.
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to Contact message to chat.
-            APIError
-                Send Contact message Failed.
-        """
-        return await self.bot.send_contact(self, contact)
-
-    async def send_invoice(self, title: str, description: str, provider_token: str, prices: List["Price"], *,
-                   photo_url: Optional[str] = None, need_name: Optional[bool] = False, need_phone_number: Optional[bool] = False,
-                       need_email: Optional[bool] = False, need_shipping_address: Optional[bool] = False, is_flexible: Optional[bool] = True):
         """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_invoice`
+        return await self.bot.send_photo(self.chat_id, photo, caption=caption,
+                                         reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-        Parameters
-        ----------
-            title: str
-                Invoice Title
-            description: str
-                Invoice Description
-            provider_token: str
-                .. note::
-                    You can use 3 methods to receive money:
-                        * Card number
-                        * Port number and acceptor number
-                        * Wallet number "Bale"
-            prices: List[:class:`bale.Price`]
-                A list of prices.
-            photo_url: Optional[:class:`str`]
-                Photo URL of Invoice.
-            need_name: Optional[:class:`bool`]
-                Get a name from "User"?
-            need_phone_number: Optional[:class:`bool`]
-                Get a Phone number from "User"?.
-            need_email: Optional[bool]
-                Get a Email from "User"?.
-            need_shipping_address: Optional[bool]
-                Get a Shipping Address from "User"?.
-            is_flexible: Optional[bool]
-                Is the Invoice Photo Flexible to the Payment button?
-        Returns
-        -------
-            :class:`Bale.Message`:
-                On success, the message sent returned.
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to send Invoice to this chat.
-            APIError
-                Send Invoice Failed.  
-        """
-        return await self.bot.send_invoice(chat=self, title=title, description=description,
-                                        provider_token=provider_token, prices=prices, photo_url=photo_url,
-                                        need_name=need_name, need_email=need_email, need_phone_number=need_phone_number,
-                                        need_shipping_address=need_shipping_address, is_flexible=is_flexible)
-
-    async def leave(self):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.leave_chat`.
-
-        Raises
-        ------
-            Forbidden
-                You do not have permission to Leave from chat.
-            APIError
-                Leave from chat Failed.
-        """
-        await self.bot.leave_chat(self)
-
-    async def add_user(self, user: "User"):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.invite_to_chat`.
-
-        Parameters
-        ----------
-            user: :class:`bale.User`
-                user
-        Raises
-        ------
-            NotFound
-                Invalid User.
-            Forbidden
-                You do not have permission to Add user to Chat.
-            APIError
-                Invite user Failed.
-        """
-        await self.bot.invite_to_chat(self, user)
-
-    async def get_chat_member(self, user: "User" | str):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.get_chat_member`.
-
-        Parameters
-        ----------
-            user: :class:`bale.User`
-                User
-
-        Returns
-        -------
-            Optional[:class:`bale.ChatMember`]:
-                The chat member or ``None`` if not found.
-
-        Raises
-        ------
-            NotFound
-                Invalid User.
-            Forbidden
-                You do not have permission to get Chat Member.
-            APIError
-                Get chat member Failed.
-        """
-        if not isinstance(user, (User, str)):
-            raise TypeError("user must be type of user or str")
-
-        if isinstance(user, User):
-            user = user.user_id
-
-        return await self.bot.get_chat_member(self, user_id=user)
-
-    async def get_chat_members_count(self):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.get_chat_members_count`.
-
-        Returns
-        -------
-            :class:`int`
-                The members count of the chat.
-
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to get Members count of the Chat.
-            APIError
-                get Members count of the Chat Failed.
-        """
-        return await self.bot.get_chat_members_count(self)
-
-    async def get_chat_administrators(self):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.get_chat_administrators`.
-
-        Raises
-        ------
-            NotFound
-                Invalid Chat ID.
-            Forbidden
-                You do not have permission to get Administrators of the Chat.
-            APIError
-                get Administrators of the Chat from chat Failed.
-        Returns
-        -------
-            Optional[List[:class:`bale.ChatMember`]]
-                On success, The chat members is returned.
+    async def reply_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
         """
-        return await self.bot.get_chat_administrators(self)
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
+        """
+        return await self.bot.send_video(self.chat_id, video, caption=caption,
+                                         reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    @classmethod
-    def from_dict(cls, data: dict, bot):
-        return cls(bot=bot, chat_id=data.get("id"), _type=ChatType(data.get("type")), title=data.get("title"),
-                   username=data.get("username"), first_name=data.get("first_name"), last_name=data.get("last_name"),
-                   pinned_message=Message.from_dict(bot=bot, data=data.get("pinned_message")) if data.get("pinned_message") else None,
-                   all_members_are_administrators=data.get("all_members_are_administrators", True))
+    async def reply_invoice(self, title: str, description: str, provider_token: str, prices: List["Price"], *,
+                            photo_url: Optional[str] = None,
+                            need_name: Optional[bool] = False, need_phone_number: Optional[bool] = False,
+                            need_email: Optional[bool] = False,
+                            need_shipping_address: Optional[bool] = False, is_flexible: Optional[bool] = True):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_invoice`
+        """
+        return await self.bot.send_invoice(self.chat_id, title, description, provider_token, prices,
+                                           photo_url=photo_url, need_name=need_name, need_email=need_email,
+                                           need_phone_number=need_phone_number,
+                                           need_shipping_address=need_shipping_address, is_flexible=is_flexible)
 
-    def to_dict(self):
-        data = {
-            "id": self.chat_id,
-            "type": self.type,
-            "title": self.title,
-            "username": self.username,
-            "first_name": self.first_name,
-            "last_name": self.last_name
-        }
-        if self.pinned_message:
-            data["pinned_message"] = self.pinned_message.to_dict()
+    async def edit(self, text: str, *, components: "Components" | "RemoveComponents" = None) -> Message:
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.edit_message`
+        """
+        return await self.bot.edit_message(self.chat_id, self.message_id, text, components=components)
 
-        return data
+    async def delete(self):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.delete_message`.
+        """
+        return await self.bot.delete_message(self.chat_id, self.message_id)
 
     def __str__(self):
-        return (str(self.username) + "#" + str(self.chat_id) if self.username else str(self.first_name) + " " + str(
-            self.last_name))
+        return str(self.message_id)
 
     def __eq__(self, other):
-        return isinstance(other, Chat) and self.chat_id == other.chat_id
+        return isinstance(other, Message) and self.message_id == other.message_id
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
-    def __hash__(self):
-        return hash(self.__str__())
-
     def __repr__(self):
-        return (f"<Chat type={self._type} first_name={self.first_name} last_name={self.last_name} user_id={self.chat_id} username={self.username}"
-            f"title={self.title}>")
+        return f"<Message message_id={self.message_id} from={self.from_user} chat={self.chat}>"
```

### Comparing `python-bale-bot-2.4.4/bale/chatmember.py` & `python-bale-bot-2.4.5/bale/chatmember.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,88 +17,104 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from bale import (Permissions, User)
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from bale import Bot
+from bale import Permissions, User
 
 __all__ = (
-    "MemberRole",
+    "ChatMemberStatus",
     "ChatMember"
 )
 
 
-class MemberRole:
-    """This object shows member's role in chat.
+class ChatMemberStatus:
+    """This object shows member's status in chat.
 
     .. container:: operations
         .. describe:: x == y
             Checks if two members role are equal.
         .. describe:: x != y
             Checks if two members role are not equal.
     """
 
     OWNER = "creator"
-    CREATOR = OWNER
     ADMIN = "administrator"
-    __slots__ = ("_role", )
+    MEMBER = "member"
+    CREATOR = OWNER
+    __slots__ = ("_status",)
 
-    def __init__(self, _role: str):
-        self._role = _role
+    def __init__(self, _status: str):
+        self._status = _status
 
     @property
-    def role(self) -> str:
-        return self._role
+    def status(self) -> str:
+        """"""
+        return self._status
 
     def is_owner(self):
         """bool:
 			Return ``True`` if Member is chat creator"""
-        return self._role == self.OWNER
+        return self._status == self.OWNER
 
     def is_admin(self):
         """bool:
-			Return ``True`` if Member have admin role"""
-        return self._role == self.ADMIN
+			Return ``True`` if Member have admin status"""
+        return self._status == self.ADMIN
+
+    def is_member(self):
+        """bool:
+            Return ``True`` if Member haven't any status"""
+        return self._status == self.MEMBER
 
     def __repr__(self):
-        return f"<MemberRole role={self.role}>"
+        return f"<MemberRole role={self.status}>"
 
     def __eq__(self, other):
-        return self._role == other
+        return self._status == other
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
 
 class ChatMember:
     """This object shows a member in chat
 
     Attributes
     ----------
-        role: :class:`bale.MemberRole`
-            User Role
         user: :class:`bale.User`
-            User
-        permissions: :class:`bale.AdminPermissions`
-            User Permissions
+            Information about the user.
+        status: :class:`bale.ChatMemberStatus`
+            The member’s status in the chat.
+        permissions: :class:`bale.Permissions`
+            The member’s permissions in the chat.
     """
     __slots__ = (
-        "role", "_user", "permissions"
+        "chat_id", "status", "user", "permissions", "bot"
     )
 
-    def __init__(self, role: "MemberRole", user, permissions):
-        self.role = role
-        self._user = user
+    def __init__(self, chat_id: int, status: "ChatMemberStatus", user: "User", permissions: "Permissions", bot: "Bot"):
+        self.chat_id = chat_id
+        self.status = status
+        self.user = user
         self.permissions = permissions
+        self.bot = bot
 
-    @property
-    def user(self) -> "User":
-        return self._user
+    async def ban(self):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.ban_chat_member`.
+        """
+        return await self.bot.ban_chat_member(self.chat_id, self.user.user_id)
 
     @classmethod
-    def from_dict(cls, data: dict):
-        return cls(permissions=Permissions.from_dict(data), user=User.from_dict(data.get("user")), role=MemberRole(data.get("status")))
+    def from_dict(cls, chat_id: int, data: dict, bot: "Bot"):
+        return cls(chat_id=chat_id, permissions=Permissions.from_dict(data), user=User.from_dict(data.get("user")),
+                   status=ChatMemberStatus(data.get("status")), bot=bot)
 
     def __repr__(self):
-        return f"<ChatMember role={self.role} user={self._user} permissions={self.permissions}>"
+        return f"<ChatMember chat_id={self.chat_id} status={self.status} user={self.user} permissions={self.permissions}>"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-bale-bot-2.4.4/bale/components.py` & `python-bale-bot-2.4.5/bale/components.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
-from typing import Dict
+from typing import Dict, Optional
 
 __all__ = (
     "Components",
     "Keyboard",
     "InlineKeyboard",
     "RemoveComponents"
 )
@@ -150,32 +150,43 @@
 class Keyboard:
     """This object shows a keyboard
 
     Attributes
     ----------
         text: str
             Keyboard Text.
+        request_contact: bool
+            If ``True``, the user’s phone number will be sent as a contact when the button is pressed.
+        request_location: bool
+            If ``True``, the user’s current location will be sent when the button is pressed. Available in private chats only.
     """
     __slots__ = (
-        "text"
+        "text",
+        "request_contact",
+        "request_location"
     )
 
-    def __init__(self, text: str):
+    def __init__(self, text: str, request_contact: Optional[bool] = False, request_location: Optional[bool] = False):
         self.text = text
+        self.request_contact = request_contact
+        self.request_location = request_location
 
     @classmethod
     def from_dict(cls, data: dict):
-        if not data.get("text"):
-            return None
-        return cls(text=data["text"])
+        return cls(text=data["text"], request_contact=data.get("request_contact", False), request_location=data.get("request_location", False))
 
     def to_dict(self):
         data = {
             "text": self.text
         }
+
+        if self.request_contact:
+            data["request_contact"] = self.request_contact
+        if self.request_location:
+            data["request_location"] = self.request_location
         return data
 
 
 class RemoveComponents:
     """This object shows a remove keyboard(s)."""
 
     def to_dict(self) -> dict:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-bale-bot-2.4.4/bale/error.py` & `python-bale-bot-2.4.5/bale/error.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/payments/invoice.py` & `python-bale-bot-2.4.5/bale/payments/invoice.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/payments/price.py` & `python-bale-bot-2.4.5/bale/payments/price.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/permissions.py` & `python-bale-bot-2.4.5/bale/permissions.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.4/bale/request/http.py` & `python-bale-bot-2.4.5/bale/request/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,18 +168,20 @@
 					async with self.__session.request(method=method, url=url, **kwargs) as response:
 						response: aiohttp.ClientResponse = response
 						parsed_response = await ResponseParser.from_response(response)
 						if response.status == ResponseStatusCode.OK:
 							return parsed_response
 						elif response.status == ResponseStatusCode.NOT_FOUND:
 							raise NotFound(parsed_response.description)
+						elif response.status == ResponseStatusCode.PERMISSION_DENIED:
+							raise Forbidden()
 						elif not parsed_response.ok or response.status in (ResponseStatusCode.NOT_INCORRECT, ResponseStatusCode.RATE_LIMIT):
 							if parsed_response.description == HTTPClientError.USER_OR_CHAT_NOT_FOUND:
 								raise NotFound("User or Chat not Found")
-							elif response.status == ResponseStatusCode.RATE_LIMIT or parsed_response.description == HTTPClientError.RATE_LIMIT or parsed_response.description == HTTPClientError.LOCAL_RATE_LIMIT:
+							elif response.status == ResponseStatusCode.RATE_LIMIT or parsed_response.description in (HTTPClientError.RATE_LIMIT, HTTPClientError.LOCAL_RATE_LIMIT):
 								if tries >= 4:
 									raise RateLimited()
 
 								if bool(self.rate_limit):
 									await self.rate_limit.new_request()
 								else:
 									self.rate_limit.enable()
@@ -222,14 +224,23 @@
 		if components:
 			payload["reply_markup"] = components
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
 		return self.request(Route("POST", "sendMessage", self.token), json=payload)
 
+	def forward_message(self, chat_id, from_chat_id, message_id):
+		payload = {
+			"chat_id": chat_id,
+			"from_chat_id": from_chat_id,
+			"message_id": message_id
+		}
+
+		return self.request(Route("POST", "forwardMessage", self.token), json=payload)
+
 	def send_document(self, chat_id, document, *, caption=None, reply_to_message_id=None):
 		payload = {
 			"chat_id": chat_id,
 			"document": document
 		}
 		if caption:
 			payload["caption"] = caption
@@ -247,14 +258,26 @@
 		if caption:
 			payload["caption"] = caption
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
 		return self.request(Route("POST", "SendPhoto", self.token), data=payload)
 
+	def send_video(self, chat_id, video, *, caption=None, reply_to_message_id=None):
+		payload = {
+			"chat_id": chat_id,
+			"video": video
+		}
+		if caption:
+			payload["caption"] = caption
+		if reply_to_message_id:
+			payload["reply_to_message_id"] = reply_to_message_id
+
+		return self.request(Route("POST", "sendVideo", self.token), data=payload)
+
 	def send_audio(self, chat_id, audio, *, caption=None, duration=None, title=None, reply_to_message_id=None):
 		payload = {
 			"chat_id": chat_id,
 			"audio": audio
 		}
 		if caption:
 			payload["caption"] = caption
@@ -338,9 +361,12 @@
 
 	def get_chat_members_count(self, chat_id):
 		return self.request(Route("GET", "getChatMemberCount", self.token), params=dict(chat_id=chat_id))
 
 	def get_chat_member(self, chat_id, member_id):
 		return self.request(Route("GET", "getChatMember", self.token), params=dict(chat_id=chat_id, user_id=member_id))
 
+	def ban_chat_member(self, chat_id, member_id):
+		return self.request(Route("POST", "banChatMember", self.token), params=dict(chat_id=chat_id, user_id=member_id))
+
 	def invite_to_chat(self, chat_id, user_id):
 		return self.request(Route("GET", "InviteUser", self.token), json=dict(chat_id=chat_id, user_id=user_id))
```

### Comparing `python-bale-bot-2.4.4/bale/request/parser.py` & `python-bale-bot-2.4.5/bale/request/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,13 @@
 		self.result = result
 		self.error_code = error_code
 		self.description = description
 		self._raw = raw
 
 	@classmethod
 	async def from_response(cls, data: "ClientResponse"):
-		if data.status == 404:
-			return cls(False, raw=dict())
-
 		data = await json_or_text(data)
 
 		if isinstance(data, str):
 			return cls(False, description=data, raw=dict(description=data))
 		else:
 			return cls(data.get("ok", False), data.get("result"), data.get("error_code"), data.get("description"), data)
```

### Comparing `python-bale-bot-2.4.4/bale/update.py` & `python-bale-bot-2.4.5/bale/update.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,34 +20,47 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING, Dict
 from bale import (Message, CallbackQuery)
+
 if TYPE_CHECKING:
     from bale import Bot
 
 __all__ = (
     "UpdateType",
     "Update"
 )
 
 
+def parse_type(data: dict) -> "UpdateType":
+    if data.get(UpdateType.CALLBACK):
+        return UpdateType(UpdateType.CALLBACK)
+    elif data.get(UpdateType.EDITED_MESSAGE):
+        return UpdateType(UpdateType.EDITED_MESSAGE)
+    elif data.get(UpdateType.MESSAGE):
+        return UpdateType(UpdateType.MESSAGE)
+    else:
+        return UpdateType(UpdateType.UNKNOWN)
+
+
 class UpdateType:
     """This object indicates an Update Type.
 
     .. container:: operations
         .. describe:: x == y
             Checks if two update type are equal.
         .. describe:: x != y
             Checks if two update type are not equal.
     """
     MESSAGE = "message"
     CALLBACK = "callback_query"
+    EDITED_MESSAGE = "edited_message"
     UNKNOWN = "unknown"
 
     __slots__ = (
         "_type",
     )
 
     def __init__(self, _type: str):
@@ -55,94 +68,98 @@
 
     @property
     def type(self) -> str:
         return self._type
 
     def is_message_update(self):
         """bool:
-			Return ``True`` if Update Type is Message"""
+        Return ``True`` if Update Type is Message"""
         return self._type == self.MESSAGE
 
     def is_callback_update(self):
         """bool:
-			Return ``True`` if Update Type is Callback"""
+        Return ``True`` if Update Type is Callback"""
         return self._type == self.CALLBACK
 
-    def __repr__(self):
-        return f"<UpdateType type={self.type}>"
+    def is_edited_message(self):
+        """bool:
+        Return ``True`` if Update Type is Edited Message"""
+        return self._type == self.EDITED_MESSAGE
+
+    def is_unknown_update(self):
+        """bool:
+        Return ``True`` if Update Type is Unknown"""
+        return self._type == self.UNKNOWN
+
+    def __str__(self):
+        return self._type
 
     def __eq__(self, other):
         return self._type == other
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
+
 class Update:
-    """This object shows an update.
+    """This object represents an incoming update.
 
     Attributes
     ----------
         update_id: int
-            Update ID
+            The update’s unique identifier. Update identifiers start from a certain positive number and increase sequentially. This ID becomes especially handy if you’re using Webhooks, since it allows you to ignore repeated updates or to restore the correct update sequence, should they get out of order. If there are no new updates for at least a week, then identifier of the next update will be chosen randomly instead of sequentially.
         callback_query: Optional[:class:`bale.CallbackQuery`]
-            Callback Query
+            New incoming callback query.
         message: Optional[:class:`bale.Message`]
-            Message
+            New incoming message of any kind - text, photo, sticker, etc.
         edited_message: Optional[:class:`bale.Message`]
-            Edited Message
+            New version of a message that is known to the bot and was edited.
     """
     __slots__ = (
         "update_id",
-        "_type",
+        "type",
         "message",
         "callback_query",
         "edited_message",
-        "bot",
-        "raw_data"
+        "bot"
     )
 
-    def __init__(self, update_id: int, _type: str, callback_query: "CallbackQuery" = None, message: "Message" = None,
-                 edited_message: "Message" = None, bot: 'Bot' = None, raw_data: dict = None):
+    def __init__(self, update_id: int, type: "UpdateType", callback_query: "CallbackQuery" = None, message: "Message" = None,
+                 edited_message: "Message" = None, bot: 'Bot' = None):
         self.update_id = int(update_id)
-        self._type = _type
+        self.type = type
         self.bot = bot
-        self.raw_data = raw_data
         self.callback_query = callback_query if callback_query is not None else None
         self.message = message if message is not None else None
         self.edited_message = edited_message if edited_message is not None else None
 
-    @property
-    def type(self) -> UpdateType:
-        return UpdateType(self._type)
-
     @classmethod
     def from_dict(cls, data: dict, bot: "Bot"):
         callback_query, message, edited_message = None, None, None
+        parsed_type: UpdateType = parse_type(data)
 
-        if data.get("callback_query"):
+        if parsed_type.is_callback_update():
             callback_query = CallbackQuery.from_dict(data.get("callback_query"), bot=bot)
-        if data.get("message"):
+        if parsed_type.is_message_update():
             message = Message.from_dict(data.get("message"), bot=bot)
-        if data.get("edited_message"):
-            edited_message = Message.from_dict(data=data.get("edited_message"), bot=bot)
+        if parsed_type.is_edited_message():
+            edited_message = Message.from_dict(data.get("edited_message"), bot=bot)
 
-        return cls(_type = UpdateType.CALLBACK if callback_query else UpdateType.MESSAGE, update_id=data["update_id"], message=message, callback_query=callback_query, edited_message=edited_message,
-                   raw_data=data, bot=bot)
+        return cls(type=parsed_type, update_id=data["update_id"],
+                   message=message, callback_query=callback_query, edited_message=edited_message, bot=bot)
 
     def to_dict(self) -> Dict:
         data = {}
 
         if self.type:
-            data["type"] = self._type
+            data["type"] = self.type
         if self.callback_query:
             data["callback_query"] = self.callback_query.to_dict()
         if self.message:
             data["message"] = self.message.to_dict()
-        if self.edited_message:
-            data["edited_message"] = self.edited_message.to_dict()
 
         return data
 
     def __eq__(self, other):
         return isinstance(other, Update) and self.update_id == other.update_id
 
     def __ne__(self, other):
@@ -166,8 +183,8 @@
 
         return self.update_id < other.update_id
 
     def __gt__(self, other):
         return not self.__lt__(other)
 
     def __repr__(self):
-        return f"<Update type={self._type} message={self.message}>"
+        return f"<Update update_id={self.update_id} type={self.type}>"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python-bale-bot-2.4.4/python_bale_bot.egg-info/PKG-INFO` & `python-bale-bot-2.4.5/python_bale_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.4
+Version: 2.4.5
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
 License: MIT License
-Project-URL: Documentation, https://python-bale-bot.rtfd.io/en/master/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
 Project-URL: Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.4 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.5 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
 bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
-Documentation, https://python-bale-bot.rtfd.io/en/master/ Project-URL:
+Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
 Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html Project-
 URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
 LICENSE # python-bale-bot
                            [python-bale-bot image]
```

### Comparing `python-bale-bot-2.4.4/python_bale_bot.egg-info/SOURCES.txt` & `python-bale-bot-2.4.5/python_bale_bot.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 bale/version.py
 bale/attachments/__init__.py
 bale/attachments/audio.py
 bale/attachments/contact.py
 bale/attachments/document.py
 bale/attachments/location.py
 bale/attachments/photo.py
+bale/attachments/video.py
 bale/payments/__init__.py
 bale/payments/invoice.py
 bale/payments/price.py
 bale/request/__init__.py
 bale/request/http.py
 bale/request/parser.py
 bale/request/utils.py
```

### Comparing `python-bale-bot-2.4.4/setup.py` & `python-bale-bot-2.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         'typing-extensions>=4.3,<5',
     ]
 }
 
 if __name__ == "__main__":
     setup(
         name="python-bale-bot",
-        version="2.4.4",
+        version="2.4.5",
         platforms=["Windows", ],
         fullname="python-bale-bot",
         description="An API wrapper for Bale written in Python",
         author="Kian Ahmadian",
         license="MIT License",
         project_urls={
-            "Documentation": "https://python-bale-bot.rtfd.io/en/master/",
+            "Documentation": "https://docs.python-bale-bot.ir/en/master/",
             "Changelog": "https://python-bale-bot.rtfd.io/en/master/whats_new.html",
             "Bug Tracker": "https://github.com/python-bale-bot/python-bale-bot/issues",
             "Source Code": "https://github.com/python-bale-bot/python-bale-bot/"
         },
         keywords=["bale", "bale-bot", "framework", "bot"],
         python_requires='>=3.8',
         extras_require=extras_require,
```

