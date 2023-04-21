# Comparing `tmp/azureChatGPT-0.0.4.tar.gz` & `tmp/azureChatGPT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureChatGPT-0.0.4.tar", last modified: Thu Apr  6 09:03:15 2023, max compression
+gzip compressed data, was "azureChatGPT-0.0.5.tar", last modified: Fri Apr 21 09:03:52 2023, max compression
```

## Comparing `azureChatGPT-0.0.4.tar` & `azureChatGPT-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 09:03:14.996453 azureChatGPT-0.0.4/
--rw-rw-rw-   0        0        0    18431 2023-03-14 07:55:11.000000 azureChatGPT-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3145 2023-04-06 09:03:14.996453 azureChatGPT-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2023-04-06 09:02:33.000000 azureChatGPT-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 09:03:14.997453 azureChatGPT-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-04-06 07:27:53.000000 azureChatGPT-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:03:14.931453 azureChatGPT-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 09:03:14.982455 azureChatGPT-0.0.4/src/azureChatGPT/
--rw-rw-rw-   0        0        0       20 2023-03-17 08:31:28.000000 azureChatGPT-0.0.4/src/azureChatGPT/__init__.py
--rw-rw-rw-   0        0        0      155 2023-03-14 07:58:27.000000 azureChatGPT-0.0.4/src/azureChatGPT/__main__.py
--rw-rw-rw-   0        0        0    14292 2023-04-06 07:56:37.000000 azureChatGPT-0.0.4/src/azureChatGPT/azure.py
--rw-rw-rw-   0        0        0     2727 2023-03-14 07:44:49.000000 azureChatGPT-0.0.4/src/azureChatGPT/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 09:03:14.994453 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/
--rw-rw-rw-   0        0        0     3145 2023-04-06 09:03:14.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-06 09:03:14.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 09:03:14.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-17 08:52:27.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-04-06 09:03:14.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-06 09:03:14.000000 azureChatGPT-0.0.4/src/azureChatGPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 09:03:52.957625 azureChatGPT-0.0.5/
+-rw-rw-rw-   0        0        0    18431 2023-03-14 07:55:11.000000 azureChatGPT-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3145 2023-04-21 09:03:52.956625 azureChatGPT-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2399 2023-04-06 09:02:33.000000 azureChatGPT-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 09:03:52.957625 azureChatGPT-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1256 2023-04-21 09:01:14.000000 azureChatGPT-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:03:52.915625 azureChatGPT-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 09:03:52.947625 azureChatGPT-0.0.5/src/azureChatGPT/
+-rw-rw-rw-   0        0        0       20 2023-03-17 08:31:28.000000 azureChatGPT-0.0.5/src/azureChatGPT/__init__.py
+-rw-rw-rw-   0        0        0      155 2023-03-14 07:58:27.000000 azureChatGPT-0.0.5/src/azureChatGPT/__main__.py
+-rw-rw-rw-   0        0        0    14286 2023-04-21 09:00:43.000000 azureChatGPT-0.0.5/src/azureChatGPT/azure.py
+-rw-rw-rw-   0        0        0     2727 2023-03-14 07:44:49.000000 azureChatGPT-0.0.5/src/azureChatGPT/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 09:03:52.955626 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/
+-rw-rw-rw-   0        0        0     3145 2023-04-21 09:03:52.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-04-21 09:03:52.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 09:03:52.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-17 08:52:27.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-04-21 09:03:52.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-21 09:03:52.000000 azureChatGPT-0.0.5/src/azureChatGPT.egg-info/top_level.txt
```

### Comparing `azureChatGPT-0.0.4/LICENSE` & `azureChatGPT-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `azureChatGPT-0.0.4/PKG-INFO` & `azureChatGPT-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureChatGPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: ChatGPT is a reverse engineering of Azure ChatGPT API
 Home-page: https://github.com/EvAnhaodong/azureChatGPT
 Author: yehaodong
 Author-email: yehaodong@genomics.cn
 License: GNU General Public License v2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `azureChatGPT-0.0.4/README.md` & `azureChatGPT-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `azureChatGPT-0.0.4/setup.py` & `azureChatGPT-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from pathlib import Path
 
 PATH = Path("README.md")
 
 setup(
     name="azureChatGPT",
-    version="0.0.4",
+    version="0.0.5",
     description="ChatGPT is a reverse engineering of Azure ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/EvAnhaodong/azureChatGPT",
     author="yehaodong",
     author_email="yehaodong@genomics.cn",
     license="GNU General Public License v2.0",
```

### Comparing `azureChatGPT-0.0.4/src/azureChatGPT/azure.py` & `azureChatGPT-0.0.5/src/azureChatGPT/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             )
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
         """
         Truncate the conversation
         """
         self.conversation["current"] = [
-            dict((key, sentence[key]) for key in sentence if key != "name")
+            dict((key, sentence[key]) for key in ["role", "content"])
             for sentence in self.conversation[convo_id]
         ]
 
         while True:
             if (
                 self.get_token_count("current") > self.max_tokens[self.engine]
                 and len(self.conversation["current"]) > 1
```

### Comparing `azureChatGPT-0.0.4/src/azureChatGPT/utils.py` & `azureChatGPT-0.0.5/src/azureChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `azureChatGPT-0.0.4/src/azureChatGPT.egg-info/PKG-INFO` & `azureChatGPT-0.0.5/src/azureChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureChatGPT
-Version: 0.0.4
+Version: 0.0.5
 Summary: ChatGPT is a reverse engineering of Azure ChatGPT API
 Home-page: https://github.com/EvAnhaodong/azureChatGPT
 Author: yehaodong
 Author-email: yehaodong@genomics.cn
 License: GNU General Public License v2.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

