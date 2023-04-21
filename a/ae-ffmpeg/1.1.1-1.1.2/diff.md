# Comparing `tmp/ae-ffmpeg-1.1.1.tar.gz` & `tmp/ae-ffmpeg-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ae-ffmpeg-1.1.1.tar", last modified: Fri Sep  2 18:30:22 2022, max compression
+gzip compressed data, was "ae-ffmpeg-1.1.2.tar", last modified: Fri Apr 21 19:23:31 2023, max compression
```

## Comparing `ae-ffmpeg-1.1.1.tar` & `ae-ffmpeg-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 18:30:22.334492 ae-ffmpeg-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     7817 2022-09-02 18:29:40.000000 ae-ffmpeg-1.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-09-02 18:30:22.334492 ae-ffmpeg-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-09-02 18:29:40.000000 ae-ffmpeg-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 18:30:22.330491 ae-ffmpeg-1.1.1/ae_ffmpeg/
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-09-02 18:29:41.000000 ae-ffmpeg-1.1.1/ae_ffmpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-02 18:29:41.000000 ae-ffmpeg-1.1.1/ae_ffmpeg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 18:30:22.334492 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-09-02 18:30:22.000000 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-02 18:30:22.000000 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 18:30:22.000000 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 18:29:51.000000 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-02 18:30:22.000000 ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-02 18:30:22.334492 ae-ffmpeg-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-09-02 18:29:41.000000 ae-ffmpeg-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:31.839658 ae-ffmpeg-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-21 19:22:53.000000 ae-ffmpeg-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-21 19:23:31.839658 ae-ffmpeg-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-21 19:22:53.000000 ae-ffmpeg-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:31.839658 ae-ffmpeg-1.1.2/ae_ffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-21 19:22:54.000000 ae-ffmpeg-1.1.2/ae_ffmpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:22:54.000000 ae-ffmpeg-1.1.2/ae_ffmpeg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:31.839658 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-21 19:23:31.000000 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-21 19:23:31.000000 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:23:31.000000 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:23:07.000000 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 19:23:31.000000 ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:23:31.839658 ae-ffmpeg-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-21 19:22:54.000000 ae-ffmpeg-1.1.2/setup.py
```

### Comparing `ae-ffmpeg-1.1.1/LICENSE.txt` & `ae-ffmpeg-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ae-ffmpeg-1.1.1/PKG-INFO` & `ae-ffmpeg-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ae-ffmpeg
-Version: 1.1.1
+Version: 1.1.2
 Summary: Static FFmpeg binaries for Auto-Editor
 Home-page: https://auto-editor.com
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: LGPLv3
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
@@ -26,15 +26,15 @@
 
 ## Install
 ```
 pip install ae-ffmpeg
 ```
 
 ## Copyright
-THe FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
+The FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
 
 ## How to Compile on MacOS
 Use https://github.com/WyattBlue/ffmpeg-build-script/
 
 ## How to Compile on Windows
 I use https://github.com/m-ab-s/media-autobuild_suite to compile on Windows.
```

### Comparing `ae-ffmpeg-1.1.1/README.md` & `ae-ffmpeg-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ## Install
 ```
 pip install ae-ffmpeg
 ```
 
 ## Copyright
-THe FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
+The FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
 
 ## How to Compile on MacOS
 Use https://github.com/WyattBlue/ffmpeg-build-script/
 
 ## How to Compile on Windows
 I use https://github.com/m-ab-s/media-autobuild_suite to compile on Windows.
```

### Comparing `ae-ffmpeg-1.1.1/ae_ffmpeg.egg-info/PKG-INFO` & `ae-ffmpeg-1.1.2/ae_ffmpeg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ae-ffmpeg
-Version: 1.1.1
+Version: 1.1.2
 Summary: Static FFmpeg binaries for Auto-Editor
 Home-page: https://auto-editor.com
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: LGPLv3
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
@@ -26,15 +26,15 @@
 
 ## Install
 ```
 pip install ae-ffmpeg
 ```
 
 ## Copyright
-THe FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
+The FFmpeg/FFprobe binaires used are under the LGPLv3. Only libraries that are compatible with the LGPLv3 are included.
 
 ## How to Compile on MacOS
 Use https://github.com/WyattBlue/ffmpeg-build-script/
 
 ## How to Compile on Windows
 I use https://github.com/m-ab-s/media-autobuild_suite to compile on Windows.
```

### Comparing `ae-ffmpeg-1.1.1/setup.py` & `ae-ffmpeg-1.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 
 def pip_version():
     with open("ae_ffmpeg/__init__.py") as f:
         version_content = f.read()
 
     version_match = re.search(
@@ -12,15 +13,15 @@
 
     if version_match:
         return version_match.group(1)
 
     raise ValueError("Unable to find version string.")
 
 
-with open("README.md", "r") as f:
+with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="ae-ffmpeg",
     version=pip_version(),
     description="Static FFmpeg binaries for Auto-Editor",
     long_description=long_description,
```

