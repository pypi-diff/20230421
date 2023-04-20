# Comparing `tmp/lift.bot-21.0.1.tar.gz` & `tmp/lift.bot-21.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lift.bot-21.0.1.tar", last modified: Thu Apr 20 22:02:34 2023, max compression
+gzip compressed data, was "lift.bot-21.1.5.tar", last modified: Thu Apr 20 22:30:23 2023, max compression
```

## Comparing `lift.bot-21.0.1.tar` & `lift.bot-21.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 22:02:34.902787 lift.bot-21.0.1/
--rw-rw-rw-   0        0        0      756 2023-04-20 22:02:34.899788 lift.bot-21.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-20 22:01:42.000000 lift.bot-21.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 22:02:34.840825 lift.bot-21.0.1/lift/
--rw-rw-rw-   0        0        0        0 2023-04-20 14:24:44.000000 lift.bot-21.0.1/lift/__init__.py
--rw-rw-rw-   0        0        0    31867 2023-04-20 17:41:00.000000 lift.bot-21.0.1/lift/coloring.py
--rw-rw-rw-   0        0        0      902 2023-04-20 22:01:03.000000 lift.bot-21.0.1/lift/console.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:02:34.895791 lift.bot-21.0.1/lift.bot.egg-info/
--rw-rw-rw-   0        0        0      756 2023-04-20 22:02:34.000000 lift.bot-21.0.1/lift.bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-20 22:02:34.000000 lift.bot-21.0.1/lift.bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 22:02:34.000000 lift.bot-21.0.1/lift.bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-20 22:02:34.000000 lift.bot-21.0.1/lift.bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-20 22:02:34.000000 lift.bot-21.0.1/lift.bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 22:02:34.904786 lift.bot-21.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-04-20 22:02:29.000000 lift.bot-21.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:30:23.738507 lift.bot-21.1.5/
+-rw-rw-rw-   0        0        0      756 2023-04-20 22:30:23.735502 lift.bot-21.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-20 22:01:42.000000 lift.bot-21.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 22:30:23.682536 lift.bot-21.1.5/lift/
+-rw-rw-rw-   0        0        0        0 2023-04-20 14:24:44.000000 lift.bot-21.1.5/lift/__init__.py
+-rw-rw-rw-   0        0        0    31867 2023-04-20 17:41:00.000000 lift.bot-21.1.5/lift/coloring.py
+-rw-rw-rw-   0        0        0     3330 2023-04-20 22:27:47.000000 lift.bot-21.1.5/lift/console.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:30:23.730506 lift.bot-21.1.5/lift.bot.egg-info/
+-rw-rw-rw-   0        0        0      756 2023-04-20 22:30:23.000000 lift.bot-21.1.5/lift.bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-20 22:30:23.000000 lift.bot-21.1.5/lift.bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 22:30:23.000000 lift.bot-21.1.5/lift.bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-20 22:30:23.000000 lift.bot-21.1.5/lift.bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-20 22:30:23.000000 lift.bot-21.1.5/lift.bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 22:30:23.739506 lift.bot-21.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-04-20 22:30:19.000000 lift.bot-21.1.5/setup.py
```

### Comparing `lift.bot-21.0.1/PKG-INFO` & `lift.bot-21.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift.bot
-Version: 21.0.1
+Version: 21.1.5
 Summary: lift.bot
 Home-page: https://github.com/bytebuildz/liftcord.py-tools/
 Author: .drmr
 Author-email: hi@icey.fr
 License: MIT License
 Keywords: lift
 Classifier: Programming Language :: Python
```

### Comparing `lift.bot-21.0.1/lift/coloring.py` & `lift.bot-21.1.5/lift/coloring.py`

 * *Files identical despite different names*

### Comparing `lift.bot-21.0.1/lift.bot.egg-info/PKG-INFO` & `lift.bot-21.1.5/lift.bot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift.bot
-Version: 21.0.1
+Version: 21.1.5
 Summary: lift.bot
 Home-page: https://github.com/bytebuildz/liftcord.py-tools/
 Author: .drmr
 Author-email: hi@icey.fr
 License: MIT License
 Keywords: lift
 Classifier: Programming Language :: Python
```

### Comparing `lift.bot-21.0.1/setup.py` & `lift.bot-21.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 setup(
     name="lift.bot",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['about_time==4.2.1', 'grapheme==0.6.0', 'discord.py'],
-    version=f"21.0.1",
+    version=f"21.1.5",
     packages=packages,
     include_package_data=True,
     license="MIT License",
     description="lift.bot",
     keywords="lift",
     url="https://github.com/bytebuildz/liftcord.py-tools/",
     author=".drmr",
```

