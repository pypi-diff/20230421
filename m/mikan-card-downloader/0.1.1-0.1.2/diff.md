# Comparing `tmp/mikan_card_downloader-0.1.1.tar.gz` & `tmp/mikan_card_downloader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-0.1.1.tar", max compression
+gzip compressed data, was "mikan_card_downloader-0.1.2.tar", max compression
```

## Comparing `mikan_card_downloader-0.1.1.tar` & `mikan_card_downloader-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.1.1/LICENSE
--rw-r--r--   0        0        0      153 2023-04-20 13:43:15.292485 mikan_card_downloader-0.1.1/default_config.cfg
--rw-r--r--   0        0        0     1074 2023-04-20 20:58:11.950927 mikan_card_downloader-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/__init__.py
--rw-r--r--   0        0        0     3952 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/classes.py
--rw-r--r--   0        0        0      947 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/config.py
--rw-r--r--   0        0        0     4984 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/downloader.py
--rw-r--r--   0        0        0     7007 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1629 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     1719 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.1/src/mikan/py.typed
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.1/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1084 2023-04-20 21:18:21.869103 mikan_card_downloader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/__init__.py
+-rw-r--r--   0        0        0     3952 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/classes.py
+-rw-r--r--   0        0        0     1028 2023-04-20 21:17:48.829303 mikan_card_downloader-0.1.2/src/mikan/config.py
+-rw-r--r--   0        0        0      153 2023-04-20 13:43:15.292485 mikan_card_downloader-0.1.2/src/mikan/default_config.cfg
+-rw-r--r--   0        0        0     4984 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/downloader.py
+-rw-r--r--   0        0        0     7007 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1629 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     1719 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.1.2/src/mikan/py.typed
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.2/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.1.2/PKG-INFO
```

### Comparing `mikan_card_downloader-0.1.1/LICENSE` & `mikan_card_downloader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/pyproject.toml` & `mikan_card_downloader-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "0.1.1"
+version = "0.1.2"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
-include = ["default_config.cfg"]
+include = ["src/mikan/default_config.cfg"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.11.1"
 aiohttp = "^3.8.4"
 lxml = "^4.9.1"
 tqdm = "^4.64.0"
```

### Comparing `mikan_card_downloader-0.1.1/src/mikan/classes.py` & `mikan_card_downloader-0.1.2/src/mikan/classes.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/src/mikan/config.py` & `mikan_card_downloader-0.1.2/src/mikan/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 
 import configparser
 import shutil
 from pathlib import Path
+import os
 
 import platformdirs
 
+ROOT_DIR = os.path.dirname(os.path.abspath(__file__))
 cfg = configparser.ConfigParser()
 
 cfg_dir = Path(platformdirs.user_config_dir("mikan", ensure_exists=True))
 cfg_file = cfg_dir / "config.cfg"
 
 if not cfg_file.exists():
-    shutil.copy("default_config.cfg", cfg_file)
+    shutil.copy(Path(ROOT_DIR) / "default_config.cfg", cfg_file)
 
 cfg.read(cfg_dir / "config.cfg")
 
 CARDS_DIR = Path(cfg["Paths"]["data_dir"])
```

### Comparing `mikan_card_downloader-0.1.1/src/mikan/downloader.py` & `mikan_card_downloader-0.1.2/src/mikan/downloader.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/src/mikan/html_parser.py` & `mikan_card_downloader-0.1.2/src/mikan/html_parser.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/src/mikan/json_utils.py` & `mikan_card_downloader-0.1.2/src/mikan/json_utils.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/src/mikan/main.py` & `mikan_card_downloader-0.1.2/src/mikan/main.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.1.1/setup.py` & `mikan_card_downloader-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tqdm>=4.64.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['mikan = mikan.main:main']}
 
 setup_kwargs = {
     'name': 'mikan-card-downloader',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Downloads cards and stills from SIFAS and SIF.',
     'long_description': 'None',
     'author': 'DemonicSavage',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mikan_card_downloader-0.1.1/PKG-INFO` & `mikan_card_downloader-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 0.1.1
+Version: 0.1.2
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

