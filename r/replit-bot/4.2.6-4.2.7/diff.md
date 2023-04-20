# Comparing `tmp/replit-bot-4.2.6.tar.gz` & `tmp/replit-bot-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.6.tar", max compression
+gzip compressed data, was "replit-bot-4.2.7.tar", max compression
```

## Comparing `replit-bot-4.2.6.tar` & `replit-bot-4.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.6/LICENSE
--rw-r--r--   0        0        0      841 2023-04-17 02:47:20.407000 replit-bot-4.2.6/pyproject.toml
--rw-r--r--   0        0        0    35912 2023-04-17 02:47:30.626973 replit-bot-4.2.6/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50447 2023-04-17 02:47:31.582970 replit-bot-4.2.6/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.6/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.6/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-17 02:47:17.355008 replit-bot-4.2.6/replit_bot/__init__.py
--rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.6/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.6/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.6/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.6/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.6/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.6/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.6/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.6/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.6/replit_bot/queries.js
--rw-r--r--   0        0        0    67496 2023-04-12 02:23:52.651575 replit-bot-4.2.6/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.6/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.6/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.6/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.6/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.6/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.6/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      850 2023-04-17 02:47:33.038161 replit-bot-4.2.6/setup.py
--rw-r--r--   0        0        0      715 2023-04-17 02:47:33.038464 replit-bot-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.7/LICENSE
+-rw-r--r--   0        0        0      822 2023-04-20 20:25:45.473473 replit-bot-4.2.7/pyproject.toml
+-rw-r--r--   0        0        0    35912 2023-04-20 20:25:44.561475 replit-bot-4.2.7/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50447 2023-04-20 20:25:44.953474 replit-bot-4.2.7/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.7/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.7/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-20 20:31:36.644857 replit-bot-4.2.7/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18805 2023-04-17 02:54:25.529892 replit-bot-4.2.7/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.7/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.7/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.7/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      978 2023-04-20 20:25:44.157476 replit-bot-4.2.7/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.7/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.7/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.7/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.7/replit_bot/queries.js
+-rw-r--r--   0        0        0    67496 2023-04-20 20:31:20.332886 replit-bot-4.2.7/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.7/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.7/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.7/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.7/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.7/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.7/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      823 2023-04-20 22:40:33.250252 replit-bot-4.2.7/setup.py
+-rw-r--r--   0        0        0      674 2023-04-20 22:40:33.250832 replit-bot-4.2.7/PKG-INFO
```

### Comparing `replit-bot-4.2.6/LICENSE` & `replit-bot-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/pyproject.toml` & `replit-bot-4.2.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.6"
+version = "4.2.7"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.6.1,<4.0.0"
 # replit db I think I can't remember lol
@@ -19,15 +19,14 @@
 # docs
 # [tool.poetry.group.docs]
 # optional = true
 
 # [tool.poetry.group.docs.dependencies]
 Flask = "^2.2.0"
 waitress = "^2.1.2"
-uvloop = "^0.17.0"
 
 [tool.poetry.dev-dependencies]
 debugpy = "^1.6.2"
 python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.0"}
 toml = "^0.10.2"
 Markdown = "^3.4.1"
```

### Comparing `replit-bot-4.2.6/replit_bot/AsyncBot.py` & `replit-bot-4.2.7/replit_bot/AsyncBot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/AsyncClient.py` & `replit-bot-4.2.7/replit_bot/AsyncClient.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.7/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/LICENSE` & `replit-bot-4.2.7/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/bot.py` & `replit-bot-4.2.7/replit_bot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             "index.html",
             html='<center><div><script authed="location.reload()" src="https://auth.util.repl.co/script.js"></script></div></center>',
         )
     if (
         command in _started_buttons
         and user in _started_buttons[command]
         and rand_chars in _started_buttons[command][user]
-        and _started_buttons[command][user][rand_chars] is None
         and user == request.headers["X-Replit-User-Name"]
     ):
         _started_buttons[command][user][rand_chars] = choice
         return render_template(
             "index.html",
             html="<center><h1>your request has been processed, you can close this tab</h1></center>",
         )
```

### Comparing `replit-bot-4.2.6/replit_bot/client.py` & `replit-bot-4.2.7/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/html_default_templates.py` & `replit-bot-4.2.7/replit_bot/html_default_templates.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/param.py` & `replit-bot-4.2.7/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/post_ql.py` & `replit-bot-4.2.7/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/queries.js` & `replit-bot-4.2.7/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/queries.py` & `replit-bot-4.2.7/replit_bot/queries.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.7/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/replit_bot/utils/lines.py` & `replit-bot-4.2.7/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.6/setup.py` & `replit-bot-4.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 {'': ['*'], 'replit_bot': ['templates/*']}
 
 install_requires = \
 ['Flask>=2.2.0,<3.0.0',
  'pyee>=9.0.4,<10.0.0',
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
- 'uvloop>=0.17.0,<0.18.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.6',
+    'version': '4.2.7',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.6/PKG-INFO` & `replit-bot-4.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.6
+Version: 4.2.7
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
 Requires-Dist: pyee (>=9.0.4,<10.0.0)
 Requires-Dist: replit (>=3.2.4,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: waitress (>=2.1.2,<3.0.0)
```

