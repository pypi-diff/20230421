# Comparing `tmp/PyQt6-Fluent-Widgets-0.7.1.tar.gz` & `tmp/PyQt6-Fluent-Widgets-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt6-Fluent-Widgets-0.7.1.tar", last modified: Sun Apr 16 09:00:30 2023, max compression
+gzip compressed data, was "dist\PyQt6-Fluent-Widgets-0.7.2.tar", last modified: Fri Apr 21 01:27:42 2023, max compression
```

## Comparing `PyQt6-Fluent-Widgets-0.7.1.tar` & `PyQt6-Fluent-Widgets-0.7.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.434733 PyQt6-Fluent-Widgets-0.7.1/
--rw-rw-rw-   0        0        0    35823 2023-04-15 14:33:45.000000 PyQt6-Fluent-Widgets-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     3565 2023-04-16 09:00:30.433312 PyQt6-Fluent-Widgets-0.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.281741 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     3565 2023-04-16 09:00:29.000000 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2956 2023-04-16 09:00:30.000000 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 09:00:29.000000 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-04-16 09:00:29.000000 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 09:00:29.000000 PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2765 2023-04-16 08:48:04.000000 PyQt6-Fluent-Widgets-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.283803 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/
--rw-rw-rw-   0        0        0      493 2023-04-16 08:50:56.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.287818 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3512847 2023-04-16 08:55:07.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.323390 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      390 2023-04-05 13:34:28.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10546 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     7332 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4775 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     4787 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7039 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/style_sheet.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.326389 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.335531 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      189 2023-04-16 08:50:56.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     7484 2023-04-16 08:52:22.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    19165 2023-04-16 08:56:26.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-04-16 08:50:56.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.350756 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    11953 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5468 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11761 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3227 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2424 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.359279 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2669 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5438 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1262 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.368290 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     4513 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    15733 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0     4931 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.384534 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5269 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8152 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6102 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    13044 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1470 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:00:30.431306 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0      998 2023-04-15 14:33:45.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4656 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0     5817 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0      304 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    13107 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8304 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0      757 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    19137 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0      870 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     6639 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0    24081 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     4545 2023-04-16 08:50:55.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     4848 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4554 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6343 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5923 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     6719 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     1686 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/three_state_button.py
--rw-rw-rw-   0        0        0     5263 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2971 2023-04-16 08:48:05.000000 PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tree_view.py
--rw-rw-rw-   0        0        0       42 2023-04-16 09:00:30.434733 PyQt6-Fluent-Widgets-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-04-16 08:51:04.000000 PyQt6-Fluent-Widgets-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.386281 PyQt6-Fluent-Widgets-0.7.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 03:28:34.000000 PyQt6-Fluent-Widgets-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     3565 2023-04-21 01:27:42.386281 PyQt6-Fluent-Widgets-0.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.240412 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     3565 2023-04-21 01:27:41.000000 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2956 2023-04-21 01:27:42.000000 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:27:41.000000 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-21 01:27:41.000000 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-21 01:27:41.000000 PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2765 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.241967 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/
+-rw-rw-rw-   0        0        0      493 2023-04-21 01:26:09.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.246660 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3512847 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.275531 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      390 2023-04-05 13:34:28.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10546 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0     7332 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4775 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     4787 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7039 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/style_sheet.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.276594 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.287746 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     7484 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    19208 2023-04-21 01:26:09.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.301372 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    11953 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5468 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11761 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3227 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2424 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.308542 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2669 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5438 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1262 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.320460 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     4513 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    15733 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0     4931 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.336656 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5269 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8152 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6102 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    13044 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1470 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:27:42.386281 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0      998 2023-04-18 03:28:35.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4656 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0     5817 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0      304 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    13107 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8304 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0      757 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    19255 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0      870 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     6639 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0    24081 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     4545 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     4848 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4554 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6343 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5923 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     6719 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     1686 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/three_state_button.py
+-rw-rw-rw-   0        0        0     5263 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2971 2023-04-21 01:25:51.000000 PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tree_view.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:27:42.386281 PyQt6-Fluent-Widgets-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-04-21 01:26:14.000000 PyQt6-Fluent-Widgets-0.7.2/setup.py
```

### Comparing `PyQt6-Fluent-Widgets-0.7.1/LICENSE` & `PyQt6-Fluent-Widgets-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/PKG-INFO` & `PyQt6-Fluent-Widgets-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 0.7.1
+Version: 0.7.2
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

### Comparing `PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Fluent-Widgets
-Version: 0.7.1
+Version: 0.7.2
 Summary: A fluent design widgets library based on PyQt6
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets/tree/PyQt6
```

### Comparing `PyQt6-Fluent-Widgets-0.7.1/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt6-Fluent-Widgets-0.7.2/PyQt6_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/README.md` & `PyQt6-Fluent-Widgets-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/resource.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/auto_wrap.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/config.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/exception_handler.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/icon.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/image_utils.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/smooth_scroll.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/common/style_sheet.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/date_picker.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/picker_base.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/picker_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         for btn in self.columns[:-1]:
             btn.setProperty('hasBorder', True)
             btn.setStyle(QApplication.style())
 
     @checkColumnIndex
     def setColumnAlignment(self, index: int, align=Qt.AlignmentFlag.AlignCenter):
         """ set the text alignment of specified column """
-        self.columns[index].setTextAlignment(align)
+        self.columns[index].setAlignment(align)
 
     @checkColumnIndex
     def setColumnWidth(self, index: int, width: int):
         """ set the width of specified column """
         self.columns[index].setFixedWidth(width)
 
     @checkColumnIndex
@@ -316,14 +316,15 @@
         button.setFixedWidth(width)
         button.setAlignment(align)
 
     def clearColumns(self):
         """ clear columns """
         while self.columns:
             btn = self.columns.pop()
+            self.hBoxLayout.removeWidget(btn)
             btn.deleteLater()
 
     def enterEvent(self, e):
         self._setButtonProperty('enter', True)
 
     def leaveEvent(self, e):
         self._setButtonProperty('enter', False)
```

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/time_picker.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/expand_layout.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/flow_layout.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/__init__.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/__init__.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/button.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/combo_box.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/info_bar.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/info_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,18 @@
 
     def _adjustText(self):
         w = 900 if not self.parent() else (self.parent().width() - 50)
         chars = max(min(w / 9, 120), 30)
         self.contentLabel.setText(TextWrap.wrap(self.content, chars, False)[0])
         self.adjustSize()
 
+    def adjustSize(self):
+        super().adjustSize()
+        self.resize(self.width(), max(self.height(), 50))
+
     def addWidget(self, widget: QWidget, stretch=0):
         """ add widget to info bar """
         self.contentLayout.addWidget(widget, stretch, Qt.AlignmentFlag.AlignLeft)
 
     def setCustomBackgroundColor(self, light, dark):
         """ set the custom background color
```

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/label.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/line_edit.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/menu.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/slider.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/spin_box.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/switch_button.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/three_state_button.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/three_state_button.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tree_view.py` & `PyQt6-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt6-Fluent-Widgets-0.7.1/setup.py` & `PyQt6-Fluent-Widgets-0.7.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt6-Fluent-Widgets",
-    version="0.7.1",
+    version="0.7.2",
     keywords="pyqt6 fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt6",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

