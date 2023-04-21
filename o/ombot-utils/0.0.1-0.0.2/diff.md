# Comparing `tmp/ombot_utils-0.0.1.tar.gz` & `tmp/ombot_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/zl/proj/ombot_utils/dist/.tmp-rklz9qmp/ombot_utils-0.0.1.tar", last modified: Thu Apr 20 10:33:47 2023, max compression
+gzip compressed data, was "/data/zl/proj/ombot_utils/dist/.tmp-2xgn9av8/ombot_utils-0.0.2.tar", last modified: Fri Apr 21 00:58:19 2023, max compression
```

## Comparing `ombot_utils-0.0.1.tar` & `ombot_utils-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/
--rw-rw-r--   0 zl        (2005) zl        (2005)     1073 2023-04-20 10:22:33.000000 ombot_utils-0.0.1/LICENSE
--rw-rw-r--   0 zl        (2005) zl        (2005)     3369 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/PKG-INFO
--rw-rw-r--   0 zl        (2005) zl        (2005)     2925 2023-04-20 10:21:39.000000 ombot_utils-0.0.1/README.md
--rw-rw-r--   0 zl        (2005) zl        (2005)      561 2023-04-20 10:33:02.000000 ombot_utils-0.0.1/pyproject.toml
--rw-rw-r--   0 zl        (2005) zl        (2005)       38 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/setup.cfg
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/
--rw-rw-r--   0 zl        (2005) zl        (2005)      169 2023-04-20 09:50:41.000000 ombot_utils-0.0.1/src/ombot_utils/__init__.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/callback_handler/
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-20 09:26:03.000000 ombot_utils-0.0.1/src/ombot_utils/callback_handler/__init__.py
--rw-rw-r--   0 zl        (2005) zl        (2005)     2516 2023-04-20 09:49:49.000000 ombot_utils-0.0.1/src/ombot_utils/callback_handler/callback.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/data_handler/
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-18 08:44:25.000000 ombot_utils-0.0.1/src/ombot_utils/data_handler/__init__.py
--rw-rw-r--   0 zl        (2005) zl        (2005)      325 2023-04-20 07:16:11.000000 ombot_utils-0.0.1/src/ombot_utils/data_handler/base_sql_data_handler.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/error_handler/
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-20 09:26:51.000000 ombot_utils-0.0.1/src/ombot_utils/error_handler/__init__.py
--rw-rw-r--   0 zl        (2005) zl        (2005)     4668 2023-04-20 10:00:54.000000 ombot_utils-0.0.1/src/ombot_utils/error_handler/error.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/log_handler/
--rw-rw-r--   0 zl        (2005) zl        (2005)       69 2023-04-20 09:50:17.000000 ombot_utils-0.0.1/src/ombot_utils/log_handler/__init__.py
--rw-rw-r--   0 zl        (2005) zl        (2005)     1670 2023-04-19 11:56:12.000000 ombot_utils-0.0.1/src/ombot_utils/log_handler/logger.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/
--rw-rw-r--   0 zl        (2005) zl        (2005)      169 2023-04-19 08:07:46.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/__init__.py
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:09:42.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/character.py
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:08:21.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/event.py
--rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:08:11.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/memory.py
--rw-rw-r--   0 zl        (2005) zl        (2005)     3570 2023-04-20 10:19:44.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/message.py
--rw-rw-r--   0 zl        (2005) zl        (2005)      539 2023-04-19 08:06:22.000000 ombot_utils-0.0.1/src/ombot_utils/schemas/opt.py
-drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils.egg-info/
--rw-rw-r--   0 zl        (2005) zl        (2005)     3369 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils.egg-info/PKG-INFO
--rw-rw-r--   0 zl        (2005) zl        (2005)      766 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 zl        (2005) zl        (2005)        1 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 zl        (2005) zl        (2005)       12 2023-04-20 10:33:47.000000 ombot_utils-0.0.1/src/ombot_utils.egg-info/top_level.txt
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/
+-rw-rw-r--   0 zl        (2005) zl        (2005)     1073 2023-04-20 10:22:33.000000 ombot_utils-0.0.2/LICENSE
+-rw-rw-r--   0 zl        (2005) zl        (2005)     3362 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 zl        (2005) zl        (2005)     2925 2023-04-20 10:21:39.000000 ombot_utils-0.0.2/README.md
+-rw-rw-r--   0 zl        (2005) zl        (2005)      554 2023-04-21 00:57:13.000000 ombot_utils-0.0.2/pyproject.toml
+-rw-rw-r--   0 zl        (2005) zl        (2005)       38 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/setup.cfg
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/
+-rw-rw-r--   0 zl        (2005) zl        (2005)      170 2023-04-20 10:43:47.000000 ombot_utils-0.0.2/src/ombot_utils/__init__.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/callback_handler/
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-20 09:26:03.000000 ombot_utils-0.0.2/src/ombot_utils/callback_handler/__init__.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)     2509 2023-04-20 10:43:24.000000 ombot_utils-0.0.2/src/ombot_utils/callback_handler/callback.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/data_handler/
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-18 08:44:25.000000 ombot_utils-0.0.2/src/ombot_utils/data_handler/__init__.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)      325 2023-04-20 07:16:11.000000 ombot_utils-0.0.2/src/ombot_utils/data_handler/base_sql_data_handler.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/error_handler/
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-20 09:26:51.000000 ombot_utils-0.0.2/src/ombot_utils/error_handler/__init__.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)     4668 2023-04-20 10:00:54.000000 ombot_utils-0.0.2/src/ombot_utils/error_handler/error.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/log_handler/
+-rw-rw-r--   0 zl        (2005) zl        (2005)       69 2023-04-20 09:50:17.000000 ombot_utils-0.0.2/src/ombot_utils/log_handler/__init__.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)     1670 2023-04-19 11:56:12.000000 ombot_utils-0.0.2/src/ombot_utils/log_handler/logger.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/
+-rw-rw-r--   0 zl        (2005) zl        (2005)      169 2023-04-19 08:07:46.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/__init__.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:09:42.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/character.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:08:21.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/event.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)        0 2023-04-19 08:08:11.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/memory.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)     3570 2023-04-20 10:19:44.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/message.py
+-rw-rw-r--   0 zl        (2005) zl        (2005)      539 2023-04-19 08:06:22.000000 ombot_utils-0.0.2/src/ombot_utils/schemas/opt.py
+drwxrwxr-x   0 zl        (2005) zl        (2005)        0 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils.egg-info/
+-rw-rw-r--   0 zl        (2005) zl        (2005)     3362 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 zl        (2005) zl        (2005)      766 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 zl        (2005) zl        (2005)        1 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 zl        (2005) zl        (2005)       12 2023-04-21 00:58:19.000000 ombot_utils-0.0.2/src/ombot_utils.egg-info/top_level.txt
```

### Comparing `ombot_utils-0.0.1/LICENSE` & `ombot_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/PKG-INFO` & `ombot_utils-0.0.2/src/ombot_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ombot_utils
-Version: 0.0.1
-Summary: A small example package
+Name: ombot-utils
+Version: 0.0.2
+Summary: Utils for OMbots
 Author-email: panregedit <panregedit@gmail.com>
 Project-URL: Homepage, https://git.linker.cc/research/misc/ombot_utils.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ombot_utils-0.0.1/README.md` & `ombot_utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/pyproject.toml` & `ombot_utils-0.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0", "sqlmodel>=0.0.8", "pymysql>=1.0.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ombot_utils"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="panregedit", email="panregedit@gmail.com" },
 ]
-description = "A small example package"
+description = "Utils for OMbots"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ombot_utils-0.0.1/src/ombot_utils/callback_handler/callback.py` & `ombot_utils-0.0.2/src/ombot_utils/callback_handler/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from ..schemas import ChatRecords, Reply, Message, OPT
 from uuid import uuid4
 from time import time
 import json
-from ..log_handler.logger import logging
+from ..log_handler import logging
 from ..error_handler.error import VQLError
 import os
 from distutils.util import strtobool
 
 IS_DEBUG = strtobool(os.environ.get('IS_DEBUG', 'false'))
```

### Comparing `ombot_utils-0.0.1/src/ombot_utils/error_handler/error.py` & `ombot_utils-0.0.2/src/ombot_utils/error_handler/error.py`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/src/ombot_utils/log_handler/logger.py` & `ombot_utils-0.0.2/src/ombot_utils/log_handler/logger.py`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/src/ombot_utils/schemas/message.py` & `ombot_utils-0.0.2/src/ombot_utils/schemas/message.py`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/src/ombot_utils/schemas/opt.py` & `ombot_utils-0.0.2/src/ombot_utils/schemas/opt.py`

 * *Files identical despite different names*

### Comparing `ombot_utils-0.0.1/src/ombot_utils.egg-info/PKG-INFO` & `ombot_utils-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ombot-utils
-Version: 0.0.1
-Summary: A small example package
+Name: ombot_utils
+Version: 0.0.2
+Summary: Utils for OMbots
 Author-email: panregedit <panregedit@gmail.com>
 Project-URL: Homepage, https://git.linker.cc/research/misc/ombot_utils.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ombot_utils-0.0.1/src/ombot_utils.egg-info/SOURCES.txt` & `ombot_utils-0.0.2/src/ombot_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

