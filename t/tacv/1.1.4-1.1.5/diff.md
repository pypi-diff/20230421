# Comparing `tmp/tacv-1.1.4.tar.gz` & `tmp/tacv-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacv-1.1.4.tar", last modified: Fri Jul 29 02:25:28 2022, max compression
+gzip compressed data, was "tacv-1.1.5.tar", last modified: Fri Apr 21 03:50:37 2023, max compression
```

## Comparing `tacv-1.1.4.tar` & `tacv-1.1.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/
--rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.4/LICENSE
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2022-07-29 02:25:28.202945 tacv-1.1.4/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     6908 2022-07-29 02:23:53.000000 tacv-1.1.4/README.md
--rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.4/pyproject.toml
--rw-rw-r--   0 tu        (1000) tu        (1000)       32 2022-07-26 16:30:33.000000 tacv-1.1.4/requirements.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)      200 2022-07-29 02:25:28.202945 tacv-1.1.4/setup.cfg
--rw-rw-r--   0 tu        (1000) tu        (1000)     1820 2022-07-29 02:25:20.000000 tacv-1.1.4/setup.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.198944 tacv-1.1.4/tacv/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.198944 tacv-1.1.4/tacv/cli/
--rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/cli/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/cli/cli.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.4/tacv/detection/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/centernet/
--rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.4/tacv/detection/centernet/CenterNet.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/Trainer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.4/tacv/detection/centernet/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/centernet/backbones/
--rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/backbones/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/backbones/resnet.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/centernet/heads/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/heads/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/centernet/losses/
--rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/losses/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/losses/losses.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/detection/centernet/utils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.4/tacv/detection/centernet/utils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/utils/common.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/utils/data_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/utils/geometry_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.4/tacv/detection/centernet/utils/infer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/utils/lightning_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.4/tacv/detection/centernet/utils/pytorch_model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/fileUtils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       24 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/fileUtils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/fileUtils/fileutils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/geometry/
--rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/geometry/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/geometry/iou.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/resources/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/resources/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/torch/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/torch/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/torch/model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/video/
--rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/video/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/video/video_proc.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.202945 tacv-1.1.4/tacv/visual/
--rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/visual/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.4/tacv/visual/draw2d.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2022-07-29 02:25:28.198944 tacv-1.1.4/tacv.egg-info/
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     1245 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        1 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       92 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/entry_points.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       33 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/requires.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        5 2022-07-29 02:25:28.000000 tacv-1.1.4/tacv.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.5/LICENSE
+-rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-04-21 03:50:37.357515 tacv-1.1.5/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     6908 2022-07-29 02:23:53.000000 tacv-1.1.5/README.md
+-rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.5/pyproject.toml
+-rw-rw-r--   0 tu        (1000) tu        (1000)       32 2022-07-26 16:30:33.000000 tacv-1.1.5/requirements.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)      200 2023-04-21 03:50:37.357515 tacv-1.1.5/setup.cfg
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1838 2023-04-21 03:50:30.000000 tacv-1.1.5/setup.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.353515 tacv-1.1.5/tacv/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/cli/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/cli/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/cli/cli.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.5/tacv/detection/centernet/CenterNet.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/Trainer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/centernet/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/backbones/
+-rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/backbones/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/backbones/resnet.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/heads/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/heads/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/losses/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/losses/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/losses/losses.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/detection/centernet/utils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.5/tacv/detection/centernet/utils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/common.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/data_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/geometry_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.5/tacv/detection/centernet/utils/infer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/lightning_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.5/tacv/detection/centernet/utils/pytorch_model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/fileUtils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       72 2023-04-21 02:49:52.000000 tacv-1.1.5/tacv/fileUtils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/fileUtils/fileutils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     5615 2023-04-21 03:48:04.000000 tacv-1.1.5/tacv/fileUtils/thread_downloader.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/geometry/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/geometry/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/geometry/iou.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/resources/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/resources/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/torch/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/torch/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/torch/model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/video/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/video/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/video/video_proc.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv/visual/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/visual/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.5/tacv/visual/draw2d.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-04-21 03:50:37.357515 tacv-1.1.5/tacv.egg-info/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1281 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/SOURCES.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/dependency_links.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       92 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/entry_points.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       33 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/requires.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        5 2023-04-21 03:50:37.000000 tacv-1.1.5/tacv.egg-info/top_level.txt
```

### Comparing `tacv-1.1.4/LICENSE` & `tacv-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/PKG-INFO` & `tacv-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tacv-1.1.4/README.md` & `tacv-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/setup.py` & `tacv-1.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from setuptools import setup
 import setuptools
 import os
 
+
 def read_version_int(version_file_path):
     if not os.path.exists(version_file_path):
         return None
-    with open(version_file_path,"r") as version_file:
+    with open(version_file_path, "r") as version_file:
         text = version_file.readlines()[0]
         version_file.close()
         batches = text.split(".")
         batches = [int(batch) for batch in batches]
         return batches
 
+
 def increase_version_by_one(version_file_path):
     batches = read_version_int(version_file_path)
     if batches is None:
         return
     batch1, batch2, batch3 = batches
     batch3 += 1
     if batch3 >= 10:
         batch3 = batch3 % 10
         batch2 += 1
         if batch2 >= 10:
             batch1 = batch1 + 1
-    version_file = open(version_file_path,"w+")
-    new_ver = str(batch1)+"."+str(batch2)+"."+str(batch3)
-    version_file.write(new_ver+"\n")
+    version_file = open(version_file_path, "w+")
+    new_ver = str(batch1) + "." + str(batch2) + "." + str(batch3)
+    version_file.write(new_ver + "\n")
     version_file.close()
     return new_ver
 
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r") as f:
     lines = f.readlines()
     required_pkgs = [item.strip() for item in lines]
 
-#version_file = "tacv/resources/version.txt"
-new_ver = "1.1.4" #increase_version_by_one(version_file)
+# version_file = "tacv/resources/version.txt"
+new_ver = "1.1.5"  # increase_version_by_one(version_file)
 print(f"Building {new_ver}")
 setup(
     name='tacv',
     version=new_ver,
     packages=setuptools.find_packages(where="."),
     url='https://github.com/TaQuangTu/TaCV',
     license='LICENSE',
```

### Comparing `tacv-1.1.4/tacv/detection/centernet/CenterNet.py` & `tacv-1.1.5/tacv/detection/centernet/CenterNet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/Trainer.py` & `tacv-1.1.5/tacv/detection/centernet/Trainer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/backbones/resnet.py` & `tacv-1.1.5/tacv/detection/centernet/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/losses/losses.py` & `tacv-1.1.5/tacv/detection/centernet/losses/losses.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/utils/data_utils.py` & `tacv-1.1.5/tacv/detection/centernet/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/utils/geometry_utils.py` & `tacv-1.1.5/tacv/detection/centernet/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/detection/centernet/utils/infer.py` & `tacv-1.1.5/tacv/detection/centernet/utils/infer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/fileUtils/fileutils.py` & `tacv-1.1.5/tacv/fileUtils/fileutils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/geometry/iou.py` & `tacv-1.1.5/tacv/geometry/iou.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/torch/model_utils.py` & `tacv-1.1.5/tacv/torch/model_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/video/video_proc.py` & `tacv-1.1.5/tacv/video/video_proc.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv/visual/draw2d.py` & `tacv-1.1.5/tacv/visual/draw2d.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.4/tacv.egg-info/PKG-INFO` & `tacv-1.1.5/tacv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
 Author: TaQuangTu
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tacv-1.1.4/tacv.egg-info/SOURCES.txt` & `tacv-1.1.5/tacv.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 tacv/detection/centernet/utils/data_utils.py
 tacv/detection/centernet/utils/geometry_utils.py
 tacv/detection/centernet/utils/infer.py
 tacv/detection/centernet/utils/lightning_utils.py
 tacv/detection/centernet/utils/pytorch_model_utils.py
 tacv/fileUtils/__init__.py
 tacv/fileUtils/fileutils.py
+tacv/fileUtils/thread_downloader.py
 tacv/geometry/__init__.py
 tacv/geometry/iou.py
 tacv/resources/__init__.py
 tacv/torch/__init__.py
 tacv/torch/model_utils.py
 tacv/video/__init__.py
 tacv/video/video_proc.py
```

