# Comparing `tmp/PyQt-Fluent-Widgets-0.7.1.tar.gz` & `tmp/PyQt-Fluent-Widgets-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.7.1.tar", last modified: Sun Apr 16 08:46:37 2023, max compression
+gzip compressed data, was "dist\PyQt-Fluent-Widgets-0.7.2.tar", last modified: Fri Apr 21 01:22:32 2023, max compression
```

## Comparing `PyQt-Fluent-Widgets-0.7.1.tar` & `PyQt-Fluent-Widgets-0.7.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.993004 PyQt-Fluent-Widgets-0.7.1/
--rw-rw-rw-   0        0        0    35823 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     4035 2023-04-16 08:46:37.991941 PyQt-Fluent-Widgets-0.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.847689 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/
--rw-rw-rw-   0        0        0     4035 2023-04-16 08:46:37.000000 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2951 2023-04-16 08:46:37.000000 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 08:46:37.000000 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-16 08:46:37.000000 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 08:46:37.000000 PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3259 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.850084 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/
--rw-rw-rw-   0        0        0      492 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.854408 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/
--rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/__init__.py
--rw-rw-rw-   0        0        0  3512847 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/resource.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.880820 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/
--rw-rw-rw-   0        0        0      390 2023-04-05 13:34:28.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/__init__.py
--rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/auto_wrap.py
--rw-rw-rw-   0        0        0    10582 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/config.py
--rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/exception_handler.py
--rw-rw-rw-   0        0        0     7266 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/icon.py
--rw-rw-rw-   0        0        0     4783 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/image_utils.py
--rw-rw-rw-   0        0        0     4791 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/smooth_scroll.py
--rw-rw-rw-   0        0        0     7026 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/style_sheet.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.883159 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/
--rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.891258 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/
--rw-rw-rw-   0        0        0      189 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/__init__.py
--rw-rw-rw-   0        0        0     7455 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/date_picker.py
--rw-rw-rw-   0        0        0    18728 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/picker_base.py
--rw-rw-rw-   0        0        0     5783 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/time_picker.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.906554 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/
--rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/__init__.py
--rw-rw-rw-   0        0        0    11778 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/color_dialog.py
--rw-rw-rw-   0        0        0     5327 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/dialog.py
--rw-rw-rw-   0        0        0    11250 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py
--rw-rw-rw-   0        0        0     3238 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py
--rw-rw-rw-   0        0        0     2500 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/message_dialog.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.916886 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/
--rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/expand_layout.py
--rw-rw-rw-   0        0        0     5433 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/flow_layout.py
--rw-rw-rw-   0        0        0     1301 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/v_box_layout.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.924640 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/
--rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/__init__.py
--rw-rw-rw-   0        0        0     4541 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_interface.py
--rw-rw-rw-   0        0        0    15536 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_panel.py
--rw-rw-rw-   0        0        0     4875 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.941907 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/
--rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/__init__.py
--rw-rw-rw-   0        0        0     5197 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/custom_color_setting_card.py
--rw-rw-rw-   0        0        0     8027 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/expand_setting_card.py
--rw-rw-rw-   0        0        0     6034 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/folder_list_setting_card.py
--rw-rw-rw-   0        0        0     2840 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/options_setting_card.py
--rw-rw-rw-   0        0        0    12825 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card.py
--rw-rw-rw-   0        0        0     1512 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card_group.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:46:37.989414 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/
--rw-rw-rw-   0        0        0      998 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/__init__.py
--rw-rw-rw-   0        0        0     4598 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/acrylic_label.py
--rw-rw-rw-   0        0        0     5695 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/button.py
--rw-rw-rw-   0        0        0      304 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/check_box.py
--rw-rw-rw-   0        0        0    12974 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/combo_box.py
--rw-rw-rw-   0        0        0     8222 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/cycle_list_widget.py
--rw-rw-rw-   0        0        0      703 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/icon_widget.py
--rw-rw-rw-   0        0        0    18837 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/info_bar.py
--rw-rw-rw-   0        0        0      835 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/label.py
--rw-rw-rw-   0        0        0     5751 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/line_edit.py
--rw-rw-rw-   0        0        0    23237 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/menu.py
--rw-rw-rw-   0        0        0     4529 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     4878 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/slider.py
--rw-rw-rw-   0        0        0     4438 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/spin_box.py
--rw-rw-rw-   0        0        0     6313 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0     5790 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/state_tool_tip.py
--rw-rw-rw-   0        0        0     6603 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/switch_button.py
--rw-rw-rw-   0        0        0     1654 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/three_state_button.py
--rw-rw-rw-   0        0        0     5157 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tool_tip.py
--rw-rw-rw-   0        0        0     2828 2023-04-15 14:33:45.000000 PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tree_view.py
--rw-rw-rw-   0        0        0       42 2023-04-16 08:46:37.993004 PyQt-Fluent-Widgets-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1222 2023-04-16 08:41:06.000000 PyQt-Fluent-Widgets-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.630751 PyQt-Fluent-Widgets-0.7.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 03:28:34.000000 PyQt-Fluent-Widgets-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     4035 2023-04-21 01:22:32.630751 PyQt-Fluent-Widgets-0.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.473613 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/
+-rw-rw-rw-   0        0        0     4035 2023-04-21 01:22:32.000000 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2951 2023-04-21 01:22:32.000000 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:22:32.000000 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-21 01:22:32.000000 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-21 01:22:32.000000 PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3259 2023-04-18 03:28:34.000000 PyQt-Fluent-Widgets-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.473613 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/
+-rw-rw-rw-   0        0        0      492 2023-04-21 01:20:58.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.481467 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/
+-rw-rw-rw-   0        0        0        0 2023-01-17 07:40:20.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/__init__.py
+-rw-rw-rw-   0        0        0  3512847 2023-04-20 16:00:58.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/resource.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.509630 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/
+-rw-rw-rw-   0        0        0      390 2023-04-05 13:34:28.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/__init__.py
+-rw-rw-rw-   0        0        0     3193 2023-01-27 14:07:06.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/auto_wrap.py
+-rw-rw-rw-   0        0        0    10582 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/config.py
+-rw-rw-rw-   0        0        0      675 2023-01-16 13:18:33.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/exception_handler.py
+-rw-rw-rw-   0        0        0     7266 2023-04-19 03:10:36.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/icon.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/image_utils.py
+-rw-rw-rw-   0        0        0     4791 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/smooth_scroll.py
+-rw-rw-rw-   0        0        0     7026 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/style_sheet.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.513740 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/
+-rw-rw-rw-   0        0        0      150 2023-04-15 14:20:48.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.522163 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/
+-rw-rw-rw-   0        0        0      189 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/__init__.py
+-rw-rw-rw-   0        0        0     7455 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/date_picker.py
+-rw-rw-rw-   0        0        0    18771 2023-04-21 01:20:58.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/picker_base.py
+-rw-rw-rw-   0        0        0     5783 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/time_picker.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.536931 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/
+-rw-rw-rw-   0        0        0      170 2023-03-14 08:29:15.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/__init__.py
+-rw-rw-rw-   0        0        0    11778 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/color_dialog.py
+-rw-rw-rw-   0        0        0     5327 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/dialog.py
+-rw-rw-rw-   0        0        0    11250 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/folder_list_dialog.py
+-rw-rw-rw-   0        0        0     3238 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/mask_dialog_base.py
+-rw-rw-rw-   0        0        0     2500 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/message_dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.547086 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/
+-rw-rw-rw-   0        0        0      114 2023-01-16 13:10:58.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/expand_layout.py
+-rw-rw-rw-   0        0        0     5433 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/flow_layout.py
+-rw-rw-rw-   0        0        0     1301 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/v_box_layout.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.556404 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/
+-rw-rw-rw-   0        0        0      261 2023-04-15 14:22:56.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/__init__.py
+-rw-rw-rw-   0        0        0     4541 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_interface.py
+-rw-rw-rw-   0        0        0    15536 2023-04-19 03:10:36.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_panel.py
+-rw-rw-rw-   0        0        0     4875 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.578307 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/
+-rw-rw-rw-   0        0        0      550 2023-03-24 06:13:50.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/__init__.py
+-rw-rw-rw-   0        0        0     5197 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/custom_color_setting_card.py
+-rw-rw-rw-   0        0        0     8027 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/expand_setting_card.py
+-rw-rw-rw-   0        0        0     6034 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/folder_list_setting_card.py
+-rw-rw-rw-   0        0        0     2840 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/options_setting_card.py
+-rw-rw-rw-   0        0        0    12825 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card.py
+-rw-rw-rw-   0        0        0     1512 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card_group.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:22:32.627376 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/
+-rw-rw-rw-   0        0        0      998 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4598 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/acrylic_label.py
+-rw-rw-rw-   0        0        0     5695 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/button.py
+-rw-rw-rw-   0        0        0      304 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/check_box.py
+-rw-rw-rw-   0        0        0    12974 2023-04-18 03:33:09.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     8222 2023-04-19 03:10:36.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/cycle_list_widget.py
+-rw-rw-rw-   0        0        0      703 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0    18955 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/info_bar.py
+-rw-rw-rw-   0        0        0      835 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/label.py
+-rw-rw-rw-   0        0        0     5751 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/line_edit.py
+-rw-rw-rw-   0        0        0    23237 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/menu.py
+-rw-rw-rw-   0        0        0     4529 2023-04-20 15:59:18.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     4878 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/slider.py
+-rw-rw-rw-   0        0        0     4438 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     6313 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0     5790 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/state_tool_tip.py
+-rw-rw-rw-   0        0        0     6603 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/switch_button.py
+-rw-rw-rw-   0        0        0     1654 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/three_state_button.py
+-rw-rw-rw-   0        0        0     5157 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tool_tip.py
+-rw-rw-rw-   0        0        0     2828 2023-04-18 03:28:35.000000 PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tree_view.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:22:32.630751 PyQt-Fluent-Widgets-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2023-04-21 01:20:58.000000 PyQt-Fluent-Widgets-0.7.2/setup.py
```

### Comparing `PyQt-Fluent-Widgets-0.7.1/LICENSE` & `PyQt-Fluent-Widgets-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/PKG-INFO` & `PyQt-Fluent-Widgets-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.7.1
+Version: 0.7.2
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

### Comparing `PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/PKG-INFO` & `PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt-Fluent-Widgets
-Version: 0.7.1
+Version: 0.7.2
 Summary: A fluent design widgets library based on PyQt5
 Home-page: https://github.com/zhiyiYo/PyQt-Fluent-Widgets
 Author: zhiyiYo
 Author-email: shokokawaii@outlook.com
 License: GPLv3
 Project-URL: Documentation, https://pyqt-fluent-widgets.readthedocs.io/
 Project-URL: Source Code, https://github.com/zhiyiYo/PyQt-Fluent-Widgets
```

### Comparing `PyQt-Fluent-Widgets-0.7.1/PyQt_Fluent_Widgets.egg-info/SOURCES.txt` & `PyQt-Fluent-Widgets-0.7.2/PyQt_Fluent_Widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/README.md` & `PyQt-Fluent-Widgets-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/_rc/resource.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/auto_wrap.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/auto_wrap.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/config.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/config.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/exception_handler.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/exception_handler.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/icon.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/icon.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/image_utils.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/image_utils.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/smooth_scroll.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/smooth_scroll.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/common/style_sheet.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/common/style_sheet.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/date_picker.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/date_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/picker_base.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/picker_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         for btn in self.columns[:-1]:
             btn.setProperty('hasBorder', True)
             btn.setStyle(QApplication.style())
 
     @checkColumnIndex
     def setColumnAlignment(self, index: int, align=Qt.AlignCenter):
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

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/date_time/time_picker.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/date_time/time_picker.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/color_dialog.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/color_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/dialog.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/folder_list_dialog.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/folder_list_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/mask_dialog_base.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/mask_dialog_base.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/dialog_box/message_dialog.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/dialog_box/message_dialog.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/expand_layout.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/expand_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/flow_layout.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/layout/v_box_layout.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/layout/v_box_layout.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_interface.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_interface.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_panel.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_panel.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/navigation/navigation_widget.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/navigation/navigation_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/__init__.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/custom_color_setting_card.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/custom_color_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/expand_setting_card.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/expand_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/folder_list_setting_card.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/folder_list_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/options_setting_card.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/options_setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/settings/setting_card_group.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/settings/setting_card_group.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/__init__.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/acrylic_label.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/acrylic_label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/button.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/combo_box.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/cycle_list_widget.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/cycle_list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/icon_widget.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/info_bar.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/info_bar.py`

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
         self.contentLayout.addWidget(widget, stretch, Qt.AlignLeft)
 
     def setCustomBackgroundColor(self, light, dark):
         """ set the custom background color
```

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/label.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/line_edit.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/menu.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/scroll_area.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/slider.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/spin_box.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/stacked_widget.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/state_tool_tip.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/state_tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/switch_button.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/switch_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/three_state_button.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/three_state_button.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tool_tip.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tool_tip.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/qfluentwidgets/components/widgets/tree_view.py` & `PyQt-Fluent-Widgets-0.7.2/qfluentwidgets/components/widgets/tree_view.py`

 * *Files identical despite different names*

### Comparing `PyQt-Fluent-Widgets-0.7.1/setup.py` & `PyQt-Fluent-Widgets-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="PyQt-Fluent-Widgets",
-    version="0.7.1",
+    version="0.7.2",
     keywords="pyqt fluent widgets",
     author="zhiyiYo",
     author_email="shokokawaii@outlook.com",
     description="A fluent design widgets library based on PyQt5",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="GPLv3",
```

