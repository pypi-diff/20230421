# Comparing `tmp/airunner-1.9.3.tar.gz` & `tmp/airunner-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airunner-1.9.3.tar", last modified: Tue Apr 18 15:31:43 2023, max compression
+gzip compressed data, was "airunner-1.9.4.tar", last modified: Fri Apr 21 15:03:39 2023, max compression
```

## Comparing `airunner-1.9.3.tar` & `airunner-1.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.023322 airunner-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 15:31:28.000000 airunner-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-18 15:31:43.023322 airunner-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-18 15:31:28.000000 airunner-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:31:43.023322 airunner-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-18 15:31:28.000000 airunner-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.019322 airunner-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.019322 airunner-1.9.3/src/airunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/balloon.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/history.py
--rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/qtcanvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/runai_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-18 15:31:28.000000 airunner-1.9.3/src/airunner/settingsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-18 15:31:29.000000 airunner-1.9.3/src/airunner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:31:43.023322 airunner-1.9.3/src/airunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 15:31:43.000000 airunner-1.9.3/src/airunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 15:03:26.000000 airunner-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-21 15:03:39.147076 airunner-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-21 15:03:26.000000 airunner-1.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:03:39.147076 airunner-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-21 15:03:26.000000 airunner-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.143076 airunner-1.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/src/airunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/balloon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64664 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32827 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/qtcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/runai_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/settingsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-04-21 15:03:26.000000 airunner-1.9.4/src/airunner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:03:39.147076 airunner-1.9.4/src/airunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 15:03:39.000000 airunner-1.9.4/src/airunner.egg-info/top_level.txt
```

### Comparing `airunner-1.9.3/LICENSE` & `airunner-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/PKG-INFO` & `airunner-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.3
+Version: 1.9.4
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `airunner-1.9.3/README.md` & `airunner-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/setup.py` & `airunner-1.9.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='airunner',
-    version="1.9.3",
+    version="1.9.4",
     author="Capsize LLC",
     description="A Stable Diffusion GUI",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
     url="https://github.com/Capsize-Games/airunner",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-        "aihandler==1.9.6",
+        "aihandler==1.9.7",
     ]
 )
```

### Comparing `airunner-1.9.3/src/airunner/balloon.py` & `airunner-1.9.4/src/airunner/balloon.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/extensions.py` & `airunner-1.9.4/src/airunner/extensions.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/filters.py` & `airunner-1.9.4/src/airunner/filters.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/main.py` & `airunner-1.9.4/src/airunner/main.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/qtcanvas.py` & `airunner-1.9.4/src/airunner/qtcanvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
         Update the image by section
         This is used by other classes to add an image to the canvas
         :param section: the section (action) that was taken to generate this image. section is a deprecated name
         :param data: the data to update the image with
         :param processed_image: the image to update the canvas with
         :return:
         """
+        processed_image = processed_image.convert("RGBA")
         section = data["action"] if not section else section
         outpaint_box_rect = data["options"]["outpaint_box_rect"]
         processed_image, image_root_point, image_pivot_point = self.handle_outpaint(
             outpaint_box_rect, processed_image, section
         )
         history_event = {
             "event": "set_image",
```

### Comparing `airunner-1.9.3/src/airunner/runai_client.py` & `airunner-1.9.4/src/airunner/runai_client.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/settingsmanager.py` & `airunner-1.9.4/src/airunner/settingsmanager.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner/utils.py` & `airunner-1.9.4/src/airunner/utils.py`

 * *Files identical despite different names*

### Comparing `airunner-1.9.3/src/airunner.egg-info/PKG-INFO` & `airunner-1.9.4/src/airunner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airunner
-Version: 1.9.3
+Version: 1.9.4
 Summary: A Stable Diffusion GUI
 Home-page: https://github.com/Capsize-Games/airunner
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

