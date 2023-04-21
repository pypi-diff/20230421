# Comparing `tmp/mikan_card_downloader-0.1.3.tar.gz` & `tmp/mikan_card_downloader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-0.1.3.tar", max compression
+gzip compressed data, was "mikan_card_downloader-0.2.0.tar", max compression
```

## Comparing `mikan_card_downloader-0.1.3.tar` & `mikan_card_downloader-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.1.3/LICENSE
--rw-r--r--   0        0        0     1084 2023-04-21 03:37:45.982634 mikan_card_downloader-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/__init__.py
--rw-r--r--   0        0        0     3952 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/classes.py
--rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-0.1.3/src/mikan/config.py
--rw-r--r--   0        0        0      153 2023-04-20 13:43:15.292485 mikan_card_downloader-0.1.3/src/mikan/default_config.cfg
--rw-r--r--   0        0        0     4984 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/downloader.py
--rw-r--r--   0        0        0     7007 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1629 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2095 2023-04-21 03:29:22.382978 mikan_card_downloader-0.1.3/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.3/src/mikan/py.typed
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.3/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1041 2023-04-21 04:15:33.143336 mikan_card_downloader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/__init__.py
+-rw-r--r--   0        0        0     3952 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/classes.py
+-rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-0.2.0/src/mikan/config.py
+-rw-r--r--   0        0        0     4984 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/downloader.py
+-rw-r--r--   0        0        0     7007 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1629 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2095 2023-04-21 03:29:22.382978 mikan_card_downloader-0.2.0/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/py.typed
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.2.0/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.2.0/PKG-INFO
```

### Comparing `mikan_card_downloader-0.1.3/LICENSE` & `mikan_card_downloader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/pyproject.toml` & `mikan_card_downloader-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "0.1.3"
+version = "0.2.0"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
-include = ["src/mikan/default_config.cfg"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.11.1"
 aiohttp = "^3.8.4"
 lxml = "^4.9.1"
 tqdm = "^4.64.0"
```

### Comparing `mikan_card_downloader-0.1.3/src/mikan/classes.py` & `mikan_card_downloader-0.2.0/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/src/mikan/config.py` & `mikan_card_downloader-0.2.0/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/src/mikan/downloader.py` & `mikan_card_downloader-0.2.0/src/mikan/downloader.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/src/mikan/html_parser.py` & `mikan_card_downloader-0.2.0/src/mikan/html_parser.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/src/mikan/json_utils.py` & `mikan_card_downloader-0.2.0/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/src/mikan/main.py` & `mikan_card_downloader-0.2.0/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.3/setup.py` & `mikan_card_downloader-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tqdm>=4.64.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['mikan = mikan.main:main']}
 
 setup_kwargs = {
     'name': 'mikan-card-downloader',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'Downloads cards and stills from SIFAS and SIF.',
     'long_description': 'None',
     'author': 'DemonicSavage',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

