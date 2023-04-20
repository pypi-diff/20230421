# Comparing `tmp/discord-qalib-2.0.0.tar.gz` & `tmp/discord-qalib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.0.0.tar", last modified: Sun Apr  2 02:31:38 2023, max compression
+gzip compressed data, was "discord-qalib-2.1.0.tar", last modified: Wed Apr 19 23:05:24 2023, max compression
```

## Comparing `discord-qalib-2.0.0.tar` & `discord-qalib-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:38.619388 discord-qalib-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-02 02:31:38.615388 discord-qalib-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:38.615388 discord-qalib-2.0.0/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-02 02:31:38.000000 discord-qalib-2.0.0/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-02 02:31:38.000000 discord-qalib-2.0.0/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 02:31:38.000000 discord-qalib-2.0.0/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-02 02:31:38.000000 discord-qalib-2.0.0/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-02 02:31:38.000000 discord-qalib-2.0.0/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-02 02:31:28.000000 discord-qalib-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:38.615388 discord-qalib-2.0.0/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-02 02:31:28.000000 discord-qalib-2.0.0/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:38.615388 discord-qalib-2.0.0/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 02:31:38.615388 discord-qalib-2.0.0/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23296 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    26083 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-02 02:31:15.000000 discord-qalib-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 02:31:38.619388 discord-qalib-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-02 02:31:28.000000 discord-qalib-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.011848 discord-qalib-2.1.0/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/setup.py
```

### Comparing `discord-qalib-2.0.0/LICENSE` & `discord-qalib-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.0.0/PKG-INFO` & `discord-qalib-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.0.0
+Version: 2.1.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -107,30 +107,32 @@
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
 
 ```python
 import datetime
+from typing import Literal
 
 import discord
 from discord.ext import commands
 
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
+Messages = Literal["test_key"]
 
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
-async def test(ctx: qalib.QalibContext):
+async def test(ctx: qalib.QalibContext[Messages]):
     callables = {"understood_button": acknowledged}
 
     await ctx.rendered_send("test_key", callables, keywords={
         "todays_date": datetime.datetime.now()
     })
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.0.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -33,16 +33,17 @@
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
 https://discordapp.com     Understood
      ``` using the above xml file, for example, you can create an embed with
-the following code: ```python import datetime import discord from discord.ext
-import commands import qalib from qalib.template_engines import formatter bot =
-commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
-async def acknowledged(interaction: discord.Interaction): await
+the following code: ```python import datetime from typing import Literal import
+discord from discord.ext import commands import qalib from
+qalib.template_engines import formatter bot = commands.AutoShardedBot
+(command_prefix="!", intents=discord.Intents.all()) Messages = Literal
+["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
-test(ctx: qalib.QalibContext): callables = {"understood_button": acknowledged}
-await ctx.rendered_send("test_key", callables, keywords={ "todays_date":
-datetime.datetime.now() }) ```
+test(ctx: qalib.QalibContext[Messages]): callables = {"understood_button":
+acknowledged} await ctx.rendered_send("test_key", callables, keywords=
+{ "todays_date": datetime.datetime.now() }) ```
```

### Comparing `discord-qalib-2.0.0/README.md` & `discord-qalib-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -90,30 +90,32 @@
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
 
 ```python
 import datetime
+from typing import Literal
 
 import discord
 from discord.ext import commands
 
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
+Messages = Literal["test_key"]
 
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
-async def test(ctx: qalib.QalibContext):
+async def test(ctx: qalib.QalibContext[Messages]):
     callables = {"understood_button": acknowledged}
 
     await ctx.rendered_send("test_key", callables, keywords={
         "todays_date": datetime.datetime.now()
     })
 ```
```

#### html2text {}

```diff
@@ -23,16 +23,17 @@
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
 https://discordapp.com     Understood
      ``` using the above xml file, for example, you can create an embed with
-the following code: ```python import datetime import discord from discord.ext
-import commands import qalib from qalib.template_engines import formatter bot =
-commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
-async def acknowledged(interaction: discord.Interaction): await
+the following code: ```python import datetime from typing import Literal import
+discord from discord.ext import commands import qalib from
+qalib.template_engines import formatter bot = commands.AutoShardedBot
+(command_prefix="!", intents=discord.Intents.all()) Messages = Literal
+["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
-test(ctx: qalib.QalibContext): callables = {"understood_button": acknowledged}
-await ctx.rendered_send("test_key", callables, keywords={ "todays_date":
-datetime.datetime.now() }) ```
+test(ctx: qalib.QalibContext[Messages]): callables = {"understood_button":
+acknowledged} await ctx.rendered_send("test_key", callables, keywords=
+{ "todays_date": datetime.datetime.now() }) ```
```

### Comparing `discord-qalib-2.0.0/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.1.0/discord_qalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.0.0
+Version: 2.1.0
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -107,30 +107,32 @@
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
 
 ```python
 import datetime
+from typing import Literal
 
 import discord
 from discord.ext import commands
 
 import qalib
 from qalib.template_engines import formatter
 
 bot = commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
 
+Messages = Literal["test_key"]
 
 async def acknowledged(interaction: discord.Interaction):
     await interaction.response.send_message("Acknowledged", ephemeral=True)
 
 
 @bot.command()
 @qalib.qalib_context(formatter.Formatter(), "templates/test.xml")
-async def test(ctx: qalib.QalibContext):
+async def test(ctx: qalib.QalibContext[Messages]):
     callables = {"understood_button": acknowledged}
 
     await ctx.rendered_send("test_key", callables, keywords={
         "todays_date": datetime.datetime.now()
     })
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.0.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.0 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -33,16 +33,17 @@
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
 https://discordapp.com     Understood
      ``` using the above xml file, for example, you can create an embed with
-the following code: ```python import datetime import discord from discord.ext
-import commands import qalib from qalib.template_engines import formatter bot =
-commands.AutoShardedBot(command_prefix="!", intents=discord.Intents.all())
-async def acknowledged(interaction: discord.Interaction): await
+the following code: ```python import datetime from typing import Literal import
+discord from discord.ext import commands import qalib from
+qalib.template_engines import formatter bot = commands.AutoShardedBot
+(command_prefix="!", intents=discord.Intents.all()) Messages = Literal
+["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
-test(ctx: qalib.QalibContext): callables = {"understood_button": acknowledged}
-await ctx.rendered_send("test_key", callables, keywords={ "todays_date":
-datetime.datetime.now() }) ```
+test(ctx: qalib.QalibContext[Messages]): callables = {"understood_button":
+acknowledged} await ctx.rendered_send("test_key", callables, keywords=
+{ "todays_date": datetime.datetime.now() }) ```
```

### Comparing `discord-qalib-2.0.0/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.1.0/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.0.0/pyproject.toml` & `discord-qalib-2.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
-  { name="YousefEZ", email="syberprojects@gmail.com" },
+    { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.0.0"
+version = "2.1.0"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
+[tool.pylint.messages_control]
+max-line-length = 120
+disable = [
+    "missing-docstring",
+    "too-few-public-methods",
+]
+
+[tool.black]
+line-length = 120
+skip-string-normalization = true
+
+[tool.isort]
+profile = "black"
+combine_as_imports = true
+combine_star = true
+line_length = 120
+
 [tool.poetry.dependencies]
 python = "^3.8"
 mock = "^5.0.0"
 typing-extensions = "^4.4.0"
 discord-py = "^2.1.0"
 emoji = "^2.2.0"
 jinja2 = "^3.1.2"
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = { file = ["requirements.txt"] }
 
 [project.urls]
 "Homepage" = "https://github.com/YousefEZ/discord-qalib"
 "Bug Tracker" = "https://github.com/YousefEZ/discord-qalib/issues"
```

### Comparing `discord-qalib-2.0.0/qalib/context.py` & `discord-qalib-2.1.0/qalib/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Any, Optional, Dict
+from typing import Any, Dict, Generic, Optional
 
 import discord.ext.commands
 import discord.message
 
 from qalib.renderer import Renderer
-from qalib.translators import Message, Callback
+from qalib.translators import Callback, Message
+from qalib.translators.parser import K
 
 
-class QalibContext(discord.ext.commands.Context):
+class QalibContext(discord.ext.commands.context.Context, Generic[K]):
     """QalibContext object is responsible for handling messages that are to be sent to the client."""
 
-    def __init__(self, ctx: discord.ext.commands.context, renderer: Renderer):
+    def __init__(self, ctx: discord.ext.commands.context.Context, renderer: Renderer[K]):
         """Constructor for the QalibContext object
 
         Args:
             ctx (commands.context): context object that is passed to the command
             renderer (RendererProxy): renderer object that is used to render the embeds and views
         """
         super().__init__(
@@ -28,15 +29,15 @@
             invoked_with=ctx.invoked_with,
             invoked_parents=ctx.invoked_parents,
             invoked_subcommand=ctx.invoked_subcommand,
             subcommand_passed=ctx.subcommand_passed,
             command_failed=ctx.command_failed,
             current_parameter=ctx.current_parameter,
             current_argument=ctx.current_argument,
-            interaction=ctx.interaction
+            interaction=ctx.interaction,
         )
         self._renderer = renderer
         self._displayed: Optional[discord.message.Message] = None
 
     def verify(self, message: discord.message.Message) -> bool:
         """Method verifies if the content of the message is in the contents
 
@@ -46,105 +47,103 @@
         Returns:
             bool: true of false that indicates whether the data is valid.
         """
         return message.author == self.message.author and message.channel == self.message.channel
 
     async def get_message(self) -> Optional[str]:
         """This method waits for a message to be sent by the user"""
-        confirm: Optional[discord.message.Message] = await self.bot.wait_for('message',
-                                                                             timeout=59.0,
-                                                                             check=self.verify)
+        confirm: Optional[discord.message.Message] = await self.bot.wait_for("message", timeout=59.0, check=self.verify)
         return confirm.content if confirm is not None else None
 
     def _render(
-            self,
-            identifier: str,
-            callables: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180
+        self,
+        identifier: K,
+        callables: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        timeout: int = 180,
     ) -> Message:
         """This method renders the embed and the view based on the identifier string given.
 
         Args:
-            identifier (str): identifies the embed in the route file
+            identifier (K): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]): item callbacks
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             timeout (Optional[int]): timeout for the view
 
         Returns (Display): tuple of the embed and the view
         """
         return self._renderer.render(identifier, callables, keywords, timeout=timeout)
 
     async def rendered_send(
-            self,
-            identifier: str,
-            callables: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180,
-            **kwargs
+        self,
+        identifier: K,
+        callables: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        timeout: int = 180,
+        **kwargs,
     ) -> discord.message.Message:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
+            timeout (int): timeout for the view
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
         message = self._render(identifier, callables, keywords, timeout)
-        return await self.send(**{**message, **kwargs})
+        return await self.send(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def display(
-            self,
-            key: str,
-            callables: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180,
-            **kwargs
+        self,
+        key: K,
+        callables: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        timeout: int = 180,
+        **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
             key (str): identifies the embed in the route file
             callables: callable coroutines that are called when the user interacts with the message
             keywords: keywords that are passed to the embed renderer to format the text
-            timeout (Optional[int]): timeout for the view
+            timeout (int): timeout for the view
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
         message = self._render(key, callables, keywords, timeout)
-        await self._display(**{**message, **kwargs})
+        await self._display(**{**message.convert_to_context_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
         """This method is responsible for sending the message to the client and keeping track of the message object.
 
         Args:
             **kwargs (Dict[str, Any]): kwargs that are passed to the context's send method
         """
         if self._displayed is None:
             self._displayed = await self.send(**kwargs)
         else:
             await self._displayed.edit(**kwargs)
 
     async def menu(
-            self,
-            key: str,
-            callbacks: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            **kwargs
+        self,
+        key: K,
+        callbacks: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        **kwargs,
     ) -> None:
         """This method is used to create a menu for the user to select from.
 
         Args:
-            key (str): identifies the menu in the template file
+            key (K): identifies the menu in the template file
             callbacks (Dict[str, Callback]): callbacks that are called when the user interacts with the menu
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             **kwargs: kwargs that are passed to the context's send method
         """
         display = self._renderer.render_menu(key, callbacks=callbacks, keywords=keywords, **kwargs)
-        await self._display(**{**display, **kwargs})
+        await self._display(**{**display.convert_to_context_message().dict(), **kwargs})
```

### Comparing `discord-qalib-2.0.0/qalib/interaction.py` & `discord-qalib-2.1.0/qalib/interaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,148 +1,180 @@
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Generic, Optional, cast
 
 import discord
+from discord.interactions import InteractionResponse
 
 from qalib.renderer import Renderer
 from qalib.translators import Callback, Message
+from qalib.translators.parser import K
 
+if TYPE_CHECKING:
+    from discord.types.interactions import Interaction as InteractionPayload
 
-class QalibInteraction(discord.Interaction):
+
+def create_interaction_payload(interaction: discord.Interaction) -> Dict[str, Any]:
+    # pylint: disable=protected-access
+    # noinspection PyProtectedMember
+    return {
+        "id": interaction.id,
+        "type": int(interaction.type.value),
+        "data": interaction.data,
+        "token": interaction.token,
+        "version": interaction.version,
+        "channel_id": interaction.channel_id,
+        "guild_id": interaction.guild_id,
+        "application_id": interaction.application_id,
+        "locale": interaction.locale,
+        "guild_locale": interaction.guild_locale,
+        "app_permissions": interaction._app_permissions,
+    }
+
+
+class QalibInteraction(discord.Interaction, Generic[K]):
     """The QalibInteraction class is a subclass of discord.Interaction, and is used to add additional functionality to
     the interaction. It is meant to be used in the on_interaction event, and is responsible for deserializing the
     requested modal and sending it to the user."""
 
-    def __init__(self, interaction: discord.Interaction, renderer: Renderer):
+    def __init__(self, interaction: discord.Interaction, renderer: Renderer[K]):
         """Constructor method for the QalibInteraction class."""
-        super().__init__(data={
-            'id': interaction.id,
-            'type': interaction.type,
-            'data': interaction.data,
-            'token': interaction.token,
-            'version': interaction.version,
-            'channel_id': interaction.channel_id,
-            'guild_id': interaction.guild_id,
-            'application_id': interaction.application_id,
-            'locale': interaction.locale,
-            'guild_locale': interaction.guild_locale,
-            'app_permissions': interaction._app_permissions,
-        }, state=interaction._state)
+        data = create_interaction_payload(interaction)
+        if TYPE_CHECKING:
+            super().__init__(
+                data=(cast(InteractionPayload, data)),
+                state=interaction._state,
+            )
+        else:
+            super().__init__(
+                data=data,
+                state=interaction._state,
+            )
         self.message = interaction.message
         self.user = interaction.user
         self._renderer = renderer
         self._displayed = False
 
     async def respond_with_modal(
             self,
-            key: str,
+            key: K,
             methods: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None) -> None:
+            keywords: Optional[Dict[str, Any]] = None,
+    ) -> None:
         """Method that is responsible for templating the document, and then deserializing the requested modal based on
         its key and sending it to the user.
 
         Args:
             methods (Dict[str, Callback]): methods that are used to override the default methods of the modal
             key (str): key that identifies the modal in the route file
             keywords (Any): keywords that are passed to the modal renderer to format the text
         """
         if methods is None:
             methods = {}
 
         if keywords is None:
             keywords = {}
-        return await self.response.send_modal(self._renderer.render_modal(key, methods, keywords))
+
+        assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
+        # pylint: disable= no-member
+        modal = self._renderer.render_modal(key, methods, keywords)
+        return await self.response.send_modal(modal)  # pyright: ignore [reportGeneralTypeIssues]
 
     def _render(
             self,
-            identifier: str,
+            identifier: K,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180
+            timeout: int = 180,
     ) -> Message:
         """This method renders the embed and the view based on the identifier string given.
 
         Args:
-            identifier (str): identifies the embed in the route file
+            identifier (K): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]): item callbacks
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             timeout (Optional[int]): timeout for the view
 
         Returns (Display): tuple of the embed and the view
         """
         return self._renderer.render(identifier, callables, keywords, timeout=timeout)
 
     async def rendered_send(
             self,
-            identifier: str,
+            identifier: K,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180,
-            **kwargs
-    ) -> discord.message.Message:
+            timeout: int = 180,
+            **kwargs,
+    ) -> None:
         """Methods that is fires a message to the client and returns the message object. Doesn't save/keep track of the
         message.
 
         Args:
             identifier (str): identifies the embed in the route file
             callables (Optional[Dict[str, Callback]]) : functions that are hooked to components
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             timeout (Optional[int]): timeout for the view
             **kwargs: kwargs that are passed to the context's send method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        display = self._render(identifier, callables, keywords, timeout)
-        return await self.response.send_message(**{**display, **kwargs})
+        message = self._render(identifier, callables, keywords, timeout)
+
+        assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
+        # pylint: disable= no-member
+        message_info = {**message.convert_to_interaction_message().dict(), **kwargs}
+        return await self.response.send_message(**message_info)  # pyright: ignore [reportGeneralTypeIssues]
 
     async def display(
             self,
-            key: str,
+            key: K,
             callables: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180,
-            **kwargs
+            timeout: int = 180,
+            **kwargs,
     ) -> None:
         """this is the main function that we use to send one message, and one message only. However, edits to that
         message can take place.
 
         Args:
-            key (str): identifies the embed in the route file
+            key (K): identifies the message in the template file
             callables: callable coroutines that are called when the user interacts with the message
             keywords: keywords that are passed to the embed renderer to format the text
             timeout (Optional[int]): timeout for the view
             **kwargs: kwargs that are passed to the context send method or the message edit method
 
         Returns (discord.message.Message): Message object that got sent to the client.
         """
-        display = self._render(key, callables, keywords, timeout)
-        await self._display(**{**display, **kwargs})
+        message = self._render(key, callables, keywords, timeout)
+        await self._display(**{**message.convert_to_interaction_message().dict(), **kwargs})
 
     async def _display(self, **kwargs: Any) -> None:
         """This method is responsible for sending the message to the client, and editing the message if there is one
         that has already been sent.
 
         Args:
             **kwargs (Dict[str, Any]): kwargs that are passed to the context's send method
         """
         if self._displayed:
             await self.edit_original_response(**kwargs)
         else:
-            await self.response.send_message(**kwargs)
+            assert isinstance(self.response, InteractionResponse)  # pyright: ignore [reportGeneralTypeIssues]
+            # pylint: disable= no-member
+            await self.response.send_message(**kwargs)  # pyright: ignore [reportGeneralTypeIssues]
             self._displayed = True
 
     async def menu(
             self,
-            key: str,
+            key: K,
             callbacks: Optional[Dict[str, Callback]] = None,
             keywords: Optional[Dict[str, Any]] = None,
-            **kwargs
+            **kwargs,
     ) -> None:
         """This method is used to create a menu for the user to select from.
 
         Args:
-            key (str): identifies the menu in the template file
+            key (K): identifies the menu in the template file
             callbacks (Dict[str, Callback]): callbacks that are called when the user interacts with the menu
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
             **kwargs: kwargs that are passed to the context's send method
         """
-        display = self._renderer.render_menu(key, callbacks=callbacks, keywords=keywords, **kwargs)
-        await self._display(**{**display, **kwargs})
+        message = self._renderer.render_menu(key, callbacks=callbacks, keywords=keywords, **kwargs)
+        await self._display(**{**message.convert_to_interaction_message().dict(), **kwargs})
```

### Comparing `discord-qalib-2.0.0/qalib/renderer.py` & `discord-qalib-2.1.0/qalib/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,101 @@
 from enum import Enum, auto
-from typing import Optional, Any, Dict, List
+from typing import Any, Dict, Generic, List, Optional, cast
 
 import discord.ui
-from discord.enums import ButtonStyle
 
 from qalib.template_engines.template_engine import TemplateEngine
-from qalib.translators import Message, Callback, MISSING
-from qalib.translators.factory import ParserFactory, DeserializerFactory
-from qalib.translators.parser import Parser
+from qalib.translators import Callback, Message
+from qalib.translators.factory import DeserializerFactory, ParserFactory
+from qalib.translators.message_parsing import ButtonComponent, create_button
+from qalib.translators.parser import K, Parser
 
 
 class RenderingOptions(Enum):
     """Options for the renderer."""
+
     PRE_TEMPLATE = auto()
 
 
-def create_arrows(left: Optional[Message], right: Optional[Message], **kwargs) -> List[discord.ui.Button]:
+def create_arrows(left: Optional[Message] = None, right: Optional[Message] = None, **kwargs) -> List[discord.ui.Button]:
     """This function creates the arrow buttons that are used to navigate between the pages.
 
     Args:
         left (Optional[Message]): embed and view of the left page
         right (Optional[Display]): embed and view of the right page
 
     Returns (List[discord.ui.Button]): list of the arrow buttons
     """
 
-    def view(display: Message):
-        async def callback(interaction):
-            await interaction.response.edit_message(embed=display.embed, view=display.view, **kwargs)
+    def view(message: Message) -> Callback:
+        async def callback(interaction: discord.Interaction):
+            await interaction.response.edit_message(**{**message.dict(), **kwargs})
 
         return callback
 
-    buttons = []
+    buttons: List[discord.ui.Button] = []
 
     def construct_button(display: Optional[Message], emoji: str):
         if display is None:
             return
-        buttons.append(discord.ui.Button(style=ButtonStyle.grey, emoji=emoji))
-        buttons[-1].callback = view(display)
+        button: ButtonComponent = {"emoji": emoji, "style": "primary", "callback": view(display)}
+        buttons.append(create_button(button))
 
     construct_button(left, "⬅️")
     construct_button(right, "➡️")
 
     return buttons
 
 
-class Renderer:
+class Renderer(Generic[K]):
     """This object is responsible for rendering the embeds, views, and menus, by first using the templating engine to
-    template the document, and then using the deserializer to deserialize the document into embeds and views."""
+    template the document, and then using the deserializer to deserialize the document into embeds and views.
+    """
 
     __slots__ = ("_template_engine", "_parser", "_filename", "_deserializer")
 
-    def __init__(
-            self,
-            template_engine: TemplateEngine,
-            filename: str,
-            *rendering_options
-    ):
+    def __init__(self, template_engine: TemplateEngine, filename: str, *rendering_options: RenderingOptions):
         self._template_engine = template_engine
-        self._parser: Optional[Parser] = None
+        self._parser: Optional[Parser[K]] = None
         if RenderingOptions.PRE_TEMPLATE not in rendering_options:
-            self._parser = ParserFactory.get_parser(filename)
+            self._parser = cast(Parser[K], ParserFactory.get_parser(filename))
         self._filename = filename
         self._deserializer = DeserializerFactory.get_deserializer(filename)
 
-    def _pre_template(self, keywords: Dict[str, Any]) -> Parser:
+    def _pre_template(self, keywords: Dict[str, Any]) -> Parser[K]:
         """Pre-Template templates the document before further processing. It returns a Parser instance that contains
         the data that is used to render the embeds and views.
 
         Args:
             keywords (Dict[str, Any]): keywords that are passed to the templating engine to template the document.
 
         Returns (Parser): Parser instance that contains the data that is used to render the embeds and views.
         """
         if self._parser is None:
-            with open(self._filename, "r") as file:
-                return ParserFactory.get_parser(self._filename,
-                                                source=self._template_engine.template(file.read(), keywords))
+            with open(self._filename, "r", encoding="utf-8") as file:
+                return cast(
+                    Parser[K],
+                    ParserFactory.get_parser(
+                        self._filename,
+                        source=self._template_engine.template(file.read(), keywords),
+                    ),
+                )
         return self._parser
 
     def render(
-            self,
-            key: str,
-            callbacks: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: int = 180
+        self,
+        key: K,
+        callbacks: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        timeout: int = 180,
     ) -> Message:
         """This method is used to render an embed and a view, and places it in a NamedTuple
 
         Args:
-            key (str): key of the embed,
+            key (K): key of the embed,
             callbacks (Optional[Dict[str, Callable]]): callbacks that are attached to the components of the view,
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text,
             timeout (int): timeout of the view
 
         Returns (Display): embed and view that can be sent for display.
         """
         if callbacks is None:
@@ -103,25 +105,25 @@
             keywords = {}
 
         embed = self._pre_template(keywords).template_message(key, self._template_engine, keywords)
 
         return self._deserializer.deserialize_into_message(embed, callbacks, timeout=timeout)
 
     def render_menu(
-            self,
-            key: str,
-            callbacks: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None,
-            timeout: Optional[int] = 180,
-            **kwargs
+        self,
+        key: K,
+        callbacks: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
+        timeout: Optional[int] = 180,
+        **kwargs,
     ) -> Message:
         """This method is used to create a menu for the user to select from.
 
         Args:
-            key (str): key of the menu
+            key (K): key of the menu
             callbacks (Optional[Dict[str, Callable]]): callbacks that are attached to the components of the view
             timeout (Optional[int]): timeout of the view
             keywords (Dict[str, Any]): keywords that are passed to the embed renderer to format the text
 
         Returns (Display): Returns the NamedTuple Display, which contains the embed and the view that has arrow buttons
         that edit the embed and view
         """
@@ -134,25 +136,26 @@
         menu = self._pre_template(keywords).template_menu(key, self._template_engine, keywords)
         messages = self._deserializer.deserialize_into_menu(menu, callbacks, timeout=timeout)
 
         for i, message in enumerate(messages):
             arrow_left = messages[i - 1] if i > 0 else None
             arrow_right = messages[i + 1] if i + 1 < len(messages) else None
 
-            message.view = discord.ui.View(timeout=timeout) if message.view is MISSING else message.view
+            view = discord.ui.View(timeout=timeout) if message.view is None else message.view
             for arrow in create_arrows(arrow_left, arrow_right, **kwargs):
-                message.view.add_item(arrow)
+                view.add_item(arrow)
+            message.view = view
 
         return messages[0]
 
     def render_modal(
-            self,
-            key: str,
-            methods: Optional[Dict[str, Callback]] = None,
-            keywords: Optional[Dict[str, Any]] = None
+        self,
+        key: K,
+        methods: Optional[Dict[str, Callback]] = None,
+        keywords: Optional[Dict[str, Any]] = None,
     ) -> discord.ui.Modal:
         if methods is None:
             methods = {}
 
         if keywords is None:
             keywords = {}
```

### Comparing `discord-qalib-2.0.0/qalib/template_engines/formatter.py` & `discord-qalib-2.1.0/qalib/template_engines/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,32 @@
     def __init__(self, key):
         self.key = key
 
     def __format__(self, spec):
         return f"{{{self.key}:{spec}}}" if spec else f"{{{self.key}}}"
 
     def __getitem__(self, index):
-        self.key = "{}[{}]".format(self.key, index)
+        self.key = f"{self.key}[{index}]"
         return self
 
     def __getattr__(self, attr):
-        self.key = "{}.{}".format(self.key, attr)
+        self.key = f"{self.key}.{attr}"
         return self
 
 
 class FormatDict(dict):
     """This class is used to format a string using the format method, and will use the FormatPlaceholder class to
-    handle missing keys, so that if they do not raise a KeyError, and are not removed."""
+    handle missing keys, so that if they do not raise a KeyError, and are not removed.
+    """
 
     def __missing__(self, key):
         return FormatPlaceholder(key)
 
 
 class Formatter(TemplateEngine):
-
     def template(self, document: str, keywords: Dict[str, Any]) -> str:
         """This method is used to format a string using the format method.
 
         Parameters:
             document (str): string that is formatted
             keywords (Dict[str, Any]): keywords that are used to format the string
```

### Comparing `discord-qalib-2.0.0/qalib/template_engines/jinja2.py` & `discord-qalib-2.1.0/qalib/template_engines/jinja2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Dict, Any
+from typing import Any, Dict
 
-from jinja2 import Environment, BaseLoader
+from jinja2 import BaseLoader, Environment
 
 from qalib.template_engines.template_engine import TemplateEngine
 
 
 class Jinja2(TemplateEngine):
-
     def template(self, document: str, keywords: Dict[str, Any]) -> str:
         """This method is used to format a string using the format method.
 
         Parameters:
             document (str): string that is formatted
             keywords (Dict[str, Any]): keywords that are used to format the string
```

### Comparing `discord-qalib-2.0.0/qalib/translators/deserializer.py` & `discord-qalib-2.1.0/qalib/translators/deserializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-from typing import Protocol, Dict, List, Any
+from typing import Any, Dict, List, Protocol
 
 import discord.ui
 
-from qalib.translators import Message, Callback
+from qalib.translators import Callback, Message
 
 
 class Deserializer(Protocol):
     """Protocol that represents the deserializer. It is meant to be placed into a Renderer, and is responsible for
     deserializing the document into embeds and views."""
 
     def deserialize_into_message(self, source: str, callables: Dict[str, Callback], **kw: Any) -> Message:
@@ -17,33 +17,33 @@
         Parameters:
             source (str): document that is deserialized
             callables (Dict[str, Callback]): callables that are used to deserialize the document
             **kw (Any: additional arguments that are used to deserialize the document
 
         Returns (Display): NamedTuple containing the embed and view.
         """
-        ...
+        raise NotImplementedError
 
     def deserialize_into_menu(self, source: str, callables: Dict[str, Callback], **kw: Any) -> List[Message]:
         """This method is used to deserialize a document into a list of NamedTuple Displays, that are connected by
         arrows in their views.
 
         Args:
             source (str): document that is deserialized
             callables (Dict[str, Callback]): callables that are used to deserialize the document
             **kw (Any): additional arguments that are used to deserialize the document
 
         Returns (List[Display]): list of NamedTuple Displays, that are connected by arrows in their views.
         """
-        ...
+        raise NotImplementedError
 
     def deserialize_into_modal(self, source: str, methods: Dict[str, Callback], **kw: Any) -> discord.ui.Modal:
         """This method is used to deserialize a document into a modal.
 
         Args:
             source (str): document that is deserialized
             methods (Dict[str, Callback]): methods that are used to deserialize the document
             **kw (Any): additional arguments that are used to deserialize the document
 
         Returns (discord.ui.Modal): modal that is deserialized from the document.
         """
-        ...
+        raise NotImplementedError
```

### Comparing `discord-qalib-2.0.0/qalib/translators/factory.py` & `discord-qalib-2.1.0/qalib/translators/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from typing import Type, Optional
+from typing import Any, Optional, Type, cast
 
 from .deserializer import Deserializer
-from .json import JSONParser, JSONDeserializer
+from .json import JSONDeserializer, JSONParser
 from .parser import Parser
-from .xml import XMLParser, XMLDeserializer
+from .xml import XMLDeserializer, XMLParser
 
 
 class ParserFactory:
     """Factory class for creating Parsers"""
 
     parsers = {".xml": XMLParser, ".json": JSONParser}
 
     @staticmethod
-    def get_parser_type(path: str) -> Type[Parser]:
+    def get_parser_type(path: str) -> Type[Parser[str]]:
         """Returns the parser type based on the file extension of the path.
 
         Args:
             path (str): path of the file that is parsed
 
         Returns (Type[Parser]): parser type that is used to parse the file
         """
         for extension, parser_type in ParserFactory.parsers.items():
             if path.endswith(extension):
-                return parser_type
+                return cast(Type[Parser[Any]], parser_type)
 
         raise ValueError("No parser found for the given file")
 
     @staticmethod
-    def get_parser(path: str, *, source: Optional[str] = None) -> Parser:
+    def get_parser(path: str, *, source: Optional[str] = None) -> Parser[str]:
         """Returns an instantiated Parser based on the file extension of the path using either the source contents or
         the path.
 
         Args:
             path (str): path of the file that is parsed
             source (Optional[str]): source contents that are parsed
 
         Returns (Parser): parser that is used to parse the file
         """
         parser = ParserFactory.get_parser_type(path)
         if source is not None:
             return parser(source=source)
-        with open(path, encoding="utf8", mode="r") as f:
-            return parser(source=f.read())
+        with open(path, encoding="utf8", mode="r") as file:
+            return parser(source=file.read())
 
 
 class DeserializerFactory:
     """Factory class for creating Deserializers"""
 
     deserializers = {".xml": XMLDeserializer, ".json": JSONDeserializer}
```

### Comparing `discord-qalib-2.0.0/qalib/translators/json.py` & `discord-qalib-2.1.0/qalib/translators/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,154 +1,341 @@
 from __future__ import annotations
 
 import json
 from copy import deepcopy
 from datetime import datetime
 from functools import partial
-from typing import Dict, List, Optional, Any, Union, cast, Type, Sequence
+from typing import Any, Callable, Dict, List, Literal, Optional, Type, TypedDict, TypeVar, Union, cast
 
 import discord
 import discord.types.embed
-import discord.ui as ui
-from discord import MessageReference
+from discord import ui
 from discord.abc import Snowflake
+from typing_extensions import NotRequired
 
-from qalib.translators import Callback, Message, MISSING, DiscordIdentifier
-from qalib.translators.deserializer import Deserializer
-from qalib.translators.parser import Parser
-from qalib.translators.message_parsing import *
 from qalib.template_engines.template_engine import TemplateEngine
+from qalib.translators import Callback, DiscordIdentifier, Message
+from qalib.translators.deserializer import Deserializer
+from qalib.translators.message_parsing import (
+    ButtonComponent,
+    ButtonStyle,
+    ChannelType,
+    CustomSelects,
+    Emoji,
+    create_button,
+    create_channel_select,
+    create_select,
+    create_text_input,
+    create_type_select,
+    make_channel_types,
+    make_colour,
+    make_emoji,
+    Field,
+    Footer,
+    Author,
+    TextInputRaw,
+    TextInputComponent,
+)
+from qalib.translators.parser import K, Parser
+
+OBJ = TypeVar("OBJ")
+
+ComponentTypes = Literal[
+    "button",
+    "select",
+    "channel_select",
+    "role_select",
+    "user_select",
+    "mentionable_select",
+    "text_input",
+]
+
+
+class Option(TypedDict):
+    """This class is used to represent the blueprint of a select menu option."""
+
+    label: str
+    value: str
+    description: str
+    emoji: NotRequired[Emoji]
+    default: bool
+
+
+class Component(TypedDict):
+    type: ComponentTypes
+
+
+class Button(Component):
+    """This class is used to represent the blueprint of a button."""
+
+    custom_id: NotRequired[str]
+    label: NotRequired[str]
+    style: NotRequired[ButtonStyle]
+    emoji: NotRequired[Emoji]
+    url: NotRequired[str]
+    disabled: NotRequired[bool]
+    row: NotRequired[int]
+
+
+class Select(Component):
+    """This class is used to represent the blueprint of a select menu."""
+
+    custom_id: NotRequired[str]
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    options: NotRequired[List[Option]]
+    row: NotRequired[int]
+
+
+class CustomSelect(Component):
+    """This class is used to represent the blueprint of a mentionable select menu."""
+
+    custom_id: NotRequired[str]
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    options: NotRequired[List[Option]]
+    row: NotRequired[int]
+
+
+class ChannelSelect(Component):
+    """This class is used to represent the blueprint of a channel select menu."""
+
+    custom_id: NotRequired[str]
+    channel_types: NotRequired[List[ChannelType]]
+    placeholder: NotRequired[str]
+    min_values: NotRequired[int]
+    max_values: NotRequired[int]
+    options: NotRequired[List[Option]]
+    row: NotRequired[int]
+
+
+class TextInput(TextInputRaw):
+    type: ComponentTypes
+
+
+Components = Union[Button, Select, CustomSelect, ChannelSelect, TextInput]
+
+
+class Timestamp(TypedDict):
+    """This class is used to represent object's timestamp."""
+
+    date: str
+    format: NotRequired[str]
+
 
+class Embed(TypedDict):
+    """This class is used to represent the blueprint of an embed."""
 
-class JSONParser(Parser):
+    title: str
+    colour: NotRequired[str]
+    color: NotRequired[str]
+    fields: List[Field]
+    description: NotRequired[str]
+    type: NotRequired[discord.types.embed.EmbedType]
+    url: NotRequired[str]
+    timestamp: NotRequired[Timestamp]
+    footer: NotRequired[Footer]
+    image: NotRequired[str]
+    thumbnail: NotRequired[str]
+    author: NotRequired[Author]
+
+
+class File(TypedDict):
+    """This class is used to represent the blueprint of a file."""
+
+    filename: str
+    spoiler: NotRequired[bool]
+    description: NotRequired[str]
+
+
+class AllowedMentions(TypedDict):
+    """This class is used to represent the blueprint of allowed mentions."""
+
+    everyone: NotRequired[bool]
+    users: NotRequired[Union[bool, List[int]]]
+    roles: NotRequired[Union[bool, List[int]]]
+    replied_user: NotRequired[bool]
+
+
+class MessageReference(TypedDict):
+    """This class is used to represent the blueprint of a message reference."""
+
+    message_id: int
+    channel_id: int
+    guild_id: NotRequired[int]
+
+
+View = Dict[str, Components]
+
+
+class JSONMessage(TypedDict):
+    """This class is used to represent the blueprint of a message."""
+
+    embed: NotRequired[Embed]
+    embeds: NotRequired[List[Embed]]
+    view: NotRequired[View]
+    content: NotRequired[str]
+    tts: NotRequired[bool]
+    nonce: NotRequired[int]
+    delete_after: NotRequired[float]
+    suppress_embeds: NotRequired[bool]
+    file: NotRequired[File]
+    files: NotRequired[List[File]]
+    allowed_mentions: NotRequired[AllowedMentions]
+    message_reference: NotRequired[MessageReference]
+    mention_author: NotRequired[bool]
+    silent: NotRequired[bool]
+
+
+JSONMenu = Dict[str, JSONMessage]
+
+
+class JSONModal(TypedDict):
+    title: str
+    components: Dict[str, Components]
+
+
+Template = Dict[str, Union[JSONMessage, JSONMenu, JSONModal]]
+
+
+class JSONParser(Parser[K]):
     """This method is used to parse the document into a menu and a list of callables for .json files"""
 
     __slots__ = ("_data",)
 
     def __init__(self, source: str):
         """This method is used to initialize the parser by parsing the source text.
 
         Args:
             source (str): source text that is parsed
         """
         self._data = json.loads(source)
 
-    def recursive_template(self, obj: Any, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> Dict[str, Any]:
+    def recursive_template(self, obj: OBJ, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> OBJ:
         """Method that is used to recursively template the object using the templater and the keywords.
 
         Args:
-            obj (Any): object that is templated
+            obj (Dict | List | str | Any): object that is templated
             template_engine (TemplateEngine): template engine that is used to template the object
             keywords (Dict[str, Any]): keywords that are used to template the object
 
         Returns (Dict[str, Any]): templated object
         """
         if isinstance(obj, dict):
             for key in obj:
                 obj[key] = self.recursive_template(obj[key], template_engine, keywords)
         elif isinstance(obj, list):
-            for i in range(len(obj)):
-                obj[i] = self.recursive_template(obj[i], template_engine, keywords)
+            for i, value in enumerate(obj):
+                obj[i] = self.recursive_template(value, template_engine, keywords)
         elif isinstance(obj, str):
-            obj = template_engine.template(obj, keywords)
+            return cast(OBJ, template_engine.template(obj, keywords))
 
         return obj
 
-    def template_message(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_message(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template the embed by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
-            key (str): key of the embed
+            key (K): key of the embed
             template_engine (TemplateEngine): template engine that is used to template the embed
             keywords (Dict[str, Any]): keywords that are used to template the embed
 
         Returns (str): templated embed in the form of string.
         """
         return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
 
-    def template_menu(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_menu(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """Method that is used to template the menu by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
-            key (str): key of the menu
+            key (K): key of the menu
             template_engine (TemplateEngine): template engine that is used to template the menu
             keywords (Dict[str, Any]): keywords that are used to template the menu
 
         Returns (str): templated menu in the form of string.
         """
         return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
 
-    def template_modal(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_modal(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """Method that is used to template the modal by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
-            key (str): key of the modal
+            key (K): key of the modal
             template_engine (TemplateEngine): template engine that is used to template the modal
             keywords (Dict[str, Any]): keywords that are used to template the modal
 
         Returns (str): templated modal in the form of string.
         """
         return json.dumps(self.recursive_template(deepcopy(self._data[key]), template_engine, keywords))
 
 
 class JSONDeserializer(Deserializer):
-
     def deserialize_into_message(self, source: str, callables: Dict[str, Callback], **kw) -> Message:
         """Method to deserialize a source into a Display object
 
         Args:
             source (str): The source text to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
             **kw: Additional keyword arguments
 
         Returns (Display): A Display object
         """
         return self.deserialize_message(json.loads(source), callables, kw)
 
+    # pylint: disable= too-many-locals
     def deserialize_message(
-            self,
-            message_tree: Dict[str, Any],
-            callables: Dict[str, Callback],
-            kw: Dict[str, Any]
+        self,
+        message_tree: JSONMessage,
+        callables: Dict[str, Callback],
+        kwargs: Dict[str, Any],
     ) -> Message:
         """Method to deserialize an embed into a Display NamedTuple containing the embed and the view
 
         Args:
             message_tree (Dict[str, Any]): The embed to deserialize
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kw (Dict[str, Any]): A dictionary containing the attributes to use for the view
+            kwargs (Dict[str, Any]): A dictionary containing the attributes to use for the view
 
         Returns (Display): A Display NamedTuple containing the embed and the view
         """
         view_tree = message_tree.get("view")
-        embed = self.render(embed_tree) if (embed_tree := message_tree.get("embed")) is not None else MISSING
-        view = MISSING if view_tree is None else self._render_view(view_tree, callables, kw)
+        embed = self.render(embed_tree) if (embed_tree := message_tree.get("embed")) is not None else None
+        view = None if view_tree is None else self._render_view(view_tree, callables, kwargs)
         return Message(
             embed=embed,
-            embeds=MISSING if (embeds := message_tree.get("embeds")) is None else list(
-                map(self.render, embeds.values())),
-            content=message_tree.get("content", MISSING),
-            tts=MISSING if (tts_element := message_tree.get("tts")) is None else (
-                    (type(tts_element) == bool and tts_element) or str(tts_element).lower() == "true"),
-            nonce=MISSING if (nonce_element := message_tree.get("nonce")) is None else int(nonce_element),
-            delete_after=MISSING if (delete_after := message_tree.get("delete_after")) is None else float(delete_after),
-            suppress_embeds=MISSING if (suppress := message_tree.get("supress_embeds")) is None else suppress,
-            file=MISSING if (file := message_tree.get("file")) is None else self._render_file(file),
-            files=MISSING if (files := message_tree.get("files")) is None else list(
-                map(self._render_file, files)),
-            allowed_mentions=MISSING if (allowed_mentions := message_tree.get(
-                "allowed_mentions")) is None else self._render_allowed_mentions(allowed_mentions),
-            reference=MISSING if (reference := message_tree.get("reference")) is None else MessageReference(
-                message_id=reference["message_id"], channel_id=reference["channel_id"],
-                guild_id=reference.get("guild_id")),
-            mention_author=MISSING if (mention := message_tree.get("mention_author")) is None else mention,
-            view=view
+            embeds=None if (embeds := message_tree.get("embeds")) is None else list(map(self.render, embeds)),
+            content=message_tree.get("content", None),
+            tts=None
+            if (tts_element := message_tree.get("tts")) is None
+            else ((isinstance(tts_element, bool) and tts_element) or str(tts_element).lower() == "true"),
+            nonce=None if (nonce_element := message_tree.get("nonce")) is None else int(nonce_element),
+            delete_after=None if (delete_after := message_tree.get("delete_after")) is None else float(delete_after),
+            suppress_embeds=None if (suppress := message_tree.get("suppress_embeds")) is None else suppress,
+            file=None if (file := message_tree.get("file")) is None else self._render_file(file),
+            files=None if (files := message_tree.get("files")) is None else list(map(self._render_file, files)),
+            allowed_mentions=None
+            if (allowed_mentions := message_tree.get("allowed_mentions")) is None
+            else self._render_allowed_mentions(allowed_mentions),
+            reference=None
+            if (reference := message_tree.get("message_reference")) is None
+            else discord.MessageReference(
+                message_id=reference["message_id"],
+                channel_id=reference["channel_id"],
+                guild_id=reference.get("guild_id"),
+            ),
+            mention_author=message_tree.get("mention_author"),
+            view=view,
+            stickers=None,
+            ephemeral=None,
+            silent=message_tree.get("silent")
         )
 
     def deserialize_into_menu(self, source: str, callables: Dict[str, Callback], **kw) -> List[Message]:
         """Method to deserialize a menu into a list of Display objects
 
         Args:
             source (str): The source text to deserialize int a Menu
@@ -168,384 +355,269 @@
             **kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
         modal_tree = json.loads(source)
         return self._render_modal(modal_tree, methods, kw)
 
-    def _render_modal(self, tree: Dict[str, Any], methods: Dict[str, Callback], kw: Dict[str, Any]) -> discord.ui.Modal:
+    def _render_modal(self, tree: JSONModal, methods: Dict[str, Callback], kwargs: Dict[str, Any]) -> discord.ui.Modal:
         """Method to render a modal from a modal tree
 
         Args:
             tree (Dict[str, Any]): The modal tree to render
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
+            kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
-        title = self.get_attribute(tree, "title")
-        modal = type(f"{title} Modal", (discord.ui.Modal,), dict(**methods))(title=title, **kw)
+        modal = type(f"{tree['title']} Modal", (discord.ui.Modal,), methods)(title=(tree["title"]), **kwargs)
+
+        components = self.render_components(tree["components"]) if "components" in tree else []
 
-        for component in self.render_components(tree.get("components"), {}):
+        for component in components:
             modal.add_item(component)
 
         return modal
 
     @staticmethod
-    def _render_allowed_mentions(allowed_mentions: Dict[str, Any]) -> discord.AllowedMentions:
-        def render_child(element: Dict[str, [int] | bool], key: str) -> Sequence[Snowflake] | bool:
-            child = element.get(key, True)
-            if type(child) == bool:
-                return child
-
-            return [DiscordIdentifier(identifier) for identifier in map(int, child)]
+    def _render_allowed_mentions(
+        allowed_mentions: AllowedMentions,
+    ) -> discord.AllowedMentions:
+        def parse_mentions(mentions: Union[bool, List[int]]) -> Union[bool, List[Snowflake]]:
+            if isinstance(mentions, bool):
+                return mentions
+            return [DiscordIdentifier(int(identifier)) for identifier in mentions]
 
         return discord.AllowedMentions(
-            everyone=render_child(allowed_mentions, "everyone"),
-            users=render_child(allowed_mentions, "users"),
-            roles=render_child(allowed_mentions, "roles"),
-            replied_user=render_child(allowed_mentions, "replied_user"),
+            everyone=allowed_mentions.get("everyone", True),
+            users=parse_mentions(allowed_mentions.get("users", True)),
+            roles=parse_mentions(allowed_mentions.get("roles", True)),
+            replied_user=allowed_mentions.get("replied_user", True),
         )
 
-    def _render_file(self, raw_file: Dict[str, str | bool]) -> discord.File:
+    @staticmethod
+    def _render_file(raw_file: File) -> discord.File:
         """Method to render a file from a file tree
 
         Args:
             raw_file (Dict[str, Any]): The file tree to render
 
         Returns (discord.File): A discord.File object
         """
         return discord.File(
-            fp=self.get_attribute(raw_file, "filename"),
-            description=self.get_attribute(raw_file, "description"),
-            spoiler=spoiler if (spoiler := self.get_attribute(raw_file, "spoiler")) != "" else False
+            fp=raw_file["filename"],
+            description=raw_file["description"] if "description" in raw_file else None,
+            spoiler=raw_file["spoiler"] if "spoiler" in raw_file else False,
         )
 
-    def _render_view(
-            self,
-            raw_view: Dict[str, ...],
-            callables: Dict[str, Callback],
-            kw: Dict[str, Any]
-    ) -> ui.View:
+    def _render_view(self, raw_view: View, callables: Dict[str, Callback], kwargs: Dict[str, Any]) -> ui.View:
         """Method to render a view element into a discord.ui.View object
 
         Args:
-            raw_view (Dict[str, ...]): The view element to render
+            raw_view (View) The view element to render
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kw (Dict[str, Any]): A dictionary containing the attributes to use for the view
+            kwargs (Dict[str, Any]): A dictionary containing the attributes to use for the view
 
         Returns (ui.View): A discord.ui.View object
         """
-        view = ui.View(**kw)
+        view = ui.View(**kwargs)
         for component in self.render_components(raw_view, callables):
             view.add_item(component)
         return view
 
     @staticmethod
-    def get_attribute(element: Dict[str, Any], attribute: str) -> Any:
-        """Render an attribute of an element
-
-        Args:
-            element (Dict[str, str]): The element to render the attribute from
-            attribute (str): The attribute to render
-
-        Returns (str): The attribute that is extracted from the element.
-        """
-        return "" if (value := element.get(attribute)) is None else value
-
-    def _render_timestamp(self, timestamp: Optional[Dict[str, str]]) -> Optional[datetime]:
+    def _render_timestamp(timestamp: Optional[Timestamp]) -> Optional[datetime]:
         """Method to render a timestamp element into a datetime object
 
         Args:
             timestamp (Optional[Dict[str, str]]): The timestamp element to render
 
         Returns (Optional[datetime]): A datetime object
         """
         if timestamp is None:
             return None
 
-        date = self.get_attribute(timestamp, "timestamp")
-        date_format = self.get_attribute(timestamp, "format")
-        if date_format == "":
-            date_format = "%Y-%m-%d %H:%M:%S.%f"
-        return datetime.strptime(date, date_format) if date != "" else None
-
-    def _render_author(self, author: Dict[str, str]) -> Optional[dict]:
-        """Method to render an author element into a dictionary containing the author attributes
-
-        Args:
-            author (Dict[str, str]): The author element to render
-
-        Returns (Optional[dict]): A dictionary containing the author attributes
-        """
-        return {
-            "name": self.get_attribute(author, "name"),
-            "url": self.get_attribute(author, "url"),
-            "icon_url": self.get_attribute(author, "icon")
-        }
-
-    def _render_footer(self, footer: Dict[str, str]) -> Optional[dict]:
-        """Method to render a footer element into a dictionary containing the footer attributes
-
-        Args:
-            footer (Dict[str, str]): The footer element to render
-
-        Returns (Optional[dict]): A dictionary containing the footer attributes
-        """
-        return {
-            "text": self.get_attribute(footer, "text"),
-            "icon_url": self.get_attribute(footer, "icon")
-        }
-
-    def _render_fields(self, fields: List[Dict[str, str]]) -> List[dict]:
-        """Method that renders a list of fields into a list of dictionaries containing the field attributes
-
-        Args:
-            fields (List[Dict[str, str]]): The list of fields to render
-
-        Returns (List[dict]): A list of dictionaries containing the field attributes
-        """
-        return [{
-            "name": self.get_attribute(field, "name"),
-            "value": self.get_attribute(field, "text"),
-            "inline": (attr := self.get_attribute(field, "inline")) or attr.lower() == "true"}
-            for field in fields
-        ]
-
-    def _render_emoji(self, emoji_element: Dict[str, str]) -> Optional[Dict[str, str]]:
-        """Method to render an emoji element into a dictionary containing the emoji attributes
-
-        Args:
-            emoji_element (Dict[str, str]): The emoji element to render
-
-        Returns (Optional[Dict[str, str]]): A dictionary containing the emoji attributes
-        """
-        emoji = {}
-        if "name" in emoji_element:
-            emoji["name"] = self.get_attribute(emoji_element, "name")
-        if "id" in emoji_element:
-            emoji["id"] = self.get_attribute(emoji_element, "id")
-        if "animated" in emoji_element:
-            animated = self.get_attribute(emoji_element, "animated")
-            emoji["animated"] = animated if type(animated) == bool else animated.lower() == "true"
-        return (None, emoji)[len(emoji) > 0]
-
-    def _extract_attributes(self, element: Dict[str, Any]) -> Dict[str, Union[str, Dict[str, str]]]:
-        """Method to extract attributes from a component element and return them as a dictionary
-
-        Args:
-            element (Dict[str, Any]): The element to extract attributes from
-
-        Returns (Dict[str, Union[str, Dict[str, str]]]): A dictionary containing the attributes
-        """
-        return {attribute: self.get_attribute(element, attribute) for attribute in element.keys()}
+        date = timestamp["date"]
+        date_format = timestamp.get("format", "%Y-%m-%d %H:%M:%S.%f")
+        return datetime.strptime(date, date_format)
 
-    def _render_button(
-            self,
-            component: Dict[str, Union[str, Dict[str, Any]]],
-            callback: Optional[Callback],
-    ) -> ui.Button:
+    @staticmethod
+    def _render_button(component: Button, callback: Optional[Callback]) -> ui.Button:
         """Renders a button from the given component's template
 
         Args:
-            component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
+            component (Button): the component's template
             callback (Optional[Callback]): the callback to be called when the button is pressed
 
         Returns (ui.Item): the rendered button
         """
+        button_component: ButtonComponent = cast(ButtonComponent, component.copy())
+        if callback is not None:
+            button_component["callback"] = callback
+        return create_button(button_component)
 
-        emoji = self._render_emoji(component.pop("emoji")) if "emoji" in component else None
-
-        attributes = self._extract_attributes(component)
-        if emoji is not None:
-            attributes["emoji"] = make_emoji(emoji)
-
-        button: ui.Button = create_button(**attributes)
-        button.callback = callback
-        return button
-
-    def _render_options(self, raw_options: List[Dict[str, Dict[str, str]]]) -> List[discord.SelectOption]:
+    @staticmethod
+    def _render_options(raw_options: List[Option]) -> List[discord.SelectOption]:
         """Renders the options for a select menu
 
         Args:
-            raw_options (List[Dict[str, Union[str, str]]]): the raw options to be rendered
+            raw_options (List[Option]): the raw options to be rendered
 
         Returns (List[discord.SelectOption]): the rendered options
         """
-        options = []
-        for option in raw_options:
-            emoji = self._render_emoji(option.pop("emoji")) if "emoji" in option else None
-            attributes = self._extract_attributes(option)
-
-            if emoji is not None:
-                attributes["emoji"] = make_emoji(emoji)
-
-            options.append(discord.SelectOption(**attributes))
-        return options
-
-    def _render_channel_select(
-            self,
-            component: Dict[str, Union[str, List[str], Dict[str, Any]]],
-            callback: Optional[Callback],
-    ) -> ui.ChannelSelect:
+
+        def parse_option(raw_option: Option) -> discord.SelectOption:
+            option: Dict[str, Any] = cast(Dict[str, Any], raw_option.copy())
+            if "emoji" in raw_option:
+                option["emoji"] = make_emoji(raw_option["emoji"])
+            return discord.SelectOption(**option)
+
+        return [parse_option(raw_option) for raw_option in raw_options]
+
+    @staticmethod
+    def _render_channel_select(component: ChannelSelect, callback: Optional[Callback]) -> ui.ChannelSelect:
         """Renders a select menu from the given component's template
 
         Args:
-            component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
+            component (ChannelSelect): the component's template
             callback (Optional[Callback]): the callback to be called when the select menu is pressed
 
         Returns (ui.Item): the rendered channel select menu
         """
 
-        channel_types: List[str] = component.pop("channel_types")
+        attributes: Dict[str, Any] = cast(Dict[str, Any], component.copy())
+        if "channel_types" in component:
+            attributes["channel_types"] = make_channel_types(component["channel_types"])
 
-        attributes: Dict[str, Any] = self._extract_attributes(component)
-        if channel_types is not None:
-            attributes["channel_types"] = make_channel_types(channel_types)
-
-        select: ui.ChannelSelect = create_channel_select(**attributes)
-        select.callback = callback
+        select: ui.ChannelSelect = create_channel_select(callback=callback, **attributes)
         return select
 
     def _render_select(
-            self,
-            component: Dict[str, Union[str, List[Dict[str, ...]], Dict[str, Any]]],
-            callback: Optional[Callback],
+        self,
+        component: Select,
+        callback: Optional[Callback],
     ) -> ui.Select:
         """Renders a select menu from the given component's template
 
         Args:
             component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
             callback (Optional[Callback]): the callback to be called when the select menu is pressed
 
         Returns (ui.Item): the rendered select menu
         """
+        raw_options = component.pop("options")
+
+        assert isinstance(raw_options, list)
 
-        options = self._render_options(component.pop("options"))
-        attributes: Dict[str, Any] = self._extract_attributes(component)
+        options = self._render_options(raw_options)
+        attributes: Dict[str, Any] = cast(Dict[str, Any], component.copy())
         attributes["options"] = options
 
-        select: ui.Select = create_select(**attributes)
-        select.callback = callback
+        select: ui.Select = create_select(callback=callback, **attributes)
         return select
 
+    @staticmethod
     def _render_type_select(
-            self,
-            select_type: Type[T],
-            component: Dict[str, Union[str, Dict[str, Any]]],
-            callback: Optional[Callback],
-    ) -> T:
+        select_type: Type[CustomSelects], component: CustomSelect, callback: Optional[Callback]
+    ) -> CustomSelects:
         """Renders a type select menu from the given component's template
 
         Args:
-            component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
+            component (component): the component's template
             callback (Optional[Callback]): the callback to be called it is selected from the select menu
 
         Returns (ui.Item): the rendered role select menu
         """
+        return create_type_select(select_type, callback=callback, **component)
 
-        attributes: Dict[str, Any] = self._extract_attributes(component)
-
-        select: T = create_type_select(select_type, **attributes)
-        select.callback = callback
-        return select
-
-    def _render_text_input(
-            self,
-            component: Dict[str, Union[str, Dict[str, Any]]],
-            callback: Optional[Callback],
-    ) -> ui.TextInput:
+    @staticmethod
+    def _render_text_input(component: TextInputComponent, callback: Optional[Callback]) -> ui.TextInput:
         """Renders a text input form the given component's template
 
         Args:
-            component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
+            component (TextInputComponent): the component's template
             callback (Optional[Callback]): the callback to be called when the text is submitted
 
         Returns (ui.TextInput): the rendered text input block.
         """
+        if callback is not None:
+            component["callback"] = callback
 
-        attributes: Dict[str, Any] = self._extract_attributes(component)
-
-        text_input: ui.TextInput = create_text_input(**attributes)
-        text_input.callback = callback
+        text_input: ui.TextInput = create_text_input(component)
         return text_input
 
     def render_component(
-            self,
-            component: Dict[str, Union[str, Dict[str, Any]]],
-            callback: Optional[Callback],
+        self,
+        component: Components,
+        callback: Optional[Callback],
     ) -> ui.Item:
-        """ Renders a component from the given component's template
+        """Renders a component from the given component's template
 
         Args:
-            component (Dict[str, Union[str, Dict[str, Any]]]): the component's template
+            component (Components): the component's template
             callback (Optional[Callback]): the callback to be called when the user interacts with the component
 
         Returns (ui.Item): the rendered component
         """
-        return {
+
+        component_renderer: Dict[ComponentTypes, Callable[[Any, Optional[Callback]], ui.Item]] = {
             "button": self._render_button,
             "select": self._render_select,
             "channel_select": self._render_channel_select,
             "role_select": partial(self._render_type_select, ui.RoleSelect),
             "user_select": partial(self._render_type_select, ui.UserSelect),
             "mentionable_select": partial(self._render_type_select, ui.MentionableSelect),
-            "text_input": self._render_text_input
-        }[component.pop("type")](component, callback)
+            "text_input": self._render_text_input,
+        }
+
+        component_type: ComponentTypes = component["type"]
+        item_renderer = component_renderer[component_type]
 
-    def render_components(
-            self,
-            view: Dict[str, ...],
-            callables: Dict[str, Callback]
-    ) -> Optional[List[ui.Item]]:
+        return item_renderer(component, callback)
+
+    def render_components(self, view: View, callables: Optional[Dict[str, Callback]] = None) -> List[ui.Item]:
         """Renders the components specified by the identifier
 
         Args:
             view (Dict[str, ...]): the dictionary containing the view component.
             callables (Dict[str, Callback]): the callbacks to be called when the user interacts with the components
 
         Returns (Optional[List[ui.Item]]): the rendered components
         """
-        return [self.render_component(component, callables.get(key, ui.Item.callback)) for key, component in
-                view.items()]
+        if callables is None:
+            callables = {}
+        return [self.render_component(component, callables.get(key)) for key, component in view.items()]
 
-    def render(self, raw_embed: Dict[str, ...]) -> discord.Embed:
+    def render(self, raw_embed: Embed) -> discord.Embed:
         """Render the desired templated embed in discord.Embed instance
 
         Args:
-           raw_embed (Dict[str, ...]): the dictionary containing the required key, values needed to render the
+           raw_embed (Embed): the dictionary containing the required key, values needed to render the
                                         embed.
 
         Returns:
-            Embed: Embed Object, discord compatible.
+            discord.Embed: Embed Object, discord compatible.
         """
-
-        def render(attribute: str) -> str:
-            return self.get_attribute(raw_embed, attribute)
-
-        embed_type: discord.types.embed.EmbedType = "rich"
-        if cast(discord.types.embed.EmbedType, given_type := render("type")) != "":
-            embed_type = cast(discord.types.embed.EmbedType, given_type)
+        assert "colour" in raw_embed or "color" in raw_embed, "Embed must have either a colour or color key"
 
         embed = discord.Embed(
-            title=render("title"),
-            colour=make_colour(
-                colour if (colour := render("colour")) != "" else render("color")),
-            type=embed_type,
-            url=render("url"),
-            description=render("description"),
-            timestamp=self._render_timestamp(raw_embed.get("timestamp"))
+            title=raw_embed["title"],
+            colour=make_colour(raw_embed["colour"] if "colour" in raw_embed else raw_embed["color"]),
+            type="rich" if "type" not in raw_embed else raw_embed["type"],
+            url=raw_embed["url"] if "url" in raw_embed else None,
+            description=raw_embed["description"] if "description" in raw_embed else None,
+            timestamp=self._render_timestamp(raw_embed.get("timestamp")),
         )
 
-        for field in self._render_fields(raw_embed["fields"]):
+        for field in raw_embed["fields"]:
             embed.add_field(**field)
 
-        if (footer := raw_embed.get("footer")) is not None:
-            embed.set_footer(**self._render_footer(footer))
+        if "footer" in raw_embed:
+            embed.set_footer(**raw_embed["footer"])
 
-        embed.set_thumbnail(url=self.get_attribute(raw_embed, "thumbnail"))
-        embed.set_image(url=self.get_attribute(raw_embed, "image"))
+        embed.set_thumbnail(url=raw_embed.get("thumbnail"))
+        embed.set_image(url=raw_embed.get("image"))
 
-        if (author := raw_embed.get("author")) is not None:
-            embed.set_author(**self._render_author(author))
+        if "author" in raw_embed:
+            embed.set_author(**raw_embed["author"])
 
         return embed
```

### Comparing `discord-qalib-2.0.0/qalib/translators/parser.py` & `discord-qalib-2.1.0/qalib/translators/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Dict, Any
+from typing import Any, Dict, Generic, TypeVar
 
 from qalib.template_engines.template_engine import TemplateEngine
 
+K = TypeVar("K", bound=str, contravariant=True)
 
-class Parser(ABC):
+
+class Parser(ABC, Generic[K]):
     """Protocol that represents the parser. It is meant to be placed into a Renderer, and is responsible for parsing the
-     document into a menu and a list of callables."""
+    document into a menu and a list of callables."""
 
     @abstractmethod
     def __init__(self, source: str):
         """This method is used to initialize the parser by parsing the source text.
 
         Args:
             source (str): source text that is parsed
         """
-        ...
+        raise NotImplementedError
 
-    def template_message(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    @abstractmethod
+    def template_message(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template the embed by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
             key (str): key of the embed
             template_engine (TemplateEngine): template engine that is used to template the embed
             keywords (Dict[str, Any]): keywords that are used to template the embed
 
         Returns (str): templated embed in the form of string.
         """
-        ...
+        raise NotImplementedError
 
-    def template_menu(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    @abstractmethod
+    def template_menu(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """Method that is used to template the menu by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
             key (str): key of the menu
             template_engine (TemplateEngine): template engine that is used to template the menu
             keywords (Dict[str, Any]): keywords that are used to template the menu
 
         Returns (str): templated menu in the form of string.
         """
-        ...
+        raise NotImplementedError
 
-    def template_modal(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    @abstractmethod
+    def template_modal(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """Method that is used to template the modal by first retrieving it using its key, and then templating it using
         the template_engine
 
         Args:
             key (str): key of the modal
             template_engine (TemplateEngine): template engine that is used to template the modal
             keywords (Dict[str, Any]): keywords that are used to template the modal
 
         Returns (str): templated modal in the form of string.
         """
-        ...
+        raise NotImplementedError
```

### Comparing `discord-qalib-2.0.0/qalib/translators/xml.py` & `discord-qalib-2.1.0/qalib/translators/xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,108 +1,127 @@
 from __future__ import annotations
 
 from datetime import datetime
 from functools import partial
-from typing import Optional, List, Dict, Any, cast, Type, Sequence
-from xml.etree import ElementTree as ElementTree
+from typing import Any, Callable, Dict, List, Optional, Sequence, Type, TypeVar, cast
+from xml.etree import ElementTree
 
 import discord
-import discord.types.embed
-import discord.ui as ui
-from discord import MessageReference
+import discord.types.embed as embed_types
+from discord import ui
 from discord.abc import Snowflake
+from typing_extensions import Concatenate, ParamSpec
 
 from qalib.template_engines.template_engine import TemplateEngine
-from qalib.translators import Callback, Message, MISSING, DiscordIdentifier
+from qalib.translators import Callback, DiscordIdentifier, Message
 from qalib.translators.deserializer import Deserializer
-from qalib.translators.parser import Parser
-from qalib.translators.message_parsing import *
+from qalib.translators.message_parsing import (
+    ButtonComponent,
+    ChannelType,
+    Emoji,
+    create_button,
+    create_channel_select,
+    create_select,
+    create_text_input,
+    create_type_select,
+    make_channel_types,
+    make_colour,
+    make_emoji,
+    Field,
+    Footer,
+    Author,
+    TextInputComponent,
+)
+from qalib.translators.parser import K, Parser
+
+M = TypeVar("M")
+N = TypeVar("N")
+P = ParamSpec("P")
 
 
-class XMLParser(Parser):
-
+class XMLParser(Parser[K]):
     def __init__(self, source: str):
         """Initialisation of the XML Parser
 
         Args:
             source (str): the text of the XML file
         """
         self.root = ElementTree.fromstring(source)
 
-    def get_message(self, identifier: str) -> str:
+    def get_message(self, identifier: K) -> str:
         """This method is used to get an embed by its key.
 
         Args:
-            identifier (str): key of the embed
+            identifier (K): key of the embed
 
         Returns (str): a raw string containing the embed.
         """
-        for embed in self.root.findall("message"):
-            if embed.get("key") == identifier:
-                return ElementTree.tostring(embed, encoding='unicode', method='xml')
+        for message in self.root.findall("message"):
+            if message.get("key") == identifier:
+                return ElementTree.tostring(message, encoding="unicode", method="xml")
         raise KeyError(f"Message with key {identifier} not found")
 
-    def get_menu(self, identifier: str) -> str:
+    def get_menu(self, identifier: K) -> str:
         """This method is used to get a menu by its key.
 
         Args:
-            identifier (str): key of the menu
+            identifier (K): key of the menu
 
         Returns (str): a raw string containing the menu.
         """
         for menu in self.root.findall("menu"):
             if menu.get("key") == identifier:
-                return ElementTree.tostring(menu, encoding='unicode', method='xml')
+                return ElementTree.tostring(menu, encoding="unicode", method="xml")
         raise KeyError(f"Menu with key {identifier} not found")
 
-    def get_modal(self, identifier: str) -> str:
+    def get_modal(self, identifier: K) -> str:
         """This method is used to get a modal by its key.
 
         Args:
-            identifier (str): key of the modal
+            identifier (K): key of the modal
 
         Returns (str): a raw string containing the modal.
         """
         for modal in self.root.findall("modal"):
             if modal.get("key") == identifier:
-                return ElementTree.tostring(modal, encoding='unicode', method='xml')
+                return ElementTree.tostring(modal, encoding="unicode", method="xml")
         raise KeyError(f"Modal with key {identifier} not found")
 
-    def template_message(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_message(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template an embed, by identifying it by its key and using the template engine to
         template it.
 
         Args:
-            key (str): key of the embed
+            key (K): key of the embed
             template_engine (TemplateEngine): template engine that is used to template the embed
             keywords (Dict[str, Any]): keywords that are used to template the embed
 
         Returns (str): templated embed
         """
         return template_engine.template(self.get_message(key), keywords)
 
-    def template_menu(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_menu(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template a menu, by identifying it by its key and using the template engine to
         template it.
 
         Args:
-            key (str): key of the menu
+            key (K): key of the menu
             template_engine (TemplateEngine): template engine that is used to template the menu
             keywords (Dict[str, Any]): keywords that are used to template the menu
 
         Returns (str): templated menu
         """
         return template_engine.template(self.get_menu(key), keywords)
 
-    def template_modal(self, key: str, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
+    def template_modal(self, key: K, template_engine: TemplateEngine, keywords: Dict[str, Any]) -> str:
         """This method is used to template a modal, by identifying it by its key and using the template engine to
         template it.
 
         Args:
-            key (str): key of the modal
+            key (K): key of the modal
             template_engine (TemplateEngine): template engine that is used to template the modal
             keywords (Dict[str, Any]): keywords that are used to template the modal
 
         Returns (str): templated modal
         """
         return template_engine.template(self.get_modal(key), keywords)
 
@@ -122,235 +141,298 @@
         """
         return self.deserialize_message(ElementTree.fromstring(source), callables, kw)
 
     def deserialize_message(
             self,
             message_tree: ElementTree.Element,
             callables: Dict[str, Callback],
-            kw: Dict[str, Any]
+            kwargs: Dict[str, Any],
     ) -> Message:
         """Deserializes an embed from an ElementTree.Element, and returns it as a Display object.
 
         Args:
             message_tree (ElementTree.Element): The element to deserialize the embed from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            kw (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
+            kwargs (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
 
-        Returns (Display): A display object containing the embed and its view.
+        Returns (Message): A display object containing the embed and its view.
         """
-        view_tree: ElementTree.Element = message_tree.find("view")
-        embed = MISSING if (tree := message_tree.find("embed")) is None else self._render_embed(tree)
-        view = MISSING if view_tree is None else self._render_view(view_tree, callables, kw)
-        return Message(embed=embed,
-                       embeds=MISSING if (embeds := message_tree.find("embeds")) is None else list(
-                           map(self._render_embed, embeds)),
-                       view=view,
-                       content=MISSING if (content := message_tree.find("content")) is None else content.text,
-                       tts=MISSING if (tts := message_tree.find("tts")) is None else tts.text.lower() == "true",
-                       nonce=MISSING if (nonce := message_tree.find("nonce")) is None else int(nonce.text),
-                       delete_after=MISSING if (delete_after := message_tree.find("delete_after")) is None else float(
-                           delete_after.text),
-                       suppress_embeds=MISSING if (suppress := message_tree.find(
-                           "suppress_embeds")) is None else self.get_attribute(suppress, "value").lower() in (
-                           "", "true"),
-                       file=MISSING if (file := message_tree.find("file")) is None else self._render_file(file),
-                       files=MISSING if (files := message_tree.find("files")) is None else list(
-                           map(self._render_file, files)),
-                       allowed_mentions=MISSING if (mentions := message_tree.find(
-                           "allowed_mentions")) is None else self._render_allowed_mentions(mentions),
-                       reference=MISSING if (reference := message_tree.find("reference")) is None else
-                       MessageReference(message_id=int(reference.find("message_id").text),
-                                        channel_id=int(reference.find("channel_id").text),
-                                        guild_id=None if (g := reference.find("guild_id")) is None else int(g.text)),
-                       mention_author=MISSING if (mention := message_tree.find(
-                           "mention_author")) is None else self.get_attribute(mention, "value") in ("", "true")
-                       )
+
+        def get_text(element_tree: ElementTree.Element, child: str) -> Optional[str]:
+            element = element_tree.find(child)
+            if element is None:
+                return None
+            return None if element.text is None else element.text
+
+        def get_element(element_tree: ElementTree.Element, child: str) -> Optional[ElementTree.Element]:
+            return None if (element := element_tree.find(child)) is None else element
+
+        def apply(
+                element: Optional[M],
+                func: Callable[Concatenate[M, P], N],
+                *args: P.args,
+                **keyword_args: P.kwargs,
+        ) -> Optional[N]:
+            if element is None:
+                return None
+            return func(element, *args, **keyword_args)
+
+        return Message(
+            embed=apply(get_element(message_tree, "embed"), self._render_embed),
+            embeds=apply(
+                get_element(message_tree, "embeds"),
+                lambda raw_tree: list(map(self._render_embed, raw_tree)),
+            ),
+            view=apply(get_element(message_tree, "view"), self._render_view, callables, kwargs),
+            content=get_text(message_tree, "content"),
+            tts=apply(get_text(message_tree, "tts"), lambda string: string.lower() == "true"),
+            nonce=apply(get_text(message_tree, "nonce"), int),
+            delete_after=apply(get_text(message_tree, "delete_after"), float),
+            suppress_embeds=apply(
+                get_element(message_tree, "suppress_embeds"),
+                lambda tree: self.get_attribute(tree, "value") in ("", "true"),
+            ),
+            file=apply(get_element(message_tree, "file"), self._render_file),
+            files=apply(
+                get_element(message_tree, "files"),
+                lambda raw_tree: list(map(self._render_file, raw_tree)),
+            ),
+            allowed_mentions=apply(
+                get_element(message_tree, "allowed_mentions"),
+                self._render_allowed_mentions,
+            ),
+            reference=apply(get_element(message_tree, "reference"), self._render_reference),
+            mention_author=apply(
+                get_element(message_tree, "mention_author"),
+                lambda tree: self.get_attribute(tree, "value") in ("", "true"),
+            ),
+            stickers=None,
+            ephemeral=None,
+            silent=apply(
+                get_element(message_tree, "silent"),
+                lambda tree: self.get_attribute(tree, "value") in ("", "true"),
+            )
+        )
 
     def deserialize_into_menu(self, source: str, callables: Dict[str, Callback], **kw) -> List[Message]:
         """Deserializes a menu from an XML file, by generating a list of displays that are connected by buttons in their
         views to navigate between them.
 
         Args:
             source (str): The XML file to deserialize.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
             **kw (Dict[str, Any]): A dictionary containing the keyword arguments to use for the views.
 
         Returns (List[Display]): List of displays that are connected by buttons in their views to navigate between them.
         """
 
-        menu_tree: ElementTree = ElementTree.fromstring(source)
+        menu_tree: ElementTree.Element = ElementTree.fromstring(source)
         return [self.deserialize_message(embed, callables, kw) for embed in menu_tree.findall("message")]
 
-    def deserialize_into_modal(self, source: str, methods: Dict[str, Callback], **kw: Any) -> discord.ui.Modal:
+    def deserialize_into_modal(self, source: str, methods: Dict[str, Callback], **kwargs: Any) -> discord.ui.Modal:
         """Method to deserialize a modal into a discord.ui.Modal object
 
         Args:
             source (str): The source text to deserialize into a modal
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            **kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
+            **kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
         modal_tree = ElementTree.fromstring(source)
-        return self._render_modal(modal_tree, methods, kw)
+        return self._render_modal(modal_tree, methods, **kwargs)
 
-    def _render_modal(
-            self,
-            tree: ElementTree.Element,
-            methods: Dict[str, Callback],
-            kw: Any
-    ) -> discord.ui.Modal:
+    def _render_modal(self, tree: ElementTree.Element, methods: Dict[str, Callback], **kwargs: Any) -> discord.ui.Modal:
         """Method to render a modal from a modal tree
 
         Args:
             tree (Dict[str, Any]): The modal tree to render
             methods (Dict[str, Callback]): A dictionary containing the callables to use for the buttons
-            kw (Dict[str, Any]): A dictionary containing the keywords to use for the view
+            kwargs (Dict[str, Any]): A dictionary containing the keywords to use for the view
 
         Returns (discord.ui.Modal): A discord.ui.Modal object
         """
         title = self.get_attribute(tree, "title")
-        modal = type(f"{title} Modal", (discord.ui.Modal,), dict(**methods, **kw))(title=title)
+        modal = type(f"{title} Modal", (discord.ui.Modal,), {**methods, **kwargs})(title=title)
 
         for component in self.render_components(tree):
             modal.add_item(component)
 
         return modal
 
+    @staticmethod
+    def _render_reference(
+            reference_tree: ElementTree.Element,
+    ) -> discord.MessageReference:
+        """Renders a message reference object from an ElementTree.Element.
+
+        Args:
+            reference_tree (ElementTree.Element): The element to render the message reference object from.
+
+        Returns (discord.MessageReference): The message reference object.
+        """
+        message_id = reference_tree.find("message_id")
+        channel_id = reference_tree.find("channel_id")
+        guild_id = reference_tree.find("guild_id")
+
+        if message_id is None or message_id.text is None:
+            raise ValueError("Message reference must have a message id")
+
+        if channel_id is None or channel_id.text is None:
+            raise ValueError("Message reference must have a channel id")
+
+        return discord.MessageReference(
+            message_id=int(message_id.text),
+            channel_id=int(channel_id.text),
+            guild_id=None if guild_id is None or guild_id.text is None else int(guild_id.text),
+        )
+
     def _render_allowed_mentions(self, raw_mentions: ElementTree.Element) -> discord.AllowedMentions:
         """Renders an allowed mentions object from an ElementTree.Element.
 
         Args:
             raw_mentions (ElementTree.Element): The element to render the allowed mentions object from.
 
         Returns (discord.AllowedMentions): The allowed mentions object.
         """
 
+        def get_value(element: Optional[ElementTree.Element] = None) -> bool:
+            if element is None:
+                return True
+            return self.get_attribute(element, "mention").lower() != "false"
+
         def extract_tags(
-                element: Optional[ElementTree.Element],
-                child_tag: Optional[str] = None
+                element: Optional[ElementTree.Element], child_tag: Optional[str] = None
         ) -> bool | Sequence[Snowflake]:
-
             if element is None:
                 return True
             if child_tag is not None and len(element) > 0:
                 return [DiscordIdentifier(int(self.get_element_text(child))) for child in element.findall(child_tag)]
 
-            return self.get_attribute(element, "mention").lower() != "false"
+            return get_value(element)
 
         return discord.AllowedMentions(
-            everyone=extract_tags(raw_mentions.find("everyone")),
+            everyone=get_value(raw_mentions.find("everyone")),
             users=extract_tags(raw_mentions.find("users"), "user"),
             roles=extract_tags(raw_mentions.find("roles"), "role"),
-            replied_user=extract_tags(raw_mentions.find("replied_user"))
+            replied_user=get_value(raw_mentions.find("replied_user")),
         )
 
     def _render_file(self, raw_file: ElementTree.Element) -> discord.File:
-        return discord.File(fp=self.get_element_text(raw_file.find("filename")),
-                            spoiler=self.get_element_text(raw_file.find("spoilers")).lower() == "true",
-                            description=self.get_element_text(raw_file.find("description")))
+        return discord.File(
+            fp=self.get_element_text(raw_file.find("filename")),
+            spoiler=self.get_element_text(raw_file.find("spoilers")).lower() == "true",
+            description=self.get_element_text(raw_file.find("description")),
+        )
 
     def _render_view(
             self,
             raw_view: ElementTree.Element,
             callables: Dict[str, Callback],
-            kw: Dict[str, Any]
+            kwargs: Dict[str, Any],
     ) -> ui.View:
         """Renders a view from an ElementTree.Element.
 
         Args:
             raw_view (ElementTree.Element): The element to render the view from.
             callables (Dict[str, Callback]): A dictionary containing the callables to use for the components.
-            kw (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
+            kwargs (Dict[str, Any]): A dictionary containing the keyword arguments to use for the view.
 
         Returns (ui.View): A view object containing the components.
         """
-        view = ui.View(**kw)
+        view = ui.View(**kwargs)
         for component in self.render_components(raw_view, callables):
             view.add_item(component)
         return view
 
     @staticmethod
     def get_element_text(element: Optional[ElementTree.Element]) -> str:
         """Renders the given ElementTree.Element by returning its text.
 
         Args:
             element (ElementTree.Element): The element to render.
 
         Returns (str): The rendered element.
         """
-        return "" if element is None else element.text
+        return "" if element is None or element.text is None else element.text
 
     @staticmethod
     def get_attribute(element: ElementTree.Element, attribute: str) -> str:
         """Renders an attribute from an ElementTree.Element.
 
         Args:
             element (ElementTree.Element): The element to render the attribute from.
             attribute (str): The name of the attribute to render.
 
         Returns (str): The value of the attribute.
         """
         return "" if (value := element.get(attribute)) is None else value
 
-    def _render_timestamp(self, timestamp_element: ElementTree.Element) -> Optional[datetime]:
+    def _render_timestamp(self, timestamp_element: Optional[ElementTree.Element]) -> Optional[datetime]:
         """Renders the timestamp from an ElementTree.Element. Element may contain an attribute "format" which will be
         used to parse the timestamp.
 
         Args:
-            timestamp_element (ElementTree.Element): The element to render the timestamp from.
+            timestamp_element (Optional[ElementTree.Element]): The element to render the timestamp from.
 
         Returns (Optional[datetime]): A datetime object containing the timestamp.
         """
         if timestamp_element is not None:
             timestamp = self.get_element_text(timestamp_element)
             date_format = self.get_attribute(timestamp_element, "format")
             if date_format == "":
                 date_format = "%Y-%m-%d %H:%M:%S.%f"
             return datetime.strptime(timestamp, date_format) if timestamp != "" else None
+        return None
 
-    def _render_author(self, author_element: ElementTree.Element) -> Optional[dict]:
+    def _render_author(self, author_element: ElementTree.Element) -> Author:
         """Renders the author from an ElementTree.Element.
 
         Args:
             author_element (ElementTree.Element): The element to render the author information from.
 
         Returns (Optional[dict]): A dictionary containing the raw author.
         """
         return {
             "name": self.get_element_text(author_element.find("name")),
             "url": self.get_element_text(author_element.find("url")),
-            "icon_url": self.get_element_text(author_element.find("icon"))
+            "icon_url": self.get_element_text(author_element.find("icon")),
         }
 
-    def _render_footer(self, footer_element: ElementTree.Element) -> Optional[dict]:
+    def _render_footer(self, footer_element: ElementTree.Element) -> Footer:
         """Renders the footer from an ElementTree.Element.
 
         Args:
             footer_element (ElementTree.Element): The element to render the footer from.
 
         Returns (Optional[dict]): A dictionary containing the raw footer.
         """
         return {
             "text": self.get_element_text(footer_element.find("text")),
-            "icon_url": self.get_element_text(footer_element.find("icon"))
+            "icon_url": self.get_element_text(footer_element.find("icon")),
         }
 
-    def _render_fields(self, fields_element: ElementTree.Element) -> List[dict]:
+    def _render_fields(self, fields_element: Optional[ElementTree.Element]) -> List[Field]:
         """Renders the fields from an ElementTree.Element.
 
         Args:
             fields_element (ElementTree.Element): The element to render the fields from.
 
         Returns (List[dict]): A list of dictionaries containing the raw fields.
         """
-        return [{"name": self.get_element_text(field.find("name")),
-                 "value": self.get_element_text(field.find("value")),
-                 "inline": self.get_attribute(field, "inline").lower() == "true"}
-                for field in fields_element.findall("field")]
+        assert fields_element is not None, "Expected Fields For Embed"
+
+        return [
+            {
+                "name": self.get_element_text(field.find("name")),
+                "value": self.get_element_text(field.find("value")),
+                "inline": self.get_attribute(field, "inline").lower() == "true",
+            }
+            for field in fields_element.findall("field")
+        ]
 
     @staticmethod
     def pop_component(component: ElementTree.Element, key: str) -> Optional[ElementTree.Element]:
         """Pops a component from the given element, and returns it.
 
         Args:
             component (ElementTree.Element): The element to pop the component from.
@@ -358,33 +440,38 @@
 
         Returns (Optional[ElementTree.Element]): The popped component, or None if it doesn't exist.
         """
         if (child_component := component.find(key)) is not None:
             component.remove(child_component)
         return child_component
 
-    def _render_emoji(self, emoji_element: Optional[ElementTree.Element]) -> Optional[Dict[str, str]]:
+    def _render_emoji(self, emoji_element: Optional[ElementTree.Element]) -> Optional[Emoji]:
         """Renders an ElementTree.Element into a dictionary.
 
         Args:
             emoji_element (Optional[ElementTree.Element]): The element to render into a Dictionary of emoji data
 
         Returns (Optional[Dict[str, str]]): The rendered emoji, or None if the element is None.
         """
         if emoji_element is None:
-            return
+            return None
 
-        emoji = {}
-        if (name := emoji_element.find("name")) is not None:
-            emoji["name"] = self.get_element_text(name)
-        if (identifier := emoji_element.find("id")) is not None:
-            emoji["id"] = self.get_element_text(identifier)
-        if (animated := emoji_element.find("animated")) is not None:
-            emoji["animated"] = self.get_element_text(animated) == "True"
-        return (None, emoji)[len(emoji) > 0]
+        if emoji_element.find("name") is None:
+            raise ValueError("Expected Name For Emoji")
+
+        emoji = Emoji(name=self.get_element_text(emoji_element.find("name")))
+
+        if (id_element := emoji_element.find("id")) is not None:
+            assert id_element.text is not None
+            emoji["id"] = int(id_element.text)
+        if (animated_element := emoji_element.find("animated")) is not None:
+            assert animated_element.text is not None
+            emoji["animated"] = animated_element.text.lower() == "true"
+
+        return emoji
 
     def _extract_elements(self, tree: ElementTree.Element) -> Dict[str, Any]:
         """Extracts the elements from the given ElementTree.Element, and returns them as a dictionary.
 
         Args:
             tree (ElementTree.Element): The element to extract the elements from.
 
@@ -399,30 +486,31 @@
             component (ElementTree.Element): The button to render, contains the template.
             callback (Optional[Callback]): The callback to use if the user interacts with this button.
 
         Returns (ui.Button): The rendered button.
         """
         emoji_component = self.pop_component(component, "emoji")
         attributes = self._extract_elements(component)
-        attributes["emoji"] = make_emoji(self._render_emoji(emoji_component))
+        attributes["emoji"] = self._render_emoji(emoji_component)
+        attributes["callback"] = callback
+        attributes["disabled"] = attributes["disabled"].lower() == "true" if "disabled" in attributes else False
 
-        button: ui.Button = create_button(**attributes)
-        button.callback = callback
+        button: ui.Button = create_button(cast(ButtonComponent, attributes))
         return button
 
     def _render_options(self, raw_options: Optional[ElementTree.Element]) -> List[discord.SelectOption]:
         """Renders a list of options based on the template in the element, and formatted values given by the keywords.
 
         Args:
             raw_options (ElementTree.Element): The options to render, contains the template.
 
         Returns (List[discord.SelectOption]): The rendered options.
         """
         options = []
-        for option in (raw_options or []):
+        for option in raw_options or []:
             emoji_component = self.pop_component(option, "emoji")
             option_attributes = self._extract_elements(option)
             option_attributes["emoji"] = make_emoji(self._render_emoji(emoji_component))
             options.append(discord.SelectOption(**option_attributes))
         return options
 
     def _render_select(
@@ -438,100 +526,102 @@
 
         Returns (ui.Select): The rendered select.
         """
         options = self._render_options(self.pop_component(component, "options"))
 
         attributes = self._extract_elements(component)
         attributes["options"] = options
+        attributes["callback"] = callback
 
         select: ui.Select = create_select(**attributes)
-        select.callback = callback
+
         return select
 
     def _render_channel_select(self, component: ElementTree.Element, callback: Optional[Callback]) -> ui.ChannelSelect:
         """Renders a channel select based on the template in the element, and formatted values given by the keywords.
 
         Args:
             component (ElementTree.Element): The channel select to render, contains the template.
             callback (Optional[Callback]): The callback to use if the user interacts with this channel select.
 
         Returns (ui.ChannelSelect): The rendered channel select.
         """
-        channel_types: ElementTree.Element = self.pop_component(component, "channel_types")
+        channel_types: Optional[ElementTree.Element] = self.pop_component(component, "channel_types")
 
         attributes = self._extract_elements(component)
         if channel_types is not None:
-            attributes["channel_types"] = make_channel_types(list(map(
-                lambda element: self.get_element_text(element),
-                channel_types.findall("channel_type")
-            )))
-
+            attributes["channel_types"] = make_channel_types(
+                [cast(ChannelType, self.get_element_text(channel)) for channel in channel_types.findall("channel_type")]
+            )
+        attributes["callback"] = callback
         select: ui.ChannelSelect = create_channel_select(**attributes)
-        select.callback = callback
         return select
 
     def _render_type_select(
             self,
-            select_type: Type[T],
             component: ElementTree.Element,
             callback: Optional[Callback],
-    ) -> T:
+            select_base: Type[ui.UserSelect | ui.RoleSelect | ui.MentionableSelect],
+    ) -> ui.UserSelect | ui.RoleSelect | ui.MentionableSelect:
         """Renders a type select based on the template in the element, and formatted values given by the keywords.
 
         Args:
             component (ElementTree.Element): The type select to render, contains the template.
             callback (Optional[Callback]): The callback to use if the user interacts with this role select.
+            select_base (Type[ui.UserSelect | ui.RoleSelect | ui.MentionableSelect]): The type of select to render.
 
         Returns (ui.RoleSelect): The rendered role select.
         """
         attributes = self._extract_elements(component)
+        select_type = type(select_base.__name__, (select_base,), {"callback": callback})
+
+        assert issubclass(select_type, (ui.UserSelect, ui.RoleSelect, ui.MentionableSelect))
 
-        select: ui.RoleSelect = create_type_select(select_type, **attributes)
-        select.callback = callback
+        select = create_type_select(select_type, **attributes)
         return select
 
     def _render_text_input(self, component: ElementTree.Element, callback: (Optional[Callback])) -> ui.TextInput:
         """Renders a text input based on the template in the element, and formatted values given by the keywords.
 
         Args:
             component (ElementTree.Element): The text input to render, contains the template.
             callback (Optional[Callback]): The callback to use if the user interacts with this text input.
 
         Returns (ui.TextInput): The rendered text input.
         """
         attributes = self._extract_elements(component)
+        attributes["callback"] = callback
+        text_input: ui.TextInput = create_text_input(cast(TextInputComponent, attributes))
 
-        text_input: ui.TextInput = create_text_input(**attributes)
-        text_input.callback = callback
         return text_input
 
     def render_component(self, component: ElementTree.Element, callback: Optional[Callback]) -> ui.Item:
         """Renders a component based on the tag in the element.
 
         Args:
             component (ElementTree.Element): The component to render, contains all template.
             callback (Optional[Callback]): The callback to use if the user interacts with this component.
 
         Returns (discord.ui.Item): The rendered component.
         """
 
-        return {
+        components: Dict[str, Callable[[ElementTree.Element, Optional[Callback]], ui.Item]] = {
             "button": self._render_button,
             "select": self._render_select,
             "channel_select": self._render_channel_select,
             "text_input": self._render_text_input,
-            "role_select": partial(self._render_type_select, ui.RoleSelect),
-            "mentionable_select": partial(self._render_type_select, ui.MentionableSelect),
-            "user_select": partial(self._render_type_select, ui.UserSelect),
-        }[component.tag](component, callback)
+            "role_select": partial(self._render_type_select, select_base=ui.RoleSelect),
+            "mentionable_select": partial(self._render_type_select, select_base=ui.MentionableSelect),
+            "user_select": partial(self._render_type_select, select_base=ui.UserSelect),
+        }
+        renderer: Callable[[ElementTree.Element, Optional[Callback]], ui.Item] = components[component.tag]
+        return renderer(component, callback)
 
     def render_components(
-            self,
-            view: ElementTree.Element,
-            callables: Optional[Dict[str, Callback]] = None
+            self, view: ElementTree.Element, callables: Optional[Dict[str, Callback]] = None
     ) -> List[ui.Item]:
         """Renders a list of components based on the identifier given.
 
         Args:
             view (ui.View): The raw view.
             callables (Dict[str, Callback]): The callbacks to use if the user interacts with the components.
 
@@ -539,15 +629,15 @@
         """
         if callables is None:
             callables = {}
 
         return [
             self.render_component(
                 component,
-                callables.get(self.get_attribute(component, "key"), ui.Item.callback),
+                callables.get(self.get_attribute(component, "key")),
             )
             for component in view
         ]
 
     def _render_embed(self, raw_embed: ElementTree.Element) -> discord.Embed:
         """Render the desired templated embed in discord.Embed instance.
 
@@ -557,25 +647,25 @@
         Returns:
             Embed: Embed Object, discord compatible.
         """
 
         def render(name: str):
             return self.get_element_text(raw_embed.find(name))
 
-        embed_type: discord.types.embed.EmbedType = "rich"
-        if cast(discord.types.embed.EmbedType, given_type := render("type")) != "":
-            embed_type = cast(discord.types.embed.EmbedType, given_type)
+        embed_type: embed_types.EmbedType = "rich"
+        if cast(embed_types.EmbedType, given_type := render("type")) != "":
+            embed_type = cast(embed_types.EmbedType, given_type)
 
         embed = discord.Embed(
             title=render("title"),
             colour=make_colour(render("colour")),
             type=embed_type,
             url=render("url"),
             description=render("description"),
-            timestamp=self._render_timestamp(raw_embed.find("timestamp"))
+            timestamp=self._render_timestamp(raw_embed.find("timestamp")),
         )
 
         for field in self._render_fields(raw_embed.find("fields")):
             embed.add_field(**field)
 
         if (footer := raw_embed.find("footer")) is not None:
             embed.set_footer(**self._render_footer(footer))
```

### Comparing `discord-qalib-2.0.0/setup.py` & `discord-qalib-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import find_packages, setup
 
-with open('requirements.txt') as f:
+with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
-    name='Discord-Qalib',
+    name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.0.0",
-    description='A library for templating responses on .xml, and .json files for discord.py',
+    version="2.1.0",
+    description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
-    license='MIT',
-    python_requires='>=3.8.0',
+    license="MIT",
+    python_requires=">=3.8.0",
     install_requires=requirements,
 )
```

