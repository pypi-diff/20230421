# Comparing `tmp/lift.bot-15.3.5.tar.gz` & `tmp/lift.bot-15.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lift.bot-15.3.5.tar", last modified: Thu Apr 20 03:44:29 2023, max compression
+gzip compressed data, was "lift.bot-15.5.1.tar", last modified: Thu Apr 20 03:50:18 2023, max compression
```

## Comparing `lift.bot-15.3.5.tar` & `lift.bot-15.5.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.806688 lift.bot-15.3.5/
--rw-rw-rw-   0        0        0      715 2023-04-20 03:44:29.803693 lift.bot-15.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2023-04-20 03:42:22.000000 lift.bot-15.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.724743 lift.bot-15.3.5/lift/
--rw-rw-rw-   0        0        0        0 2023-04-20 03:08:06.000000 lift.bot-15.3.5/lift/__init__.py
--rw-rw-rw-   0        0        0    31867 2023-04-20 03:08:04.000000 lift.bot-15.3.5/lift/gradient.py
--rw-rw-rw-   0        0        0     3040 2023-04-20 03:08:03.000000 lift.bot-15.3.5/lift/lft.py
--rw-rw-rw-   0        0        0     1175 2023-04-20 03:08:07.000000 lift.bot-15.3.5/lift/status.py
-drwxrwxrwx   0        0        0        0 2023-04-20 03:44:29.797693 lift.bot-15.3.5/lift.bot.egg-info/
--rw-rw-rw-   0        0        0      715 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-20 03:44:29.000000 lift.bot-15.3.5/lift.bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 03:44:29.806688 lift.bot-15.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-04-20 03:10:09.000000 lift.bot-15.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:50:18.164396 lift.bot-15.5.1/
+-rw-rw-rw-   0        0        0     2163 2023-04-20 03:50:18.162394 lift.bot-15.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1403 2023-04-20 03:42:22.000000 lift.bot-15.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 03:50:18.116423 lift.bot-15.5.1/lift/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:08:06.000000 lift.bot-15.5.1/lift/__init__.py
+-rw-rw-rw-   0        0        0    31867 2023-04-20 03:08:04.000000 lift.bot-15.5.1/lift/gradient.py
+-rw-rw-rw-   0        0        0     3037 2023-04-20 03:49:34.000000 lift.bot-15.5.1/lift/lft.py
+-rw-rw-rw-   0        0        0     1175 2023-04-20 03:08:07.000000 lift.bot-15.5.1/lift/status.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:50:18.152403 lift.bot-15.5.1/lift.bot.egg-info/
+-rw-rw-rw-   0        0        0     2163 2023-04-20 03:50:17.000000 lift.bot-15.5.1/lift.bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-04-20 03:50:17.000000 lift.bot-15.5.1/lift.bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:50:17.000000 lift.bot-15.5.1/lift.bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-20 03:50:17.000000 lift.bot-15.5.1/lift.bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 03:50:17.000000 lift.bot-15.5.1/lift.bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:45:54.000000 lift.bot-15.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:50:18.164396 lift.bot-15.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-04-20 03:49:14.000000 lift.bot-15.5.1/setup.py
```

### Comparing `lift.bot-15.3.5/README.md` & `lift.bot-15.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lift.bot-15.3.5/lift/gradient.py` & `lift.bot-15.5.1/lift/gradient.py`

 * *Files identical despite different names*

### Comparing `lift.bot-15.3.5/lift/lft.py` & `lift.bot-15.5.1/lift/lft.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                                       ██║     ██║█████╗     ██║   
                                       ██║     ██║██╔══╝     ██║   
                                       ███████╗██║██║        ██║   
                                       ╚══════╝╚═╝╚═╝        ╚═╝   
                                                 
                                         
      ┌────────────────────────────────────────────────────────────────────────────────────────┐
-                      Current Version: {dataver} | Discord: https://discord.gg/pupnvCNbwN
+                      Current Version: 15.5.1 | Discord: https://discord.gg/pupnvCNbwN
      └────────────────────────────────────────────────────────────────────────────────────────┘
      
      """))
 
 @bot.event
 async def on_command(ctx):
     print(Colorate.Horizontal(Colors.red_to_yellow, f"""
```

### Comparing `lift.bot-15.3.5/lift/status.py` & `lift.bot-15.5.1/lift/status.py`

 * *Files identical despite different names*

### Comparing `lift.bot-15.3.5/setup.py` & `lift.bot-15.5.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from setuptools import find_packages, setup
 from urllib.request import urlopen
 
 file_url = 'https://raw.githubusercontent.com/devliftz/lift.bot/main/version.txt'
 dataver = urlopen(file_url).read(203).decode('utf-8')
 
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 packages = [
     'lift'
 ]
 
 setup(
     name="lift.bot",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     install_requires=['about_time==4.2.1', 'grapheme==0.6.0', 'discord.py'],
-    version=f"{dataver}",
+    version=f"15.5.1",
     packages=packages,
     include_package_data=True,
     license="MIT License",
     description="lift.bot",
     keywords="lift",
     url="https://github.com/bytebuildz/liftcord.py-tools/",
     author=".drmr",
```

