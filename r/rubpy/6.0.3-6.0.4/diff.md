# Comparing `tmp/rubpy-6.0.3.tar.gz` & `tmp/rubpy-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.0.3.tar", last modified: Sun Apr 16 01:20:14 2023, max compression
+gzip compressed data, was "rubpy-6.0.4.tar", last modified: Fri Apr 21 01:44:12 2023, max compression
```

## Comparing `rubpy-6.0.3.tar` & `rubpy-6.0.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.901879 rubpy-6.0.3/
--rw-rw-rw-   0        0        0     3595 2023-04-16 01:20:14.901879 rubpy-6.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.870637 rubpy-6.0.3/rubpy/
--rw-rw-rw-   0        0        0      193 2023-04-16 01:20:00.000000 rubpy-6.0.3/rubpy/__init__.py
--rw-rw-rw-   0        0        0    11974 2023-04-16 00:00:51.000000 rubpy-6.0.3/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.886259 rubpy-6.0.3/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.901879 rubpy-6.0.3/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      909 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    28859 2023-04-16 01:18:52.000000 rubpy-6.0.3/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.901879 rubpy-6.0.3/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.3/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.901879 rubpy-6.0.3/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.901879 rubpy-6.0.3/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15142 2022-09-12 11:03:20.000000 rubpy-6.0.3/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:20:14.886259 rubpy-6.0.3/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3595 2023-04-16 01:20:14.000000 rubpy-6.0.3/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-04-16 01:20:14.000000 rubpy-6.0.3/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 01:20:14.000000 rubpy-6.0.3/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-16 01:20:14.000000 rubpy-6.0.3/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-16 01:20:14.000000 rubpy-6.0.3/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 01:20:14.901879 rubpy-6.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-04-16 01:19:52.000000 rubpy-6.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.822224 rubpy-6.0.4/
+-rw-rw-rw-   0        0        0     3351 2023-04-21 01:44:12.822224 rubpy-6.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2211 2023-04-21 01:42:49.000000 rubpy-6.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.774895 rubpy-6.0.4/rubpy/
+-rw-rw-rw-   0        0        0      193 2023-04-21 01:36:02.000000 rubpy-6.0.4/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    11974 2023-04-16 00:00:51.000000 rubpy-6.0.4/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.790916 rubpy-6.0.4/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      909 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25221 2023-04-19 09:40:07.000000 rubpy-6.0.4/rubpy/gadgets/json_methods.py
+-rw-rw-rw-   0        0        0    14160 2023-04-21 01:05:40.000000 rubpy-6.0.4/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.4/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.806539 rubpy-6.0.4/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.822224 rubpy-6.0.4/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15142 2022-09-12 11:03:20.000000 rubpy-6.0.4/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:12.790916 rubpy-6.0.4/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3351 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 01:44:12.000000 rubpy-6.0.4/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:44:12.822224 rubpy-6.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-21 01:43:31.000000 rubpy-6.0.4/setup.py
```

### Comparing `rubpy-6.0.3/PKG-INFO` & `rubpy-6.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.3
+Version: 6.0.4
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,15 +30,15 @@
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
     •
-    <a href="https://github.com/shayanheidari01/rubika/raw/master/docs/rubpy-documents.pdf">
+    <a href="https://github.com/shayanheidari01/rubika/tree/master/docs">
         Documentation
     </a>
     •
     <a href="https://pypi.org/project/rubpy/#history">
         Releases
     </a>
     •
@@ -46,67 +46,41 @@
         News
     </a>
 </p>
 
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
-### Bots Examples
-```python
-from rubpy import Bot
-
-app = Bot('token')
-
-async def my_bot(bot):
-    me = await bot.getMe()
-    print(me)
-
-app.run(my_bot)
-```
-**OR**
-```python
-from rubpy import Bot
-
-app = Bot('token')
 
-async def my_bot(bot):
-    me = await bot.sendMessage('chat_id', 'text')
-    print(me)
-
-app.run(my_bot)
-```
 ### Accounts
-``` python
-from rubpy import Client, Methods, Message
+```python
+import asyncio
+from rubpy import Client, handlers
 
-app = Client(
-    'MY-AUTH',
-    "my_guid"
-)
-
-@app.MessageUpdates
-async def my_bot(bot: Methods, message: Message):
-    await message.reply('``Hello`` __from__ **Rubpy**!')
+async def main():
+    async with Client(session='rubpy') as client:
+        @client.on(handlers.MessageUpdates())
+        async def updates(update):
+            await update.reply('`hello` __from__ **rubpy**')
+        await client.run_until_disconnected()
 
+asyncio.run(main())
 ```
 
 **Another example:**
-``` python
-from rubpy import Client, Methods
-
-app = Client(
-    "my_account_auth",
-    "my_account_guid"
-)
-
-async def my_bot(bot: Methods):
-    await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
+```python
+from rubpy import Client
+from asyncio import run
 
-app.run(my_bot)
+async def main():
+    async with Client(session='rubpy') as client:
+        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        print(result)
 
+run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
@@ -117,9 +91,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==5.2.2
+pip3 install rubpy==6.0.4
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.3 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.4 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -13,29 +13,26 @@
 :: Python Modules Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
-users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
-('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
-(my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
-def my_bot(bot): me = await bot.sendMessage('chat_id', 'text') print(me)
-app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client, Methods,
-Message app = Client( 'MY-AUTH', "my_guid" ) @app.MessageUpdates async def
-my_bot(bot: Methods, message: Message): await message.reply('``Hello`` __from__
-**Rubpy**!') ``` **Another example:** ``` python from rubpy import Client,
-Methods app = Client( "my_account_auth", "my_account_guid" ) async def my_bot
-(bot: Methods): await bot.sendText('object_guid', '``Hello`` __from__
-**Rubpy**!') app.run(my_bot) ``` **Rubpy** is a modern, elegant and
-asynchronous framework. It enables you to easily interact with the main Rubika
-API through a user account (custom client) or a bot identity (bot API
-alternative) using Python. ### Key Features - **Ready**: Install Rubpy with pip
-and start building your applications right away. - **Easy**: Makes the Rubika
-API simple and intuitive, while still allowing advanced usages. - **Elegant**:
-Low-level details are abstracted and re-presented in a more convenient way. -
-**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
-written in C. - **Async**: Fully asynchronous (also usable synchronously if
-wanted, for convenience). - **Powerful**: Full access to Rubika's API to
-execute any official client action and more. ### Installing ``` bash pip3
-install rubpy==5.2.2 ```
+users and bots ### Accounts ```python import asyncio from rubpy import Client,
+handlers async def main(): async with Client(session='rubpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
+Client from asyncio import run async def main(): async with Client
+(session='rubpy') as client: result = await client.send_message('GUID',
+'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
+modern, elegant and asynchronous framework. It enables you to easily interact
+with the main Rubika API through a user account (custom client) or a bot
+identity (bot API alternative) using Python. ### Key Features - **Ready**:
+Install Rubpy with pip and start building your applications right away. -
+**Easy**: Makes the Rubika API simple and intuitive, while still allowing
+advanced usages. - **Elegant**: Low-level details are abstracted and re-
+presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
+high-performance cryptography library written in C. - **Async**: Fully
+asynchronous (also usable synchronously if wanted, for convenience). -
+**Powerful**: Full access to Rubika's API to execute any official client action
+and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
```

### Comparing `rubpy-6.0.3/README.md` & `rubpy-6.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
     •
-    <a href="https://github.com/shayanheidari01/rubika/raw/master/docs/rubpy-documents.pdf">
+    <a href="https://github.com/shayanheidari01/rubika/tree/master/docs">
         Documentation
     </a>
     •
     <a href="https://pypi.org/project/rubpy/#history">
         Releases
     </a>
     •
@@ -21,67 +21,41 @@
         News
     </a>
 </p>
 
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
-### Bots Examples
-```python
-from rubpy import Bot
-
-app = Bot('token')
-
-async def my_bot(bot):
-    me = await bot.getMe()
-    print(me)
-
-app.run(my_bot)
-```
-**OR**
-```python
-from rubpy import Bot
-
-app = Bot('token')
 
-async def my_bot(bot):
-    me = await bot.sendMessage('chat_id', 'text')
-    print(me)
-
-app.run(my_bot)
-```
 ### Accounts
-``` python
-from rubpy import Client, Methods, Message
+```python
+import asyncio
+from rubpy import Client, handlers
 
-app = Client(
-    'MY-AUTH',
-    "my_guid"
-)
-
-@app.MessageUpdates
-async def my_bot(bot: Methods, message: Message):
-    await message.reply('``Hello`` __from__ **Rubpy**!')
+async def main():
+    async with Client(session='rubpy') as client:
+        @client.on(handlers.MessageUpdates())
+        async def updates(update):
+            await update.reply('`hello` __from__ **rubpy**')
+        await client.run_until_disconnected()
 
+asyncio.run(main())
 ```
 
 **Another example:**
-``` python
-from rubpy import Client, Methods
-
-app = Client(
-    "my_account_auth",
-    "my_account_guid"
-)
-
-async def my_bot(bot: Methods):
-    await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
+```python
+from rubpy import Client
+from asyncio import run
 
-app.run(my_bot)
+async def main():
+    async with Client(session='rubpy') as client:
+        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        print(result)
 
+run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
@@ -92,9 +66,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==5.2.2
+pip3 install rubpy==6.0.4
 ```
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
-users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
-('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
-(my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
-def my_bot(bot): me = await bot.sendMessage('chat_id', 'text') print(me)
-app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client, Methods,
-Message app = Client( 'MY-AUTH', "my_guid" ) @app.MessageUpdates async def
-my_bot(bot: Methods, message: Message): await message.reply('``Hello`` __from__
-**Rubpy**!') ``` **Another example:** ``` python from rubpy import Client,
-Methods app = Client( "my_account_auth", "my_account_guid" ) async def my_bot
-(bot: Methods): await bot.sendText('object_guid', '``Hello`` __from__
-**Rubpy**!') app.run(my_bot) ``` **Rubpy** is a modern, elegant and
-asynchronous framework. It enables you to easily interact with the main Rubika
-API through a user account (custom client) or a bot identity (bot API
-alternative) using Python. ### Key Features - **Ready**: Install Rubpy with pip
-and start building your applications right away. - **Easy**: Makes the Rubika
-API simple and intuitive, while still allowing advanced usages. - **Elegant**:
-Low-level details are abstracted and re-presented in a more convenient way. -
-**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
-written in C. - **Async**: Fully asynchronous (also usable synchronously if
-wanted, for convenience). - **Powerful**: Full access to Rubika's API to
-execute any official client action and more. ### Installing ``` bash pip3
-install rubpy==5.2.2 ```
+users and bots ### Accounts ```python import asyncio from rubpy import Client,
+handlers async def main(): async with Client(session='rubpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
+Client from asyncio import run async def main(): async with Client
+(session='rubpy') as client: result = await client.send_message('GUID',
+'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
+modern, elegant and asynchronous framework. It enables you to easily interact
+with the main Rubika API through a user account (custom client) or a bot
+identity (bot API alternative) using Python. ### Key Features - **Ready**:
+Install Rubpy with pip and start building your applications right away. -
+**Easy**: Makes the Rubika API simple and intuitive, while still allowing
+advanced usages. - **Elegant**: Low-level details are abstracted and re-
+presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
+high-performance cryptography library written in C. - **Async**: Fully
+asynchronous (also usable synchronously if wanted, for convenience). -
+**Powerful**: Full access to Rubika's API to execute any official client action
+and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
```

### Comparing `rubpy-6.0.3/rubpy/client.py` & `rubpy-6.0.4/rubpy/client.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/crypto/crypto.py` & `rubpy-6.0.4/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/gadgets/classino.py` & `rubpy-6.0.4/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/gadgets/exceptions.py` & `rubpy-6.0.4/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/gadgets/thumbnail.py` & `rubpy-6.0.4/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/network/connection.py` & `rubpy-6.0.4/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/network/proxies.py` & `rubpy-6.0.4/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/sessions/sqliteSession.py` & `rubpy-6.0.4/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/sessions/stringSession.py` & `rubpy-6.0.4/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/structs/handlers.py` & `rubpy-6.0.4/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/structs/models.py` & `rubpy-6.0.4/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/structs/results.py` & `rubpy-6.0.4/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy/structs/struct.py` & `rubpy-6.0.4/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.3/rubpy.egg-info/PKG-INFO` & `rubpy-6.0.4/rubpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.3
+Version: 6.0.4
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,15 +30,15 @@
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
     •
-    <a href="https://github.com/shayanheidari01/rubika/raw/master/docs/rubpy-documents.pdf">
+    <a href="https://github.com/shayanheidari01/rubika/tree/master/docs">
         Documentation
     </a>
     •
     <a href="https://pypi.org/project/rubpy/#history">
         Releases
     </a>
     •
@@ -46,67 +46,41 @@
         News
     </a>
 </p>
 
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
-### Bots Examples
-```python
-from rubpy import Bot
-
-app = Bot('token')
-
-async def my_bot(bot):
-    me = await bot.getMe()
-    print(me)
-
-app.run(my_bot)
-```
-**OR**
-```python
-from rubpy import Bot
-
-app = Bot('token')
 
-async def my_bot(bot):
-    me = await bot.sendMessage('chat_id', 'text')
-    print(me)
-
-app.run(my_bot)
-```
 ### Accounts
-``` python
-from rubpy import Client, Methods, Message
+```python
+import asyncio
+from rubpy import Client, handlers
 
-app = Client(
-    'MY-AUTH',
-    "my_guid"
-)
-
-@app.MessageUpdates
-async def my_bot(bot: Methods, message: Message):
-    await message.reply('``Hello`` __from__ **Rubpy**!')
+async def main():
+    async with Client(session='rubpy') as client:
+        @client.on(handlers.MessageUpdates())
+        async def updates(update):
+            await update.reply('`hello` __from__ **rubpy**')
+        await client.run_until_disconnected()
 
+asyncio.run(main())
 ```
 
 **Another example:**
-``` python
-from rubpy import Client, Methods
-
-app = Client(
-    "my_account_auth",
-    "my_account_guid"
-)
-
-async def my_bot(bot: Methods):
-    await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
+```python
+from rubpy import Client
+from asyncio import run
 
-app.run(my_bot)
+async def main():
+    async with Client(session='rubpy') as client:
+        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        print(result)
 
+run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
@@ -117,9 +91,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==5.2.2
+pip3 install rubpy==6.0.4
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.3 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.4 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -13,29 +13,26 @@
 :: Python Modules Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
-users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
-('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
-(my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
-def my_bot(bot): me = await bot.sendMessage('chat_id', 'text') print(me)
-app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client, Methods,
-Message app = Client( 'MY-AUTH', "my_guid" ) @app.MessageUpdates async def
-my_bot(bot: Methods, message: Message): await message.reply('``Hello`` __from__
-**Rubpy**!') ``` **Another example:** ``` python from rubpy import Client,
-Methods app = Client( "my_account_auth", "my_account_guid" ) async def my_bot
-(bot: Methods): await bot.sendText('object_guid', '``Hello`` __from__
-**Rubpy**!') app.run(my_bot) ``` **Rubpy** is a modern, elegant and
-asynchronous framework. It enables you to easily interact with the main Rubika
-API through a user account (custom client) or a bot identity (bot API
-alternative) using Python. ### Key Features - **Ready**: Install Rubpy with pip
-and start building your applications right away. - **Easy**: Makes the Rubika
-API simple and intuitive, while still allowing advanced usages. - **Elegant**:
-Low-level details are abstracted and re-presented in a more convenient way. -
-**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
-written in C. - **Async**: Fully asynchronous (also usable synchronously if
-wanted, for convenience). - **Powerful**: Full access to Rubika's API to
-execute any official client action and more. ### Installing ``` bash pip3
-install rubpy==5.2.2 ```
+users and bots ### Accounts ```python import asyncio from rubpy import Client,
+handlers async def main(): async with Client(session='rubpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
+Client from asyncio import run async def main(): async with Client
+(session='rubpy') as client: result = await client.send_message('GUID',
+'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
+modern, elegant and asynchronous framework. It enables you to easily interact
+with the main Rubika API through a user account (custom client) or a bot
+identity (bot API alternative) using Python. ### Key Features - **Ready**:
+Install Rubpy with pip and start building your applications right away. -
+**Easy**: Makes the Rubika API simple and intuitive, while still allowing
+advanced usages. - **Elegant**: Low-level details are abstracted and re-
+presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
+high-performance cryptography library written in C. - **Async**: Fully
+asynchronous (also usable synchronously if wanted, for convenience). -
+**Powerful**: Full access to Rubika's API to execute any official client action
+and more. ### Installing ``` bash pip3 install rubpy==6.0.4 ```
```

### Comparing `rubpy-6.0.3/rubpy.egg-info/SOURCES.txt` & `rubpy-6.0.4/rubpy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 rubpy.egg-info/requires.txt
 rubpy.egg-info/top_level.txt
 rubpy/crypto/__init__.py
 rubpy/crypto/crypto.py
 rubpy/gadgets/__init__.py
 rubpy/gadgets/classino.py
 rubpy/gadgets/exceptions.py
+rubpy/gadgets/json_methods.py
 rubpy/gadgets/methods.py
 rubpy/gadgets/thumbnail.py
 rubpy/network/__init__.py
 rubpy/network/connection.py
 rubpy/network/proxies.py
 rubpy/sessions/__init__.py
 rubpy/sessions/sqliteSession.py
```

### Comparing `rubpy-6.0.3/setup.py` & `rubpy-6.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-requirements = ['aiohttp', 'pycryptodome']
+requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.0.3',
+    version = '6.0.4',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

