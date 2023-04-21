# Comparing `tmp/curses-menu-0.6.6.tar.gz` & `tmp/curses-menu-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curses-menu-0.6.6.tar", max compression
+gzip compressed data, was "curses-menu-0.6.7.tar", max compression
```

## Comparing `curses-menu-0.6.6.tar` & `curses-menu-0.6.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      850 2022-09-08 01:18:11.567367 curses-menu-0.6.6/CHANGELOG.rst
--rw-r--r--   0        0        0     1100 2020-04-07 07:01:49.000000 curses-menu-0.6.6/LICENSE.md
--rw-r--r--   0        0        0     3039 2022-09-08 01:18:00.287027 curses-menu-0.6.6/README.rst
--rw-r--r--   0        0        0      651 2020-04-07 07:01:49.000000 curses-menu-0.6.6/acknowledgements.md
--rw-r--r--   0        0        0      376 2022-09-08 01:18:00.287787 curses-menu-0.6.6/cursesmenu/__init__.py
--rw-r--r--   0        0        0    18213 2022-09-08 01:18:00.288537 curses-menu-0.6.6/cursesmenu/curses_menu.py
--rw-r--r--   0        0        0     3553 2022-09-08 01:18:00.289236 curses-menu-0.6.6/cursesmenu/item_group.py
--rw-r--r--   0        0        0      345 2021-11-25 21:29:19.218608 curses-menu-0.6.6/cursesmenu/items/__init__.py
--rw-r--r--   0        0        0     2702 2022-09-08 01:18:00.289923 curses-menu-0.6.6/cursesmenu/items/command_item.py
--rw-r--r--   0        0        0     1299 2022-08-10 00:50:43.361815 curses-menu-0.6.6/cursesmenu/items/exit_item.py
--rw-r--r--   0        0        0      807 2021-11-25 21:29:19.219882 curses-menu-0.6.6/cursesmenu/items/external_item.py
--rw-r--r--   0        0        0     1969 2022-08-02 03:13:09.109619 curses-menu-0.6.6/cursesmenu/items/function_item.py
--rw-r--r--   0        0        0     2377 2022-08-10 00:50:43.361990 curses-menu-0.6.6/cursesmenu/items/menu_item.py
--rw-r--r--   0        0        0      801 2022-08-02 03:13:09.110281 curses-menu-0.6.6/cursesmenu/items/selection_item.py
--rw-r--r--   0        0        0     2796 2022-08-02 03:13:09.110095 curses-menu-0.6.6/cursesmenu/items/submenu_item.py
--rw-r--r--   0        0        0     1758 2021-11-25 21:29:19.221780 curses-menu-0.6.6/cursesmenu/old_curses_menu.py
--rw-r--r--   0        0        0      818 2022-08-01 23:24:12.896911 curses-menu-0.6.6/cursesmenu/utils.py
--rw-r--r--   0        0        0      638 2021-11-25 21:29:19.222551 curses-menu-0.6.6/docs/Makefile
--rw-r--r--   0        0        0     2019 2022-09-08 01:18:00.290736 curses-menu-0.6.6/docs/source/conf.py
--rw-r--r--   0        0        0     1527 2021-11-25 21:29:19.264392 curses-menu-0.6.6/docs/source/cursesmenu/CursesMenu.rst
--rw-r--r--   0        0        0      107 2021-11-25 21:29:19.225033 curses-menu-0.6.6/docs/source/cursesmenu/ItemGroup.rst
--rw-r--r--   0        0        0       95 2021-11-25 21:29:19.263852 curses-menu-0.6.6/docs/source/cursesmenu/functions.rst
--rw-r--r--   0        0        0      130 2021-11-25 21:29:19.263350 curses-menu-0.6.6/docs/source/cursesmenu/items/CommandItem.rst
--rw-r--r--   0        0        0      117 2021-11-25 21:29:19.262886 curses-menu-0.6.6/docs/source/cursesmenu/items/ExitItem.rst
--rw-r--r--   0        0        0      129 2021-11-25 21:29:19.262315 curses-menu-0.6.6/docs/source/cursesmenu/items/ExternalItem.rst
--rw-r--r--   0        0        0      133 2021-11-25 21:29:19.261852 curses-menu-0.6.6/docs/source/cursesmenu/items/FunctionItem.rst
--rw-r--r--   0        0        0       74 2021-11-25 21:29:19.261374 curses-menu-0.6.6/docs/source/cursesmenu/items/MenuItem.rst
--rw-r--r--   0        0        0      126 2021-11-25 21:29:19.260962 curses-menu-0.6.6/docs/source/cursesmenu/items/SubmenuItem.rst
--rw-r--r--   0        0        0      145 2021-11-25 21:29:19.264990 curses-menu-0.6.6/docs/source/cursesmenu.rst
--rw-r--r--   0        0        0      490 2021-11-25 21:29:19.260433 curses-menu-0.6.6/docs/source/index.rst
--rw-r--r--   0        0        0      100 2021-11-25 21:29:19.227467 curses-menu-0.6.6/docs/source/installation.rst
--rw-r--r--   0        0        0      231 2021-11-25 21:29:19.259904 curses-menu-0.6.6/docs/source/items.rst
--rw-r--r--   0        0        0     1735 2021-11-25 21:29:19.257379 curses-menu-0.6.6/docs/source/usage.rst
--rw-r--r--   0        0        0     3793 2022-09-08 01:18:11.567669 curses-menu-0.6.6/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-25 21:29:19.232373 curses-menu-0.6.6/test/__init__.py
--rw-r--r--   0        0        0     2009 2022-08-01 23:24:12.898690 curses-menu-0.6.6/test/conftest.py
--rw-r--r--   0        0        0        0 2021-11-25 21:29:19.233785 curses-menu-0.6.6/test/example_menus/__init__.py
--rw-r--r--   0        0        0      134 2021-11-25 21:29:19.234232 curses-menu-0.6.6/test/example_menus/basic_menu.py
--rw-r--r--   0        0        0      290 2021-11-25 21:29:19.234624 curses-menu-0.6.6/test/example_menus/menu_with_items.py
--rw-r--r--   0        0        0      283 2022-08-02 01:28:06.278287 curses-menu-0.6.6/test/example_menus/menu_with_lots_of_items.py
--rw-r--r--   0        0        0      298 2022-09-08 01:18:00.305476 curses-menu-0.6.6/test/example_menus/zero_padded_menu_with_lots_of_items.py
--rw-r--r--   0        0        0      552 2022-08-01 04:41:23.745334 curses-menu-0.6.6/test/test_clear.py
--rw-r--r--   0        0        0     1761 2022-09-08 01:18:00.306202 curses-menu-0.6.6/test/test_command_item.py
--rw-r--r--   0        0        0     5483 2022-09-08 01:18:00.307068 curses-menu-0.6.6/test/test_curses_menu.py
--rw-r--r--   0        0        0     1030 2022-09-08 01:18:00.307703 curses-menu-0.6.6/test/test_example_menus.py
--rw-r--r--   0        0        0      630 2021-11-25 21:29:19.238787 curses-menu-0.6.6/test/test_exit_item.py
--rw-r--r--   0        0        0      890 2021-11-25 21:29:19.239213 curses-menu-0.6.6/test/test_external_item.py
--rw-r--r--   0        0        0      537 2021-11-25 21:29:19.239616 curses-menu-0.6.6/test/test_function_item.py
--rw-r--r--   0        0        0     3861 2022-09-08 01:18:00.308490 curses-menu-0.6.6/test/test_graphics.py
--rw-r--r--   0        0        0     2283 2021-11-25 21:29:19.240293 curses-menu-0.6.6/test/test_item_group.py
--rw-r--r--   0        0        0      808 2021-11-25 21:29:19.240708 curses-menu-0.6.6/test/test_menu_item.py
--rw-r--r--   0        0        0      283 2021-11-25 21:29:19.241114 curses-menu-0.6.6/test/test_selection_item.py
--rw-r--r--   0        0        0      378 2021-11-25 21:29:19.241525 curses-menu-0.6.6/test/test_selection_menu.py
--rw-r--r--   0        0        0     2838 2021-11-25 21:29:19.241942 curses-menu-0.6.6/test/test_submenu_item.py
--rw-r--r--   0        0        0     1631 2022-09-08 01:18:00.309336 curses-menu-0.6.6/tox.ini
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 curses-menu-0.6.6/setup.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 curses-menu-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      922 2022-10-31 02:59:45.963476 curses-menu-0.6.7/CHANGELOG.rst
+-rw-r--r--   0        0        0     1100 2020-04-07 07:01:49.000000 curses-menu-0.6.7/LICENSE.md
+-rw-r--r--   0        0        0     2896 2022-10-31 02:59:34.275960 curses-menu-0.6.7/README.rst
+-rw-r--r--   0        0        0      651 2020-04-07 07:01:49.000000 curses-menu-0.6.7/acknowledgements.md
+-rw-r--r--   0        0        0      376 2022-09-08 01:18:00.287787 curses-menu-0.6.7/cursesmenu/__init__.py
+-rw-r--r--   0        0        0    18213 2022-09-08 01:18:00.288537 curses-menu-0.6.7/cursesmenu/curses_menu.py
+-rw-r--r--   0        0        0     3553 2022-09-08 01:18:00.289236 curses-menu-0.6.7/cursesmenu/item_group.py
+-rw-r--r--   0        0        0      345 2021-11-25 21:29:19.218608 curses-menu-0.6.7/cursesmenu/items/__init__.py
+-rw-r--r--   0        0        0     2702 2022-09-08 01:18:00.289923 curses-menu-0.6.7/cursesmenu/items/command_item.py
+-rw-r--r--   0        0        0     1299 2022-08-10 00:50:43.361815 curses-menu-0.6.7/cursesmenu/items/exit_item.py
+-rw-r--r--   0        0        0      807 2021-11-25 21:29:19.219882 curses-menu-0.6.7/cursesmenu/items/external_item.py
+-rw-r--r--   0        0        0     1969 2022-08-02 03:13:09.109619 curses-menu-0.6.7/cursesmenu/items/function_item.py
+-rw-r--r--   0        0        0     2377 2022-08-10 00:50:43.361990 curses-menu-0.6.7/cursesmenu/items/menu_item.py
+-rw-r--r--   0        0        0      801 2022-08-02 03:13:09.110281 curses-menu-0.6.7/cursesmenu/items/selection_item.py
+-rw-r--r--   0        0        0     2796 2022-08-02 03:13:09.110095 curses-menu-0.6.7/cursesmenu/items/submenu_item.py
+-rw-r--r--   0        0        0     1758 2021-11-25 21:29:19.221780 curses-menu-0.6.7/cursesmenu/old_curses_menu.py
+-rw-r--r--   0        0        0      818 2022-08-01 23:24:12.896911 curses-menu-0.6.7/cursesmenu/utils.py
+-rw-r--r--   0        0        0      638 2021-11-25 21:29:19.222551 curses-menu-0.6.7/docs/Makefile
+-rw-r--r--   0        0        0     2019 2022-09-08 01:18:00.290736 curses-menu-0.6.7/docs/source/conf.py
+-rw-r--r--   0        0        0     1527 2021-11-25 21:29:19.264392 curses-menu-0.6.7/docs/source/cursesmenu/CursesMenu.rst
+-rw-r--r--   0        0        0      107 2021-11-25 21:29:19.225033 curses-menu-0.6.7/docs/source/cursesmenu/ItemGroup.rst
+-rw-r--r--   0        0        0       95 2021-11-25 21:29:19.263852 curses-menu-0.6.7/docs/source/cursesmenu/functions.rst
+-rw-r--r--   0        0        0      130 2021-11-25 21:29:19.263350 curses-menu-0.6.7/docs/source/cursesmenu/items/CommandItem.rst
+-rw-r--r--   0        0        0      117 2021-11-25 21:29:19.262886 curses-menu-0.6.7/docs/source/cursesmenu/items/ExitItem.rst
+-rw-r--r--   0        0        0      129 2021-11-25 21:29:19.262315 curses-menu-0.6.7/docs/source/cursesmenu/items/ExternalItem.rst
+-rw-r--r--   0        0        0      133 2021-11-25 21:29:19.261852 curses-menu-0.6.7/docs/source/cursesmenu/items/FunctionItem.rst
+-rw-r--r--   0        0        0       74 2021-11-25 21:29:19.261374 curses-menu-0.6.7/docs/source/cursesmenu/items/MenuItem.rst
+-rw-r--r--   0        0        0      126 2021-11-25 21:29:19.260962 curses-menu-0.6.7/docs/source/cursesmenu/items/SubmenuItem.rst
+-rw-r--r--   0        0        0      145 2021-11-25 21:29:19.264990 curses-menu-0.6.7/docs/source/cursesmenu.rst
+-rw-r--r--   0        0        0      490 2021-11-25 21:29:19.260433 curses-menu-0.6.7/docs/source/index.rst
+-rw-r--r--   0        0        0      100 2021-11-25 21:29:19.227467 curses-menu-0.6.7/docs/source/installation.rst
+-rw-r--r--   0        0        0      231 2021-11-25 21:29:19.259904 curses-menu-0.6.7/docs/source/items.rst
+-rw-r--r--   0        0        0     1735 2021-11-25 21:29:19.257379 curses-menu-0.6.7/docs/source/usage.rst
+-rw-r--r--   0        0        0     3793 2022-10-31 02:59:45.963750 curses-menu-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-25 21:29:19.232373 curses-menu-0.6.7/test/__init__.py
+-rw-r--r--   0        0        0     2009 2022-08-01 23:24:12.898690 curses-menu-0.6.7/test/conftest.py
+-rw-r--r--   0        0        0        0 2021-11-25 21:29:19.233785 curses-menu-0.6.7/test/example_menus/__init__.py
+-rw-r--r--   0        0        0      134 2021-11-25 21:29:19.234232 curses-menu-0.6.7/test/example_menus/basic_menu.py
+-rw-r--r--   0        0        0      290 2021-11-25 21:29:19.234624 curses-menu-0.6.7/test/example_menus/menu_with_items.py
+-rw-r--r--   0        0        0      283 2022-08-02 01:28:06.278287 curses-menu-0.6.7/test/example_menus/menu_with_lots_of_items.py
+-rw-r--r--   0        0        0      298 2022-09-08 01:18:00.305476 curses-menu-0.6.7/test/example_menus/zero_padded_menu_with_lots_of_items.py
+-rw-r--r--   0        0        0      552 2022-08-01 04:41:23.745334 curses-menu-0.6.7/test/test_clear.py
+-rw-r--r--   0        0        0     1761 2022-09-08 01:18:00.306202 curses-menu-0.6.7/test/test_command_item.py
+-rw-r--r--   0        0        0     5483 2022-09-08 01:18:00.307068 curses-menu-0.6.7/test/test_curses_menu.py
+-rw-r--r--   0        0        0     1030 2022-09-08 01:18:00.307703 curses-menu-0.6.7/test/test_example_menus.py
+-rw-r--r--   0        0        0      630 2021-11-25 21:29:19.238787 curses-menu-0.6.7/test/test_exit_item.py
+-rw-r--r--   0        0        0      890 2021-11-25 21:29:19.239213 curses-menu-0.6.7/test/test_external_item.py
+-rw-r--r--   0        0        0      537 2021-11-25 21:29:19.239616 curses-menu-0.6.7/test/test_function_item.py
+-rw-r--r--   0        0        0     3861 2022-09-08 01:18:00.308490 curses-menu-0.6.7/test/test_graphics.py
+-rw-r--r--   0        0        0     2283 2021-11-25 21:29:19.240293 curses-menu-0.6.7/test/test_item_group.py
+-rw-r--r--   0        0        0      808 2021-11-25 21:29:19.240708 curses-menu-0.6.7/test/test_menu_item.py
+-rw-r--r--   0        0        0      283 2021-11-25 21:29:19.241114 curses-menu-0.6.7/test/test_selection_item.py
+-rw-r--r--   0        0        0      378 2021-11-25 21:29:19.241525 curses-menu-0.6.7/test/test_selection_menu.py
+-rw-r--r--   0        0        0     2838 2021-11-25 21:29:19.241942 curses-menu-0.6.7/test/test_submenu_item.py
+-rw-r--r--   0        0        0     1635 2022-10-31 02:59:34.276905 curses-menu-0.6.7/tox.ini
+-rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 curses-menu-0.6.7/setup.py
+-rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 curses-menu-0.6.7/PKG-INFO
```

### Comparing `curses-menu-0.6.6/CHANGELOG.rst` & `curses-menu-0.6.7/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 0.6.7
+-------------
+* Test on release python 3.11
+* Fix readme
+
 Version 0.6.5
 -------------
 * Fix bug caused by not having Deprecated as install dependency.
 
 Version 0.6.5
 -------------
```

### Comparing `curses-menu-0.6.6/LICENSE.md` & `curses-menu-0.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/acknowledgements.md` & `curses-menu-0.6.7/acknowledgements.md`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/curses_menu.py` & `curses-menu-0.6.7/cursesmenu/curses_menu.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/item_group.py` & `curses-menu-0.6.7/cursesmenu/item_group.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/command_item.py` & `curses-menu-0.6.7/cursesmenu/items/command_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/exit_item.py` & `curses-menu-0.6.7/cursesmenu/items/exit_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/external_item.py` & `curses-menu-0.6.7/cursesmenu/items/external_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/function_item.py` & `curses-menu-0.6.7/cursesmenu/items/function_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/menu_item.py` & `curses-menu-0.6.7/cursesmenu/items/menu_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/selection_item.py` & `curses-menu-0.6.7/cursesmenu/items/selection_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/items/submenu_item.py` & `curses-menu-0.6.7/cursesmenu/items/submenu_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/old_curses_menu.py` & `curses-menu-0.6.7/cursesmenu/old_curses_menu.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/cursesmenu/utils.py` & `curses-menu-0.6.7/cursesmenu/utils.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/docs/Makefile` & `curses-menu-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/docs/source/conf.py` & `curses-menu-0.6.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/docs/source/cursesmenu/CursesMenu.rst` & `curses-menu-0.6.7/docs/source/cursesmenu/CursesMenu.rst`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/docs/source/usage.rst` & `curses-menu-0.6.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/pyproject.toml` & `curses-menu-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "curses-menu"
-version = "0.6.6"
+version = "0.6.7"
 description = "A simple console menu system using curses"
 authors = ["Paul Barrett <pmbarrett314@gmail.com>"]
 license = "MIT"
 repository = "http://github.com/pmbarrett314/curses-menu"
 packages = [{ include = "cursesmenu" }]
 readme = "README.rst"
 classifiers = [
@@ -119,15 +119,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.2"
 tox = "^3.25.1"
 coverage = { version = "^6.4.2", extras = ["toml"] }
 pyte = "^0.8.1"
 pexpect = "^4.8.0"
 types-Deprecated = "^1.2.9"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 coverage-conditional-plugin = "^0.5.0"
 
 [tool.poetry.group.type]
 
 [tool.poetry.group.type.dependencies]
 types-Deprecated = "^1.2.9"
 mypy = "^0.971"
```

### Comparing `curses-menu-0.6.6/test/conftest.py` & `curses-menu-0.6.7/test/conftest.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_clear.py` & `curses-menu-0.6.7/test/test_clear.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_command_item.py` & `curses-menu-0.6.7/test/test_command_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_curses_menu.py` & `curses-menu-0.6.7/test/test_curses_menu.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_example_menus.py` & `curses-menu-0.6.7/test/test_example_menus.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_exit_item.py` & `curses-menu-0.6.7/test/test_exit_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_external_item.py` & `curses-menu-0.6.7/test/test_external_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_function_item.py` & `curses-menu-0.6.7/test/test_function_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_graphics.py` & `curses-menu-0.6.7/test/test_graphics.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_item_group.py` & `curses-menu-0.6.7/test/test_item_group.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_menu_item.py` & `curses-menu-0.6.7/test/test_menu_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/test/test_submenu_item.py` & `curses-menu-0.6.7/test/test_submenu_item.py`

 * *Files identical despite different names*

### Comparing `curses-menu-0.6.6/tox.ini` & `curses-menu-0.6.7/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tox]
-envlist = clean,py{37,38,39,310},py,pypy3,type,lint,docs
+envlist = clean,py{37,38,39,310,311},py,pypy3,type,lint,docs
 isolated_build = True
 
 [tox:.package]
 # note tox will use the same python version as under what tox is installed to package
 # so unless this is python 3 you can require a given python version for the packaging
 # environment via the basepython key
 basepython = python3
 
 [testenv]
 deps =
     deprecated >= 1.2.13, < 2
     coverage[toml] >= 6.4.2, < 7
     coverage-conditional-plugin >= 0.5.0, < 1
     pytest >= 7.1.2, < 8
-    pytest-cov >= 3.0.0, < 4
+    pytest-cov >= 4.0.0, < 5
     pexpect >= 4.8.0, < 5
     pyte >= 0.8.1, < 1
     windows-curses == 2.3.0;sys_platform=='win32'
 commands =
     pytest
 setenv =
     PYTHONWARNINGS=all
```

