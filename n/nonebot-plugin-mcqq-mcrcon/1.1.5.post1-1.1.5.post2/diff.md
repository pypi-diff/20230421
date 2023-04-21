# Comparing `tmp/nonebot-plugin-mcqq-mcrcon-1.1.5.post1.tar.gz` & `tmp/nonebot-plugin-mcqq-mcrcon-1.1.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-mcqq-mcrcon-1.1.5.post1.tar", last modified: Fri Apr 21 10:03:32 2023, max compression
+gzip compressed data, was "nonebot-plugin-mcqq-mcrcon-1.1.5.post2.tar", last modified: Fri Apr 21 10:06:48 2023, max compression
```

## Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1.tar` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:03:32.950126 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/
--rw-rw-rw-   0        0        0    35184 2022-12-23 05:54:07.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/LICENSE
--rw-rw-rw-   0        0        0     2654 2023-04-21 10:03:32.950126 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/PKG-INFO
--rw-rw-rw-   0        0        0     2144 2023-01-11 13:57:47.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 10:03:32.939115 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/
--rw-rw-rw-   0        0        0     1510 2023-04-21 09:39:09.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/__init__.py
--rw-rw-rw-   0        0        0     3004 2023-04-21 09:40:07.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/data_source.py
--rw-rw-rw-   0        0        0     1030 2023-04-21 09:36:25.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:03:32.949124 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/
--rw-rw-rw-   0        0        0     2654 2023-04-21 10:03:32.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-21 10:03:32.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:03:32.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-21 10:03:32.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-21 10:03:32.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 10:03:32.951126 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-04-21 10:01:27.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:06:48.901858 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/
+-rw-rw-rw-   0        0        0    35184 2022-12-23 05:54:07.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/LICENSE
+-rw-rw-rw-   0        0        0     2654 2023-04-21 10:06:48.900856 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     2144 2023-01-11 13:57:47.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 10:06:48.890847 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/
+-rw-rw-rw-   0        0        0     1510 2023-04-21 09:39:09.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/__init__.py
+-rw-rw-rw-   0        0        0     3004 2023-04-21 09:40:07.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/data_source.py
+-rw-rw-rw-   0        0        0     1030 2023-04-21 09:36:25.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:06:48.899855 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/
+-rw-rw-rw-   0        0        0     2654 2023-04-21 10:06:48.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-21 10:06:48.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:06:48.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-04-21 10:06:48.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-21 10:06:48.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 10:06:48.901858 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1249 2023-04-21 10:06:29.000000 nonebot-plugin-mcqq-mcrcon-1.1.5.post2/setup.py
```

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/LICENSE` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/PKG-INFO` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq-mcrcon
-Version: 1.1.5.post1
+Version: 1.1.5.post2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/README.md` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/__init__.py` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/data_source.py` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon/utils.py` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/nonebot_plugin_mcqq_mcrcon.egg-info/PKG-INFO` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/nonebot_plugin_mcqq_mcrcon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mcqq-mcrcon
-Version: 1.1.5.post1
+Version: 1.1.5.post2
 Summary: 基于NoneBot的QQ群聊与Minecraft Server消息互通插件
 Home-page: https://github.com/17TheWord/nonebot-plugin-mcqq
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot-plugin-mcqq-mcrcon-1.1.5.post1/setup.py` & `nonebot-plugin-mcqq-mcrcon-1.1.5.post2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-mcqq-mcrcon",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="1.1.5-post1",  # 程序版本
+    version="1.1.5-post2",  # 程序版本
     author="17TheWord",  # 项目作者
     author_email="17theword@gmail.com",  # 作者邮件
     description="基于NoneBot的QQ群聊与Minecraft Server消息互通插件",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/17TheWord/nonebot-plugin-mcqq",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     classifiers=[
         "Programming Language :: Python :: 3.9",  # 使用Python3.10
         "License :: OSI Approved :: GNU Affero General Public License v3",  # 开源协议
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        'mcqq-tool>=0.0.1',
         'nonebot2>=2.0.0rc3',
         'nonebot-adapter-onebot>=2.1.1',
         'nonebot-plugin-guild-patch>=0.2.0',
         'websockets>=10.3',
         'mcrcon>=0.7.0',
     ],
 )
```

