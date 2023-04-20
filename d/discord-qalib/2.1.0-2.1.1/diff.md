# Comparing `tmp/discord-qalib-2.1.0.tar.gz` & `tmp/discord-qalib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.1.0.tar", last modified: Wed Apr 19 23:05:24 2023, max compression
+gzip compressed data, was "discord-qalib-2.1.1.tar", last modified: Thu Apr 20 22:00:46 2023, max compression
```

## Comparing `discord-qalib-2.1.0.tar` & `discord-qalib-2.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.011848 discord-qalib-2.1.0/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 23:05:24.000000 discord-qalib-2.1.0/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 23:04:52.000000 discord-qalib-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:05:24.015848 discord-qalib-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-19 23:05:11.000000 discord-qalib-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:46.595987 discord-qalib-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:00:46.591987 discord-qalib-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:46.587986 discord-qalib-2.1.1/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-20 22:00:46.000000 discord-qalib-2.1.1/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-20 22:00:46.000000 discord-qalib-2.1.1/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:00:46.000000 discord-qalib-2.1.1/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 22:00:46.000000 discord-qalib-2.1.1/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 22:00:46.000000 discord-qalib-2.1.1/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-20 22:00:34.000000 discord-qalib-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:46.587986 discord-qalib-2.1.1/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-20 22:00:34.000000 discord-qalib-2.1.1/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:46.591987 discord-qalib-2.1.1/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:00:46.591987 discord-qalib-2.1.1/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23241 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 22:00:18.000000 discord-qalib-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:00:46.595987 discord-qalib-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-20 22:00:34.000000 discord-qalib-2.1.1/setup.py
```

### Comparing `discord-qalib-2.1.0/LICENSE` & `discord-qalib-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/PKG-INFO` & `discord-qalib-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.1.0
+Version: 2.1.1
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.1.0/README.md` & `discord-qalib-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.1.1/discord_qalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.1.0
+Version: 2.1.1
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.0 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.1.1 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
```

### Comparing `discord-qalib-2.1.0/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.1.1/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/pyproject.toml` & `discord-qalib-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.1.0"
+version = "2.1.1"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.1.0/qalib/__init__.py` & `discord-qalib-2.1.1/qalib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .template_engines.jinja2 import Jinja2
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
     template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.1.0/qalib/context.py` & `discord-qalib-2.1.1/qalib/context.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/interaction.py` & `discord-qalib-2.1.1/qalib/interaction.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/renderer.py` & `discord-qalib-2.1.1/qalib/renderer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/template_engines/formatter.py` & `discord-qalib-2.1.1/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/template_engines/jinja2.py` & `discord-qalib-2.1.1/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/__init__.py` & `discord-qalib-2.1.1/qalib/translators/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from dataclasses import dataclass, asdict
+import dataclasses
+from dataclasses import dataclass
 from typing import Any, Awaitable, Callable, Dict, Optional, Sequence, TypeVar, Union
 
 import discord
 from discord.abc import Snowflake
 
 V_co = TypeVar("V_co", bound=discord.ui.View, covariant=True)
 
@@ -28,19 +29,20 @@
     ephemeral: Optional[bool]
     allowed_mentions: Optional[discord.AllowedMentions]
     suppress_embeds: Optional[bool]
     silent: Optional[bool]
     delete_after: Optional[float]
 
     def dict(self) -> Dict[str, Any]:
-        return {key: value for key, value in asdict(self).items() if value is not None}
+        return {key.name: attr for key in dataclasses.fields(self) if (attr := getattr(self, key.name)) is not None}
 
     def __iter__(self):
         # Order is preserved in Python 3.7+: https://mail.python.org/pipermail/python-dev/2017-December/151283.html
-        for value in self.__dict__.values():
+        for key in dataclasses.fields(self):
+            value = getattr(self, key.name)
             if value is None:
                 continue
             yield value
 
 
 @dataclass
 class ContextMessage(BaseMessage):
@@ -98,8 +100,8 @@
             view=self.view,
             tts=self.tts,
             ephemeral=self.ephemeral,
             allowed_mentions=self.allowed_mentions,
             suppress_embeds=self.suppress_embeds,
             silent=self.silent,
             delete_after=self.delete_after,
-        )
+        )
```

### Comparing `discord-qalib-2.1.0/qalib/translators/deserializer.py` & `discord-qalib-2.1.1/qalib/translators/deserializer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/factory.py` & `discord-qalib-2.1.1/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/json.py` & `discord-qalib-2.1.1/qalib/translators/json.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/message_parsing.py` & `discord-qalib-2.1.1/qalib/translators/message_parsing.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/parser.py` & `discord-qalib-2.1.1/qalib/translators/parser.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/qalib/translators/xml.py` & `discord-qalib-2.1.1/qalib/translators/xml.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.1.0/setup.py` & `discord-qalib-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,14 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.1.0",
+    version="2.1.1",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
 )
```

