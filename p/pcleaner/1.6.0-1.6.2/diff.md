# Comparing `tmp/pcleaner-1.6.0.tar.gz` & `tmp/pcleaner-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.6.0.tar", last modified: Tue Apr 18 20:41:45 2023, max compression
+gzip compressed data, was "pcleaner-1.6.2.tar", last modified: Fri Apr 21 16:14:32 2023, max compression
```

## Comparing `pcleaner-1.6.0.tar` & `pcleaner-1.6.2.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.6.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-18 20:41:45.614643 pcleaner-1.6.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.6.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.607976 pcleaner-1.6.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-18 20:40:27.000000 pcleaner-1.6.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    17227 2023-04-18 15:30:05.000000 pcleaner-1.6.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.6.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.6.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    36360 2023-04-18 15:36:00.000000 pcleaner-1.6.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.6.0/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.6.0/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.6.0/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1076 2023-04-18 01:52:48.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3206 2022-08-27 14:37:25.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.6.0/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.6.0/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.6.0/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.6.0/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35231 2023-04-18 16:17:08.000000 pcleaner-1.6.0/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2938 2023-04-18 16:38:05.000000 pcleaner-1.6.0/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    80116 2023-04-18 01:36:08.000000 pcleaner-1.6.0/pcleaner/gui/rc_generated_files/icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.614643 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    29181 2023-04-18 18:34:09.000000 pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.6.0/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.6.0/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23327 2023-04-18 15:30:05.000000 pcleaner-1.6.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    26399 2023-04-18 20:02:05.000000 pcleaner-1.6.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.6.0/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.6.0/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-04-18 20:36:25.000000 pcleaner-1.6.0/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.6.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.6.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-18 20:41:45.611310 pcleaner-1.6.0/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11664 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1945 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-18 20:41:45.000000 pcleaner-1.6.0/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.6.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1058 2023-04-18 20:41:45.614643 pcleaner-1.6.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.6.0/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.6.2/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11713 2023-04-21 16:14:32.144190 pcleaner-1.6.2/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11039 2023-04-12 00:54:25.000000 pcleaner-1.6.2/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-04-21 14:42:06.000000 pcleaner-1.6.2/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-04-21 13:38:35.000000 pcleaner-1.6.2/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5841 2023-04-14 16:52:21.000000 pcleaner-1.6.2/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    40890 2023-04-21 14:58:00.000000 pcleaner-1.6.2/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.6.2/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.6.2/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.6.2/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.6.2/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.6.2/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2573 2023-04-21 14:17:14.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1104 2023-04-21 15:08:03.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.6.2/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.6.2/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-04-17 02:04:01.000000 pcleaner-1.6.2/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1904 2023-04-17 01:26:57.000000 pcleaner-1.6.2/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    36580 2023-04-21 14:12:49.000000 pcleaner-1.6.2/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    15167 2023-04-21 15:23:47.000000 pcleaner-1.6.2/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    82099 2023-04-21 14:48:43.000000 pcleaner-1.6.2/pcleaner/gui/rc_generated_files/icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.140857 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    29657 2023-04-21 14:26:59.000000 pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-04-17 16:45:08.000000 pcleaner-1.6.2/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1321 2023-04-17 02:10:39.000000 pcleaner-1.6.2/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23339 2023-04-20 18:43:01.000000 pcleaner-1.6.2/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    26308 2023-04-20 18:43:01.000000 pcleaner-1.6.2/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.6.2/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.6.2/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-04-18 20:36:25.000000 pcleaner-1.6.2/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7546 2023-01-23 03:12:00.000000 pcleaner-1.6.2/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.6.2/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-04-21 16:14:32.137524 pcleaner-1.6.2/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11713 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2058 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-04-21 16:14:32.000000 pcleaner-1.6.2/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.6.2/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-04-21 16:14:32.144190 pcleaner-1.6.2/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.6.2/setup.py
```

### Comparing `pcleaner-1.6.0/LICENSE` & `pcleaner-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/PKG-INFO` & `pcleaner-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.6.0
+Version: 1.6.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # Panel Cleaner
```

### Comparing `pcleaner-1.6.0/README.md` & `pcleaner-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/analytics.py` & `pcleaner-1.6.2/pcleaner/analytics.py`

 * *Files 25% similar despite different names*

```diff
@@ -435,7 +435,15 @@
             prefix = prefix[:-1]
             if not prefix:
                 return ""
     # If the prefix doesnt exist, cut away the mangled directory name.
     if not Path(prefix).exists():
         prefix = str(Path(prefix).parent)
     return prefix
+
+
+""" Analytics HTML template
+<html><head><meta name="qrichtext" content="1" /><style type="text/css">
+p, li { white-space: pre-wrap; font-family: Noto Mono, Monospace; size: 12pt}
+</style></head><body>
+<p style=" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;"><span style=" ">Mask Fitment Analytics <br />---------------------- <br />Total boxes: 5 | Masks succeeded: 5 (100%) | Masks failed: </span><span style="color:#b21818;">0</span><span style=" "> <br />Perfect masks: </span><span style="color:#18b2b2;">5</span><span style=" "> (100%) | Average border deviation: 0.00 <br /><br />Mask usage by mask size (smallest to largest): <br />Mask 0  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 1  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 2  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 3  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 4  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 5  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 6  : </span><span style="color:#18b2b2;">████████████████████████████████████████</span><span style=" "> </span><span style="color:#18b2b2;">1</span><span style=" "> / 1 <br />Mask 7  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 8  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 9  :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Mask 10 :  </span><span style="color:#18b2b2;">0</span><span style=" "> / 0 <br />Box mask: </span><span style="color:#18b2b2;">████████████████████████████████████████</span><span style=" "> </span><span style="color:#18b2b2;">4</span><span style=" "> / 4 <br /><br /></span><span style="color:#18b2b2;">█ Perfect</span><span style=" "> | █ Total<br /><br /></span></p></body></html>
+"""
```

### Comparing `pcleaner-1.6.0/pcleaner/cli_utils.py` & `pcleaner-1.6.2/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.6.2/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/config.py` & `pcleaner-1.6.2/pcleaner/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,123 +1,147 @@
+import re
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
+from typing import Any, NewType
 
 import configupdater as cu
 from logzero import logger
 
 from pcleaner import cli_utils as cli
 from pcleaner import model_downloader as md
 
+RESERVED_PROFILE_NAMES = ["builtin", "none", "default"]
 
-RESERVED_PROFILE_NAMES = ["builtin", "none"]
+# Supported image suffixes.
+SUPPORTED_IMG_TYPES = [
+    ".jpeg",
+    ".jpg",
+    ".png",
+    ".bmp",
+    ".tiff",
+    ".tif",
+    ".jp2",
+    ".dib",
+    ".webp",
+    ".ppm",
+]
+SUPPORTED_MASK_TYPES = [".png", ".bmp", ".tiff", ".tif", ".dib", ".webp", ".ppm"]
+
+# Create a dummy type to signify numbers need to be greater than 0.
+GreaterZero = NewType("GreaterZero", int)
 
 
 @dataclass
 class GeneralConfig:
     preferred_file_type: str | None = None
-    preferred_mask_file_type: str | None = None
-    input_size_scale: float = 1.0
+    preferred_mask_file_type: str = ".png"
+    input_size_scale: float | GreaterZero = 1.0
 
-    def export_to_conf(self, config_updater: cu.ConfigUpdater) -> None:
+    def export_to_conf(self, config_updater: cu.ConfigUpdater, gui_mode: bool = False) -> None:
         """
         Write the config to the config updater object.
 
         No add_after_section here since it is the first section.
 
         :param config_updater: An existing config updater object.
+        :param gui_mode: Whether the config is being exported for the GUI.
         """
 
         config_str = f"""\
         [General]
         
         # Preferred file type to save the cleaned image as.
-        # If no file type is specified, the original file type will be used.
+        [CLI: # If no file type is specified, the original file type will be used.]
         preferred_file_type = {self.preferred_file_type if self.preferred_file_type else ""}
 
         # Preferred file type to save the mask as.
-        # If no file type is specified, png will be used.
-        # This is because the mask image must use transparency, which is not supported by all image formats.
+        # Only image formats that allow for transparency are supported.
         preferred_mask_file_type = {self.preferred_mask_file_type if self.preferred_mask_file_type else ""}
         
         # Scale the input image by this amount before processing.
         # This is useful for significantly speeding up processing on large images.
         # The image will be scaled down, processed, and then only the mask is scaled back up.
         # Meaning that the cleaned output will still use the original, unscaled image to prevent any loss in quality.
         # Images larger than 3000x3000 pixels should be scaled down, so that they fall within this range.
         # E.g. an Image with the size 7000x10000 pixels should be scaled down with a factor of 0.25,
         # so that it has the size 1750x2500 pixels during processing.
         # The default value is 1.0, which means no scaling.
         input_size_scale = {self.input_size_scale}
         
         """
-        config_updater.read_string(multi_left_strip(config_str))
+        config_updater.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
         section = "General"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, section, str | None, "preferred_file_type")
-        try_to_load(self, config_updater, section, str | None, "preferred_mask_file_type")
-        try_to_load(self, config_updater, section, float, "input_size_scale")
+        try_to_load(self, config_updater, section, str, "preferred_mask_file_type")
+        try_to_load(self, config_updater, section, float | GreaterZero, "input_size_scale")
 
 
 @dataclass
 class TextDetectorConfig:
     model_path: str | None = None
-    concurrent_models: int = 1
+    concurrent_models: int | GreaterZero = 1
 
-    def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
+    def export_to_conf(
+        self, config_updater: cu.ConfigUpdater, add_after_section: str, gui_mode: bool = False
+    ) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the config after.
+        :param gui_mode: Whether the config is being exported for the GUI.
         """
 
         config_str = f"""\
         [TextDetector]
         
         # Path to the text detection model, leave empty to use the built-in model.
-        # The model can be found here:
-        # https://github.com/zyddnys/manga-image-translator/releases/latest
+        [CLI: # You can download older versions of the model here:]
+        [CLI: # https://github.com/zyddnys/manga-image-translator/releases/latest]
+        [GUI: # You can download older versions of the model ]
+        [GUI: # <a href="https://github.com/zyddnys/manga-image-translator/releases/latest">here.</a>]
         model_path = {none_to_empty(self.model_path)}
         
         # Number of models to run in parallel. This is useful if you have enough RAM
         # (or VRAM with CUDA) to run multiple models at the same time.
         # This, of course, will increase the speed of the process, but can also
         # crash your computer if you overestimate your hardware.
         # I recommend using 1 model per 2 GB of memory available.
         concurrent_models = {self.concurrent_models}
         
         """
         detector_conf = cu.ConfigUpdater()
-        detector_conf.read_string(multi_left_strip(config_str))
+        detector_conf.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
         general_section = detector_conf["TextDetector"]
         config_updater[add_after_section].add_after.space(2).section(general_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
         if not config_updater.has_section("TextDetector"):
             logger.info("No TextDetector section found in the profile, using defaults.")
             return
 
         try_to_load(self, config_updater, "TextDetector", str | None, "model_path")
-        try_to_load(self, config_updater, "TextDetector", int, "concurrent_models")
+        try_to_load(self, config_updater, "TextDetector", int | GreaterZero, "concurrent_models")
 
 
 @dataclass
 class PreProcessorConfig:
     box_min_size: int = 20 * 20
     suspicious_box_min_size: int = 200 * 200
     ocr_enabled: bool = True
@@ -125,72 +149,75 @@
     ocr_blacklist_pattern: str = "[～．ー！？０-９]*"
     box_padding_initial: int = 2
     box_right_padding_initial: int = 3
     box_padding_extended: int = 5
     box_right_padding_extended: int = 5
     box_reference_padding: int = 20
 
-    def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
+    def export_to_conf(
+        self, config_updater: cu.ConfigUpdater, add_after_section: str, gui_mode: bool = False
+    ) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the config after.
+        :param gui_mode: Whether the config is being exported for the GUI.
         """
         config_str = f"""\
         [PreProcessor]
         
         # Box sizes are given in the total number of pixels, so a box of 200x200 pixels has a size of 200 * 200 = 40000.
-        # To see these boxes visualized, use the --show-masks flag when cleaning and look inside the cache folder.
+        # [CLI: To see these boxes visualized, use the --show-masks flag when cleaning and look inside the cache folder.]
 
-        # Minimum size of any box to keep it. 
+        # Minimum size of any box to keep it.
         box_min_size = {self.box_min_size}
         
         # Minimum size of a box with "unknown" language to keep it. This language is typically assigned to logos and other
         # badly behaved text elements.
         suspicious_box_min_size = {self.suspicious_box_min_size}
         
         # Whether to use OCR to detect boxes that aren't worth cleaning, like ones that only contain numbers or symbols.
         ocr_enabled = {self.ocr_enabled}
         
         # Maximum size of a box to perform OCR on.
         # These useless boxes are usually small, and OCR is slow, so use this as a cutoff.
         ocr_max_size = {self.ocr_max_size}
         
-        # Regex pattern to match against OCR results. 
+        # Regex pattern to match against OCR results.
         # Anything matching this pattern is discarded.
         # Note that the OCR model returns full-width characters, so this pattern should match them.
         ocr_blacklist_pattern = {self.ocr_blacklist_pattern}
         
         # Padding to add to each side of a box.
         # This is added to the initial boxes created by the text detector AI.
-        # These boxes are visualized in green with the --cache-masks flag.
+        # These boxes are visualized in green[CLI:  with the --cache-masks flag].
         box_padding_initial = {self.box_padding_initial}
         
         # Padding to add to the right side of a box.
         # This extension helps to cover rubytext that floats off to the right of vertical text.
         box_right_padding_initial = {self.box_right_padding_initial}
         
         # Padding to add to each side of a box.
         # This is added to an extended set of boxes, used to cut out false positives by the text detector AI's mask.
-        # These boxes are visualized in purple with the --cache-masks flag.
+        # These boxes are visualized in purple[CLI:  with the --cache-masks flag].
         box_padding_extended = {self.box_padding_extended}
         
         # Padding to add to the right side of a box.
         # This extension helps to cover rubytext that floats off to the right of vertical text.
         box_right_padding_extended = {self.box_right_padding_extended}
         
         # Padding to add to each side of a box.
         # This is added to the reference boxes used to sample the original image while analyzing what mask to use.
-        # These boxes are visualized in blue with the --cache-masks flag.
+        # These boxes are visualized in blue[CLI:  with the --cache-masks flag].
         box_reference_padding = {self.box_reference_padding}
 
         """
         preproc_conf = cu.ConfigUpdater()
-        preproc_conf.read_string(multi_left_strip(config_str))
+        preproc_conf.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
         preproc_section = preproc_conf["PreProcessor"]
         config_updater[add_after_section].add_after.space(2).section(preproc_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
@@ -211,28 +238,31 @@
         try_to_load(self, config_updater, section, int, "box_padding_extended")
         try_to_load(self, config_updater, section, int, "box_right_padding_extended")
         try_to_load(self, config_updater, section, int, "box_reference_padding")
 
 
 @dataclass
 class MaskerConfig:
-    mask_growth_step_pixels: int = 2
+    mask_growth_step_pixels: int | GreaterZero = 2
     mask_growth_steps: int = 11
     off_white_max_threshold: int = 240
     mask_improvement_threshold: float = 0.1
     mask_selection_fast: bool = False
     mask_max_standard_deviation: float = 15
     debug_mask_color: tuple[int, int, int, int] = (108, 30, 240, 127)
 
-    def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
+    def export_to_conf(
+        self, config_updater: cu.ConfigUpdater, add_after_section: str, gui_mode: bool = False
+    ) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
+        :param gui_mode: Whether to format the config for the GUI.
         """
         config_str = f"""\
         [Masker]
         
         
         # Number of pixels to grow the mask by each step.
         # This bulks up the outline of the mask, so smaller values will be more accurate but slower.
@@ -254,44 +284,44 @@
         # which means it doesn't intersect any text or other objects.
         # Setting a higher value here requires a higher improvement to consider a smaller mask,
         # to give a preference to larger masks.
         mask_improvement_threshold = {self.mask_improvement_threshold}
         
         
         # Whether to use the fast mask selection algorithm.
-        # When true, the mask selection algorith with pick the first perfect mask, if one if found early.
+        # When true, the mask selection algorith will pick the first perfect mask, if one is found early.
         # This is faster, but may not find the best mask, if a slightly bigger one would have been better.
         mask_selection_fast = {self.mask_selection_fast}
         
         # The maximum standard deviation of a mask to consider.
         # A high value here means a higher tolerance for the mask intersecting text or other objects,
         # which isn't a good mask, as it will require inpainting anyway.
         mask_max_standard_deviation = {self.mask_max_standard_deviation}
         
-        # Color to use for the debug mask. This is a tuple of RGBA values.
+        # Color to use for the debug mask. [CLI: This is a tuple of RGBA values.]
         debug_mask_color = {','.join(map(str, self.debug_mask_color))}
         
         """
         masker_conf = cu.ConfigUpdater()
-        masker_conf.read_string(multi_left_strip(config_str))
+        masker_conf.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
         masker_section = masker_conf["Masker"]
         config_updater[add_after_section].add_after.space(2).section(masker_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
         :param config_updater: An existing config updater object.
         """
         section = "Masker"
         if not config_updater.has_section(section):
             logger.info(f"No {section} section found in the profile, using defaults.")
             return
 
-        try_to_load(self, config_updater, section, int, "mask_growth_step_pixels")
+        try_to_load(self, config_updater, section, int | GreaterZero, "mask_growth_step_pixels")
         try_to_load(self, config_updater, section, int, "mask_growth_steps")
         try_to_load(self, config_updater, section, int, "off_white_max_threshold")
         try_to_load(self, config_updater, section, float, "mask_improvement_threshold")
         try_to_load(self, config_updater, section, bool, "mask_selection_fast")
         try_to_load(self, config_updater, section, float, "mask_max_standard_deviation")
         try:
             color_tuple: tuple[int, ...] = tuple(
@@ -316,20 +346,23 @@
     colored_images: bool = False
     filter_strength: int = 10
     color_filter_strength: int = 10
     template_window_size: int = 7
     search_window_size: int = 21
     # TODO respect denoising enabled
 
-    def export_to_conf(self, config_updater: cu.ConfigUpdater, add_after_section: str) -> None:
+    def export_to_conf(
+        self, config_updater: cu.ConfigUpdater, add_after_section: str, gui_mode: bool = False
+    ) -> None:
         """
         Write the config to the config updater object.
 
         :param config_updater: An existing config updater object.
         :param add_after_section: The section to add the new section after.
+        :param gui_mode: Whether to format the config for the GUI.
         """
         config_str = f"""\
         [Denoiser]
         
         # When a bit of text is hard to mask off, the cleaning step likely had to choose a
         # small mask, which leaves a lot of jpeg-artifacts behind, if they were around the text.
         
@@ -369,15 +402,15 @@
         template_window_size = {self.template_window_size}
         
         # Size in pixels of the window that is used to compute weighted average for given pixel. Should be odd.
         search_window_size = {self.search_window_size}
         
         """
         denoiser_conf = cu.ConfigUpdater()
-        denoiser_conf.read_string(multi_left_strip(config_str))
+        denoiser_conf.read_string(multi_left_strip(format_for_version(config_str, gui_mode)))
         denoiser_section = denoiser_conf["Denoiser"]
         config_updater[add_after_section].add_after.space(2).section(denoiser_section.detach())
 
     def import_from_conf(self, config_updater: cu.ConfigUpdater) -> None:
         """
         Read the config from the config updater object.
 
@@ -406,24 +439,27 @@
 
     general: GeneralConfig = GeneralConfig()
     text_detector: TextDetectorConfig = TextDetectorConfig()
     pre_processor: PreProcessorConfig = PreProcessorConfig()
     masker: MaskerConfig = MaskerConfig()
     denoiser: DenoiserConfig = DenoiserConfig()
 
-    def bundle_config(self) -> cu.ConfigUpdater:
+    def bundle_config(self, gui_mode: bool = False) -> cu.ConfigUpdater:
         """
         Bundle the config into a ConfigUpdater object.
+
+        :param gui_mode: When true, strips out the CLI-specific options and keeps the GUI-specific ones,
+            and vice versa.
         """
         config_updater = cu.ConfigUpdater()
-        self.general.export_to_conf(config_updater)
-        self.text_detector.export_to_conf(config_updater, "General")
-        self.pre_processor.export_to_conf(config_updater, "TextDetector")
-        self.masker.export_to_conf(config_updater, "PreProcessor")
-        self.denoiser.export_to_conf(config_updater, "Masker")
+        self.general.export_to_conf(config_updater, gui_mode=gui_mode)
+        self.text_detector.export_to_conf(config_updater, "General", gui_mode=gui_mode)
+        self.pre_processor.export_to_conf(config_updater, "TextDetector", gui_mode=gui_mode)
+        self.masker.export_to_conf(config_updater, "PreProcessor", gui_mode=gui_mode)
+        self.denoiser.export_to_conf(config_updater, "Masker", gui_mode=gui_mode)
         return config_updater
 
     def write(self, path: Path) -> bool:
         """
         Write the profile to a file.
 
         :param path: The path to write the profile to.
@@ -455,14 +491,31 @@
             profile.denoiser.import_from_conf(config)
         except Exception as e:
             logger.error(f"Failed to load profile from {path}:\n{e}")
             profile = cls()
             print("Failed to load profile, using default profile.")
         return profile
 
+    def get(self, section: str, option: str) -> Any:
+        """
+        Get the value of a config option.
+        """
+        return getattr(getattr(self, section), option)
+
+    def set(self, section: str, option: str, value: Any) -> None:
+        """
+        Set the value of a config option.
+        """
+        # Check that the attribute exists.
+        if not hasattr(self, section):
+            raise AttributeError(f"No such section: {section}")
+        if not hasattr(getattr(self, section), option):
+            raise AttributeError(f"No such option: {option}")
+        setattr(getattr(self, section), option, value)
+
 
 @dataclass
 class Config:
     """
     The main configuration class.
     These setting are saved to disk.
 
@@ -830,14 +883,46 @@
             attr_value = float(conf_data)
         except ValueError as e:
             print(
                 f"Option {attr_name} in section {section} should be floating point number.\n"
                 f"Failed to parse '{conf_data}': {e}"
             )
             return
+    elif attr_type == int | GreaterZero:
+        # GreaterZero is just a signifier to check for positive numbers.
+        try:
+            attr_value = int(conf_data)
+        except ValueError as e:
+            print(
+                f"Option {attr_name} in section {section} should be an integer.\n"
+                f"Failed to parse '{conf_data}': {e}"
+            )
+            return
+        if attr_value <= 0:
+            print(
+                f"Option {attr_name} in section {section} should be greater than zero. Limiting to 1."
+            )
+            attr_value = 1
+
+    elif attr_type == float | GreaterZero:
+        # GreaterZero is just a signifier to check for positive numbers.
+        try:
+            attr_value = float(conf_data)
+        except ValueError as e:
+            print(
+                f"Option {attr_name} in section {section} should be floating point number.\n"
+                f"Failed to parse '{conf_data}': {e}"
+            )
+            return
+        if attr_value <= 0:
+            print(
+                f"Option {attr_name} in section {section} should be greater than zero. Setting to 1."
+            )
+            attr_value = 0.01
+
     elif attr_type == Path:
         try:
             attr_value = Path(conf_data)
         except ValueError as e:
             print(
                 f"Option {attr_name} in section {section} should be file path.\n"
                 f"Failed to parse '{conf_data}': {e}"
@@ -872,7 +957,33 @@
     Strip all leading whitespace from all lines in a string.
 
     :param string: The string to strip.
     :return: The stripped string.
     """
     stripped_lines = (line.lstrip() for line in string.splitlines())
     return "\n".join(stripped_lines)
+
+
+def format_for_version(conf_string: str, gui_mode: bool) -> str:
+    """
+    Format the config string for the current version of the program.
+
+    In CLI mode, remove all GUI-only options, and vice versa.
+    The comments that need to be replaces are marked as follows:
+    [CLI: ...] and [GUI: ...]
+
+    :param conf_string: The config string to format.
+    :param gui_mode: Whether to format for GUI mode.
+    :return: The formatted config string.
+    """
+    if gui_mode:
+        conf_string = re.sub(r"^\s*\[CLI: (.*?)]\s*$", "", conf_string, flags=re.MULTILINE)
+        conf_string = re.sub(r"^\s*\[GUI: (.*?)]\s*$", r"\1", conf_string, flags=re.MULTILINE)
+        conf_string = re.sub(r"\[CLI: (.*?)]", "", conf_string)
+        conf_string = re.sub(r"\[GUI: (.*?)]", r"\1", conf_string)
+    else:
+        conf_string = re.sub(r"^\s*\[GUI: (.*?)]\s*$", "", conf_string, flags=re.MULTILINE)
+        conf_string = re.sub(r"^\s*\[CLI: (.*?)]\s*$", r"\1", conf_string, flags=re.MULTILINE)
+        conf_string = re.sub(r"\[GUI: (.*?)]", "", conf_string)
+        conf_string = re.sub(r"\[CLI: (.*?)]", r"\1", conf_string)
+
+    return conf_string
```

### Comparing `pcleaner-1.6.0/pcleaner/ctd_interface.py` & `pcleaner-1.6.2/pcleaner/ctd_interface.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/denoiser.py` & `pcleaner-1.6.2/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-1.6.2/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import PySide6.QtWidgets as Qw
 
 from logzero import logger
 
 
+# noinspection PyPep8Naming
 class CComboBox(Qw.QComboBox):
     """
     Extends the functionality with custom helpers
     And includes a secondary array for data linked to each item
     """
 
     def __init__(self, parent=None):
```

### Comparing `pcleaner-1.6.0/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.6.2/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import PySide6.QtWidgets as Qw
 import PySide6.QtGui as Qg
 import PySide6.QtCore as Qc
 
 
+# noinspection PyPep8Naming
 class CTableWidget(Qw.QTableWidget):
     """
     Extends the functionality with custom helpers
     """
 
     finished_drop = Qc.Signal()
```

### Comparing `pcleaner-1.6.0/pcleaner/gui/file_table.py` & `pcleaner-1.6.2/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/gui/launcher.py` & `pcleaner-1.6.2/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.6.2/pcleaner/gui/mainwindow_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import shutil
 from functools import partial
 from pathlib import Path
+from importlib import resources
 
 import PySide6.QtCore as Qc
 import PySide6.QtGui as Qg
 import PySide6.QtWidgets as Qw
 from PySide6.QtCore import Signal
 from logzero import logger
 
 import pcleaner.cli_utils as cu
 import pcleaner.helpers as hp
 import pcleaner.config as cfg
 import pcleaner.gui.profile_parser as pp
 from pcleaner.gui.ui_generated_files.ui_Mainwindow import Ui_MainWindow
 from pcleaner.gui.file_table import Column
 from pcleaner import __display_name__, __version__
+from pcleaner import data
 
 
 # noinspection PyUnresolvedReferences
 class MainWindow(Qw.QMainWindow, Ui_MainWindow):
 
     config: cfg.Config = None
     # glossary: st.Glossary = None
@@ -26,14 +28,16 @@
 
     # text_params_changed = Signal(st.Glossary)
     # text_output_changed = Signal()
     # abort_translation_worker = Signal()
 
     label_stats: Qw.QLabel
 
+    toolBox_profile: pp.ProfileToolBox
+
     def __init__(self):
         Qw.QMainWindow.__init__(self)
         self.setupUi(self)
         self.setWindowTitle(f"{__display_name__} {__version__}")
         self.setWindowIcon(Qg.QIcon(":/logo-tiny.png"))
         self.processing = False
 
@@ -58,14 +62,15 @@
     def initialize_ui(self):
         self.hide_progress()
         self.start_button_enabled(False)
         self.show_button_start()
         self.update_input_buttons()
         self.set_up_statusbar()
         self.initialize_profiles()
+        self.initialize_analytics_view()
 
         # Allow the table to accept file drops and hide the ID column.
         self.file_table.setAcceptDrops(True)
         self.file_table.setColumnHidden(Column.ID, True)
         self.file_table.setColumnWidth(Column.FILENAME, 200)
         self.file_table.setColumnWidth(Column.STATUS, 200)
 
@@ -354,14 +359,30 @@
 
     def update_file_table_params(self):
         """
         Update the file table with the current parameters.
         """
         self.text_params_changed.emit(self.glossary)
 
+    def initialize_analytics_view(self):
+        """
+        Set up the text edit for analytics.
+        """
+        # Set the font to monospace, using the included font.
+        # The font is stored in the data module. Noto Mono is a free font.
+        # Load it from file to be cross platform.
+        font_path = resources.path(data, "NotoMono-Regular.ttf")
+        font_id = Qg.QFontDatabase.addApplicationFont(str(font_path))
+        if font_id != -1:
+            logger.info("Loaded included font")
+        else:
+            logger.error(f"Failed to load included font. Using backup monospace font")
+        self.textEdit_analytics.setReadOnly(True)
+        self.textEdit_analytics.setLineWrapMode(Qw.QTextEdit.NoWrap)
+
     """
     Profiles
     """
 
     def initialize_profiles(self):
         """
         Load the available profiles and display the default profile.
@@ -370,24 +391,34 @@
         for profile_name, profile_path in self.config.saved_profiles.items():
             all_profiles.append((profile_name, profile_path))
 
         self.comboBox_current_profile.clear()
         for profile_name, profile_path in all_profiles:
             self.comboBox_current_profile.addTextItemLinkedData(profile_name, profile_path)
 
+        # Load the ProfileToolBox widget.
+        self.toolBox_profile = pp.ProfileToolBox(self)
+        inner_layout = Qw.QVBoxLayout()
+        inner_layout.setContentsMargins(0, 0, 0, 0)
+        inner_layout.addWidget(self.toolBox_profile)
+        self.toolBox_profile_frame.setLayout(inner_layout)
+        self.config.load_profile(self.comboBox_current_profile.currentText())
+
+        # Load the structure.
+        structure = pp.parse_profile_structure(self.config.current_profile)
+        self.toolBox_profile.load_profile_structure(structure)
+
         self.load_current_profile()
 
     def load_current_profile(self):
         """
         Load the current profile.
         """
         logger.debug("Loading current profile.")
-        self.config.load_profile(self.comboBox_current_profile.currentText())
-
-        pp.parse_profile_structure(self.config.current_profile)
+        self.toolBox_profile.set_profile_values(self.config.current_profile)
 
     """
     Glossary
     """
 
     def load_glossary(self):
         """
```

### Comparing `pcleaner-1.6.0/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.6.2/pcleaner/gui/rc_generated_files/icons_rc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1060,14 +1060,56 @@
 921875 6 L 3 6 L\
  3 3 z M 3 7 L 1\
 3 7 L 13 13 L 3 \
 13 L 3 7 z \x22\x0a   \
   class=\x22ColorSc\
 heme-Text\x22\x0a     \
 />\x0a</svg>\x0a\
+\x00\x00\x02y\
+<\
+svg id=\x22svg6\x22 ve\
+rsion=\x221.1\x22 view\
+Box=\x220 0 16 16\x22 \
+xmlns=\x22http://ww\
+w.w3.org/2000/sv\
+g\x22>\x0a    <style i\
+d=\x22current-color\
+-scheme\x22 type=\x22t\
+ext/css\x22>.ColorS\
+cheme-Text {\x0a   \
+         color:#\
+232629;\x0a        \
+}</style>\x0a    <p\
+ath id=\x22path4\x22 c\
+lass=\x22ColorSchem\
+e-Text\x22 d=\x22m7.5 \
+2-3.5 3.5 3.5 3.\
+5 0.71875-0.7187\
+5-2.3125-2.28125\
+h3.59375c1.93299\
+8 0 3.5 1.566998\
+4 3.5 3.5 0 1.93\
+3002-1.567002 3.\
+5-3.5 3.5h-1.5v1\
+h1.5c2.485283 0 \
+4.5-2.014748 4.5\
+-4.5 0-2.4852521\
+-2.014717-4.5-4.\
+5-4.5h-3.59375l2\
+.3125-2.28125z\x22 \
+fill=\x22currentCol\
+or\x22/>\x0a    <rect \
+id=\x22rect837\x22 cla\
+ss=\x22ColorScheme-\
+Text\x22 x=\x222\x22 y=\x222\
+\x22 width=\x221\x22 heig\
+ht=\x227\x22 fill=\x22cur\
+rentColor\x22 fill-\
+rule=\x22evenodd\x22/>\
+\x0a</svg>\x0a\
 \x00\x00\x02\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
@@ -2342,14 +2384,56 @@
 921875 6 L 3 6 L\
  3 3 z M 3 7 L 1\
 3 7 L 13 13 L 3 \
 13 L 3 7 z \x22\x0a   \
   class=\x22ColorSc\
 heme-Text\x22\x0a     \
 />\x0a</svg>\x0a\
+\x00\x00\x02y\
+<\
+svg id=\x22svg6\x22 ve\
+rsion=\x221.1\x22 view\
+Box=\x220 0 16 16\x22 \
+xmlns=\x22http://ww\
+w.w3.org/2000/sv\
+g\x22>\x0a    <style i\
+d=\x22current-color\
+-scheme\x22 type=\x22t\
+ext/css\x22>.ColorS\
+cheme-Text {\x0a   \
+         color:#\
+eff0f1;\x0a        \
+}</style>\x0a    <p\
+ath id=\x22path4\x22 c\
+lass=\x22ColorSchem\
+e-Text\x22 d=\x22m7.5 \
+2-3.5 3.5 3.5 3.\
+5 0.71875-0.7187\
+5-2.3125-2.28125\
+h3.59375c1.93299\
+8 0 3.5 1.566998\
+4 3.5 3.5 0 1.93\
+3002-1.567002 3.\
+5-3.5 3.5h-1.5v1\
+h1.5c2.485283 0 \
+4.5-2.014748 4.5\
+-4.5 0-2.4852521\
+-2.014717-4.5-4.\
+5-4.5h-3.59375l2\
+.3125-2.28125z\x22 \
+fill=\x22currentCol\
+or\x22/>\x0a    <rect \
+id=\x22rect837\x22 cla\
+ss=\x22ColorScheme-\
+Text\x22 x=\x222\x22 y=\x222\
+\x22 width=\x221\x22 heig\
+ht=\x227\x22 fill=\x22cur\
+rentColor\x22 fill-\
+rule=\x22evenodd\x22/>\
+\x0a</svg>\x0a\
 \x00\x00\x02\xdd\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 viewBox=\x22\
 0 0 16 16\x22>\x0a  <d\
 efs id=\x22defs3051\
@@ -2945,14 +3029,18 @@
 \x00e\
 \x00d\x00i\x00t\x00-\x00d\x00e\x00l\x00e\x00t\x00e\x00.\x00s\x00v\x00g\
 \x00\x18\
 \x0e\x10\x8e\xe7\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00o\x00p\x00e\x00n\x00-\x00f\x00o\x00l\
 \x00d\x00e\x00r\x00.\x00s\x00v\x00g\
+\x00\x0e\
+\x0f\xc9\xd1\xa7\
+\x00e\
+\x00d\x00i\x00t\x00-\x00r\x00e\x00s\x00e\x00t\x00.\x00s\x00v\x00g\
 \x00\x11\
 \x0f\xe3\xd8\xe7\
 \x00d\
 \x00o\x00c\x00u\x00m\x00e\x00n\x00t\x00-\x00s\x00a\x00v\x00e\x00.\x00s\x00v\x00g\
 \
 \x00\x11\
 \x01\xa6\xc9\x07\
@@ -3013,131 +3101,135 @@
 \x00i\
 \x00m\x00a\x00g\x00e\x00-\x00p\x00n\x00g\x00.\x00s\x00v\x00g\
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00:\x00\x02\x00\x00\x00\x03\x00\x00\x00 \
+\x00\x00\x00:\x00\x02\x00\x00\x00\x03\x00\x00\x00!\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x1a\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x87\x8c\xdf\x0e\xff\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x03\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1a\
+\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x00\x1b\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00`\x05\
+\x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00b\x82\
 \x00\x00\x01\x82\xfe\x95\xbc\x1d\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x12\x00\x00\x00\x08\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x13\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x00\x84\x81\
+\x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x00\x86\xfe\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02&\x00\x00\x00\x00\x00\x01\x00\x00\x90J\
+\x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x00\x95D\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00\x9b\xed\
+\x00\x00\x03:\x00\x00\x00\x00\x00\x01\x00\x00\xa0\xe7\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03@\x00\x00\x00\x00\x00\x01\x00\x00\x9e\xef\
+\x00\x00\x03b\x00\x00\x00\x00\x00\x01\x00\x00\xa3\xe9\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00q\xeb\
+\x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00th\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00~\x14\
+\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00\x80\x91\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9a\x18\
+\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00\x9f\x12\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00w\xd4\
+\x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00zQ\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00{\xb5\
+\x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00~2\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00nv\
+\x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00p\xf3\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x00\x95\x85\
+\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x9a\x7f\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x89e\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00\x8b\xe2\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00\x97s\
+\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00\x9cm\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x8b\x0a\
+\x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x8d\x87\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02N\x00\x00\x00\x00\x00\x01\x00\x00\x92\x5c\
+\x00\x00\x02p\x00\x00\x00\x00\x00\x01\x00\x00\x97V\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00u\xe1\
+\x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00x^\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\x80\x00\x00\x00\x00\x00\x01\x00\x00\x94n\
+\x00\x00\x02\xa2\x00\x00\x00\x00\x00\x01\x00\x00\x99h\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x8di\
+\x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xe6\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02 \x00\x00\x00\x00\x00\x01\x00\x00\x92c\
 \x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x00\x1b\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x00\x1c\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\xda\x00\x00\x00\x00\x00\x01\x00\x00\xa8\x11\
+\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\xad\x0b\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00\xaaw\
+\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00\xafq\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xba\x00\x00\x00\x00\x00\x01\x00\x00\xa5\xaf\
+\x00\x00\x03\xdc\x00\x00\x00\x00\x00\x01\x00\x00\xaa\xa9\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00\xa0\xeb\
+\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00\xa5\xe5\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00\xa3M\
+\x00\x00\x03\xb0\x00\x00\x00\x00\x00\x01\x00\x00\xa8G\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x006\
+\x00\x00\x00h\x00\x02\x00\x00\x00\x01\x00\x00\x008\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00#\
+\x00\x00\x00\x80\x00\x02\x00\x00\x00\x01\x00\x00\x00$\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00L\x00\x01\x00\x00\x00\x01\x00\x00\x14h\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x12\x00\x00\x00$\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x13\x00\x00\x00%\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x01\x80\x00\x00\x00\x00\x00\x01\x00\x007\xa9\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02&\x00\x00\x00\x00\x00\x01\x00\x00Cr\
+\x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x00E\xef\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00O\x15\
+\x00\x00\x03:\x00\x00\x00\x00\x00\x01\x00\x00Q\x92\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x03@\x00\x00\x00\x00\x00\x01\x00\x00R\x17\
+\x00\x00\x03b\x00\x00\x00\x00\x00\x01\x00\x00T\x94\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x00\xc4\x00\x00\x00\x00\x00\x01\x00\x00%\x13\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x001<\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00M@\
+\x00\x00\x03\x18\x00\x00\x00\x00\x00\x01\x00\x00O\xbd\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01\x14\x00\x00\x00\x00\x00\x01\x00\x00*\xfc\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x014\x00\x00\x00\x00\x00\x01\x00\x00.\xdd\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x00\x9e\x00\x00\x00\x00\x00\x01\x00\x00!\x9e\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xb6\x00\x00\x00\x00\x00\x01\x00\x00H\xad\
+\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00K*\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00<\x8d\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\xd4\x00\x00\x00\x00\x00\x01\x00\x00J\x9b\
+\x00\x00\x02\xf6\x00\x00\x00\x00\x00\x01\x00\x00M\x18\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01\xc8\x00\x00\x00\x00\x00\x01\x00\x00>2\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02N\x00\x00\x00\x00\x00\x01\x00\x00E\x84\
+\x00\x00\x02p\x00\x00\x00\x00\x00\x01\x00\x00H\x01\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x00\xf2\x00\x00\x00\x00\x00\x01\x00\x00)\x09\
 \x00\x00\x01\x81\xc0B\xdb\x80\
-\x00\x00\x02\x80\x00\x00\x00\x00\x00\x01\x00\x00G\x96\
+\x00\x00\x02\xa2\x00\x00\x00\x00\x00\x01\x00\x00J\x13\
 \x00\x00\x01\x81\xc0B\xdb\x80\
 \x00\x00\x01\xfe\x00\x00\x00\x00\x00\x01\x00\x00@\x91\
+\x00\x00\x01\x86\xac\x9ffH\
+\x00\x00\x02 \x00\x00\x00\x00\x00\x01\x00\x00C\x0e\
 \x00\x00\x01\x83\x9f\xda\x12\xf9\
-\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x007\
+\x00\x00\x00\x94\x00\x02\x00\x00\x00\x05\x00\x00\x009\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\xda\x00\x00\x00\x00\x00\x01\x00\x00[9\
+\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00]\xb6\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xfc\x00\x00\x00\x00\x00\x01\x00\x00]\x9f\
+\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00`\x1c\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\xba\x00\x00\x00\x00\x00\x01\x00\x00X\xd7\
+\x00\x00\x03\xdc\x00\x00\x00\x00\x00\x01\x00\x00[T\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00T\x13\
+\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00V\x90\
 \x00\x00\x01\x86\xac\x9ffH\
-\x00\x00\x03\x8e\x00\x00\x00\x00\x00\x01\x00\x00Vu\
+\x00\x00\x03\xb0\x00\x00\x00\x00\x00\x01\x00\x00X\xf2\
 \x00\x00\x01\x86\xac\x9ffH\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.6.2/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     QPainter, QPalette, QPixmap, QRadialGradient,
     QTransform)
 from PySide6.QtWidgets import (QAbstractItemView, QApplication, QCheckBox, QFormLayout,
     QFrame, QGroupBox, QHBoxLayout, QHeaderView,
     QLabel, QLineEdit, QMainWindow, QMenu,
     QMenuBar, QProgressBar, QPushButton, QRadioButton,
     QSizePolicy, QSpacerItem, QSplitter, QStatusBar,
-    QTabWidget, QTableWidgetItem, QTextEdit, QToolBox,
-    QVBoxLayout, QWidget)
+    QTabWidget, QTableWidgetItem, QTextEdit, QVBoxLayout,
+    QWidget)
 
 from pcleaner.gui.CustomQ.CComboBox import CComboBox
 from pcleaner.gui.file_table import FileTable
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         if not MainWindow.objectName():
@@ -70,15 +70,15 @@
         self.action_temp.setObjectName(u"action_temp")
         self.action_temp_2 = QAction(MainWindow)
         self.action_temp_2.setObjectName(u"action_temp_2")
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName(u"centralwidget")
         self.verticalLayout = QVBoxLayout(self.centralwidget)
         self.verticalLayout.setObjectName(u"verticalLayout")
-        self.verticalLayout.setContentsMargins(1, 1, 1, 1)
+        self.verticalLayout.setContentsMargins(1, 4, 1, 1)
         self.splitter = QSplitter(self.centralwidget)
         self.splitter.setObjectName(u"splitter")
         self.splitter.setOrientation(Qt.Horizontal)
         self.splitter.setHandleWidth(10)
         self.groupBox = QGroupBox(self.splitter)
         self.groupBox.setObjectName(u"groupBox")
         self.verticalLayout_2 = QVBoxLayout(self.groupBox)
@@ -89,14 +89,15 @@
         self.comboBox_current_profile.addItem("")
         self.comboBox_current_profile.setObjectName(u"comboBox_current_profile")
         sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.comboBox_current_profile.sizePolicy().hasHeightForWidth())
         self.comboBox_current_profile.setSizePolicy(sizePolicy)
+        self.comboBox_current_profile.setMinimumSize(QSize(48, 0))
 
         self.horizontalLayout_2.addWidget(self.comboBox_current_profile)
 
         self.pushButton_save_pofile = QPushButton(self.groupBox)
         self.pushButton_save_pofile.setObjectName(u"pushButton_save_pofile")
         icon = QIcon()
         iconThemeName = u"document-save"
@@ -136,22 +137,23 @@
         self.pushButton_apply_profile.setIcon(icon2)
 
         self.horizontalLayout_2.addWidget(self.pushButton_apply_profile)
 
 
         self.verticalLayout_2.addLayout(self.horizontalLayout_2)
 
-        self.toolBox_profile = QToolBox(self.groupBox)
-        self.toolBox_profile.setObjectName(u"toolBox_profile")
-        self.page_placeholder = QWidget()
-        self.page_placeholder.setObjectName(u"page_placeholder")
-        self.page_placeholder.setGeometry(QRect(0, 0, 643, 447))
-        self.toolBox_profile.addItem(self.page_placeholder, u"Profile Section")
+        self.toolBox_profile_frame = QWidget(self.groupBox)
+        self.toolBox_profile_frame.setObjectName(u"toolBox_profile_frame")
+        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Expanding)
+        sizePolicy1.setHorizontalStretch(0)
+        sizePolicy1.setVerticalStretch(0)
+        sizePolicy1.setHeightForWidth(self.toolBox_profile_frame.sizePolicy().hasHeightForWidth())
+        self.toolBox_profile_frame.setSizePolicy(sizePolicy1)
 
-        self.verticalLayout_2.addWidget(self.toolBox_profile)
+        self.verticalLayout_2.addWidget(self.toolBox_profile_frame)
 
         self.splitter.addWidget(self.groupBox)
         self.tabWidget_files = QTabWidget(self.splitter)
         self.tabWidget_files.setObjectName(u"tabWidget_files")
         self.tabWidget_table_page = QWidget()
         self.tabWidget_table_page.setObjectName(u"tabWidget_table_page")
         self.verticalLayout_3 = QVBoxLayout(self.tabWidget_table_page)
@@ -214,19 +216,19 @@
 
         self.verticalLayout_9.addItem(self.verticalSpacer)
 
         self.verticalLayout_7 = QVBoxLayout()
         self.verticalLayout_7.setObjectName(u"verticalLayout_7")
         self.label_warning = QLabel(self.groupBox_4)
         self.label_warning.setObjectName(u"label_warning")
-        sizePolicy1 = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
-        sizePolicy1.setHorizontalStretch(0)
-        sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.label_warning.sizePolicy().hasHeightForWidth())
-        self.label_warning.setSizePolicy(sizePolicy1)
+        sizePolicy2 = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+        sizePolicy2.setHorizontalStretch(0)
+        sizePolicy2.setVerticalStretch(0)
+        sizePolicy2.setHeightForWidth(self.label_warning.sizePolicy().hasHeightForWidth())
+        self.label_warning.setSizePolicy(sizePolicy2)
 
         self.verticalLayout_7.addWidget(self.label_warning)
 
         self.pushButton_start = QPushButton(self.groupBox_4)
         self.pushButton_start.setObjectName(u"pushButton_start")
         icon3 = QIcon()
         iconThemeName = u"media-playback-start"
@@ -383,14 +385,17 @@
         self.menu_Theme.setObjectName(u"menu_Theme")
         self.menu_Help = QMenu(self.menubar)
         self.menu_Help.setObjectName(u"menu_Help")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
         self.statusbar.setObjectName(u"statusbar")
         MainWindow.setStatusBar(self.statusbar)
+#if QT_CONFIG(shortcut)
+        self.label_4.setBuddy(self.lineEdit_out_directory)
+#endif // QT_CONFIG(shortcut)
 
         self.menubar.addAction(self.menu_File.menuAction())
         self.menubar.addAction(self.menu_Profile.menuAction())
         self.menubar.addAction(self.menu_Settings.menuAction())
         self.menubar.addAction(self.menu_Help.menuAction())
         self.menu_File.addAction(self.action_Open_Files)
         self.menu_File.addAction(self.action_Clear_Files)
@@ -416,17 +421,14 @@
         self.menu_Help.addAction(self.action_Panel_Cleaner_Documentation)
         self.menu_Help.addAction(self.action_Source_Code)
         self.menu_Help.addSeparator()
         self.menu_Help.addAction(self.actionShow_Terminal_Command)
 
         self.retranslateUi(MainWindow)
 
-        self.toolBox_profile.setCurrentIndex(0)
-
-
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"Panel Cleaner", None))
         self.action_Open_Files.setText(QCoreApplication.translate("MainWindow", u"Open Files", None))
         self.action_Clear_Files.setText(QCoreApplication.translate("MainWindow", u"Clear Files", None))
@@ -448,15 +450,14 @@
         self.action_temp_2.setText(QCoreApplication.translate("MainWindow", u"<temp>", None))
         self.groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Profile", None))
         self.comboBox_current_profile.setItemText(0, QCoreApplication.translate("MainWindow", u"Default", None))
 
         self.pushButton_save_pofile.setText(QCoreApplication.translate("MainWindow", u"Save", None))
         self.pushButton_reset_profile.setText(QCoreApplication.translate("MainWindow", u"Reset All", None))
         self.pushButton_apply_profile.setText(QCoreApplication.translate("MainWindow", u"Apply", None))
-        self.toolBox_profile.setItemText(self.toolBox_profile.indexOf(self.page_placeholder), QCoreApplication.translate("MainWindow", u"Profile Section", None))
         ___qtablewidgetitem = self.file_table.horizontalHeaderItem(0)
         ___qtablewidgetitem.setText(QCoreApplication.translate("MainWindow", u"id", None));
         ___qtablewidgetitem1 = self.file_table.horizontalHeaderItem(1)
         ___qtablewidgetitem1.setText(QCoreApplication.translate("MainWindow", u"File", None));
         ___qtablewidgetitem2 = self.file_table.horizontalHeaderItem(2)
         ___qtablewidgetitem2.setText(QCoreApplication.translate("MainWindow", u"Size", None));
         ___qtablewidgetitem3 = self.file_table.horizontalHeaderItem(3)
@@ -476,18 +477,18 @@
         self.checkBox_save_text.setText(QCoreApplication.translate("MainWindow", u"Extracted Text", None))
         self.label_4.setText(QCoreApplication.translate("MainWindow", u"Output Directory:", None))
         self.pushButton_browse_out_dir.setText("")
         self.textEdit_analytics.setHtml(QCoreApplication.translate("MainWindow", u"<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
 "p, li { white-space: pre-wrap; }\n"
 "</style></head><body style=\" font-family:'Noto Sans'; font-size:10pt; font-weight:400; font-style:normal;\">\n"
-"<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-family:'monospace';\">Mask Fitment Analytics <br />---------------------- <br />Total boxes: 5 | Masks succeeded: 5 (100%) | Masks failed: </span><span style=\" font-family:'monospace'; color:#b21818;\">0</span><span style=\" font-family:'monospace';\"> <br />Perfect masks: </span><span style=\" font-family:'monospace'; color:#18b2b2;\">5</span><span style=\" font-family:'monospace';\"> (100%) | Average border deviation: 0.00 <br /><br />Mask usage by mask size (smallest to largest): <br />Mask 0  :  </span><span style=\" font-family:'monosp"
-                        "ace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 1  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 2  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 3  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 4  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 5  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 6  : </span><span style=\" font-family:'monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588"
-                        "\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'monospace';\"> </span><span style=\" font-family:'monospace'; color:#18b2b2;\">1</span><span style=\" font-family:'monospace';\"> / 1 <br />Mask 7  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 8  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 9  :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Mask 10 :  </span><span style=\" font-family:'monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'monospace';\"> / 0 <br />Box mask: </span><span style=\" font-family:'monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588"
-                        "\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'monospace';\"> </span><span style=\" font-family:'monospace'; color:#18b2b2;\">4</span><span style=\" font-family:'monospace';\"> / 4 <br /><br /></span><span style=\" font-family:'monospace'; color:#18b2b2;\">\u2588 Perfect</span><span style=\" font-family:'monospace';\"> | \u2588 Total<br /><br /></span></p></body></html>", None))
+"<p style=\" margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><span style=\" font-family:'Noto Mono','Monospace';\">Mask Fitment Analytics <br />---------------------- <br />Total boxes: 5 | Masks succeeded: 5 (100%) | Masks failed: </span><span style=\" font-family:'Noto Mono','Monospace'; color:#b21818;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> <br />Perfect masks: </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">5</span><span style=\" font-family:'Noto Mono','Monospace';\"> (100%) | Average border deviation: 0.00 <br /><br />Mask usage by mask size (smallest to largest)"
+                        ": <br />Mask 0  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 1  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 2  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 3  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 4  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 5  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 6  : </span><span style=\" font-family:'Noto Mono','"
+                        "Monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'Noto Mono','Monospace';\"> </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">1</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 1 <br />Mask 7  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 8  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 9  :  </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Mask 10 :  </span><span style=\" font-family:'Noto Mono','Monospa"
+                        "ce'; color:#18b2b2;\">0</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 0 <br />Box mask: </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588</span><span style=\" font-family:'Noto Mono','Monospace';\"> </span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">4</span><span style=\" font-family:'Noto Mono','Monospace';\"> / 4 <br /><br /></span><span style=\" font-family:'Noto Mono','Monospace'; color:#18b2b2;\">\u2588 Perfect</span><span style=\" font-family:'Noto Mono','Monospace';\"> | \u2588 Total<br /><br /></span></p></body></html>", None))
         self.label_progress_step.setText(QCoreApplication.translate("MainWindow", u"Current Step:", None))
         self.label_2.setText(QCoreApplication.translate("MainWindow", u"Total Progress:", None))
         self.menu_File.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
         self.menu_Profile.setTitle(QCoreApplication.translate("MainWindow", u"Profile", None))
         self.menuCurrent_Profile.setTitle(QCoreApplication.translate("MainWindow", u"Current Profile", None))
         self.menuSet_Default.setTitle(QCoreApplication.translate("MainWindow", u"Set Default", None))
         self.menu_Settings.setTitle(QCoreApplication.translate("MainWindow", u"Settings", None))
```

### Comparing `pcleaner-1.6.0/pcleaner/gui/worker_thread.py` & `pcleaner-1.6.2/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/helpers.py` & `pcleaner-1.6.2/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/image_ops.py` & `pcleaner-1.6.2/pcleaner/image_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,15 +566,15 @@
     # Create a blank canvas.
     text_image = Image.new("RGBA", base_image.size, (0, 0, 0, 0))
     # Paste the base image onto the canvas using the mask.
     text_image.paste(base_image, (0, 0), mask)
     return text_image
 
 
-# IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
+# SUPPORTED_IMG_TYPES = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
 
 suffix_to_format: dict[str, str] = {
     ".jpg": "JPEG",
     ".jpeg": "JPEG",
     ".png": "PNG",
     ".webp": "WEBP",
     ".tiff": "TIFF",
```

### Comparing `pcleaner-1.6.0/pcleaner/main.py` & `pcleaner-1.6.2/pcleaner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,14 @@
 import pcleaner.structures as st
 import pcleaner.profile_cli as pc
 import pcleaner.denoiser as dn
 import pcleaner.model_downloader as md
 import pcleaner.helpers as hp
 import pcleaner.gui.launcher as gui
 
-# Supported image suffixes.
-IMG_EXT = [".jpeg", ".jpg", ".png", ".bmp", ".tiff", ".tif", ".jp2", ".dib", ".webp", ".ppm"]
-
 # Allow loading of large images.
 Image.MAX_IMAGE_PIXELS = 2**32
 
 
 def main():
 
     args = magic_docopt(__doc__, version=f"Panel Cleaner {__version__}")
@@ -582,15 +579,15 @@
 
     # Convert all strings to paths.
     img_paths = [Path(path) for path in img_paths]
 
     for img_path in img_paths:
         if img_path.is_dir():
             img_list.extend(find_all_images_shallow(img_path))
-        elif img_path.is_file() and img_path.suffix.lower() in IMG_EXT:
+        elif img_path.is_file() and img_path.suffix.lower() in cfg.SUPPORTED_IMG_TYPES:
             img_list.append(img_path)
         else:
             raise FileNotFoundError(f"Image path {img_path} does not exist.")
 
     # Ensure all paths are absolute.
     img_list = [path.resolve() for path in img_list]
 
@@ -600,15 +597,15 @@
     return img_list
 
 
 def find_all_images_shallow(img_dir: Path) -> list[Path]:
     image_list: list[Path] = []
     for file_path in img_dir.glob("*"):
         file_suffix = file_path.suffix
-        if file_suffix.lower() not in IMG_EXT:
+        if file_suffix.lower() not in cfg.SUPPORTED_IMG_TYPES:
             continue
         else:
             image_list.append(file_path)
     return image_list
 
 
 def is_5_channel_tiff(path: Path) -> bool:
```

### Comparing `pcleaner-1.6.0/pcleaner/masker.py` & `pcleaner-1.6.2/pcleaner/masker.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/model_downloader.py` & `pcleaner-1.6.2/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/pre_processor.py` & `pcleaner-1.6.2/pcleaner/pre_processor.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/profile_cli.py` & `pcleaner-1.6.2/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner/structures.py` & `pcleaner-1.6.2/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.6.0/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.6.2/pcleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.6.0
+Version: 1.6.2
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Natural Language :: English
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
 
 # Panel Cleaner
```

### Comparing `pcleaner-1.6.0/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.6.2/pcleaner.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,24 @@
 pcleaner/comic_text_detector/utils/imgproc_utils.py
 pcleaner/comic_text_detector/utils/io_utils.py
 pcleaner/comic_text_detector/utils/loss.py
 pcleaner/comic_text_detector/utils/textblock.py
 pcleaner/comic_text_detector/utils/textmask.py
 pcleaner/comic_text_detector/utils/weight_init.py
 pcleaner/comic_text_detector/utils/yolov5_utils.py
+pcleaner/data/LiberationSans-Regular.ttf
+pcleaner/data/NotoMono-Regular.ttf
 pcleaner/data/__init__.py
 pcleaner/gui/__init__.py
 pcleaner/gui/file_table.py
 pcleaner/gui/launcher.py
 pcleaner/gui/mainwindow_driver.py
 pcleaner/gui/profile_parser.py
 pcleaner/gui/worker_thread.py
+pcleaner/gui/CustomQ/CColorButton.py
 pcleaner/gui/CustomQ/CComboBox.py
 pcleaner/gui/CustomQ/CTableWidget.py
 pcleaner/gui/CustomQ/__init__.py
 pcleaner/gui/rc_generated_files/__init__.py
 pcleaner/gui/rc_generated_files/icons_rc.py
 pcleaner/gui/ui_generated_files/__init__.py
 pcleaner/gui/ui_generated_files/ui_ImageDetails.py
```

### Comparing `pcleaner-1.6.0/setup.cfg` & `pcleaner-1.6.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 url = https://github.com/VoxelCubes/PanelCleaner
 keywords = image processing, cleaning, text removal, manga, ai, machine learning
 license_files = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: POSIX :: Linux
+	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Natural Language :: English
 
 [options]
 install_requires = 
 	opencv-python
 	manga_ocr
@@ -36,14 +37,17 @@
 	requests
 	xdg
 	tifffile
 	PySide6
 python_requires = >=3.10
 packages = find:
 
+[options.package_data]
+pcleaner = data/*
+
 [options.packages.find]
 exclude = tests*
 
 [options.entry_points]
 console_scripts = 
 	pcleaner = pcleaner.main:main
```

