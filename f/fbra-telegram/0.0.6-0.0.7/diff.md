# Comparing `tmp/fbra-telegram-0.0.6.tar.gz` & `tmp/fbra-telegram-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbra-telegram-0.0.6.tar", last modified: Wed Apr  5 06:14:26 2023, max compression
+gzip compressed data, was "fbra-telegram-0.0.7.tar", last modified: Fri Apr 21 09:02:14 2023, max compression
```

## Comparing `fbra-telegram-0.0.6.tar` & `fbra-telegram-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/
--rw-rw-rw-   0        0        0    35823 2023-04-03 07:47:06.000000 fbra-telegram-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      439 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3422 2023-04-05 05:45:27.000000 fbra-telegram-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/fbra_telegram.egg-info/
--rw-rw-rw-   0        0        0      439 2023-04-05 06:14:26.000000 fbra-telegram-0.0.6/fbra_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      508 2023-04-05 06:14:26.000000 fbra-telegram-0.0.6/fbra_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 06:14:26.000000 fbra-telegram-0.0.6/fbra_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-04-05 06:14:26.000000 fbra-telegram-0.0.6/fbra_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 06:14:26.000000 fbra-telegram-0.0.6/fbra_telegram.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/fbratelegram/
--rw-rw-rw-   0        0        0        2 2023-04-03 09:56:22.000000 fbra-telegram-0.0.6/fbratelegram/__init__.py
--rw-rw-rw-   0        0        0    17402 2023-04-05 05:48:16.000000 fbra-telegram-0.0.6/fbratelegram/client.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/fbratelegram/examples/
--rw-rw-rw-   0        0        0        0 2023-04-03 18:57:01.000000 fbra-telegram-0.0.6/fbratelegram/examples/__init__.py
--rw-rw-rw-   0        0        0     3098 2023-04-03 13:11:03.000000 fbra-telegram-0.0.6/fbratelegram/examples/asyncio_to_thread.py
--rw-rw-rw-   0        0        0     1408 2023-04-04 20:17:46.000000 fbra-telegram-0.0.6/fbratelegram/examples/quick_start.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/fbratelegram/extras/
--rw-rw-rw-   0        0        0        0 2023-04-03 10:34:22.000000 fbra-telegram-0.0.6/fbratelegram/extras/__init__.py
--rw-rw-rw-   0        0        0     1938 2023-04-04 09:45:57.000000 fbra-telegram-0.0.6/fbratelegram/extras/config_parser.py
--rw-rw-rw-   0        0        0        0 2023-04-04 07:45:49.000000 fbra-telegram-0.0.6/fbratelegram/extras/crypto.py
--rw-rw-rw-   0        0        0     1236 2023-04-02 18:29:39.000000 fbra-telegram-0.0.6/fbratelegram/extras/stderr_logger.py
--rw-rw-rw-   0        0        0       42 2023-04-05 06:14:26.493778 fbra-telegram-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-04-05 05:46:54.000000 fbra-telegram-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:02:14.238413 fbra-telegram-0.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-03 07:47:06.000000 fbra-telegram-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      439 2023-04-21 09:02:14.238413 fbra-telegram-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3412 2023-04-05 09:58:49.000000 fbra-telegram-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 09:02:14.226403 fbra-telegram-0.0.7/fbra_telegram.egg-info/
+-rw-rw-rw-   0        0        0      439 2023-04-21 09:02:14.000000 fbra-telegram-0.0.7/fbra_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      508 2023-04-21 09:02:14.000000 fbra-telegram-0.0.7/fbra_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:02:14.000000 fbra-telegram-0.0.7/fbra_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-04-21 09:02:14.000000 fbra-telegram-0.0.7/fbra_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 09:02:14.000000 fbra-telegram-0.0.7/fbra_telegram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:02:14.226403 fbra-telegram-0.0.7/fbratelegram/
+-rw-rw-rw-   0        0        0        2 2023-04-03 09:56:22.000000 fbra-telegram-0.0.7/fbratelegram/__init__.py
+-rw-rw-rw-   0        0        0    17402 2023-04-05 05:48:16.000000 fbra-telegram-0.0.7/fbratelegram/client.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:02:14.230411 fbra-telegram-0.0.7/fbratelegram/examples/
+-rw-rw-rw-   0        0        0        0 2023-04-03 18:57:01.000000 fbra-telegram-0.0.7/fbratelegram/examples/__init__.py
+-rw-rw-rw-   0        0        0     3098 2023-04-03 13:11:03.000000 fbra-telegram-0.0.7/fbratelegram/examples/asyncio_to_thread.py
+-rw-rw-rw-   0        0        0     1408 2023-04-04 20:17:46.000000 fbra-telegram-0.0.7/fbratelegram/examples/quick_start.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:02:14.234412 fbra-telegram-0.0.7/fbratelegram/extras/
+-rw-rw-rw-   0        0        0        0 2023-04-03 10:34:22.000000 fbra-telegram-0.0.7/fbratelegram/extras/__init__.py
+-rw-rw-rw-   0        0        0     1938 2023-04-04 09:45:57.000000 fbra-telegram-0.0.7/fbratelegram/extras/config_parser.py
+-rw-rw-rw-   0        0        0        0 2023-04-04 07:45:49.000000 fbra-telegram-0.0.7/fbratelegram/extras/crypto.py
+-rw-rw-rw-   0        0        0     1594 2023-04-21 08:26:43.000000 fbra-telegram-0.0.7/fbratelegram/extras/stderr_logger.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:02:14.238413 fbra-telegram-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-04-21 08:20:03.000000 fbra-telegram-0.0.7/setup.py
```

### Comparing `fbra-telegram-0.0.6/LICENSE` & `fbra-telegram-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fbra-telegram-0.0.6/README.md` & `fbra-telegram-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -81,23 +81,22 @@
 # If you don't need commands anymore, you can stop the loop.
 telegram.stop_loop()
 ```
 ```python
 # predefined functions are:
 /info, /stop, /restart and /help
 ```
-```
 ## Client Configuration
-```python
+```
 **kwargs of Client:
 ----------------------------
 - bot_token=<TELEGRAM-TOKEN>  # is required to allow a connection to a bot
 - save_token=False # if you set it to True, it will save your token in config.ini - file for easier use
 - chat_id=None # provide chat_id for specific chat
-- log_lvl=logging.DEBUG # set the loggin level of you bot
+- log_lvl=logging.DEBUG # set the logging level of you bot
 - log_stderr=False # redirect stderr output to display in bot
 - other_logger=None  # redirect other_logger output to display in bot
 - encrypt_vars=False # if set to True, you can give an key [with the help of environment_var] to encrypt token and chat_id
 - environment_var # name of the environment variable
 ```
 ## Exceptions
 >This error happens if you run more than one Client connection.
```

#### html2text {}

```diff
@@ -22,20 +22,20 @@
 ```python # Retrieve arguments from command, e.g. type '/what stuff' ... def
 command_with_args(update, context): try: arg = context.args[0] except
 IndexError: arg = 'crazy' telegram.double_log_msg(f"This is {arg} stuff my
 friend.") telegram.add_command("what", command_with_args) ... ``` ```python #
 If blocking is set to False, the telegram loop works # as long as the main
 thread is alive. telegram.start_loop(blocking=False) #  # If you don't need
 commands anymore, you can stop the loop. telegram.stop_loop() ``` ```python #
-predefined functions are: /info, /stop, /restart and /help ``` ``` ## Client
-Configuration ```python **kwargs of Client: ---------------------------- -
-bot_token= # is required to allow a connection to a bot - save_token=False # if
-you set it to True, it will save your token in config.ini - file for easier use
-- chat_id=None # provide chat_id for specific chat - log_lvl=logging.DEBUG #
-set the loggin level of you bot - log_stderr=False # redirect stderr output to
+predefined functions are: /info, /stop, /restart and /help ``` ## Client
+Configuration ``` **kwargs of Client: ---------------------------- - bot_token=
+# is required to allow a connection to a bot - save_token=False # if you set it
+to True, it will save your token in config.ini - file for easier use -
+chat_id=None # provide chat_id for specific chat - log_lvl=logging.DEBUG # set
+the logging level of you bot - log_stderr=False # redirect stderr output to
 display in bot - other_logger=None # redirect other_logger output to display in
 bot - encrypt_vars=False # if set to True, you can give an key [with the help
 of environment_var] to encrypt token and chat_id - environment_var # name of
 the environment variable ``` ## Exceptions >This error happens if you run more
 than one Client connection. > ![error-getUpdates_2023-04-03_21-16-18.jpg]
 (fbratelegram%2Fexamples%2Ferror-getUpdates_2023-04-03_21-16-18.jpg) ##
 Donations ```python BTC: 'bc1qed0e8ej4nmyz88sy5zzwvrjfkft0y5aca7cqyw' ETH:
```

### Comparing `fbra-telegram-0.0.6/fbratelegram/client.py` & `fbra-telegram-0.0.7/fbratelegram/client.py`

 * *Files identical despite different names*

### Comparing `fbra-telegram-0.0.6/fbratelegram/examples/asyncio_to_thread.py` & `fbra-telegram-0.0.7/fbratelegram/examples/asyncio_to_thread.py`

 * *Files identical despite different names*

### Comparing `fbra-telegram-0.0.6/fbratelegram/examples/quick_start.py` & `fbra-telegram-0.0.7/fbratelegram/examples/quick_start.py`

 * *Files identical despite different names*

### Comparing `fbra-telegram-0.0.6/fbratelegram/extras/config_parser.py` & `fbra-telegram-0.0.7/fbratelegram/extras/config_parser.py`

 * *Files identical despite different names*

### Comparing `fbra-telegram-0.0.6/setup.py` & `fbra-telegram-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Send Messages to Telegram'
 LONG_DESCRIPTION = 'Wrapper around the python-telegram-bot to use in threads'
 
 setup(
     name="fbra-telegram",
     version=VERSION,
     author="Felix Brändli",
```

