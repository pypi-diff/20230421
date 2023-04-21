# Comparing `tmp/annotation_tool-0.8.1.tar.gz` & `tmp/annotation_tool-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annotation_tool-0.8.1.tar", max compression
+gzip compressed data, was "annotation_tool-0.8.2.tar", max compression
```

## Comparing `annotation_tool-0.8.1.tar` & `annotation_tool-0.8.2.tar`

### file list

```diff
@@ -1,88 +1,96 @@
--rw-r--r--   0        0        0     1085 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/LICENSE
--rw-r--r--   0        0        0     1280 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/README.md
--rw-r--r--   0        0        0       68 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/__init__.py
--rw-r--r--   0        0        0     8480 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/annotation_base.py
--rw-r--r--   0        0        0     5170 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/controller.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/manual/__init__.py
--rw-r--r--   0        0        0     5852 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/manual/controller.py
--rw-r--r--   0        0        0     3075 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/manual/main_widget.py
--rw-r--r--   0        0        0     2456 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/manual/tool_widget.py
--rw-r--r--   0        0        0       80 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/modes.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/__init__.py
--rw-r--r--   0        0        0    12649 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/controller.py
--rw-r--r--   0        0        0     3828 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/main_widget.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
--rw-r--r--   0        0        0      917 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/element.py
--rw-r--r--   0        0        0     1969 2023-03-17 14:50:41.734486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
--rw-r--r--   0        0        0     2184 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
--rw-r--r--   0        0        0     6370 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
--rw-r--r--   0        0        0    12318 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/query.py
--rw-r--r--   0        0        0     8256 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
--rw-r--r--   0        0        0     2013 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/retrieval/tool_widget.py
--rw-r--r--   0        0        0    14145 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/annotation/timeline.py
--rw-r--r--   0        0        0      479 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/__init__.py
--rw-r--r--   0        0        0     7726 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/annotation.py
--rw-r--r--   0        0        0     2077 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/annotation_scheme.py
--rw-r--r--   0        0        0     3003 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/dataset.py
--rw-r--r--   0        0        0      795 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/media_type.py
--rw-r--r--   0        0        0     4014 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/model.py
--rw-r--r--   0        0        0     2040 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/project.py
--rw-r--r--   0        0        0     3664 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/sample.py
--rw-r--r--   0        0        0     6412 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/data_model/single_annotation.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/__init__.py
--rw-r--r--   0        0        0    12197 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/annotation_dialog.py
--rw-r--r--   0        0        0    10523 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/annotation_list.py
--rw-r--r--   0        0        0     1956 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/dialog_manager.py
--rw-r--r--   0        0        0     7082 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/edit_datasets.py
--rw-r--r--   0        0        0    10994 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/import_annotation_dialog.py
--rw-r--r--   0        0        0     5706 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/load_annotation_dialog.py
--rw-r--r--   0        0        0     3670 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/local_files.py
--rw-r--r--   0        0        0    10576 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/network_list.py
--rw-r--r--   0        0        0     6899 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/new_annotation_dialog.py
--rw-r--r--   0        0        0    19491 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/dialogs/settings_dialog.py
--rw-r--r--   0        0        0      197 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/file_cache/__init__.py
--rw-r--r--   0        0        0     9586 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/file_cache/_file_cache.py
--rw-r--r--   0        0        0     8506 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/gui.py
--rw-r--r--   0        0        0    12111 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/main_controller.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/__init__.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/__init__.py
--rw-r--r--   0        0        0     9921 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/controller.py
--rw-r--r--   0        0        0     7918 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/player.py
--rw-r--r--   0        0        0     1795 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/queue.py
--rw-r--r--   0        0        0     9170 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/timer.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/type_specific_player/__init__.py
--rw-r--r--   0        0        0     8527 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/type_specific_player/mocap.py
--rw-r--r--   0        0        0     8002 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/backend/type_specific_player/video.py
--rw-r--r--   0        0        0     2249 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media/media.py
--rw-r--r--   0        0        0      357 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media_reader/__init__.py
--rw-r--r--   0        0        0    10789 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media_reader/base.py
--rw-r--r--   0        0        0     5750 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media_reader/mocap.py
--rw-r--r--   0        0        0     3107 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/media_reader/video.py
--rw-r--r--   0        0        0     4154 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/mediator.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/LARa/__init__.py
--rw-r--r--   0        0        0    12119 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/LARa/attr_per_class.txt
--rw-r--r--   0        0        0     5583 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/LARa/lara_specifics.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/__init__.py
--rw-r--r--   0        0        0     7267 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/controller.py
--rw-r--r--   0        0        0    27224 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/network/network.py
--rw-r--r--   0        0        0     7556 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/playback.py
--rw-r--r--   0        0        0     1546 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
--rw-r--r--   0        0        0     4401 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/checkable_combobox.py
--rw-r--r--   0        0        0     2170 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/display_scheme.py
--rw-r--r--   0        0        0     1798 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/histogram.py
--rw-r--r--   0        0        0      458 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/line_edit_adapted.py
--rw-r--r--   0        0        0      403 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/lines.py
--rw-r--r--   0        0        0     1077 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/own_slider.py
--rw-r--r--   0        0        0     1480 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/settings.py
--rw-r--r--   0        0        0     4037 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/user_actions.py
--rw-r--r--   0        0        0        0 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/__init__.py
--rw-r--r--   0        0        0     4818 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/decorators.py
--rw-r--r--   0        0        0    11854 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/filehandler.py
--rw-r--r--   0        0        0     4059 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/functions.py
--rw-r--r--   0        0        0     2153 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/networking.py
--rw-r--r--   0        0        0     4469 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/priority_queue.py
--rw-r--r--   0        0        0    53863 2023-03-17 14:50:41.738486 annotation_tool-0.8.1/annotation_tool/utility/resources.py
--rw-r--r--   0        0        0     1938 2023-03-17 14:50:41.742486 annotation_tool-0.8.1/main.py
--rw-r--r--   0        0        0     1899 2023-03-17 14:50:41.742486 annotation_tool-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 annotation_tool-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1280 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/README.md
+-rw-r--r--   0        0        0       68 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/__init__.py
+-rw-r--r--   0        0        0     8480 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/annotation_base.py
+-rw-r--r--   0        0        0     5170 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/controller.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/__init__.py
+-rw-r--r--   0        0        0     5852 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/controller.py
+-rw-r--r--   0        0        0     3075 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/main_widget.py
+-rw-r--r--   0        0        0     2456 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/manual/tool_widget.py
+-rw-r--r--   0        0        0       80 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/modes.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/__init__.py
+-rw-r--r--   0        0        0    12649 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/controller.py
+-rw-r--r--   0        0        0     3828 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/main_widget.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/__init__.py
+-rw-r--r--   0        0        0      917 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/element.py
+-rw-r--r--   0        0        0     1969 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter.py
+-rw-r--r--   0        0        0     2184 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py
+-rw-r--r--   0        0        0     6370 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/loader.py
+-rw-r--r--   0        0        0    12318 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/query.py
+-rw-r--r--   0        0        0     8256 2023-04-21 14:45:35.790131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/queue.py
+-rw-r--r--   0        0        0     2013 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/annotation/retrieval/tool_widget.py
+-rw-r--r--   0        0        0    14145 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/annotation/timeline.py
+-rw-r--r--   0        0        0      479 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/__init__.py
+-rw-r--r--   0        0        0     7726 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/annotation.py
+-rw-r--r--   0        0        0     2077 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/annotation_scheme.py
+-rw-r--r--   0        0        0     3003 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/dataset.py
+-rw-r--r--   0        0        0      795 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/media_type.py
+-rw-r--r--   0        0        0     4014 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/model.py
+-rw-r--r--   0        0        0     2040 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/project.py
+-rw-r--r--   0        0        0     3664 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/sample.py
+-rw-r--r--   0        0        0     6412 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/data_model/single_annotation.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/__init__.py
+-rw-r--r--   0        0        0    12197 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/annotation_dialog.py
+-rw-r--r--   0        0        0    10523 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/annotation_list.py
+-rw-r--r--   0        0        0     1956 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/dialog_manager.py
+-rw-r--r--   0        0        0     7082 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/edit_datasets.py
+-rw-r--r--   0        0        0    10994 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/import_annotation_dialog.py
+-rw-r--r--   0        0        0     5706 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/load_annotation_dialog.py
+-rw-r--r--   0        0        0     3670 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/local_files.py
+-rw-r--r--   0        0        0    10576 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/network_list.py
+-rw-r--r--   0        0        0     6899 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/new_annotation_dialog.py
+-rw-r--r--   0        0        0    19491 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/dialogs/settings_dialog.py
+-rw-r--r--   0        0        0      197 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/file_cache/__init__.py
+-rw-r--r--   0        0        0     9586 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/file_cache/_file_cache.py
+-rw-r--r--   0        0        0     8506 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/gui.py
+-rw-r--r--   0        0        0    12322 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/main_controller.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/__init__.py
+-rw-r--r--   0        0        0    10152 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/controller.py
+-rw-r--r--   0        0        0     4220 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/player.py
+-rw-r--r--   0        0        0     5327 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/timer.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/__init__.py
+-rw-r--r--   0        0        0     8424 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/mocap.py
+-rw-r--r--   0        0        0     7082 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/video.py
+-rw-r--r--   0        0        0     2286 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media/media.py
+-rw-r--r--   0        0        0      357 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/__init__.py
+-rw-r--r--   0        0        0     8866 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/base.py
+-rw-r--r--   0        0        0     2167 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap.py
+-rw-r--r--   0        0        0      121 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/__init__.py
+-rw-r--r--   0        0        0     3128 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/base.py
+-rw-r--r--   0        0        0     4745 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/cache.py
+-rw-r--r--   0        0        0     6020 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/lara_reader.py
+-rw-r--r--   0        0        0     1787 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video.py
+-rw-r--r--   0        0        0      157 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/__init__.py
+-rw-r--r--   0        0        0     4096 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/base.py
+-rw-r--r--   0        0        0     3668 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/decord_reader.py
+-rw-r--r--   0        0        0     4321 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/evaluation.py
+-rw-r--r--   0        0        0     7496 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/media_reader/video_readers/opencv_reader.py
+-rw-r--r--   0        0        0     4170 2023-04-21 14:45:35.794131 annotation_tool-0.8.2/annotation_tool/mediator.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/__init__.py
+-rw-r--r--   0        0        0    12119 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/attr_per_class.txt
+-rw-r--r--   0        0        0     5583 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/LARa/lara_specifics.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/__init__.py
+-rw-r--r--   0        0        0     7267 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/controller.py
+-rw-r--r--   0        0        0    27224 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/network/network.py
+-rw-r--r--   0        0        0     7556 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/playback.py
+-rw-r--r--   0        0        0     1546 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py
+-rw-r--r--   0        0        0     4401 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/checkable_combobox.py
+-rw-r--r--   0        0        0     2170 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/display_scheme.py
+-rw-r--r--   0        0        0     1798 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/histogram.py
+-rw-r--r--   0        0        0      458 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/line_edit_adapted.py
+-rw-r--r--   0        0        0      403 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/lines.py
+-rw-r--r--   0        0        0     1077 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/own_slider.py
+-rw-r--r--   0        0        0     1480 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/settings.py
+-rw-r--r--   0        0        0     4037 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/user_actions.py
+-rw-r--r--   0        0        0        0 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/__init__.py
+-rw-r--r--   0        0        0     4818 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/decorators.py
+-rw-r--r--   0        0        0    11854 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/filehandler.py
+-rw-r--r--   0        0        0     4059 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/functions.py
+-rw-r--r--   0        0        0     2153 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/networking.py
+-rw-r--r--   0        0        0     4469 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/priority_queue.py
+-rw-r--r--   0        0        0    53863 2023-04-21 14:45:35.798131 annotation_tool-0.8.2/annotation_tool/utility/resources.py
+-rw-r--r--   0        0        0     1938 2023-04-21 14:45:35.802132 annotation_tool-0.8.2/main.py
+-rw-r--r--   0        0        0     1949 2023-04-21 14:45:35.802132 annotation_tool-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 annotation_tool-0.8.2/PKG-INFO
```

### Comparing `annotation_tool-0.8.1/LICENSE` & `annotation_tool-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/README.md` & `annotation_tool-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/annotation_base.py` & `annotation_tool-0.8.2/annotation_tool/annotation/annotation_base.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/controller.py` & `annotation_tool-0.8.2/annotation_tool/annotation/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/manual/controller.py` & `annotation_tool-0.8.2/annotation_tool/annotation/manual/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/manual/main_widget.py` & `annotation_tool-0.8.2/annotation_tool/annotation/manual/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/manual/tool_widget.py` & `annotation_tool-0.8.2/annotation_tool/annotation/manual/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/controller.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/main_widget.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/main_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/element.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/element.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/filter.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/filter_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/loader.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/loader.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/query.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/query.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/retrieval_backend/queue.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/retrieval_backend/queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/retrieval/tool_widget.py` & `annotation_tool-0.8.2/annotation_tool/annotation/retrieval/tool_widget.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/annotation/timeline.py` & `annotation_tool-0.8.2/annotation_tool/annotation/timeline.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/annotation.py` & `annotation_tool-0.8.2/annotation_tool/data_model/annotation.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/annotation_scheme.py` & `annotation_tool-0.8.2/annotation_tool/data_model/annotation_scheme.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/dataset.py` & `annotation_tool-0.8.2/annotation_tool/data_model/dataset.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/media_type.py` & `annotation_tool-0.8.2/annotation_tool/data_model/media_type.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/model.py` & `annotation_tool-0.8.2/annotation_tool/data_model/model.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/project.py` & `annotation_tool-0.8.2/annotation_tool/data_model/project.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/sample.py` & `annotation_tool-0.8.2/annotation_tool/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/data_model/single_annotation.py` & `annotation_tool-0.8.2/annotation_tool/data_model/single_annotation.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/annotation_dialog.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/annotation_list.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/annotation_list.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/dialog_manager.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/dialog_manager.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/edit_datasets.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/edit_datasets.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/import_annotation_dialog.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/import_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/load_annotation_dialog.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/load_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/local_files.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/local_files.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/network_list.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/network_list.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/new_annotation_dialog.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/new_annotation_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/dialogs/settings_dialog.py` & `annotation_tool-0.8.2/annotation_tool/dialogs/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/file_cache/_file_cache.py` & `annotation_tool-0.8.2/annotation_tool/file_cache/_file_cache.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/gui.py` & `annotation_tool-0.8.2/annotation_tool/gui.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/main_controller.py` & `annotation_tool-0.8.2/annotation_tool/main_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # init media_reader
 set_fallback_fps(settings.refresh_rate)
 
 
 class MainApplication(qtw.QApplication):
     update_media_pos = qtc.pyqtSignal(int)
     update_annotation_pos = qtc.pyqtSignal(int)
+    load_media = qtc.pyqtSignal(str, list)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         # Controll-Attributes
         self.current_annotation = None
         self.n_frames = 0
@@ -63,14 +64,15 @@
         self.playback.paused.connect(self.media_player.pause)
         self.playback.replay_speed_changed.connect(self.media_player.set_replay_speed)
 
         # from media_player
         self.media_player.additional_media_changed.connect(
             self.set_additional_media_paths
         )
+        self.load_media.connect(self.media_player.load)
         self.media_player.loaded.connect(self.media_player_loaded)
 
         # from QAnnotationWidget
         self.annotation_controller.samples_changed.connect(self.timeline.set_samples)
         self.annotation_controller.right_widget_changed.connect(
             lambda w: self.gui.set_widget(w, LayoutPosition.RIGHT)
         )
@@ -113,21 +115,24 @@
     def load_state(self, annotation: Annotation):
         if annotation is not None:
             # store annotation
             self.current_annotation = annotation
 
             media = media_reader(path=annotation.path)
             duration = media.duration
-            n_frames = media.n_frames
+            n_frames = len(media)
 
             FrameTimeMapper.instance().update(n_frames=n_frames, millis=duration)
 
             # load media
-            self.media_player.additional_media_changed.disconnect()  # disconnect to filter out outdated signals
-            self.media_player.load(media.path)
+            # self.media_player.additional_media_changed.disconnect()  # disconnect to filter out outdated signals
+            # self.media_player.load(media.path)
+            self.load_media.emit(
+                annotation.path, annotation.get_additional_media_paths()
+            )  # noqa TODO: Make get_additional_media_paths() a property
 
             # update network module
             network.update_file(media.path)
 
             # save for later reuse
             self.n_frames = n_frames
 
@@ -147,37 +152,37 @@
             self.annotation_controller.load(
                 annotation.samples,
                 annotation.dataset.scheme,
                 annotation.dataset.dependencies,
                 n_frames,
             )
 
-            self.mediator.set_position(0, force_update=True)
+            # self.mediator.set_position(0, force_update=True)
+            self.mediator.reset_position()
 
             self.save_annotation()
 
         else:
             raise RuntimeError("State must not be None")
 
     @qtc.pyqtSlot(list)
     def set_additional_media_paths(self, paths: list):
         assert self.current_annotation is not None
-        logging.debug(
-            f"self.global_state: {self.current_annotation.path = } {self.current_annotation.get_additional_media_paths() = }"
-        )
         self.current_annotation.set_additional_media_paths(paths)
 
     @qtc.pyqtSlot()
     def media_player_loaded(self):
         assert self.current_annotation is not None
         self.media_player.additional_media_changed.connect(
             self.set_additional_media_paths
         )  # reconnect after loading
-        additional_media = self.current_annotation.get_additional_media_paths()
-        self.media_player.set_additional_media(additional_media)
+
+        # additional_media = self.current_annotation.get_additional_media_paths()
+        # self.media_player.set_additional_media(additional_media)
+        logging.debug("media_player_loaded")
 
     def save_annotation(self):
         if self.current_annotation is not None:
             samples = self.annotation_controller.controller.samples
 
             if len(samples) > 0:
                 assert samples[-1].end_position + 1 == self.n_frames
@@ -203,15 +208,15 @@
         filehandler.set_logging_level(settings.logging_level)
 
         set_fallback_fps(settings.refresh_rate)
 
         if self.current_annotation is not None:
             media = media_reader(path=self.current_annotation.path)
             duration = media.duration
-            n_frames = media.n_frames
+            n_frames = len(media)
 
             FrameTimeMapper.instance().update(n_frames=n_frames, millis=duration)
 
         self.timeline.update()
 
     def update_theme(self):
         self.setStyle("Fusion")
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media/backend/controller.py` & `annotation_tool-0.8.2/annotation_tool/media/backend/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import enum
 import logging
-from typing import List, Tuple
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
 
 from annotation_tool.media.backend.player import AbstractMediaPlayer
-from annotation_tool.media.backend.timer import Timer
+from annotation_tool.media.backend.timer import Synchronizer
 from annotation_tool.media.backend.type_specific_player.mocap import MocapPlayer
 from annotation_tool.media.backend.type_specific_player.video import VideoPlayer
 from annotation_tool.media_reader import media_type_of
 
 media_proxy_map = {}
 
 
@@ -18,169 +18,180 @@
     ACK_timeout: qtc.pyqtSignal = qtc.pyqtSignal(qtc.QObject)
     ACK_setpos: qtc.pyqtSignal = qtc.pyqtSignal(qtc.QObject)
     set_position = qtc.pyqtSignal(int)
     timeout = qtc.pyqtSignal()
 
     def __init__(self, media_widget: AbstractMediaPlayer):
         super().__init__()
-        media_widget.ACK_timeout.connect(self.forward_ACK_timeout)
-        media_widget.ACK_setpos.connect(self.forward_ACK_setpos)
-        self.timeout.connect(media_widget.on_timeout)
         self.set_position.connect(media_widget.set_position)
 
         media_proxy_map[id(media_widget)] = self
         self.media_widget = media_widget
 
-        self.fps = media_widget.fps
-
-    @qtc.pyqtSlot(qtc.QObject)
-    def on_timeout_(self, proxy):
-        if proxy is self:
-            self.timeout.emit()
+        self._fps = media_widget.fps
 
     @qtc.pyqtSlot(qtc.QObject, int)
     def set_position_(self, proxy, position):
         if proxy is self:
             self.set_position.emit(position)
 
-    @qtc.pyqtSlot()
-    def forward_ACK_timeout(self):
-        self.ACK_timeout.emit(self)
-
-    @qtc.pyqtSlot()
-    def forward_ACK_setpos(self):
-        self.ACK_setpos.emit(self)
-
     @property
     def position(self):
         return self.media_widget.position
 
     @property
+    def fps(self):
+        return self._fps
+
+    @property
+    def n_frames(self):
+        return self.media_widget.n_frames
+
+    @property
     def main_replay_widget(self):
         return self.media_widget._is_main_replay_widget
 
 
+class MediaState(enum.Enum):
+    LOADING = 0
+    AVAILABLE = 1
+
+
 class QMediaMainController(qtw.QWidget):
-    position_changed = qtc.pyqtSignal(int)
+    timeout = qtc.pyqtSignal(int)
     query_position_update = qtc.pyqtSignal(int)
     setPaused = qtc.pyqtSignal(bool)
     stop = qtc.pyqtSignal()
     replay_speed_changed = qtc.pyqtSignal(float)
     subscribe = qtc.pyqtSignal(qtc.QObject)
     unsubscribe = qtc.pyqtSignal(qtc.QObject)
     reset = qtc.pyqtSignal()
     additional_media_changed = qtc.pyqtSignal(list)
     loaded = qtc.pyqtSignal()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.replay_widgets = []
 
+        self.STATE = MediaState.AVAILABLE
+        self._open_loading_tasks = 0
+
         self.grid = qtw.QGridLayout(self)
         self.grid.setContentsMargins(0, 0, 0, 10)
         self.MAX_WIDGETS = 4
 
         self.init_timer()
 
         self.vbox = qtw.QVBoxLayout()
         self.vbox.setContentsMargins(0, 0, 0, 0)
         self.grid.addLayout(self.vbox, 0, 1)
 
         self._dead_widgets = []
         self._widget_2_path = {}
 
-        self._loading_idx = 0  # keep track of how many times load() was called
-        self._loading_widgets: List[Tuple[AbstractMediaPlayer, int]] = []
+    @qtc.pyqtSlot(str, list)
+    def load(self, file, additional_media=[]):
+        if self.STATE == MediaState.AVAILABLE:
+            self.STATE = MediaState.LOADING
+            self._load(file, additional_media)
+        else:
+            logging.warning("Media is already loading -> ignoring new loading")
 
-    @qtc.pyqtSlot(str)
-    def load(self, file):
-        self._loading_idx += 1
+    def _load(self, file, additional_media=[]):
         self.pause()
         self.clear(notify=False)
         self.reset.emit()
-        self.add_replay_widget(file, is_main_widget=True)
+
+        assert (
+            self._open_loading_tasks == 0
+        ), f"Open loading tasks must be 0 but is {self._open_loading_tasks}"
+        assert (
+            len(self.replay_widgets) == 0
+        ), f"Replay widgets must be 0 but is {len(self.replay_widgets)}"
+        assert (
+            self.STATE == MediaState.LOADING
+        ), f"State must be LOADING but is {self.STATE}"
+
+        self._open_loading_tasks = 1 + len(additional_media)
+
+        self.add_replay_widget(file, is_main_widget=True, from_load=True)
+        for path in additional_media:
+            self.add_replay_widget(path, from_load=True)
 
     def clear(self, notify=True):
         while self.replay_widgets:
             self.remove_replay_source(self.replay_widgets[0], notify)
 
-    def add_replay_widget(self, path, is_main_widget=False):
+    def add_replay_widget(self, path, is_main_widget=False, from_load=False):
+        if self.STATE == MediaState.LOADING and not from_load:
+            logging.warning("Media is loading -> ignoring new replay widget")
+            return
         if len(self.replay_widgets) < self.MAX_WIDGETS:
             # is_main_widget = len(self.replay_widgets) == 0
 
             # select correct media_player
 
             media_type = media_type_of(path)
             if media_type == "video":
                 widget = VideoPlayer(is_main_widget, self)
             elif media_type == "mocap":
                 widget = MocapPlayer(is_main_widget, self)
             else:
-                raise NotImplementedError("Media type not supported")
+                raise NotImplementedError(f"Media type {media_type} is not supported")
 
             if widget.is_main_replay_widget:
-                widget.position_changed.connect(self.position_changed)
                 self.grid.addWidget(widget, 0, 0)
             else:
-                widget._reference_fps = self.replay_widgets[0].fps
-                widget._reference_N = self.replay_widgets[0].n_frames
                 widget.remove_wanted.connect(self.remove_replay_source)
                 self.vbox.addWidget(widget)
 
             if not widget.is_main_replay_widget:
                 self._widget_2_path[id(widget)] = path
 
             widget.loaded.connect(self.widget_loaded)
             widget.failed.connect(self.widget_failed)
-            self._loading_widgets.append(
-                (widget, self._loading_idx)
-            )  # keep track of which widget was loaded when
             widget.load(path)
 
-    @qtc.pyqtSlot(AbstractMediaPlayer)
-    def widget_loaded(self, widget: AbstractMediaPlayer):
-        # remove widget from loading list
-        for i, (w, idx) in enumerate(self._loading_widgets):
-            if w is widget:
-                _, idx_ = self._loading_widgets.pop(i)
-                break
+    def _check_loading_finished(self):
+        if self.STATE == MediaState.LOADING:
+            self._open_loading_tasks -= 1
+            if self._open_loading_tasks == 0:
+                self.STATE = MediaState.AVAILABLE
+                self.loaded.emit()
+            assert (
+                self._open_loading_tasks >= 0
+            ), f"Open loading tasks must be >= 0 but is {self._open_loading_tasks}"
         else:
-            raise RuntimeError("Widget was not in loading list")
+            assert (
+                self._open_loading_tasks == 0
+            ), f"Open loading tasks must be 0 but is {self._open_loading_tasks}"
 
+    @qtc.pyqtSlot(AbstractMediaPlayer)
+    def widget_loaded(self, widget: AbstractMediaPlayer):
         # check if widget belongs to current loading process
-        if idx_ != self._loading_idx:
-            self.remove_replay_source(widget, ignore_errors=True)
-            logging.debug(
-                f"Widget {widget} was loaded in a previous loading process. Ignoring it."
-            )
-            return
 
         widget.new_input_wanted.connect(self.add_replay_widget)
         widget.finished.connect(self.widget_terminated)
         self.replay_widgets.append(widget)
         proxy = MediaProxy(widget)
 
-        if not widget.is_main_replay_widget:
-            self.additional_media_changed.emit(self._widget_2_path.values())
-        else:
-            self.loaded.emit()
         self.subscribe.emit(proxy)
 
+        if not widget.is_main_replay_widget and self.STATE != MediaState.LOADING:
+            self.additional_media_changed.emit(self._widget_2_path.values())
+
+        self._check_loading_finished()  # check if loading is finished
+
     @qtc.pyqtSlot(AbstractMediaPlayer)
     def widget_failed(self, widget):
-        # remove widget from loading list
-        for i, (w, idx) in enumerate(self._loading_widgets):
-            if w is widget:
-                _, idx_ = self._loading_widgets.pop(i)
-                break
-        else:
-            raise RuntimeError("Widget was not in loading list")
-
         self.remove_replay_source(widget, ignore_errors=True)
         logging.error(f"COULD NOT LOAD {widget = }")
+
+        self._check_loading_finished()  # check if loading is finished
+
         raise RuntimeError
 
     def remove_replay_source(self, widget, notify=True, ignore_errors=False):
         self.grid.removeWidget(widget)
         self.vbox.removeWidget(widget)
         proxy = media_proxy_map.get(id(widget))
         if proxy:
@@ -230,33 +241,36 @@
     def set_position(self, pos):
         self.query_position_update.emit(pos)
 
     @qtc.pyqtSlot(float)
     def set_replay_speed(self, x):
         self.replay_speed_changed.emit(x)
 
+    def on_timeout(self, pos):
+        self.timeout.emit(pos)
+
     def init_timer(self):
         self.timer_thread = qtc.QThread()
-        self.timer_worker = Timer()
+        self.timer_worker = Synchronizer()
         self.timer_worker.moveToThread(self.timer_thread)
 
         # connecting worker and thread
-        self.timer_thread.started.connect(self.timer_worker.run)
         self.timer_worker.finished.connect(self.timer_thread.quit)
         self.timer_worker.finished.connect(self.timer_worker.deleteLater)
         self.timer_thread.finished.connect(self.timer_thread.deleteLater)
 
         # connecting signals and slots
-        self.setPaused.connect(self.timer_worker.setPaused)
+        self.setPaused.connect(self.timer_worker.set_paused)
         self.stop.connect(self.timer_worker.stop)
         self.reset.connect(self.timer_worker.reset)
         self.replay_speed_changed.connect(self.timer_worker.set_replay_speed)
         self.subscribe.connect(self.timer_worker.subscribe)
         self.unsubscribe.connect(self.timer_worker.unsubscribe)
-        self.query_position_update.connect(self.timer_worker.query_position_update)
+        self.query_position_update.connect(self.timer_worker.set_position)
+        self.timer_worker.timeout.connect(self.on_timeout)
 
         self.timer_thread.start()
 
     def shutdown(self):
         self.clear(notify=False)
         self.stop.emit()
         self.timer_thread.quit()
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media/backend/type_specific_player/mocap.py` & `annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/mocap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import logging
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtWidgets as qtw
 import numpy as np
 import pyqtgraph.opengl as gl
 
-from annotation_tool.media.backend.player import AbstractMediaPlayer, UpdateReason
+from annotation_tool.media.backend.player import AbstractMediaPlayer
 from annotation_tool.media_reader import media_reader as mr
 
 
 class MocapPlayer(AbstractMediaPlayer):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.media_backend = MocapBackend(self)  # setting parent to self
 
     def load(self, path):
         media = mr(path)
         self.media_backend.media = media
         self.layout().addWidget(self.media_backend)
         self.n_frames = len(media)
-        self.update_media_position(UpdateReason.INIT)
+        self.update_media_position()
         self.loaded.emit(self)
 
-    def update_media_position(self, update_reason: UpdateReason):
+    def update_media_position(self):
         pos = self.position + self.offset
         pos_adjusted = max(0, min(pos, self.n_frames - 1))
         self.media_backend.set_position(pos_adjusted)
-        self.confirm_update(update_reason)
 
     def shutdown(self):
         self.setFixedSize(0, 0)
         self.hide()
         self.media_backend.shutdown()
         self.media_backend = None
         self.terminated = True
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media/backend/type_specific_player/video.py` & `annotation_tool-0.8.2/annotation_tool/media/backend/type_specific_player/video.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,85 @@
 import logging
+from threading import Thread
+from time import sleep
 
 import PyQt6.QtCore as qtc
 import PyQt6.QtGui as qtg
 import PyQt6.QtWidgets as qtw
-import cv2
 
-from annotation_tool.media.backend.player import AbstractMediaPlayer, UpdateReason
+from annotation_tool.media.backend.player import AbstractMediaPlayer
 from annotation_tool.media_reader import media_reader as mr
 
 
+def check_resize(vp):
+    w, h = vp.lblVid.width(), vp.lblVid.height()
+    while True:
+        try:
+            active = vp._active  # noqa
+        except:  # noqa
+            break
+        if not active:
+            break
+        if w != vp.lblVid.width() or h != vp.lblVid.height():
+            vp.get_update.emit()
+            w, h = vp.lblVid.width(), vp.lblVid.height()
+        sleep(0.1)
+
+
 class VideoPlayer(AbstractMediaPlayer):
-    get_update = qtc.pyqtSignal(UpdateReason)
+    get_update = qtc.pyqtSignal()
     media_loaded = qtc.pyqtSignal(object)
     load_worker = qtc.pyqtSignal(str)
     stop_worker = qtc.pyqtSignal()
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
         self.lblVid = qtw.QLabel(self)
         self.lblVid.setSizePolicy(
             qtw.QSizePolicy.Policy.Ignored, qtw.QSizePolicy.Policy.Ignored
         )
         self.lblVid.setAlignment(qtc.Qt.AlignmentFlag.AlignCenter)
         self.layout().addWidget(self.lblVid)
 
-        self._pix = None
-        self._pix_mutex = qtc.QMutex()
-
         # design
-        p = self.palette()
-        p.setColor(self.backgroundRole(), qtc.Qt.GlobalColor.black)
-        self.setPalette(p)
         self.layout().setContentsMargins(0, 0, 0, 0)
-        # self.setAutoFillBackground(True)
 
         self.worker_thread = qtc.QThread()
         self.worker = VideoHelper(self)
         self.init_worker()
 
         self._active = True
 
+        self.resize_worker = Thread(target=check_resize, args=(self,), daemon=True)
+        self.resize_worker.start()
+
     def load(self, path):
         self.load_worker.emit(path)
 
-    @qtc.pyqtSlot(int, int)
+    @qtc.pyqtSlot(float, int)
     def worker_loaded(self, fps, n_frames):
         self.fps = fps
         self.n_frames = n_frames
         self.loaded.emit(self)
         self.adjustSize()
 
-    def resizeEvent(self, event):
-        qtw.QWidget.resizeEvent(self, event)
-        self.lblVid.resize(event.size())
-        self.get_update.emit(UpdateReason.IGNORE)
-
-    def update_media_position(self, update_reason: UpdateReason):
-        self.get_update.emit(update_reason)
-
-    @qtc.pyqtSlot(UpdateReason)
-    def update_pixmap(self, update_reason: UpdateReason):
-        self.lblVid.setPixmap(self.pix)
-        self.confirm_update(update_reason)
-
-    @qtc.pyqtSlot(UpdateReason)
-    def no_update_needed(self, update_reason):
-        self.confirm_update(update_reason)
+    def update_media_position(self):
+        self.get_update.emit()
+
+    @qtc.pyqtSlot(qtg.QPixmap)
+    def update_pixmap(self, pix):
+        self.lblVid.setPixmap(pix)
 
     def init_worker(self):
         self.worker.moveToThread(self.worker_thread)
 
         # connecting to worker
         self.load_worker.connect(self.worker.load)
         self.get_update.connect(self.worker.update)
-        self.worker.no_update_needed.connect(self.no_update_needed)
         self.worker.image_ready.connect(self.update_pixmap)
         self.worker.loaded.connect(self.worker_loaded)
         self.stop_worker.connect(self.worker.stop)
 
         # setup nice exit
         self.worker.finished.connect(self.worker_thread.quit)
         self.worker_thread.finished.connect(self.thread_finished)
@@ -118,29 +119,18 @@
             try:
                 self.worker_thread.quit()
                 self.worker_thread.wait()
             except RuntimeError:
                 logging.debug("VideoPlayer: Worker-Thread already terminated.")
             self.worker_thread = None
 
-    @property
-    def pix(self):
-        with qtc.QMutexLocker(self._pix_mutex):
-            return self._pix
-
-    @pix.setter
-    def pix(self, pix):
-        with qtc.QMutexLocker(self._pix_mutex):
-            self._pix = pix
-
 
 class VideoHelper(qtc.QObject):
-    image_ready = qtc.pyqtSignal(UpdateReason)
-    no_update_needed = qtc.pyqtSignal(UpdateReason)
-    loaded = qtc.pyqtSignal(int, int)
+    image_ready = qtc.pyqtSignal(qtg.QPixmap)
+    loaded = qtc.pyqtSignal(float, int)
     finished = qtc.pyqtSignal()
 
     def __init__(self, video_player: VideoPlayer):
         super().__init__()
         self._video_player = video_player
         self.media = None
 
@@ -167,35 +157,34 @@
             return self.media.fps
 
     @property
     def path(self):
         if self.media:
             return self.media.path
 
-    @qtc.pyqtSlot(UpdateReason)
-    def update(self, update_reason):
+    @qtc.pyqtSlot()
+    def update(self):
         if self._finished:
             return
-        self.__update__(update_reason)
+        self.__update__()
 
-    def __update__(self, update_reason):
+    def __update__(self):
         pos = self._video_player.position + self._video_player.offset
         width, height = (
             self._video_player.lblVid.width(),
             self._video_player.lblVid.height(),
         )
 
         pos = max(0, min(self.n_frames - 1, pos))
 
         dims_changed = width != self._last_w or height != self._last_h
         pos_changed = pos != self._last_pos
 
         if not pos_changed and not dims_changed:
             # no update needed
-            self.no_update_needed.emit(update_reason)
             return
 
         self._last_pos = pos
         self._last_w = width
         self._last_h = height
 
         if not pos_changed:
@@ -204,27 +193,25 @@
             img = img.scaled(
                 width,
                 height,
                 qtc.Qt.AspectRatioMode.KeepAspectRatio,
                 qtc.Qt.TransformationMode.SmoothTransformation,
             )
             pix = qtg.QPixmap.fromImage(img)
-            self._video_player.pix = pix  # set pixmap
 
             try:
-                self.image_ready.emit(update_reason)
+                self.image_ready.emit(pix)
             except RuntimeError:
                 # widget already deleted
                 pass
             return
 
         # full update
         frame = self.media[pos]  # Loading image and pixmap
         if frame is not None:
-            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
 
             h, w, ch = frame.shape
             bytes_per_line = ch * w
 
             img = qtg.QImage(
                 frame, w, h, bytes_per_line, qtg.QImage.Format.Format_RGB888
             )
@@ -235,22 +222,16 @@
                 width,
                 height,
                 qtc.Qt.AspectRatioMode.KeepAspectRatio,
                 qtc.Qt.TransformationMode.SmoothTransformation,
             )
             pix = qtg.QPixmap.fromImage(img)
 
-            self._video_player.pix = pix  # set pixmap
-            try:
-                self.image_ready.emit(update_reason)
-            except RuntimeError:
-                pass  # widget already deleted
-        else:
             try:
-                self.no_update_needed.emit(update_reason)
+                self.image_ready.emit(pix)
             except RuntimeError:
                 pass  # widget already deleted
 
     @qtc.pyqtSlot()
     def stop(self):
         self._finished = True
         # self._video_player = None
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media/media.py` & `annotation_tool-0.8.2/annotation_tool/media/media.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class QMediaWidget(qtw.QWidget):
     """
     A simple facade, forwarding all necessary slots and signals
     between the main-application and the media-backend.
 
     Signals:
         position_changed
-            Transports the current position of the main replaysource
+            Transports the current position of the main replay source
             (always the leftmost on the screen)
 
     Slots:
         load
            Expects an Annotation-instance
         set_position
             Updates the current displayed frame
@@ -34,24 +34,24 @@
     position_changed = qtc.pyqtSignal(int)
     loaded = qtc.pyqtSignal()
     additional_media_changed = qtc.pyqtSignal(list)
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.controller = QMediaMainController()
-        self.controller.position_changed.connect(self.position_changed)
+        self.controller.timeout.connect(self.position_changed)
         self.controller.additional_media_changed.connect(self.additional_media_changed)
         self.controller.loaded.connect(self.loaded)
         self._layout = qtw.QHBoxLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(self.controller)
 
-    @qtc.pyqtSlot(str)
-    def load(self, file):
-        self.controller.load(file)
+    @qtc.pyqtSlot(str, list)
+    def load(self, file, additional_media=[]):
+        self.controller.load(file, additional_media)
 
     @qtc.pyqtSlot(list)
     def set_additional_media(self, files):
         for f in files:
             self.controller.add_replay_widget(f)
 
     @qtc.pyqtSlot(int)
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media_reader/base.py` & `annotation_tool-0.8.2/annotation_tool/media_reader/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 import logging
 import os
 from typing import Optional, Union
 
-import cv2 as cv
 import numpy as np
 
 __FALLBACK_FPS__ = 30  # fallback framerate if no framerate can be determined
 
 
 def set_fallback_fps(fps: float) -> None:
     """
@@ -35,108 +34,67 @@
 
 
 class MediaReader(abc.ABC):
     """
     Baseclass for media readers (e.g. video, mocap, etc.)
     """
 
+    @abc.abstractmethod
     def __init__(self, path: os.PathLike, **kwargs) -> None:
         """
         Initializes a new __MediaReader object.
 
         Args:
             path: The path to the media file.
             kwargs: {fps: The framerate of the media data., n_frames: The number of frames in the media data.}
 
         Raises:
             FileNotFoundError: If the file does not exist.
         """
-
-        # check parameters
-        if not os.path.isfile(path):
-            raise FileNotFoundError(path)
-
-        self._path: os.PathLike = path
-
-        if "fps" in kwargs:
-            fps = kwargs["fps"]
-            assert (
-                isinstance(fps, (int, float)) and fps > 0 or fps is None
-            ), f"Framerate must be a positive number or None, not {fps}."
-            self._fps = fps
-        else:
-            self._fps = self.__detect_fps__()
-
-        if "n_frames" in kwargs:
-            n_frames = kwargs["n_frames"]
-            assert (
-                isinstance(n_frames, int) and n_frames > 0
-            ), f"Number of frames must be an positive integer, not {n_frames}."
-            self._n_frames = n_frames
-        else:
-            self._n_frames = self.__detect_n_frames__()
-
-    @property
-    def path(self) -> os.PathLike:
-        return self._path
+        if not os.path.exists(path):
+            raise FileNotFoundError(f"File {path} does not exist.")
 
     @property
     def duration(self) -> int:
         """
         Returns the duration of the media in milliseconds.
         """
-        return int(self.n_frames / self.fps) * 1000
+        try:
+            _duration = self.__get_duration__()
+        except NotImplementedError:
+            _duration = None
+        if _duration:
+            return int(self.__get_duration__()) * 1000
+        else:
+            return int(len(self) / self.fps) * 1000
 
     @property
     def fps(self) -> float:
-        if self._fps:
-            return self._fps
+        _fps = self.__get_fps__()
+        if _fps:
+            return _fps
         else:
             return get_fallback_fps()
 
     @fps.setter
     def fps(self, fps: Union[int, float]) -> None:
-        if isinstance(fps, (int, float)):
-            self._fps = fps
-        else:
-            raise TypeError("Framerate must be a number.")
-
-    @property
-    def n_frames(self) -> int:
-        return self._n_frames
+        self.__set_fps__(fps)
 
     @property
-    def media(self):
-        return __memoizer__(self)
-
-    def raw_fps(self) -> Optional[float]:
-        """
-        Returns the framerate of the media data.
-        If the framerate cannot be determined, returns None.
-
-        Returns:
-            The framerate of the media data.
-        """
-        return self._fps
+    def path(self) -> os.PathLike:
+        return self.__get_path__()
 
     def __len__(self):
-        return self.n_frames
-
-    def __eq__(self, other) -> bool:
-        if isinstance(other, MediaReader):
-            return self.id == other.id
-        return False
-
-    def __del__(self):
-        __memoizer__.remove(self)
+        return self.__get_frame_count__()
 
     def __getitem__(self, idx):
         """
         Returns the frame at the given index.
         If the index is a slice, returns a list of frames.
+        The shape of the frame depends on the media type, e.g. for video it is (h,w,c) with c being the 3-RGB channels.
 
         Args:
             idx: The index/indices of the frame(s) to return.
         Returns:
             The frame(s) at the given indices.
         Raises:
             IndexError: If the index is out of range.
@@ -150,94 +108,75 @@
         elif isinstance(idx, int):
             if idx >= len(self):
                 raise IndexError("Index out of range.")
             return self.__get_frame__(idx)
         else:
             raise TypeError("Invalid argument type.")
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.__del__()
+    def __iter__(self):
+        return self[:]
 
     @abc.abstractmethod
     def __get_frame__(self, idx: int) -> np.ndarray:
         """
         Returns the frame at the given index.
 
         Args:
             idx: The index of the frame to return.
         Returns:
             The frame at the given index.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __read_media__(self):
+    def __get_frame_count__(self) -> int:
         """
-        Reads the media file.
+        Returns the number of frames in the media file.
+
+        Returns:
+            The number of frames in the media file.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __detect_fps__(self) -> Optional[float]:
+    def __get_duration__(self) -> Optional[float]:
         """
-        Detects the framerate of the media file.
-
-        Returns:
-            The framerate of the media file if it can be detected, None otherwise.
+        Returns the duration of the media in seconds.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def __detect_n_frames__(self) -> int:
+    def __get_fps__(self) -> Optional[float]:
         """
-        Detects the number of frames in the media file.
+        Detects the framerate of the media file.
 
         Returns:
-            The number of frames in the media file.
+            The framerate of the media file if it can be detected, None otherwise.
         """
         raise NotImplementedError
 
-
-class __Memoizer:
-    def __init__(self):
-        self._cache = {}
-
-    def __call__(self, mr: MediaReader) -> Union[cv.VideoCapture, np.ndarray]:
+    @abc.abstractmethod
+    def __get_path__(self) -> os.PathLike:
         """
-        Returns the memorized version of the given __MediaReader.
-
-        Args:
-            mr: The __MediaReader to memorize.
+        Returns the path to the media file.
 
         Returns:
-            The memorized version of the __MediaReader.
+            The path to the media file.
         """
-        if not isinstance(mr, MediaReader):
-            raise TypeError("Invalid argument type.")
-        key = id(mr)
-        if key not in self._cache:
-            media = mr.__read_media__()
-            self._cache[key] = media
-
-        return self._cache[key]
+        raise NotImplementedError
 
-    def remove(self, mr: MediaReader) -> None:
+    @abc.abstractmethod
+    def __set_fps__(self, fps: Union[int, float]) -> None:
         """
-        Removes the given __MediaReader from the cache.
+        Sets the framerate of the media file.
 
         Args:
-            mr: The __MediaReader to remove.
+            fps: The framerate to set.
         """
-        key = id(mr)
-        if key in self._cache:
-            del self._cache[key]
-            logging.debug(f"Removed {mr} from cache. Cache size: {len(self._cache)}")
+        raise NotImplementedError
 
 
 class __MediaSelector:
     def __init__(self):
         self._selector_functions = {}
 
     def register(self, media_type: str, selector_function: callable) -> None:
@@ -312,18 +251,16 @@
         factory = self._builders.get(media_type)
         if factory is None:
             raise ValueError(f"Unsupported media type: {media_type}")
         return factory(**kwargs)
 
 
 # Global variables, should be singleton instances
-__memoizer__ = __Memoizer()
 __media_selector__ = __MediaSelector()
 __media_factory__ = __MediaFactory()
-__kwarg_dict__ = {}
 
 
 def register_media_reader(
     media_type: str, selector_function: callable, factory: callable
 ) -> None:
     """
     Registers a new media reader.
@@ -336,39 +273,31 @@
     Raises:
         TypeError: If the media_type is not a string or the selector_function or factory is not a callable.
     """
     __media_selector__.register(media_type, selector_function)
     __media_factory__.register(media_type, factory)
 
 
-def media_reader(path: os.PathLike, **ignored) -> MediaReader:
+def media_reader(path: os.PathLike, **kwargs) -> MediaReader:
     """
     Returns a MediaReader for the given path.
 
     Args:
         path: The path to the media file.
-        **kwargs: Additional arguments to pass to the MediaReader constructor.
 
     Returns:
         A MediaReader for the given path.
 
     Raises:
         ValueError: If the media type could not be determined.
     """
 
-    kwargs = __kwarg_dict__.get(path, {})
-
     media_type = __media_selector__.select(path)
     mr = __media_factory__.create(media_type, path=path, **kwargs)
 
-    __kwarg_dict__[path] = {
-        "fps": mr.raw_fps(),
-        "n_frames": mr.n_frames,
-    }  # fps-property hides None-values, raw_fps() does not
-
     return mr
 
 
 def media_type_of(path: os.PathLike) -> str:
     """
     Returns the media type of the given path.
```

### Comparing `annotation_tool-0.8.1/annotation_tool/media_reader/mocap.py` & `annotation_tool-0.8.2/annotation_tool/media_reader/mocap_readers/lara_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,63 @@
-from functools import lru_cache
 import logging
 import os
+from pathlib import Path
 from typing import Optional
 
 import numpy as np
 
-from .base import MediaReader, register_media_reader
+try:
+    from .cache import get_cache
+except ImportError:
+    from cache import get_cache
+except Exception:
+    get_cache = None
+
+try:
+    from .base import MocapReaderBase, register_mocap_reader
+except ImportError:
+    from base import MocapReaderBase, register_mocap_reader
 
 
-@lru_cache(maxsize=1)
-def get_settings():
-    from ..settings import settings
-
-    return settings
-
-
-def get_mocap(*args):
-    return load_mocap(*args)
-
-
-@lru_cache(maxsize=10)
-def load_mocap(path: os.PathLike, data_type: np.dtype = np.float32) -> np.ndarray:
+def load_lara_mocap(path: Path, data_type: np.dtype = float) -> np.ndarray:
     """
-    Load Motion-capture data from file to numpy array.
-    The mocap data is cached, so that the same mocap data is not loaded twice.
+    Loads the LARa-mocap data from a file.
 
     Args:
-        path (os.PathLike): Path to motion-capture data.
-        data_type (np.dtype, optional): Data type of the returned array. Defaults to np.float32.
-    Raises:
-        TypeError: If the path could not be parsed as a Motion-capture file.
+        path (os.PathLike): The path to the LARa-mocap file.
+        data_type (np.dtype): The data type of the returned data.
 
     Returns:
-        np.ndarray: Array containing the loaded motion-capture data.
+        np.ndarray: The mocap data.
+
+    Raises:
+        AssertionError: If the data type is not supported.
     """
-    try:
-        array = __load_lara_mocap__(path)
-        return array.astype(data_type)
-    except TypeError as e:
-        raise TypeError("Loading mocap failed.") from e
+    assert data_type in [
+        np.float16,
+        np.float32,
+        np.float64,
+        float,
+    ], f"Invalid dtype {data_type} for mocap data."
+    assert isinstance(path, Path), "Path must be a pathlib.Path object."
+
+    if get_cache is None:
+        logging.warning("Cache not available. Loading mocap from file.")
+        return __load_lara_mocap__(path).astype(data_type)
+    else:
+        mocap_cache = get_cache()
+
+        if path in mocap_cache:
+            logging.debug(f"Loaded mocap from cache: {path}")
+            return mocap_cache[path].astype(data_type)
+        else:
+            logging.debug(f"Loaded mocap from file: {path}")
+            mocap = __load_lara_mocap__(path).astype(data_type)
+            mocap_cache[path] = mocap
+            return mocap
 
 
 def __load_lara_mocap__(path: os.PathLike) -> np.ndarray:
     """
     Loads the LARa-mocap data from a file.
     Right now the LARa-file is expected to contain either 1 or 5 header lines.
     There should be 132 columns of data + 2 columns for the frame number and the subject.
@@ -126,81 +141,68 @@
     normalizing_vector = array[:, 66:72]  # 66:72 are the columns for lower back
     for _ in range(21):
         normalizing_vector = np.hstack((normalizing_vector, array[:, 66:72]))
     array = np.subtract(array, normalizing_vector)
     return array
 
 
-class MocapReader(MediaReader):
+class LARaMocapReader(MocapReaderBase):
     """Class for reading mocap data."""
 
     def __init__(self, path, **kwargs) -> None:
         """
         Initializes a new MocapReader object.
 
         Args:
             path (os.PathLike): The path to the mocap file.
             fps (float): The framerate of the mocap data.
 
         Raises:
             FileNotFoundError: If the file does not exist.
         """
 
-        super().__init__(path, **kwargs)
+        self.path = path
+        self._dtype = kwargs.get("dtype", float)
+        self.mocap = load_lara_mocap(Path(self.path), self._dtype)
 
-    def __get_frame__(self, idx: int) -> np.ndarray:
+    def get_frame(self, frame_idx: int) -> np.ndarray:
         """
         Returns the skeleton at the given frame index.
 
         Args:
-            idx (int): Frame index.
+            frame_idx (int): Frame index.
 
         Returns:
             np.ndarray: Skeleton at the given frame index.
 
         Raises:
             IndexError: If the index is out of range.
         """
-        if idx < 0 or idx >= len(self):
+        if frame_idx < 0 or frame_idx >= self.get_frame_count():
             raise IndexError("Index out of range.")
 
-        return self.media[idx]
+        return self.mocap[frame_idx]
 
-    def __read_media__(self):
-        return np.copy(load_mocap(self.path))
+    def get_frame_count(self) -> int:
+        return self.mocap.shape[0]
 
-    def __detect_fps__(self) -> Optional[float]:
+    def get_fps(self) -> Optional[float]:
         return None
 
-    def __detect_n_frames__(self) -> int:
-        return len(self.media)
-
-
-def __is_mocap__(path: os.PathLike) -> bool:
-    if not os.path.isfile(path):
-        return False
-    try:
-        load_mocap(path)
-        return True
-    except TypeError:
-        return False
-
-
-def __mocap_builder__(path: os.PathLike, **kwargs) -> MocapReader:
-    """
-    Builds a MocapReader object from the given path.
-
-    Args:
-        path (os.PathLike): The path to the mocap file.
-        fps (float): The framerate of the mocap data.
+    def get_duration(self) -> float:
+        return None
 
-    Returns:
-        MocapReader: The MocapReader object.
-    """
-    return MocapReader(path, **kwargs)
+    def get_path(self) -> os.PathLike:
+        return self.path
 
+    @staticmethod
+    def is_supported(path: os.PathLike) -> bool:
+        # TODO: improve this
+        try:
+            load_lara_mocap(Path(path))
+            return True
+        except:  # noqa E722
+            return False
 
-register_media_reader(
-    media_type="mocap", selector_function=__is_mocap__, factory=__mocap_builder__
-)
 
-logging.debug("MocapReader registered.")
+register_mocap_reader(LARaMocapReader, 0)
+logging.info("Registered LARa mocap reader.")
```

### Comparing `annotation_tool-0.8.1/annotation_tool/mediator.py` & `annotation_tool-0.8.2/annotation_tool/mediator.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,31 +69,34 @@
         if check1 and check2:
             if self.looping:
                 x = min(self.upper, max(self.lower, x))
             self.position = x
             for rec in self.receivers:
                 rec.set_position(x)
 
+    def reset_position(self):
+        self.position = 0
+        for rec in self.receivers:
+            rec.set_position(0)
+        for rec in self.emitters:
+            rec.set_position(0)
+
     @qtc.pyqtSlot(int)
     def on_timeout(self, x):
-        assert (0 <= x < self.n_frames) or (x == 0 == self.n_frames)
+        if (0 <= x < self.n_frames) or (x == 0 == self.n_frames):
 
-        # Filter valid timeouts -> remove outdated ones
-        if x == self.position + 1:
+            # Filter valid timeouts -> remove outdated ones
             if self.looping and x >= self.upper:
                 self.set_position(self.lower)
                 return
-            # only update non-mediaWidgets
-            self.position += 1
+
+            self.position = x
             for rec in self.receivers:
                 if not isinstance(rec, QMediaWidget):
                     rec.set_position(self.position)
-        else:
-            # logging.debug(f"Filtered outdated update = {x = }")
-            pass
 
     @qtc.pyqtSlot(bool, bool)
     def skip_frames(self, forward_step, fast):
         n = settings.big_skip if fast else settings.small_skip
         if not forward_step:
             n *= -1
```

### Comparing `annotation_tool-0.8.1/annotation_tool/network/LARa/attr_per_class.txt` & `annotation_tool-0.8.2/annotation_tool/network/LARa/attr_per_class.txt`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/network/LARa/lara_specifics.py` & `annotation_tool-0.8.2/annotation_tool/network/LARa/lara_specifics.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/network/controller.py` & `annotation_tool-0.8.2/annotation_tool/network/controller.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/network/network.py` & `annotation_tool-0.8.2/annotation_tool/network/network.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/playback.py` & `annotation_tool-0.8.2/annotation_tool/playback.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py` & `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/adaptive_scroll_area.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/checkable_combobox.py` & `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/checkable_combobox.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/display_scheme.py` & `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/display_scheme.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/histogram.py` & `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/qt_helper_widgets/own_slider.py` & `annotation_tool-0.8.2/annotation_tool/qt_helper_widgets/own_slider.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/settings.py` & `annotation_tool-0.8.2/annotation_tool/settings.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/user_actions.py` & `annotation_tool-0.8.2/annotation_tool/user_actions.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/decorators.py` & `annotation_tool-0.8.2/annotation_tool/utility/decorators.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/filehandler.py` & `annotation_tool-0.8.2/annotation_tool/utility/filehandler.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/functions.py` & `annotation_tool-0.8.2/annotation_tool/utility/functions.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/networking.py` & `annotation_tool-0.8.2/annotation_tool/utility/networking.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/priority_queue.py` & `annotation_tool-0.8.2/annotation_tool/utility/priority_queue.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/annotation_tool/utility/resources.py` & `annotation_tool-0.8.2/annotation_tool/utility/resources.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/main.py` & `annotation_tool-0.8.2/main.py`

 * *Files identical despite different names*

### Comparing `annotation_tool-0.8.1/pyproject.toml` & `annotation_tool-0.8.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "annotation-tool"
-version = "0.8.1"
+version = "0.8.2"
 description = "Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more."
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/TUD-Patrec/annotation-tool"
 authors = [
     "Fernando Moya Rueda <fernando.moya@cs.tu-dortmund.de>",
     "Erik Altermann <erik.altermann@tu-dortmund.de>",
@@ -29,18 +29,19 @@
 numpy = "~1.23.5"
 opencv-python = "~4.5.3.56"
 PyOpenGL = "^3.1.6"
 PyOpenGL-accelerate = "^3.1.6"
 PyQt6 = "^6.4.0"
 pyqtgraph = "^0.12.4"
 scipy = "^1.10.0"
-torch = "~1.12.0"
+torch = "^2.0.0"
 sortedcontainers = "^2.4.0"
 fcache = "^0.4.7"
 appdirs = "^1.4.4"
+decord = { version = "^0.6.0", platform = "win32"}
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 flake8 = "^5.0.4"
 isort = "^5.11.4"
 pyinstaller = "~5.4"
@@ -63,15 +64,15 @@
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 line_length = 88
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.8.1"
+version = "0.8.2"
 tag_format = "v$version"
 major_version_zero = true
 version_files = [
     "annotation_tool/__init__.py:^__version__",
     "pyproject.toml:^version"
 ]
 update_changelog_on_bump = false
```

### Comparing `annotation_tool-0.8.1/PKG-INFO` & `annotation_tool-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annotation-tool
-Version: 0.8.1
+Version: 0.8.2
 Summary: Tool for annotating time series data from sources such as IMUs, MoCap, Videos and more.
 Home-page: https://github.com/TUD-Patrec/annotation-tool
 License: MIT
 Author: Fernando Moya Rueda
 Author-email: fernando.moya@cs.tu-dortmund.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,23 +12,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyOpenGL (>=3.1.6,<4.0.0)
 Requires-Dist: PyOpenGL-accelerate (>=3.1.6,<4.0.0)
 Requires-Dist: PyQt6 (>=6.4.0,<7.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: decord (>=0.6.0,<0.7.0) ; sys_platform == "win32"
 Requires-Dist: distinctipy (>=1.2.2,<2.0.0)
 Requires-Dist: fcache (>=0.4.7,<0.5.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: opencv-python (>=4.5.3.56,<4.6.0.0)
 Requires-Dist: pyqtgraph (>=0.12.4,<0.13.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
-Requires-Dist: torch (>=1.12.0,<1.13.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ![PyPI - Version](https://img.shields.io/pypi/v/annotation-tool)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/annotation-tool)
 ![PyPI - License](https://img.shields.io/pypi/l/annotation-tool?color=brightgreen)
```

