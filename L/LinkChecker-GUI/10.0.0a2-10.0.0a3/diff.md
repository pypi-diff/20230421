# Comparing `tmp/LinkChecker_GUI-10.0.0a2.tar.gz` & `tmp/LinkChecker_GUI-10.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Dec  5 19:35:48 2022, max compression
+gzip compressed data, last modified: Fri Apr 21 18:37:43 2023, max compression
```

## Comparing `LinkChecker_GUI-10.0.0a2.tar` & `LinkChecker_GUI-10.0.0a3.tar`

### file list

```diff
@@ -1,74 +1,76 @@
--rw-r--r--   0        0        0      752 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/.flake8
--rw-r--r--   0        0        0      104 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/.yamllint
--rw-r--r--   0        0        0      115 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/changelog.txt
--rw-r--r--   0        0        0      689 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/pyoxidizer.bzl
--rw-r--r--   0        0        0      450 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/tox.ini
--rw-r--r--   0        0        0     3330 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/de.po
--rw-r--r--   0        0        0      214 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/linkchecker-gui.desktop
--rw-r--r--   0        0        0      127 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/po4a.conf
--rw-r--r--   0        0        0     1003 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/de/linkchecker-gui.1
--rw-r--r--   0        0        0      686 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/en/linkchecker-gui.1
--rw-r--r--   0        0        0    67271 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/favicon.icns
--rw-r--r--   0        0        0     3638 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/favicon.ico
--rw-r--r--   0        0        0      144 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/html.footer
--rw-r--r--   0        0        0      764 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/html.header
--rw-r--r--   0        0        0     6893 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/index.txt
--rw-r--r--   0        0        0      746 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/lccollection.qhcp
--rw-r--r--   0        0        0      476 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/lcdoc.qhp
--rw-r--r--   0        0        0     3224 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/pygments.css
--rw-r--r--   0        0        0     5382 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/sphinxdoc.css
--rw-r--r--   0        0        0    26618 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/logo/128x128/linkchecker-gui.png
--rw-r--r--   0        0        0     1085 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/logo/16x16/linkchecker-gui.png
--rw-r--r--   0        0        0     3254 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/logo/32x32/linkchecker-gui.png
--rw-r--r--   0        0        0     6232 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/logo/48x48/linkchecker-gui.png
--rw-r--r--   0        0        0     9761 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/doc/html/logo/64x64/linkchecker-gui.png
--rw-r--r--   0        0        0    24351 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/__init__.py
--rw-r--r--   0        0        0     2510 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/__main__.py
--rw-r--r--   0        0        0      212 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/_release.py
--rw-r--r--   0        0        0     1573 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/checker.py
--rw-r--r--   0        0        0     2545 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/configuration.py
--rw-r--r--   0        0        0     2580 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/contextmenu.py
--rw-r--r--   0        0        0     1541 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/debug.py
--rw-r--r--   0        0        0     6618 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/editor.py
--rw-r--r--   0        0        0     3937 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/editor_qsci.py
--rw-r--r--   0        0        0     6075 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/editor_qt.py
--rw-r--r--   0        0        0     2893 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/help.py
--rw-r--r--   0        0        0     9432 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/lineedit.py
--rw-r--r--   0        0        0    52172 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_rc.py
--rw-r--r--   0        0        0     1557 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_debug.py
--rw-r--r--   0        0        0     2570 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_editor.py
--rw-r--r--   0        0        0    53491 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_main.py
--rw-r--r--   0        0        0     8541 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_options.py
--rw-r--r--   0        0        0     2442 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/logger.py
--rw-r--r--   0        0        0     4135 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/options.py
--rw-r--r--   0        0        0     7581 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/projects.py
--rw-r--r--   0        0        0     2896 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/properties.py
--rw-r--r--   0        0        0     3289 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/recentdocs.py
--rw-r--r--   0        0        0     5746 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/settings.py
--rw-r--r--   0        0        0     2060 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/statistics.py
--rw-r--r--   0        0        0     3568 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/syntax.py
--rw-r--r--   0        0        0     3551 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/updater.py
--rw-r--r--   0        0        0     6756 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/urlmodel.py
--rw-r--r--   0        0        0     2720 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/urlsave.py
--rw-r--r--   0        0        0     1407 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/validator.py
--rw-r--r--   0        0        0    73728 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/data/help/lccollection.qhc
--rw-r--r--   0        0        0    77824 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/data/help/lcdoc.qch
--rw-r--r--   0        0        0        0 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/__init__.py
--rw-r--r--   0        0        0     1171 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/containers.py
--rw-r--r--   0        0        0     1259 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/fileutil.py
--rw-r--r--   0        0        0        0 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/__init__.py
--rw-r--r--   0        0        0     2347 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/chrome.py
--rw-r--r--   0        0        0     2550 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/chromium.py
--rw-r--r--   0        0        0     1733 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/firefox.py
--rw-r--r--   0        0        0     1700 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/opera.py
--rw-r--r--   0        0        0     1428 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/safari.py
--rw-r--r--   0        0        0     1302 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/winutil.py
--rw-r--r--   0        0        0     1668 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/tests/__init__.py
--rw-r--r--   0        0        0     1088 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/tests/test_containers.py
--rw-r--r--   0        0        0     1275 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/tests/test_gui.py
--rw-r--r--   0        0        0     3068 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/tools/hatch_build.py
--rw-r--r--   0        0        0      897 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/.gitignore
--rw-r--r--   0        0        0    35141 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/LICENSE
--rw-r--r--   0        0        0      754 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/README.md
--rw-r--r--   0        0        0     2249 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1545 2022-12-05 19:35:48.000000 linkchecker_gui-10.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      752 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.flake8
+-rw-r--r--   0        0        0      125 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.git_archival.txt
+-rw-r--r--   0        0        0       31 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.gitattributes
+-rw-r--r--   0        0        0      104 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.yamllint
+-rw-r--r--   0        0        0      115 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/changelog.txt
+-rw-r--r--   0        0        0      689 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/pyoxidizer.bzl
+-rw-r--r--   0        0        0      456 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tox.ini
+-rw-r--r--   0        0        0     3330 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/de.po
+-rw-r--r--   0        0        0      214 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/linkchecker-gui.desktop
+-rw-r--r--   0        0        0      127 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/po4a.conf
+-rw-r--r--   0        0        0     1003 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/de/linkchecker-gui.1
+-rw-r--r--   0        0        0      686 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/en/linkchecker-gui.1
+-rw-r--r--   0        0        0    67271 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/favicon.icns
+-rw-r--r--   0        0        0     3638 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/favicon.ico
+-rw-r--r--   0        0        0      144 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/html.footer
+-rw-r--r--   0        0        0      764 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/html.header
+-rw-r--r--   0        0        0     6893 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/index.txt
+-rw-r--r--   0        0        0      746 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/lccollection.qhcp
+-rw-r--r--   0        0        0      476 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/lcdoc.qhp
+-rw-r--r--   0        0        0     3224 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/pygments.css
+-rw-r--r--   0        0        0     5382 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/sphinxdoc.css
+-rw-r--r--   0        0        0    26618 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/128x128/linkchecker-gui.png
+-rw-r--r--   0        0        0     1085 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/16x16/linkchecker-gui.png
+-rw-r--r--   0        0        0     3254 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/32x32/linkchecker-gui.png
+-rw-r--r--   0        0        0     6232 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/48x48/linkchecker-gui.png
+-rw-r--r--   0        0        0     9761 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/doc/html/logo/64x64/linkchecker-gui.png
+-rw-r--r--   0        0        0    24421 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/__init__.py
+-rw-r--r--   0        0        0     2508 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/__main__.py
+-rw-r--r--   0        0        0      212 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/_release.py
+-rw-r--r--   0        0        0     1573 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/checker.py
+-rw-r--r--   0        0        0     2545 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/configuration.py
+-rw-r--r--   0        0        0     2580 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/contextmenu.py
+-rw-r--r--   0        0        0     1541 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/debug.py
+-rw-r--r--   0        0        0     6677 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor.py
+-rw-r--r--   0        0        0     4004 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qsci.py
+-rw-r--r--   0        0        0     6194 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qt.py
+-rw-r--r--   0        0        0     2905 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/help.py
+-rw-r--r--   0        0        0     9685 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/lineedit.py
+-rw-r--r--   0        0        0    52172 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_rc.py
+-rw-r--r--   0        0        0     1666 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_debug.py
+-rw-r--r--   0        0        0     2717 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_editor.py
+-rw-r--r--   0        0        0    56784 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_main.py
+-rw-r--r--   0        0        0     8958 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_options.py
+-rw-r--r--   0        0        0     2442 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/logger.py
+-rw-r--r--   0        0        0     4135 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/options.py
+-rw-r--r--   0        0        0     7561 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/projects.py
+-rw-r--r--   0        0        0     2896 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/properties.py
+-rw-r--r--   0        0        0     3333 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/recentdocs.py
+-rw-r--r--   0        0        0     5746 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/settings.py
+-rw-r--r--   0        0        0     2060 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/statistics.py
+-rw-r--r--   0        0        0     3480 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/syntax.py
+-rw-r--r--   0        0        0     3561 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/updater.py
+-rw-r--r--   0        0        0     6925 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/urlmodel.py
+-rw-r--r--   0        0        0     2720 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/urlsave.py
+-rw-r--r--   0        0        0     1419 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/validator.py
+-rw-r--r--   0        0        0    94208 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lccollection.qhc
+-rw-r--r--   0        0        0    77824 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lcdoc.qch
+-rw-r--r--   0        0        0        0 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/__init__.py
+-rw-r--r--   0        0        0     1171 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/containers.py
+-rw-r--r--   0        0        0     1259 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/fileutil.py
+-rw-r--r--   0        0        0        0 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/__init__.py
+-rw-r--r--   0        0        0     2347 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chrome.py
+-rw-r--r--   0        0        0     2550 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chromium.py
+-rw-r--r--   0        0        0     1733 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/firefox.py
+-rw-r--r--   0        0        0     1700 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/opera.py
+-rw-r--r--   0        0        0     1428 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/safari.py
+-rw-r--r--   0        0        0     1302 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/winutil.py
+-rw-r--r--   0        0        0     1668 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/test_containers.py
+-rw-r--r--   0        0        0     1287 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tests/test_gui.py
+-rw-r--r--   0        0        0     4084 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/tools/hatch_build.py
+-rw-r--r--   0        0        0      897 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/.gitignore
+-rw-r--r--   0        0        0    35141 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/LICENSE
+-rw-r--r--   0        0        0      761 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/README.md
+-rw-r--r--   0        0        0     2286 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1558 2023-04-21 18:37:43.000000 linkchecker_gui-10.0.0a3/PKG-INFO
```

### Comparing `linkchecker_gui-10.0.0a2/.flake8` & `linkchecker_gui-10.0.0a3/.flake8`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/pyoxidizer.bzl` & `linkchecker_gui-10.0.0a3/pyoxidizer.bzl`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     exe = dist.to_python_executable(
         name="linkchecker-gui",
         packaging_policy=policy,
         config=python_config,
     )
 
-    for resource in exe.pip_download(["PyQt5"]):
+    for resource in exe.pip_download(["PyQt6"]):
         resource.add_location = "filesystem-relative:lib"
         exe.add_python_resource(resource)
 
     exe.add_python_resources(exe.pip_install([CWD]))
     return exe
 
 register_target("exe", make_exe)
```

### Comparing `linkchecker_gui-10.0.0a2/doc/de.po` & `linkchecker_gui-10.0.0a3/doc/de.po`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/de/linkchecker-gui.1` & `linkchecker_gui-10.0.0a3/doc/de/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/en/linkchecker-gui.1` & `linkchecker_gui-10.0.0a3/doc/en/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/favicon.icns` & `linkchecker_gui-10.0.0a3/doc/html/favicon.icns`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/favicon.ico` & `linkchecker_gui-10.0.0a3/doc/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/html.header` & `linkchecker_gui-10.0.0a3/doc/html/html.header`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/index.txt` & `linkchecker_gui-10.0.0a3/doc/html/index.txt`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/lccollection.qhcp` & `linkchecker_gui-10.0.0a3/doc/html/lccollection.qhcp`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/pygments.css` & `linkchecker_gui-10.0.0a3/doc/html/pygments.css`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/sphinxdoc.css` & `linkchecker_gui-10.0.0a3/doc/html/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/logo/128x128/linkchecker-gui.png` & `linkchecker_gui-10.0.0a3/doc/html/logo/128x128/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/logo/16x16/linkchecker-gui.png` & `linkchecker_gui-10.0.0a3/doc/html/logo/16x16/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/logo/32x32/linkchecker-gui.png` & `linkchecker_gui-10.0.0a3/doc/html/logo/32x32/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/logo/48x48/linkchecker-gui.png` & `linkchecker_gui-10.0.0a3/doc/html/logo/48x48/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/doc/html/logo/64x64/linkchecker-gui.png` & `linkchecker_gui-10.0.0a3/doc/html/logo/64x64/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/__init__.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from linkcheck import LinkCheckerError
 from linkcheck import checker as linkchecker_checker
 from linkcheck import configuration as linkchecker_configuration
 from linkcheck import (director, get_link_pat, httputil, i18n, logconf,
                        mimeutil, strformat)
 from linkcheck import url as urlutil
 from linkcheck.parser import parse_text
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 from . import configuration
 from .checker import CheckerThread
 from .contextmenu import ContextMenu
 from .debug import LinkCheckerDebug
 from .editor import EditorWindow
 from .help import HelpWindow
@@ -53,15 +53,15 @@
 
 MaxMessageLength = 60
 
 
 def get_icon(name):
     """Return QIcon with given pixmap resource name."""
     icon = QtGui.QIcon()
-    icon.addPixmap(QtGui.QPixmap(name), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+    icon.addPixmap(QtGui.QPixmap(name), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
     return icon
 
 
 def warninglines2regex(lines):
     """Convert a list of strings to a regular expression matching any of
     the given strings."""
     return "|".join([re.escape(line) for line in lines])
@@ -75,15 +75,16 @@
     log_stats_signal = QtCore.pyqtSignal(object)
     error_signal = QtCore.pyqtSignal(str)
 
     def __init__(self, parent=None, url=None, project=None):
         """Initialize UI."""
         super().__init__(parent)
         self.setupUi(self)
-        self.setWindowFlags(self.windowFlags() | QtCore.Qt.WindowContextHelpButtonHint)
+        self.setWindowFlags(
+            self.windowFlags() | QtCore.Qt.WindowType.WindowContextHelpButtonHint)
         self.setWindowTitle(configuration.App)
         # app settings
         self.settings = Settings(RegistryBase, configuration.AppName)
         # init subdialogs
         self.options = LinkCheckerOptions(parent=self)
         self.debug = LinkCheckerDebug(parent=self)
         self.checker = CheckerThread(parent=self)
@@ -92,15 +93,15 @@
         self.assistant = HelpWindow(self, self.get_qhcpath())
         self.actionHelp.setVisible(True)
         self.actionCheckUpdates.setVisible(False)  # XXX
         self.config_error = None
         self.icon_start = get_icon(":/icons/start.png")
         self.icon_stop = get_icon(":/icons/stop.png")
         self.movie = QtGui.QMovie(":/icons/busy.gif")
-        self.movie.setCacheMode(QtGui.QMovie.CacheAll)
+        self.movie.setCacheMode(QtGui.QMovie.CacheMode.CacheAll)
         self.label_busy.setText("")
         self.label_busy.setMovie(self.movie)
         # init the rest
         self.init_logging()
         self.init_url(url)
         self.init_treeview()
         self.connect_widgets()
@@ -129,15 +130,15 @@
     def init_menu(self):
         """Add menu entries for bookmark file checking."""
         self.urlinput.addMenuEntries(self.menuEdit)
         return  # XXX
         self.menuLang = self.menuEdit.addMenu(_('Languages'))
         self.menuLang.setTitle(_("&Language"))
         # ensure only one action is checked
-        langActionGroup = QtWidgets.QActionGroup(self)
+        langActionGroup = QtGui.QActionGroup(self)
         langActionGroup.triggered.connect(self.switch_language)
         for i, lang in enumerate(sorted(i18n.supported_languages)):
             action = self.menuLang.addAction("&%d %s" % (i, lang))
             action.setCheckable(True)
             action.setData(lang)
             if lang == i18n.default_language:
                 action.setChecked(True)
@@ -198,15 +199,15 @@
         """Configure application shortcuts."""
 
         def selectUrl():
             """Highlight URL input textbox."""
             self.urlinput.setFocus()
             self.urlinput.selectAll()
 
-        shortcut = QtWidgets.QShortcut(QtGui.QKeySequence("Ctrl+L"), self)
+        shortcut = QtGui.QShortcut(QtGui.QKeySequence("Ctrl+L"), self)
         shortcut.activated.connect(selectUrl)
 
     def init_treeview(self):
         """Set treeview model and layout."""
         self.model = UrlItemModel()
         self.treeView.setModel(self.model)
         data = self.settings.read_treeviewcols()
@@ -310,15 +311,15 @@
         if status == Status.idle:
             self.aggregate = None
             self.controlButton.setText(_("Start"))
             self.controlButton.setIcon(self.icon_start)
             self.controlButton.setEnabled(True)
             self.actionSave.setEnabled(True)
             self.actionDebug.setEnabled(self.options.get_options()["debug"])
-            self.treeView.sortByColumn(0, QtCore.Qt.AscendingOrder)
+            self.treeView.sortByColumn(0, QtCore.Qt.SortOrder.AscendingOrder)
             self.treeView.setSortingEnabled(True)
             self.treeView.scrollToTop()
             self.movie.stop()
             # Reset progress information.
             self.label_active.setText("0")
             self.label_queued.setText("0")
             self.label_checked.setText("0")
@@ -347,15 +348,15 @@
         """Show help page."""
         url = QtCore.QUrl("%sindex.html" % DocBaseUrl)
         self.assistant.showDocumentation(url)
 
     @QtCore.pyqtSlot()
     def on_actionOptions_triggered(self):
         """Show option dialog."""
-        self.options.exec_()
+        self.options.exec()
 
     @QtCore.pyqtSlot()
     def on_actionQuit_triggered(self):
         """Quit application."""
         self.close()
 
     def closeEvent(self, e=None):
@@ -560,15 +561,15 @@
     @QtCore.pyqtSlot()
     def on_actionCopyToClipboard_triggered(self):
         """Copy item URL to clipboard."""
         urlitem = self.model.getUrlItem(self.treeView.currentIndex())
         if urlitem:
             clipboard = QtWidgets.QApplication.clipboard()
             clipboard.setText(urlitem.url_data.url)
-            event = QtCore.QEvent(QtCore.QEvent.Clipboard)
+            event = QtCore.QEvent(QtCore.QEvent.Type.Clipboard)
             QtWidgets.QApplication.sendEvent(clipboard, event)
 
     def set_statusmsg(self, msg):
         """Show given status message."""
         self.statusBar.showMessage(msg)
         if len(msg) > MaxMessageLength:
             self.label_status.setToolTip(msg)
@@ -591,19 +592,19 @@
         """Set statistic information for selected URL."""
         set_statistics(self, statistics)
 
     def internal_error(self, msg):
         """Display internal error message. Triggered by sys.excepthook()."""
         msgBox = QtWidgets.QMessageBox(self)
         msgBox.setStyleSheet("QLabel{min-width:500 px; font-size: 12px;}")
-        msgBox.setIcon(QtWidgets.QMessageBox.Warning)
+        msgBox.setIcon(QtWidgets.QMessageBox.Icon.Warning)
         msgBox.setWindowTitle(_("LinkChecker internal error"))
         msgBox.setText(msg)
-        msgBox.setStandardButtons(QtWidgets.QMessageBox.Close)
-        msgBox.exec_()
+        msgBox.setStandardButtons(QtWidgets.QMessageBox.StandardButton.Close)
+        msgBox.exec()
 
     def handleDragEvent(self, event):
         """Handle drag enter of move event."""
         mime = event.mimeData()
         if not mime.hasUrls():
             return event.ignore()
         url = mime.urls()[0]
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/__main__.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 import signal
 import sys
 
 from linkcheck import configuration
 from linkcheck.command.linkchecker import drop_privileges
 from linkcheck.fileutil import is_readable
-from PyQt5.QtWidgets import QApplication
+from PyQt6.QtWidgets import QApplication
 
 from . import LinkCheckerMain
 from .projects import ProjectExt
 
 
 def excepthook(window, etype, evalue, tb):
     """Catch unhandled exceptions."""
@@ -53,18 +53,18 @@
         fileorurl = args[1]
         if is_readable(fileorurl) and fileorurl.lower().endswith(ProjectExt):
             mainkwargs["project"] = fileorurl
         else:
             mainkwargs["url"] = fileorurl
     signal.signal(signal.SIGINT, signal.SIG_DFL)
     # use local variable here to avoid garbage collection of the main
-    # window before app.exec_() finishes
+    # window before app.exec() finishes
     window = LinkCheckerMain(**mainkwargs)
     window.show()
     window.raise_()  # this will raise the window on Mac OS X
     drop_privileges()
     sys.excepthook = lambda etype, evalue, tb: excepthook(window, etype, evalue, tb)
-    sys.exit(app.exec_())
+    sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/checker.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-from PyQt5 import QtCore
+from PyQt6 import QtCore
 from linkcheck import director
 
 
 class CheckerThread(QtCore.QThread):
     """Separate checker thread."""
 
     def __init__(self, parent=None):
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/configuration.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 certain conditions. Look at the file `LICENSE' within this distribution."""
 )
 
 
 # List Python modules in the form (module, name, version attribute)
 Modules = (
     # required modules
-    ("PyQt5.QtCore", "PyQt5", "PYQT_VERSION_STR"),
-    ("PyQt5.Qsci", "QScintilla", "QSCINTILLA_VERSION_STR"),
+    ("PyQt6.QtCore", "PyQt6", "PYQT_VERSION_STR"),
+    ("PyQt6.Qsci", "QScintilla", "QSCINTILLA_VERSION_STR"),
 )
 
 
 def get_modules_info():
     """Return unicode string with detected module info."""
     module_infos = []
     for (mod, name, version_attr) in Modules:
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/contextmenu.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/contextmenu.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-from PyQt5 import QtWidgets
+from PyQt6 import QtWidgets
 import os
 import urllib.parse
 
 from linkcheck.checker.fileurl import get_os_filename
 
 
 class ContextMenu(QtWidgets.QMenu):
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/debug.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 from .linkchecker_ui_debug import Ui_DebugDialog
 
 
 class LinkCheckerDebug(QtWidgets.QDialog, Ui_DebugDialog):
     """Show debug text."""
 
     log_msg_signal = QtCore.pyqtSignal(str)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/editor.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import os
 import urllib.parse
 
-from PyQt5 import QtWidgets, QtCore
+from PyQt6 import QtWidgets, QtCore
 
 from .linkchecker_ui_editor import Ui_EditorDialog
 from linkcheck.checker.fileurl import get_os_filename
 
 try:
     from .editor_qsci import ContentTypeLexers, Editor
 except ImportError:
@@ -99,23 +99,24 @@
             # unchanged
             e.accept()
 
     def wants_save(self):
         """Ask user if he wants to save changes. Return True if user
         wants to save, else False."""
         dialog = QtWidgets.QMessageBox(parent=self)
-        dialog.setIcon(QtWidgets.QMessageBox.Question)
+        dialog.setIcon(QtWidgets.QMessageBox.Icon.Question)
         dialog.setWindowTitle(_("Save file?"))
         dialog.setText(_("The document has been modified."))
         dialog.setInformativeText(_("Do you want to save your changes?"))
         dialog.setStandardButtons(
-            QtWidgets.QMessageBox.Save | QtWidgets.QMessageBox.Discard
+            QtWidgets.QMessageBox.StandardButton.Save |
+            QtWidgets.QMessageBox.StandardButton.Discard
         )
-        dialog.setDefaultButton(QtWidgets.QMessageBox.Save)
-        return dialog.exec_() == QtWidgets.QMessageBox.Save
+        dialog.setDefaultButton(QtWidgets.QMessageBox.StandardButton.Save)
+        return dialog.exec() == QtWidgets.QMessageBox.StandardButton.Save
 
     def save(self):
         """Save editor contents to file."""
         if not self.filename:
             title = _("Save File As")
             res = QtWidgets.QFileDialog.getSaveFileName(self, title, self.basedir)
             if not res:
@@ -129,25 +130,25 @@
             if not os.access(self.filename, os.W_OK):
                 return
         fh = None
         saved = False
         try:
             try:
                 fh = QtCore.QFile(self.filename)
-                if not fh.open(QtCore.QIODevice.WriteOnly):
+                if not fh.open(QtCore.QIODevice.OpenModeFlag.WriteOnly):
                     raise OSError(fh.errorString())
                 stream = QtCore.QTextStream(fh)
                 stream.setCodec("UTF-8")
                 stream << self.editor.text()
                 self.editor.setModified(False)
                 saved = True
             except OSError as e:
                 err = QtWidgets.QMessageBox(self)
                 err.setText(str(e))
-                err.exec_()
+                err.exec()
         finally:
             if fh is not None:
                 fh.close()
         if saved:
             self.saved.emit(self.filename)
         return saved
 
@@ -164,22 +165,21 @@
             title = self.filename
         self.setWindowTitle(title)
         fh = None
         loaded = False
         try:
             try:
                 fh = QtCore.QFile(self.filename)
-                if not fh.open(QtCore.QIODevice.ReadOnly):
+                if not fh.open(QtCore.QIODevice.OpenModeFlag.ReadOnly):
                     raise OSError(fh.errorString())
                 stream = QtCore.QTextStream(fh)
-                stream.setCodec("UTF-8")
                 self.setText(stream.readAll())
                 loaded = True
             except OSError as e:
                 err = QtWidgets.QMessageBox(self)
                 err.setText(str(e))
-                err.exec_()
+                err.exec()
         finally:
             if fh is not None:
                 fh.close()
         if loaded:
             self.loaded.emit(self.filename)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/editor_qsci.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qsci.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 Text editor implemented with QScintilla
 """
-from PyQt5 import QtGui, Qsci
+from PyQt6 import QtGui, Qsci
 
 # Map MIME type to Scintilla lexer class
 ContentTypeLexers = {
     "application/x-shellscript": Qsci.QsciLexerBash,
     "application/x-sh": Qsci.QsciLexerBash,
     "application/x-msdos-program": Qsci.QsciLexerBatch,
     # "": Qsci.QsciLexerCMake,
@@ -68,27 +68,27 @@
 
         # Set the default font of the editor
         # and take the same font for line numbers
         self.setFont(font)
         self.setMarginsFont(font)
 
         # line number margin for 4 digits (plus 2px extra space)
-        margin = QtGui.QFontMetrics(font).width("0" * 4) + 2
+        margin = QtGui.QFontMetrics(font).boundingRect("0" * 4).width() + 2
         # Display line numbers, margin 0 is for line numbers
         self.setMarginWidth(0, margin)
         self.setMarginLineNumbers(0, True)
 
         # Show whitespace to help detect whitespace errors
-        self.setWhitespaceVisibility(True)
+        self.setWhitespaceVisibility(self.WhitespaceVisibility.WsVisible)
 
         # Use boxes as folding visual
-        self.setFolding(self.BoxedTreeFoldStyle)
+        self.setFolding(self.FoldStyle.BoxedTreeFoldStyle)
 
         # Braces matching
-        self.setBraceMatching(self.SloppyBraceMatch)
+        self.setBraceMatching(self.BraceMatch.SloppyBraceMatch)
 
         # Editing line color
         self.setCaretLineVisible(True)
         self.setCaretLineBackgroundColor(QtGui.QColor("#e5e5cb"))
 
         # line numbers margin colors
         self.setMarginsBackgroundColor(QtGui.QColor("#e5e5e5"))
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/editor_qt.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/editor_qt.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 Text editor implemented with Qt
 """
-from PyQt5 import QtWidgets, QtGui, QtCore
+from PyQt6 import QtWidgets, QtGui, QtCore
 from . import syntax
 
 # Map MIME type to QSyntaxHighlighter class
 ContentTypeLexers = {
     "text/html": syntax.HtmlHighlighter,
     "application/xml": syntax.XmlHighlighter,
     "text/plain+ini": syntax.IniHighlighter,
@@ -82,50 +82,49 @@
         """Move cursor to given line and column. Line counting starts
         with zero."""
         block = self.document().findBlockByNumber(line)
         if block.isValid():
             cursor = QtGui.QTextCursor(block)
             if column > 0:
                 cursor.movePosition(
-                    QtGui.QTextCursor.Right,
-                    QtGui.QTextCursor.MoveAnchor,
+                    QtGui.QTextCursor.MoveOperation.Right,
+                    QtGui.QTextCursor.MoveMode.MoveAnchor,
                     column,
                 )
             self.setTextCursor(cursor)
             self.centerCursor()
 
     def lineNumberAreaPaintEvent(self, event):
         """Paint line numbers."""
         painter = QtGui.QPainter(self.lineNumberArea)
-        painter.fillRect(event.rect(), QtCore.Qt.lightGray)
+        painter.fillRect(event.rect(), QtCore.Qt.GlobalColor.lightGray)
         block = self.firstVisibleBlock()
         blockNumber = block.blockNumber()
         top = self.blockBoundingGeometry(block).translated(self.contentOffset()).top()
         bottom = top + self.blockBoundingRect(block).height()
         while block.isValid() and top <= event.rect().bottom():
             if block.isVisible() and bottom >= event.rect().top():
                 number = str(blockNumber + 1)
-                painter.setPen(QtCore.Qt.black)
+                painter.setPen(QtCore.Qt.GlobalColor.black)
                 painter.drawText(
-                    0,
-                    top,
-                    self.lineNumberArea.width(),
-                    self.fontMetrics().height(),
-                    QtCore.Qt.AlignRight,
+                    QtCore.QRectF(
+                        0, top,
+                        self.lineNumberArea.width(), self.fontMetrics().height()),
+                    QtCore.Qt.AlignmentFlag.AlignRight,
                     number,
                 )
-            block = next(block)
+            block = block.next()
             top = bottom
             bottom = top + self.blockBoundingRect(block).height()
             blockNumber += 1
 
     def lineNumberAreaWidth(self):
         """Calculate line number area width."""
         digits = max(1, len(str(self.blockCount())))
-        onecharwidth = self.fontMetrics().width('9')
+        onecharwidth = self.fontMetrics().boundingRect('9').width()
         space = 3 + onecharwidth * digits
         return space
 
     def resizeEvent(self, event):
         """Resize line number area together with editor."""
         super().resizeEvent(event)
         cr = self.contentsRect()
@@ -138,17 +137,18 @@
         self.setViewportMargins(self.lineNumberAreaWidth(), 0, 0, 0)
 
     def highlightCurrentLine(self):
         """Highlight the current line."""
         extraSelections = []
         if not self.isReadOnly():
             selection = QtWidgets.QTextEdit.ExtraSelection()
-            lineColor = QtGui.QColor(QtCore.Qt.yellow).lighter(160)
+            lineColor = QtGui.QColor(QtCore.Qt.GlobalColor.yellow).lighter(160)
             selection.format.setBackground(lineColor)
-            selection.format.setProperty(QtGui.QTextFormat.FullWidthSelection, True)
+            selection.format.setProperty(
+                QtGui.QTextFormat.Property.FullWidthSelection, True)
             selection.cursor = self.textCursor()
             selection.cursor.clearSelection()
             extraSelections.append(selection)
         self.setExtraSelections(extraSelections)
 
     def updateLineNumberArea(self, rect, dy):
         """Update the line number area."""
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/help.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from . import configuration
-from PyQt5 import QtCore, QtWidgets, QtHelp
+from PyQt6 import QtCore, QtWidgets, QtHelp
 
 
 class HelpWindow(QtWidgets.QDialog):
     """A custom help display dialog."""
 
     def __init__(self, parent, qhcpath):
         """Initialize dialog and load qhc help project from given path."""
@@ -28,15 +28,15 @@
         self.engine.setupData()
         self.setWindowTitle("%s Help" % configuration.AppName)
         self.build_ui()
 
     def build_ui(self):
         """Build UI for the help window."""
         splitter = QtWidgets.QSplitter()
-        splitter.setOrientation(QtCore.Qt.Vertical)
+        splitter.setOrientation(QtCore.Qt.Orientation.Vertical)
         self.browser = HelpBrowser(splitter, self.engine)
         self.tree = self.engine.contentWidget()
         self.tree.setExpandsOnDoubleClick(False)
         self.tree.linkActivated.connect(self.browser.setSource)
         splitter.addWidget(self.tree)
         splitter.addWidget(self.browser)
         splitter.setSizes((70, 530))
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/lineedit.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/lineedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class LineEdit(QtWidgets.QLineEdit):
     """A line edit widget displaying a clear button if there is some text
     and a down-arrow button displaying a list of strings (eg. recent
     documents)."""
 
@@ -33,82 +33,86 @@
 
     def setup_clear_button(self):
         """Initialize the clear button."""
         self.clearButton = QtWidgets.QToolButton(self)
         pixmap = QtGui.QPixmap(":/icons/clear.png")
         self.clearButton.setIcon(QtGui.QIcon(pixmap))
         self.clearButton.setIconSize(pixmap.size())
-        self.clearButton.setCursor(QtCore.Qt.ArrowCursor)
+        self.clearButton.setCursor(QtCore.Qt.CursorShape.ArrowCursor)
         style = "QToolButton { border: none; padding: 0px; }"
         self.clearButton.setStyleSheet(style)
         self.clearButton.hide()
         self.clearButton.clicked.connect(self.clear)
         self.textChanged.connect(self.updateCloseButton)
 
     def setup_list_button(self):
         """Initialize the dropdown list button."""
         self.listButton = QtWidgets.QToolButton(self)
         pixmap = QtGui.QPixmap(":/icons/arrow_down.png")
         self.listButton.setIcon(QtGui.QIcon(pixmap))
         self.listButton.setIconSize(pixmap.size())
-        self.listButton.setCursor(QtCore.Qt.ArrowCursor)
+        self.listButton.setCursor(QtCore.Qt.CursorShape.ArrowCursor)
         style = "QToolButton { border: none; padding: 0px; }"
         self.listButton.setStyleSheet(style)
         self.listButton.hide()
         self.listButton.clicked.connect(self.toggle_list)
 
     def setModel(self, model):
         """Set list model for list of recent documents."""
         self.listmodel = model
         self.listview = QtWidgets.QListView()
         self.listview.setModel(model)
-        self.listview.setWindowFlags(QtCore.Qt.Popup)
-        self.listview.setFocusPolicy(QtCore.Qt.NoFocus)
+        self.listview.setWindowFlags(QtCore.Qt.WindowType.Popup)
+        self.listview.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
         self.listview.setFocusProxy(self)
         self.listview.setMouseTracking(True)
         self.listview.setUniformItemSizes(True)
-        self.listview.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self.listview.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
-        self.listview.setFrameStyle(QtWidgets.QFrame.Box | QtWidgets.QFrame.Plain)
-        self.listview.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
+        self.listview.setEditTriggers(
+            QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
+        self.listview.setSelectionBehavior(
+            QtWidgets.QAbstractItemView.SelectionBehavior.SelectRows)
+        self.listview.setFrameStyle(
+            QtWidgets.QFrame.Shape.Box | QtWidgets.QFrame.Shadow.Plain)
+        self.listview.setHorizontalScrollBarPolicy(
+            QtCore.Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
         self.listview.installEventFilter(self)
         self.listview.clicked.connect(self.selectRecentDocument)
         self.listview.hide()
         def updatefunc(parent, start, end): return self.updateListButton
         self.listmodel.rowsInserted.connect(updatefunc)
         self.listmodel.rowsRemoved.connect(updatefunc)
         self.updateListButton()
 
     def eventFilter(self, obj, event):
         """Handle events from the listview popup."""
         if obj != self.listview:
             return False
 
-        if event.type() == QtCore.QEvent.MouseButtonPress:
+        if event.type() == QtCore.QEvent.Type.MouseButtonPress:
             self.listview.hide()
             self.setFocus()
             return True
 
-        if event.type() == QtCore.QEvent.KeyPress:
+        if event.type() == QtCore.QEvent.Type.KeyPress:
             consumed = False
             key = event.key()
-            if key in (QtCore.Qt.Key_Enter, QtCore.Qt.Key_Return):
+            if key in (QtCore.Qt.Key.Key_Enter, QtCore.Qt.Key.Key_Return):
                 self.doneCompletion()
                 consumed = True
-            elif key == QtCore.Qt.Key_Escape:
+            elif key == QtCore.Qt.Key.Key_Escape:
                 self.setFocus()
                 self.listview.hide()
                 consumed = True
             elif key in (
-                QtCore.Qt.Key_Up,
-                QtCore.Qt.Key_Down,
-                QtCore.Qt.Key_Home,
-                QtCore.Qt.Key_End,
-                QtCore.Qt.Key_PageUp,
-                QtCore.Qt.Key_PageDown,
+                QtCore.Qt.Key.Key_Up,
+                QtCore.Qt.Key.Key_Down,
+                QtCore.Qt.Key.Key_Home,
+                QtCore.Qt.Key.Key_End,
+                QtCore.Qt.Key.Key_PageUp,
+                QtCore.Qt.Key.Key_PageDown,
             ):
                 pass
             else:
                 self.setFocus()
                 self.event(event)
                 self.listview.hide()
             return consumed
@@ -118,15 +122,16 @@
         """Select recent document text after click on the list view."""
         self.listview.hide()
         item = self.listmodel.data(index)
         self.setText(item.value())
 
     def setup_size_metrics(self):
         """Set widget size including the buttons."""
-        frameWidth = self.style().pixelMetric(QtWidgets.QStyle.PM_DefaultFrameWidth)
+        frameWidth = self.style().pixelMetric(
+            QtWidgets.QStyle.PixelMetric.PM_DefaultFrameWidth)
         padding_right = self.clearButton.sizeHint().width() + frameWidth + 1
         padding_left = self.listButton.sizeHint().width() + frameWidth + 1
         style = "QLineEdit { padding-left: %dpx; padding-right: %dpx } " % (
             padding_left,
             padding_right,
         )
         self.setStyleSheet(style)
@@ -140,15 +145,16 @@
         )
         minHeight = max(minSize.height(), buttonHeight + frameWidth * 2)
         # set minimum size
         self.setMinimumSize(minWidth, minHeight)
 
     def resizeEvent(self, event):
         """Move the buttons due to resize event."""
-        frameWidth = self.style().pixelMetric(QtWidgets.QStyle.PM_DefaultFrameWidth)
+        frameWidth = self.style().pixelMetric(
+            QtWidgets.QStyle.PixelMetric.PM_DefaultFrameWidth)
         bottom = self.rect().y() + self.rect().height()
         # clear button
         sizeHint = self.clearButton.sizeHint()
         x = self.rect().right() - frameWidth - sizeHint.width()
         y = (bottom - sizeHint.height()) // 2
         self.clearButton.move(x, y)
         # list button
@@ -196,15 +202,15 @@
             action = menu.addAction(name % {"browser": "Safari"})
             action.triggered.connect(lambda: self.setText(find_safari()))
 
     def contextMenuEvent(self, event):
         """Handle context menu event."""
         menu = self.createStandardContextMenu()
         self.addMenuEntries(menu)
-        menu.exec_(event.globalPos())
+        menu.exec(event.globalPos())
 
 
 def find_firefox():
     """Return Firefox bookmark filename or empty string if not found."""
     from .library.bookmarks.firefox import find_bookmark_file
 
     return find_bookmark_file()
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_rc.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Resource object code
 #
 # Created: Wed May 11 00:26:36 2011
 #      by: The Resource Compiler for PyQt (Qt v4.7.2)
 #
 # WARNING! All changes made in this file will be lost!
 
-from PyQt5 import QtCore
+from PyQt6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x01\xbc\
 \x89\
 \x50\x4e\x47\x0d\x0a\x1a\x0a\x00\x00\x00\x0d\x49\x48\x44\x52\x00\
 \x00\x00\x0c\x00\x00\x00\x0c\x08\x06\x00\x00\x00\x56\x75\x5c\xe7\
 \x00\x00\x00\x01\x73\x52\x47\x42\x00\xae\xce\x1c\xe9\x00\x00\x00\
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_debug.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_debug.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'ui/debug.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.1
+# Created by: PyQt6 UI code generator 6.4.2
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_DebugDialog(object):
     def setupUi(self, DebugDialog):
         DebugDialog.setObjectName("DebugDialog")
-        DebugDialog.setWindowModality(QtCore.Qt.ApplicationModal)
+        DebugDialog.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
         DebugDialog.resize(564, 547)
         self.verticalLayout = QtWidgets.QVBoxLayout(DebugDialog)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.frame = QtWidgets.QFrame(DebugDialog)
-        self.frame.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.frame.setFrameShadow(QtWidgets.QFrame.Raised)
+        self.frame = QtWidgets.QFrame(parent=DebugDialog)
+        self.frame.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.frame.setFrameShadow(QtWidgets.QFrame.Shadow.Raised)
         self.frame.setObjectName("frame")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.frame)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.textEdit = QtWidgets.QPlainTextEdit(self.frame)
+        self.textEdit = QtWidgets.QPlainTextEdit(parent=self.frame)
         self.textEdit.setUndoRedoEnabled(False)
         self.textEdit.setReadOnly(True)
         self.textEdit.setPlainText("")
         self.textEdit.setObjectName("textEdit")
         self.verticalLayout_2.addWidget(self.textEdit)
         self.verticalLayout.addWidget(self.frame)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_editor.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'ui/editor.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.1
+# Created by: PyQt6 UI code generator 6.4.2
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_EditorDialog(object):
     def setupUi(self, EditorDialog):
         EditorDialog.setObjectName("EditorDialog")
-        EditorDialog.setWindowModality(QtCore.Qt.ApplicationModal)
+        EditorDialog.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
         EditorDialog.resize(640, 600)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(EditorDialog.sizePolicy().hasHeightForWidth())
         EditorDialog.setSizePolicy(sizePolicy)
         self.verticalLayout = QtWidgets.QVBoxLayout(EditorDialog)
         self.verticalLayout.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.menubar = QtWidgets.QMenuBar(EditorDialog)
+        self.menubar = QtWidgets.QMenuBar(parent=EditorDialog)
         self.menubar.setObjectName("menubar")
-        self.menuFile = QtWidgets.QMenu(self.menubar)
+        self.menuFile = QtWidgets.QMenu(parent=self.menubar)
         self.menuFile.setObjectName("menuFile")
         self.verticalLayout.addWidget(self.menubar)
-        self.frame = QtWidgets.QFrame(EditorDialog)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        self.frame = QtWidgets.QFrame(parent=EditorDialog)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.frame.sizePolicy().hasHeightForWidth())
         self.frame.setSizePolicy(sizePolicy)
-        self.frame.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.frame.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.frame.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.frame.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.frame.setLineWidth(0)
         self.frame.setObjectName("frame")
         self.verticalLayout.addWidget(self.frame)
-        self.actionSave = QtWidgets.QAction(EditorDialog)
+        self.actionSave = QtGui.QAction(parent=EditorDialog)
         self.actionSave.setObjectName("actionSave")
         self.menuFile.addAction(self.actionSave)
         self.menubar.addAction(self.menuFile.menuAction())
 
         self.retranslateUi(EditorDialog)
         QtCore.QMetaObject.connectSlotsByName(EditorDialog)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_main.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,753 +1,752 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'ui/main.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.1
+# Created by: PyQt6 UI code generator 6.4.2
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(713, 627)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(MainWindow.sizePolicy().hasHeightForWidth())
         MainWindow.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap(":/icons/app.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon.addPixmap(QtGui.QPixmap(":/icons/app.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         MainWindow.setWindowIcon(icon)
         MainWindow.setStatusTip("")
-        self.centralwidget = QtWidgets.QWidget(MainWindow)
+        self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout.setContentsMargins(4, 4, 4, 4)
         self.verticalLayout.setObjectName("verticalLayout")
         self.horizontalLayout_3 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_3.setObjectName("horizontalLayout_3")
-        self.label = QtWidgets.QLabel(self.centralwidget)
+        self.label = QtWidgets.QLabel(parent=self.centralwidget)
         self.label.setObjectName("label")
         self.horizontalLayout_3.addWidget(self.label)
-        spacerItem = QtWidgets.QSpacerItem(4, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem = QtWidgets.QSpacerItem(4, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem)
-        self.urlinput = LineEdit(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        self.urlinput = LineEdit(parent=self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(1)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.urlinput.sizePolicy().hasHeightForWidth())
         self.urlinput.setSizePolicy(sizePolicy)
         self.urlinput.setMaxLength(2048)
         self.urlinput.setObjectName("urlinput")
         self.horizontalLayout_3.addWidget(self.urlinput)
-        spacerItem1 = QtWidgets.QSpacerItem(10, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem1 = QtWidgets.QSpacerItem(10, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem1)
-        self.controlButton = QtWidgets.QPushButton(self.centralwidget)
+        self.controlButton = QtWidgets.QPushButton(parent=self.centralwidget)
         self.controlButton.setStatusTip("")
         icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap(":/icons/start.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon1.addPixmap(QtGui.QPixmap(":/icons/start.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.controlButton.setIcon(icon1)
         self.controlButton.setDefault(True)
         self.controlButton.setObjectName("controlButton")
         self.horizontalLayout_3.addWidget(self.controlButton)
         self.verticalLayout.addLayout(self.horizontalLayout_3)
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
-        self.horizontalLayout_4.setSizeConstraint(QtWidgets.QLayout.SetDefaultConstraint)
+        self.horizontalLayout_4.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetDefaultConstraint)
         self.horizontalLayout_4.setContentsMargins(0, 0, -1, -1)
         self.horizontalLayout_4.setObjectName("horizontalLayout_4")
-        self.label_29 = QtWidgets.QLabel(self.centralwidget)
+        self.label_29 = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_29.setObjectName("label_29")
         self.horizontalLayout_4.addWidget(self.label_29)
-        self.label_32 = QtWidgets.QLabel(self.centralwidget)
+        self.label_32 = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_32.setObjectName("label_32")
         self.horizontalLayout_4.addWidget(self.label_32)
-        self.label_active = QtWidgets.QLabel(self.centralwidget)
+        self.label_active = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_active.setMinimumSize(QtCore.QSize(40, 0))
         self.label_active.setObjectName("label_active")
         self.horizontalLayout_4.addWidget(self.label_active)
-        self.label_30 = QtWidgets.QLabel(self.centralwidget)
+        self.label_30 = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_30.setObjectName("label_30")
         self.horizontalLayout_4.addWidget(self.label_30)
-        self.label_queued = QtWidgets.QLabel(self.centralwidget)
+        self.label_queued = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_queued.setMinimumSize(QtCore.QSize(40, 0))
         self.label_queued.setObjectName("label_queued")
         self.horizontalLayout_4.addWidget(self.label_queued)
-        self.label_28 = QtWidgets.QLabel(self.centralwidget)
+        self.label_28 = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_28.setObjectName("label_28")
         self.horizontalLayout_4.addWidget(self.label_28)
-        self.label_checked = QtWidgets.QLabel(self.centralwidget)
+        self.label_checked = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_checked.setMinimumSize(QtCore.QSize(50, 0))
         self.label_checked.setObjectName("label_checked")
         self.horizontalLayout_4.addWidget(self.label_checked)
-        self.label_15 = QtWidgets.QLabel(self.centralwidget)
+        self.label_15 = QtWidgets.QLabel(parent=self.centralwidget)
         self.label_15.setObjectName("label_15")
         self.horizontalLayout_4.addWidget(self.label_15)
-        self.label_busy = QtWidgets.QLabel(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
+        self.label_busy = QtWidgets.QLabel(parent=self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Fixed, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(16)
         sizePolicy.setVerticalStretch(16)
         sizePolicy.setHeightForWidth(self.label_busy.sizePolicy().hasHeightForWidth())
         self.label_busy.setSizePolicy(sizePolicy)
         self.label_busy.setMinimumSize(QtCore.QSize(16, 16))
         self.label_busy.setObjectName("label_busy")
         self.horizontalLayout_4.addWidget(self.label_busy)
-        self.label_status = QtWidgets.QLabel(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.label_status = QtWidgets.QLabel(parent=self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_status.sizePolicy().hasHeightForWidth())
         self.label_status.setSizePolicy(sizePolicy)
         self.label_status.setText("")
         self.label_status.setObjectName("label_status")
         self.horizontalLayout_4.addWidget(self.label_status)
         self.verticalLayout.addLayout(self.horizontalLayout_4)
-        self.treeView = QtWidgets.QTreeView(self.centralwidget)
-        self.treeView.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
-        self.treeView.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.treeView = QtWidgets.QTreeView(parent=self.centralwidget)
+        self.treeView.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
+        self.treeView.setEditTriggers(QtWidgets.QAbstractItemView.EditTrigger.NoEditTriggers)
         self.treeView.setAlternatingRowColors(True)
-        self.treeView.setSelectionMode(QtWidgets.QAbstractItemView.ExtendedSelection)
+        self.treeView.setSelectionMode(QtWidgets.QAbstractItemView.SelectionMode.ExtendedSelection)
         self.treeView.setRootIsDecorated(False)
         self.treeView.setUniformRowHeights(True)
         self.treeView.setItemsExpandable(False)
         self.treeView.setSortingEnabled(False)
         self.treeView.setAllColumnsShowFocus(True)
         self.treeView.setExpandsOnDoubleClick(False)
         self.treeView.setObjectName("treeView")
         self.verticalLayout.addWidget(self.treeView)
         self.horizontalLayout = QtWidgets.QHBoxLayout()
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.url_properties = QtWidgets.QGroupBox(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
+        self.url_properties = QtWidgets.QGroupBox(parent=self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.url_properties.sizePolicy().hasHeightForWidth())
         self.url_properties.setSizePolicy(sizePolicy)
-        self.url_properties.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignTop)
+        self.url_properties.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignTop)
         self.url_properties.setObjectName("url_properties")
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout(self.url_properties)
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        self.frame = QtWidgets.QFrame(self.url_properties)
-        self.frame.setFrameShape(QtWidgets.QFrame.NoFrame)
-        self.frame.setFrameShadow(QtWidgets.QFrame.Plain)
+        self.frame = QtWidgets.QFrame(parent=self.url_properties)
+        self.frame.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
+        self.frame.setFrameShadow(QtWidgets.QFrame.Shadow.Plain)
         self.frame.setLineWidth(0)
         self.frame.setObjectName("frame")
         self.formLayout = QtWidgets.QFormLayout(self.frame)
-        self.formLayout.setFieldGrowthPolicy(QtWidgets.QFormLayout.ExpandingFieldsGrow)
+        self.formLayout.setFieldGrowthPolicy(QtWidgets.QFormLayout.FieldGrowthPolicy.ExpandingFieldsGrow)
         self.formLayout.setObjectName("formLayout")
-        self.label_2 = QtWidgets.QLabel(self.frame)
+        self.label_2 = QtWidgets.QLabel(parent=self.frame)
         self.label_2.setObjectName("label_2")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_2)
-        self.prop_url = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_2)
+        self.prop_url = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_url.sizePolicy().hasHeightForWidth())
         self.prop_url.setSizePolicy(sizePolicy)
         self.prop_url.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_url.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_url.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_url.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_url.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_url.setText("")
-        self.prop_url.setTextFormat(QtCore.Qt.RichText)
+        self.prop_url.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.prop_url.setOpenExternalLinks(True)
-        self.prop_url.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_url.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_url.setObjectName("prop_url")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.prop_url)
-        self.label_3 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_url)
+        self.label_3 = QtWidgets.QLabel(parent=self.frame)
         self.label_3.setObjectName("label_3")
-        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_3)
-        self.prop_name = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_3)
+        self.prop_name = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_name.sizePolicy().hasHeightForWidth())
         self.prop_name.setSizePolicy(sizePolicy)
         self.prop_name.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_name.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_name.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_name.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_name.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_name.setText("")
-        self.prop_name.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_name.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_name.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_name.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_name.setObjectName("prop_name")
-        self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.prop_name)
-        self.label_4 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_name)
+        self.label_4 = QtWidgets.QLabel(parent=self.frame)
         self.label_4.setObjectName("label_4")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_4)
-        self.prop_parenturl = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_4)
+        self.prop_parenturl = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_parenturl.sizePolicy().hasHeightForWidth())
         self.prop_parenturl.setSizePolicy(sizePolicy)
         self.prop_parenturl.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_parenturl.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_parenturl.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_parenturl.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_parenturl.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_parenturl.setText("")
-        self.prop_parenturl.setTextFormat(QtCore.Qt.RichText)
+        self.prop_parenturl.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.prop_parenturl.setOpenExternalLinks(True)
-        self.prop_parenturl.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_parenturl.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_parenturl.setObjectName("prop_parenturl")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.prop_parenturl)
-        self.label_5 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_parenturl)
+        self.label_5 = QtWidgets.QLabel(parent=self.frame)
         self.label_5.setObjectName("label_5")
-        self.formLayout.setWidget(3, QtWidgets.QFormLayout.LabelRole, self.label_5)
-        self.prop_base = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_5)
+        self.prop_base = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_base.sizePolicy().hasHeightForWidth())
         self.prop_base.setSizePolicy(sizePolicy)
         self.prop_base.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_base.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_base.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_base.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_base.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_base.setText("")
-        self.prop_base.setTextFormat(QtCore.Qt.RichText)
+        self.prop_base.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.prop_base.setOpenExternalLinks(False)
-        self.prop_base.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_base.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_base.setObjectName("prop_base")
-        self.formLayout.setWidget(3, QtWidgets.QFormLayout.FieldRole, self.prop_base)
-        self.label_7 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_base)
+        self.label_7 = QtWidgets.QLabel(parent=self.frame)
         self.label_7.setObjectName("label_7")
-        self.formLayout.setWidget(4, QtWidgets.QFormLayout.LabelRole, self.label_7)
-        self.prop_checktime = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_7)
+        self.prop_checktime = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_checktime.sizePolicy().hasHeightForWidth())
         self.prop_checktime.setSizePolicy(sizePolicy)
         self.prop_checktime.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_checktime.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_checktime.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_checktime.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_checktime.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_checktime.setText("")
-        self.prop_checktime.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_checktime.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_checktime.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_checktime.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_checktime.setObjectName("prop_checktime")
-        self.formLayout.setWidget(4, QtWidgets.QFormLayout.FieldRole, self.prop_checktime)
-        self.label_8 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_checktime)
+        self.label_8 = QtWidgets.QLabel(parent=self.frame)
         self.label_8.setObjectName("label_8")
-        self.formLayout.setWidget(5, QtWidgets.QFormLayout.LabelRole, self.label_8)
-        self.prop_dltime = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_8)
+        self.prop_dltime = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_dltime.sizePolicy().hasHeightForWidth())
         self.prop_dltime.setSizePolicy(sizePolicy)
         self.prop_dltime.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_dltime.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_dltime.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_dltime.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_dltime.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_dltime.setText("")
-        self.prop_dltime.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_dltime.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_dltime.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_dltime.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_dltime.setObjectName("prop_dltime")
-        self.formLayout.setWidget(5, QtWidgets.QFormLayout.FieldRole, self.prop_dltime)
-        self.label_9 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_dltime)
+        self.label_9 = QtWidgets.QLabel(parent=self.frame)
         self.label_9.setObjectName("label_9")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.LabelRole, self.label_9)
-        self.prop_size = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_9)
+        self.prop_size = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_size.sizePolicy().hasHeightForWidth())
         self.prop_size.setSizePolicy(sizePolicy)
         self.prop_size.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_size.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_size.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_size.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_size.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_size.setText("")
-        self.prop_size.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_size.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_size.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_size.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_size.setObjectName("prop_size")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.FieldRole, self.prop_size)
-        self.label_10 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_size)
+        self.label_10 = QtWidgets.QLabel(parent=self.frame)
         self.label_10.setObjectName("label_10")
-        self.formLayout.setWidget(8, QtWidgets.QFormLayout.LabelRole, self.label_10)
-        self.prop_info = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(8, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_10)
+        self.prop_info = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_info.sizePolicy().hasHeightForWidth())
         self.prop_info.setSizePolicy(sizePolicy)
         self.prop_info.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_info.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_info.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_info.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_info.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_info.setText("")
-        self.prop_info.setTextFormat(QtCore.Qt.PlainText)
+        self.prop_info.setTextFormat(QtCore.Qt.TextFormat.PlainText)
         self.prop_info.setWordWrap(True)
-        self.prop_info.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_info.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_info.setObjectName("prop_info")
-        self.formLayout.setWidget(8, QtWidgets.QFormLayout.FieldRole, self.prop_info)
-        self.label_11 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(8, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_info)
+        self.label_11 = QtWidgets.QLabel(parent=self.frame)
         self.label_11.setObjectName("label_11")
-        self.formLayout.setWidget(9, QtWidgets.QFormLayout.LabelRole, self.label_11)
-        self.prop_warning = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(9, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_11)
+        self.prop_warning = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_warning.sizePolicy().hasHeightForWidth())
         self.prop_warning.setSizePolicy(sizePolicy)
         self.prop_warning.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_warning.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_warning.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_warning.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_warning.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_warning.setText("")
-        self.prop_warning.setTextFormat(QtCore.Qt.PlainText)
+        self.prop_warning.setTextFormat(QtCore.Qt.TextFormat.PlainText)
         self.prop_warning.setScaledContents(True)
         self.prop_warning.setWordWrap(True)
-        self.prop_warning.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_warning.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_warning.setObjectName("prop_warning")
-        self.formLayout.setWidget(9, QtWidgets.QFormLayout.FieldRole, self.prop_warning)
-        self.label_12 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(9, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_warning)
+        self.label_12 = QtWidgets.QLabel(parent=self.frame)
         self.label_12.setObjectName("label_12")
-        self.formLayout.setWidget(10, QtWidgets.QFormLayout.LabelRole, self.label_12)
-        self.prop_result = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(10, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_12)
+        self.prop_result = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_result.sizePolicy().hasHeightForWidth())
         self.prop_result.setSizePolicy(sizePolicy)
         self.prop_result.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_result.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_result.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_result.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_result.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_result.setText("")
-        self.prop_result.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_result.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_result.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_result.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_result.setObjectName("prop_result")
-        self.formLayout.setWidget(10, QtWidgets.QFormLayout.FieldRole, self.prop_result)
-        self.label_16 = QtWidgets.QLabel(self.frame)
+        self.formLayout.setWidget(10, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_result)
+        self.label_16 = QtWidgets.QLabel(parent=self.frame)
         self.label_16.setObjectName("label_16")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.LabelRole, self.label_16)
-        self.prop_modified = QtWidgets.QLabel(self.frame)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.MinimumExpanding, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_16)
+        self.prop_modified = QtWidgets.QLabel(parent=self.frame)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.MinimumExpanding, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.prop_modified.sizePolicy().hasHeightForWidth())
         self.prop_modified.setSizePolicy(sizePolicy)
         self.prop_modified.setMinimumSize(QtCore.QSize(300, 0))
-        self.prop_modified.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.prop_modified.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.prop_modified.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.prop_modified.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.prop_modified.setText("")
-        self.prop_modified.setTextFormat(QtCore.Qt.PlainText)
-        self.prop_modified.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextSelectableByMouse)
+        self.prop_modified.setTextFormat(QtCore.Qt.TextFormat.PlainText)
+        self.prop_modified.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.prop_modified.setObjectName("prop_modified")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.FieldRole, self.prop_modified)
+        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.prop_modified)
         self.horizontalLayout_2.addWidget(self.frame)
         self.horizontalLayout.addWidget(self.url_properties)
-        self.statistics = QtWidgets.QFrame(self.centralwidget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.statistics = QtWidgets.QFrame(parent=self.centralwidget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.statistics.sizePolicy().hasHeightForWidth())
         self.statistics.setSizePolicy(sizePolicy)
         self.statistics.setLineWidth(0)
         self.statistics.setObjectName("statistics")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.statistics)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.groupBox = QtWidgets.QGroupBox(self.statistics)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.groupBox = QtWidgets.QGroupBox(parent=self.statistics)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.groupBox.sizePolicy().hasHeightForWidth())
         self.groupBox.setSizePolicy(sizePolicy)
         font = QtGui.QFont()
         font.setBold(True)
         font.setWeight(75)
         self.groupBox.setFont(font)
         self.groupBox.setObjectName("groupBox")
         self.gridLayout = QtWidgets.QGridLayout(self.groupBox)
         self.gridLayout.setObjectName("gridLayout")
-        self.label_24 = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_24 = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_24.sizePolicy().hasHeightForWidth())
         self.label_24.setSizePolicy(sizePolicy)
-        self.label_24.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_24.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_24.setObjectName("label_24")
         self.gridLayout.addWidget(self.label_24, 0, 0, 1, 1)
-        self.stats_valid_urls = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_valid_urls = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_valid_urls.sizePolicy().hasHeightForWidth())
         self.stats_valid_urls.setSizePolicy(sizePolicy)
         self.stats_valid_urls.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_valid_urls.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_valid_urls.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_valid_urls.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_valid_urls.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_valid_urls.setText("")
-        self.stats_valid_urls.setTextFormat(QtCore.Qt.RichText)
+        self.stats_valid_urls.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_valid_urls.setOpenExternalLinks(True)
         self.stats_valid_urls.setObjectName("stats_valid_urls")
         self.gridLayout.addWidget(self.stats_valid_urls, 0, 1, 1, 1)
-        self.label_26 = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_26 = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_26.sizePolicy().hasHeightForWidth())
         self.label_26.setSizePolicy(sizePolicy)
-        self.label_26.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_26.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_26.setObjectName("label_26")
         self.gridLayout.addWidget(self.label_26, 0, 2, 1, 1)
-        self.stats_warnings = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_warnings = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_warnings.sizePolicy().hasHeightForWidth())
         self.stats_warnings.setSizePolicy(sizePolicy)
         self.stats_warnings.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_warnings.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_warnings.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_warnings.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_warnings.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_warnings.setText("")
-        self.stats_warnings.setTextFormat(QtCore.Qt.RichText)
+        self.stats_warnings.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_warnings.setOpenExternalLinks(True)
         self.stats_warnings.setObjectName("stats_warnings")
         self.gridLayout.addWidget(self.stats_warnings, 0, 3, 1, 1)
-        self.label_25 = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_25 = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_25.sizePolicy().hasHeightForWidth())
         self.label_25.setSizePolicy(sizePolicy)
-        self.label_25.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_25.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_25.setObjectName("label_25")
         self.gridLayout.addWidget(self.label_25, 1, 0, 1, 1)
-        self.stats_invalid_urls = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_invalid_urls = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_invalid_urls.sizePolicy().hasHeightForWidth())
         self.stats_invalid_urls.setSizePolicy(sizePolicy)
         self.stats_invalid_urls.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_invalid_urls.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_invalid_urls.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_invalid_urls.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_invalid_urls.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_invalid_urls.setText("")
-        self.stats_invalid_urls.setTextFormat(QtCore.Qt.RichText)
+        self.stats_invalid_urls.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_invalid_urls.setOpenExternalLinks(True)
         self.stats_invalid_urls.setObjectName("stats_invalid_urls")
         self.gridLayout.addWidget(self.stats_invalid_urls, 1, 1, 1, 1)
         self.verticalLayout_2.addWidget(self.groupBox)
-        self.groupBox_3 = QtWidgets.QGroupBox(self.statistics)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.groupBox_3 = QtWidgets.QGroupBox(parent=self.statistics)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.groupBox_3.sizePolicy().hasHeightForWidth())
         self.groupBox_3.setSizePolicy(sizePolicy)
         self.groupBox_3.setObjectName("groupBox_3")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.groupBox_3)
         self.gridLayout_2.setObjectName("gridLayout_2")
-        self.label_6 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_6 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_6.sizePolicy().hasHeightForWidth())
         self.label_6.setSizePolicy(sizePolicy)
-        self.label_6.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_6.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_6.setObjectName("label_6")
         self.gridLayout_2.addWidget(self.label_6, 0, 0, 1, 1)
-        self.stats_content_image = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_image = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_image.sizePolicy().hasHeightForWidth())
         self.stats_content_image.setSizePolicy(sizePolicy)
         self.stats_content_image.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_image.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_image.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_image.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_image.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_image.setText("")
-        self.stats_content_image.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_image.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_image.setOpenExternalLinks(True)
         self.stats_content_image.setObjectName("stats_content_image")
         self.gridLayout_2.addWidget(self.stats_content_image, 0, 1, 1, 1)
-        self.label_13 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_13 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_13.sizePolicy().hasHeightForWidth())
         self.label_13.setSizePolicy(sizePolicy)
-        self.label_13.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_13.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_13.setObjectName("label_13")
         self.gridLayout_2.addWidget(self.label_13, 0, 2, 1, 1)
-        self.stats_content_text = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_text = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_text.sizePolicy().hasHeightForWidth())
         self.stats_content_text.setSizePolicy(sizePolicy)
         self.stats_content_text.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_text.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_text.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_text.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_text.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_text.setText("")
-        self.stats_content_text.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_text.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_text.setOpenExternalLinks(True)
         self.stats_content_text.setObjectName("stats_content_text")
         self.gridLayout_2.addWidget(self.stats_content_text, 0, 3, 1, 1)
-        self.label_27 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_27 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_27.sizePolicy().hasHeightForWidth())
         self.label_27.setSizePolicy(sizePolicy)
-        self.label_27.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_27.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_27.setObjectName("label_27")
         self.gridLayout_2.addWidget(self.label_27, 0, 4, 1, 1)
-        self.stats_content_application = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_application = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_application.sizePolicy().hasHeightForWidth())
         self.stats_content_application.setSizePolicy(sizePolicy)
         self.stats_content_application.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_application.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_application.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_application.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_application.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_application.setText("")
-        self.stats_content_application.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_application.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_application.setOpenExternalLinks(True)
         self.stats_content_application.setObjectName("stats_content_application")
         self.gridLayout_2.addWidget(self.stats_content_application, 0, 5, 1, 1)
-        self.label_17 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_17 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_17.sizePolicy().hasHeightForWidth())
         self.label_17.setSizePolicy(sizePolicy)
-        self.label_17.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_17.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_17.setObjectName("label_17")
         self.gridLayout_2.addWidget(self.label_17, 1, 0, 1, 1)
-        self.stats_content_audio = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_audio = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_audio.sizePolicy().hasHeightForWidth())
         self.stats_content_audio.setSizePolicy(sizePolicy)
         self.stats_content_audio.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_audio.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_audio.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_audio.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_audio.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_audio.setText("")
-        self.stats_content_audio.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_audio.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_audio.setOpenExternalLinks(True)
         self.stats_content_audio.setObjectName("stats_content_audio")
         self.gridLayout_2.addWidget(self.stats_content_audio, 1, 1, 1, 1)
-        self.label_21 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_21 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_21.sizePolicy().hasHeightForWidth())
         self.label_21.setSizePolicy(sizePolicy)
-        self.label_21.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_21.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_21.setObjectName("label_21")
         self.gridLayout_2.addWidget(self.label_21, 1, 2, 1, 1)
-        self.stats_content_video = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_video = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_video.sizePolicy().hasHeightForWidth())
         self.stats_content_video.setSizePolicy(sizePolicy)
         self.stats_content_video.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_video.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_video.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_video.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_video.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_video.setText("")
-        self.stats_content_video.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_video.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_video.setOpenExternalLinks(True)
         self.stats_content_video.setObjectName("stats_content_video")
         self.gridLayout_2.addWidget(self.stats_content_video, 1, 3, 1, 1)
-        self.stats_content_other = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_other = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_other.sizePolicy().hasHeightForWidth())
         self.stats_content_other.setSizePolicy(sizePolicy)
         self.stats_content_other.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_other.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_other.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_other.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_other.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_other.setText("")
-        self.stats_content_other.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_other.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_other.setOpenExternalLinks(True)
         self.stats_content_other.setObjectName("stats_content_other")
         self.gridLayout_2.addWidget(self.stats_content_other, 2, 5, 1, 1)
-        self.label_23 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_23 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_23.sizePolicy().hasHeightForWidth())
         self.label_23.setSizePolicy(sizePolicy)
-        self.label_23.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_23.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_23.setObjectName("label_23")
         self.gridLayout_2.addWidget(self.label_23, 2, 4, 1, 1)
-        self.stats_content_mail = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_content_mail = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_content_mail.sizePolicy().hasHeightForWidth())
         self.stats_content_mail.setSizePolicy(sizePolicy)
         self.stats_content_mail.setMinimumSize(QtCore.QSize(40, 0))
-        self.stats_content_mail.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_content_mail.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_content_mail.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_content_mail.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_content_mail.setText("")
-        self.stats_content_mail.setTextFormat(QtCore.Qt.RichText)
+        self.stats_content_mail.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_content_mail.setOpenExternalLinks(True)
         self.stats_content_mail.setObjectName("stats_content_mail")
         self.gridLayout_2.addWidget(self.stats_content_mail, 1, 5, 1, 1)
-        self.label_22 = QtWidgets.QLabel(self.groupBox_3)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_22 = QtWidgets.QLabel(parent=self.groupBox_3)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_22.sizePolicy().hasHeightForWidth())
         self.label_22.setSizePolicy(sizePolicy)
-        self.label_22.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_22.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_22.setObjectName("label_22")
         self.gridLayout_2.addWidget(self.label_22, 1, 4, 1, 1)
         self.verticalLayout_2.addWidget(self.groupBox_3)
-        self.groupBox_2 = QtWidgets.QGroupBox(self.statistics)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.groupBox_2 = QtWidgets.QGroupBox(parent=self.statistics)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.groupBox_2.sizePolicy().hasHeightForWidth())
         self.groupBox_2.setSizePolicy(sizePolicy)
         self.groupBox_2.setObjectName("groupBox_2")
         self.gridLayout_3 = QtWidgets.QGridLayout(self.groupBox_2)
         self.gridLayout_3.setObjectName("gridLayout_3")
-        self.label_18 = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_18 = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_18.sizePolicy().hasHeightForWidth())
         self.label_18.setSizePolicy(sizePolicy)
-        self.label_18.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_18.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_18.setObjectName("label_18")
         self.gridLayout_3.addWidget(self.label_18, 0, 0, 1, 1)
-        self.stats_url_minlen = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_url_minlen = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_url_minlen.sizePolicy().hasHeightForWidth())
         self.stats_url_minlen.setSizePolicy(sizePolicy)
         self.stats_url_minlen.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_url_minlen.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_url_minlen.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_url_minlen.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_url_minlen.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_url_minlen.setText("")
-        self.stats_url_minlen.setTextFormat(QtCore.Qt.RichText)
+        self.stats_url_minlen.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_url_minlen.setOpenExternalLinks(True)
         self.stats_url_minlen.setObjectName("stats_url_minlen")
         self.gridLayout_3.addWidget(self.stats_url_minlen, 0, 1, 1, 1)
-        self.label_20 = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_20 = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_20.sizePolicy().hasHeightForWidth())
         self.label_20.setSizePolicy(sizePolicy)
-        self.label_20.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_20.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_20.setObjectName("label_20")
         self.gridLayout_3.addWidget(self.label_20, 0, 2, 1, 1)
-        self.stats_url_avglen = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_url_avglen = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_url_avglen.sizePolicy().hasHeightForWidth())
         self.stats_url_avglen.setSizePolicy(sizePolicy)
         self.stats_url_avglen.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_url_avglen.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_url_avglen.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_url_avglen.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_url_avglen.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_url_avglen.setText("")
-        self.stats_url_avglen.setTextFormat(QtCore.Qt.RichText)
+        self.stats_url_avglen.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_url_avglen.setOpenExternalLinks(True)
         self.stats_url_avglen.setObjectName("stats_url_avglen")
         self.gridLayout_3.addWidget(self.stats_url_avglen, 0, 3, 1, 1)
-        self.label_19 = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.label_19 = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.label_19.sizePolicy().hasHeightForWidth())
         self.label_19.setSizePolicy(sizePolicy)
-        self.label_19.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+        self.label_19.setAlignment(QtCore.Qt.AlignmentFlag.AlignRight|QtCore.Qt.AlignmentFlag.AlignTrailing|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.label_19.setObjectName("label_19")
         self.gridLayout_3.addWidget(self.label_19, 1, 0, 1, 1)
-        self.stats_url_maxlen = QtWidgets.QLabel(self.groupBox_2)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.stats_url_maxlen = QtWidgets.QLabel(parent=self.groupBox_2)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.stats_url_maxlen.sizePolicy().hasHeightForWidth())
         self.stats_url_maxlen.setSizePolicy(sizePolicy)
         self.stats_url_maxlen.setMinimumSize(QtCore.QSize(30, 0))
-        self.stats_url_maxlen.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.stats_url_maxlen.setFrameShadow(QtWidgets.QFrame.Sunken)
+        self.stats_url_maxlen.setFrameShape(QtWidgets.QFrame.Shape.StyledPanel)
+        self.stats_url_maxlen.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.stats_url_maxlen.setText("")
-        self.stats_url_maxlen.setTextFormat(QtCore.Qt.RichText)
+        self.stats_url_maxlen.setTextFormat(QtCore.Qt.TextFormat.RichText)
         self.stats_url_maxlen.setOpenExternalLinks(True)
         self.stats_url_maxlen.setObjectName("stats_url_maxlen")
         self.gridLayout_3.addWidget(self.stats_url_maxlen, 1, 1, 1, 1)
         self.verticalLayout_2.addWidget(self.groupBox_2)
         self.horizontalLayout.addWidget(self.statistics)
         self.verticalLayout.addLayout(self.horizontalLayout)
         MainWindow.setCentralWidget(self.centralwidget)
-        self.menubar = QtWidgets.QMenuBar(MainWindow)
+        self.menubar = QtWidgets.QMenuBar(parent=MainWindow)
         self.menubar.setGeometry(QtCore.QRect(0, 0, 713, 20))
         self.menubar.setObjectName("menubar")
-        self.menuEdit = QtWidgets.QMenu(self.menubar)
+        self.menuEdit = QtWidgets.QMenu(parent=self.menubar)
         self.menuEdit.setObjectName("menuEdit")
-        self.menuFile = QtWidgets.QMenu(self.menubar)
+        self.menuFile = QtWidgets.QMenu(parent=self.menubar)
         self.menuFile.setObjectName("menuFile")
-        self.menuHelp = QtWidgets.QMenu(self.menubar)
+        self.menuHelp = QtWidgets.QMenu(parent=self.menubar)
         self.menuHelp.setObjectName("menuHelp")
         MainWindow.setMenuBar(self.menubar)
-        self.statusBar = QtWidgets.QStatusBar(MainWindow)
+        self.statusBar = QtWidgets.QStatusBar(parent=MainWindow)
         self.statusBar.setObjectName("statusBar")
         MainWindow.setStatusBar(self.statusBar)
-        self.actionAbout = QtWidgets.QAction(MainWindow)
+        self.actionAbout = QtGui.QAction(parent=MainWindow)
         icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap(":/icons/about.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon2.addPixmap(QtGui.QPixmap(":/icons/about.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionAbout.setIcon(icon2)
         self.actionAbout.setObjectName("actionAbout")
-        self.actionHelp = QtWidgets.QAction(MainWindow)
+        self.actionHelp = QtGui.QAction(parent=MainWindow)
         icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap(":/icons/help.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon3.addPixmap(QtGui.QPixmap(":/icons/help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionHelp.setIcon(icon3)
         self.actionHelp.setObjectName("actionHelp")
-        self.actionViewOnline = QtWidgets.QAction(MainWindow)
+        self.actionViewOnline = QtGui.QAction(parent=MainWindow)
         icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap(":/icons/online.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon4.addPixmap(QtGui.QPixmap(":/icons/online.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionViewOnline.setIcon(icon4)
         self.actionViewOnline.setObjectName("actionViewOnline")
-        self.actionOptions = QtWidgets.QAction(MainWindow)
+        self.actionOptions = QtGui.QAction(parent=MainWindow)
         icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap(":/icons/preferences.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon5.addPixmap(QtGui.QPixmap(":/icons/preferences.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionOptions.setIcon(icon5)
         self.actionOptions.setObjectName("actionOptions")
-        self.actionCopyToClipboard = QtWidgets.QAction(MainWindow)
+        self.actionCopyToClipboard = QtGui.QAction(parent=MainWindow)
         icon6 = QtGui.QIcon()
-        icon6.addPixmap(QtGui.QPixmap(":/icons/copy.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon6.addPixmap(QtGui.QPixmap(":/icons/copy.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionCopyToClipboard.setIcon(icon6)
         self.actionCopyToClipboard.setObjectName("actionCopyToClipboard")
-        self.actionViewParentOnline = QtWidgets.QAction(MainWindow)
+        self.actionViewParentOnline = QtGui.QAction(parent=MainWindow)
         self.actionViewParentOnline.setIcon(icon4)
         self.actionViewParentOnline.setObjectName("actionViewParentOnline")
-        self.actionViewParentSource = QtWidgets.QAction(MainWindow)
+        self.actionViewParentSource = QtGui.QAction(parent=MainWindow)
         self.actionViewParentSource.setIcon(icon4)
         self.actionViewParentSource.setObjectName("actionViewParentSource")
-        self.actionDebug = QtWidgets.QAction(MainWindow)
+        self.actionDebug = QtGui.QAction(parent=MainWindow)
         self.actionDebug.setObjectName("actionDebug")
-        self.actionViewProperties = QtWidgets.QAction(MainWindow)
+        self.actionViewProperties = QtGui.QAction(parent=MainWindow)
         self.actionViewProperties.setObjectName("actionViewProperties")
-        self.actionSave = QtWidgets.QAction(MainWindow)
+        self.actionSave = QtGui.QAction(parent=MainWindow)
         icon7 = QtGui.QIcon()
-        icon7.addPixmap(QtGui.QPixmap(":/icons/save.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon7.addPixmap(QtGui.QPixmap(":/icons/save.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionSave.setIcon(icon7)
         self.actionSave.setObjectName("actionSave")
-        self.actionQuit = QtWidgets.QAction(MainWindow)
+        self.actionQuit = QtGui.QAction(parent=MainWindow)
         icon8 = QtGui.QIcon()
-        icon8.addPixmap(QtGui.QPixmap(":/icons/exit.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
+        icon8.addPixmap(QtGui.QPixmap(":/icons/exit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
         self.actionQuit.setIcon(icon8)
         self.actionQuit.setObjectName("actionQuit")
-        self.actionCheckUpdates = QtWidgets.QAction(MainWindow)
+        self.actionCheckUpdates = QtGui.QAction(parent=MainWindow)
         self.actionCheckUpdates.setObjectName("actionCheckUpdates")
-        self.actionDonate = QtWidgets.QAction(MainWindow)
+        self.actionDonate = QtGui.QAction(parent=MainWindow)
         self.actionDonate.setObjectName("actionDonate")
-        self.actionOpen_project = QtWidgets.QAction(MainWindow)
+        self.actionOpen_project = QtGui.QAction(parent=MainWindow)
         self.actionOpen_project.setObjectName("actionOpen_project")
-        self.actionSave_project = QtWidgets.QAction(MainWindow)
+        self.actionSave_project = QtGui.QAction(parent=MainWindow)
         self.actionSave_project.setObjectName("actionSave_project")
         self.menuEdit.addAction(self.actionOptions)
         self.menuFile.addAction(self.actionOpen_project)
         self.menuFile.addAction(self.actionSave_project)
         self.menuFile.addAction(self.actionSave)
         self.menuFile.addAction(self.actionQuit)
         self.menuHelp.addAction(self.actionAbout)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/linkchecker_ui_options.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/linkchecker_ui_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-# -*- coding: utf-8 -*-
-
 # Form implementation generated from reading ui file 'ui/options.ui'
 #
-# Created by: PyQt5 UI code generator 5.14.1
+# Created by: PyQt6 UI code generator 6.4.2
 #
-# WARNING! All changes made in this file will be lost!
+# WARNING: Any manual changes made to this file will be lost when pyuic6 is
+# run again.  Do not edit this file unless you know what you are doing.
 
 
-from PyQt5 import QtCore, QtGui, QtWidgets
+from PyQt6 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Options(object):
     def setupUi(self, Options):
         Options.setObjectName("Options")
         Options.resize(455, 570)
         Options.setMinimumSize(QtCore.QSize(400, 570))
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(Options)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
-        self.groupBox_2 = QtWidgets.QGroupBox(Options)
+        self.groupBox_2 = QtWidgets.QGroupBox(parent=Options)
         self.groupBox_2.setObjectName("groupBox_2")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.groupBox_2)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.widget = QtWidgets.QWidget(self.groupBox_2)
+        self.widget = QtWidgets.QWidget(parent=self.groupBox_2)
         self.widget.setObjectName("widget")
         self.formLayout = QtWidgets.QFormLayout(self.widget)
-        self.formLayout.setFieldGrowthPolicy(QtWidgets.QFormLayout.ExpandingFieldsGrow)
+        self.formLayout.setFieldGrowthPolicy(QtWidgets.QFormLayout.FieldGrowthPolicy.ExpandingFieldsGrow)
         self.formLayout.setObjectName("formLayout")
-        self.label = QtWidgets.QLabel(self.widget)
+        self.label = QtWidgets.QLabel(parent=self.widget)
         self.label.setObjectName("label")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label)
-        self.recursionlevel = QtWidgets.QSpinBox(self.widget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Preferred)
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label)
+        self.recursionlevel = QtWidgets.QSpinBox(parent=self.widget)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.recursionlevel.sizePolicy().hasHeightForWidth())
         self.recursionlevel.setSizePolicy(sizePolicy)
         self.recursionlevel.setMinimumSize(QtCore.QSize(0, 25))
         self.recursionlevel.setMinimum(-1)
         self.recursionlevel.setMaximum(100)
         self.recursionlevel.setProperty("value", -1)
         self.recursionlevel.setObjectName("recursionlevel")
-        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.recursionlevel)
-        self.label_2 = QtWidgets.QLabel(self.widget)
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.recursionlevel)
+        self.label_2 = QtWidgets.QLabel(parent=self.widget)
         self.label_2.setObjectName("label_2")
-        self.formLayout.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_2)
-        self.verbose = QtWidgets.QCheckBox(self.widget)
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_2)
+        self.verbose = QtWidgets.QCheckBox(parent=self.widget)
         self.verbose.setEnabled(True)
         self.verbose.setText("")
         self.verbose.setObjectName("verbose")
-        self.formLayout.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.verbose)
-        self.label_4 = QtWidgets.QLabel(self.widget)
+        self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.verbose)
+        self.label_4 = QtWidgets.QLabel(parent=self.widget)
         self.label_4.setObjectName("label_4")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.LabelRole, self.label_4)
-        self.debug = QtWidgets.QCheckBox(self.widget)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_4)
+        self.debug = QtWidgets.QCheckBox(parent=self.widget)
         self.debug.setText("")
         self.debug.setObjectName("debug")
-        self.formLayout.setWidget(2, QtWidgets.QFormLayout.FieldRole, self.debug)
+        self.formLayout.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.debug)
         self.verticalLayout.addWidget(self.widget)
-        spacerItem = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout.addItem(spacerItem)
-        self.label_5 = QtWidgets.QLabel(self.groupBox_2)
+        self.label_5 = QtWidgets.QLabel(parent=self.groupBox_2)
         self.label_5.setObjectName("label_5")
         self.verticalLayout.addWidget(self.label_5)
-        self.warninglines = QtWidgets.QPlainTextEdit(self.groupBox_2)
+        self.warninglines = QtWidgets.QPlainTextEdit(parent=self.groupBox_2)
         self.warninglines.setMaximumSize(QtCore.QSize(16777215, 150))
         self.warninglines.setObjectName("warninglines")
         self.verticalLayout.addWidget(self.warninglines)
-        self.label_6 = QtWidgets.QLabel(self.groupBox_2)
+        self.label_6 = QtWidgets.QLabel(parent=self.groupBox_2)
         self.label_6.setObjectName("label_6")
         self.verticalLayout.addWidget(self.label_6)
-        self.ignorelines = QtWidgets.QPlainTextEdit(self.groupBox_2)
+        self.ignorelines = QtWidgets.QPlainTextEdit(parent=self.groupBox_2)
         self.ignorelines.setMaximumSize(QtCore.QSize(16777215, 150))
         self.ignorelines.setObjectName("ignorelines")
         self.verticalLayout.addWidget(self.ignorelines)
         self.verticalLayout_3.addWidget(self.groupBox_2)
-        self.groupBox = QtWidgets.QGroupBox(Options)
+        self.groupBox = QtWidgets.QGroupBox(parent=Options)
         self.groupBox.setObjectName("groupBox")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.groupBox)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
-        self.label_3 = QtWidgets.QLabel(self.groupBox)
+        self.label_3 = QtWidgets.QLabel(parent=self.groupBox)
         self.label_3.setWordWrap(True)
         self.label_3.setObjectName("label_3")
         self.verticalLayout_2.addWidget(self.label_3)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem1 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_2.addItem(spacerItem1)
-        self.user_config_filename = QtWidgets.QLabel(self.groupBox)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
+        self.user_config_filename = QtWidgets.QLabel(parent=self.groupBox)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.user_config_filename.sizePolicy().hasHeightForWidth())
         self.user_config_filename.setSizePolicy(sizePolicy)
-        self.user_config_filename.setFrameShape(QtWidgets.QFrame.NoFrame)
+        self.user_config_filename.setFrameShape(QtWidgets.QFrame.Shape.NoFrame)
         self.user_config_filename.setLineWidth(0)
-        self.user_config_filename.setAlignment(QtCore.Qt.AlignLeading|QtCore.Qt.AlignLeft|QtCore.Qt.AlignVCenter)
+        self.user_config_filename.setAlignment(QtCore.Qt.AlignmentFlag.AlignLeading|QtCore.Qt.AlignmentFlag.AlignLeft|QtCore.Qt.AlignmentFlag.AlignVCenter)
         self.user_config_filename.setWordWrap(True)
-        self.user_config_filename.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
+        self.user_config_filename.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.user_config_filename.setObjectName("user_config_filename")
         self.verticalLayout_2.addWidget(self.user_config_filename)
-        self.user_config_button = QtWidgets.QPushButton(self.groupBox)
+        self.user_config_button = QtWidgets.QPushButton(parent=self.groupBox)
         self.user_config_button.setEnabled(False)
         self.user_config_button.setToolTip("")
         self.user_config_button.setObjectName("user_config_button")
         self.verticalLayout_2.addWidget(self.user_config_button)
         self.verticalLayout_3.addWidget(self.groupBox)
-        spacerItem2 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        spacerItem2 = QtWidgets.QSpacerItem(20, 10, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_3.addItem(spacerItem2)
-        self.widget_2 = QtWidgets.QWidget(Options)
+        self.widget_2 = QtWidgets.QWidget(parent=Options)
         self.widget_2.setObjectName("widget_2")
         self.horizontalLayout = QtWidgets.QHBoxLayout(self.widget_2)
         self.horizontalLayout.setObjectName("horizontalLayout")
-        self.closeButton = QtWidgets.QPushButton(self.widget_2)
+        self.closeButton = QtWidgets.QPushButton(parent=self.widget_2)
         self.closeButton.setObjectName("closeButton")
         self.horizontalLayout.addWidget(self.closeButton)
-        spacerItem3 = QtWidgets.QSpacerItem(317, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        spacerItem3 = QtWidgets.QSpacerItem(317, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout.addItem(spacerItem3)
         self.verticalLayout_3.addWidget(self.widget_2)
 
         self.retranslateUi(Options)
         QtCore.QMetaObject.connectSlotsByName(Options)
 
     def retranslateUi(self, Options):
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/logger.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/logger.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/options.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import os
-from PyQt5 import QtWidgets
+from PyQt6 import QtWidgets
 from .linkchecker_ui_options import Ui_Options
 from .editor import EditorWindow
 from .library.fileutil import is_writable
 from linkcheck import configuration
 
 
 class LinkCheckerOptions(QtWidgets.QDialog, Ui_Options):
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/projects.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 import re
 import os
 import shutil
 import urllib.parse
 
-from PyQt5 import QtWidgets
+from PyQt6 import QtWidgets
 from linkcheck.configuration import get_user_config, confparse
 from linkcheck.url import default_ports, splitport
 from linkcheck.fileutil import is_readable
 from .library.fileutil import is_writable
 
 ProjectExt = ".lcp"
 ProjectFilter = _("LinkChecker project (*%(ext)s)") % dict(ext=ProjectExt)
@@ -95,27 +95,26 @@
 
 
 def url_split(url):
     """Split url in a tuple (scheme, hostname, port, document) where
     hostname is always lowercased.
     Precondition: url is syntactically correct URI (eg has no whitespace)
     """
-    scheme, netloc = urllib.parse.splittype(url)
-    host, document = urllib.parse.splithost(netloc)
-    port = default_ports.get(scheme, 0)
-    if host:
+    o = urllib.parse.urlparse(url)
+    port = default_ports.get(o.scheme, 0)
+    if host := o.netloc:
         host = host.lower()
         host, port = splitport(host, port=port)
-    return scheme, host, port, document
+    return o.scheme, host, port, o.path
 
 
 def url_to_filename(url, extension):
     # filter host and document
     parts = url_split(url)
-    value = parts[1] + parts[3]
+    value = f"{'' if parts[1] is None else parts[1]}{parts[3]}"
     # normalize
     import unicodedata
 
     value = unicodedata.normalize('NFKD', value)
     # replace non-alpha characters and convert to lowercase
     value = re.sub(r'[^\w-]+', '_', value).strip().lower()
     # add extension
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/properties.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/properties.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/recentdocs.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/recentdocs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-from PyQt5 import QtCore
+from PyQt6 import QtCore
 
 EmptyQVariant = QtCore.QVariant()
 
 
 class RecentDocumentModel(QtCore.QAbstractListModel):
     """Model class for list of recent documents."""
 
@@ -31,37 +31,37 @@
         """Return number of documents."""
         return len(self.documents)
 
     def index(self, row, column=0, parent=QtCore.QModelIndex()):
         """Return index of document in given row."""
         return self.createIndex(row, column)
 
-    def data(self, index, role=QtCore.Qt.DisplayRole):
+    def data(self, index, role=QtCore.Qt.ItemDataRole.DisplayRole):
         """Return data at given index for given role."""
         V = QtCore.QVariant
         if (
             not index.isValid()
             or not (0 <= index.row() < len(self.documents))
             or index.column() != 0
         ):
             return EmptyQVariant
-        if role == QtCore.Qt.DisplayRole:
+        if role == QtCore.Qt.ItemDataRole.DisplayRole:
             return V(self.documents[index.row()])
         return EmptyQVariant
 
     def headerData(self, section, orientation, role):
         """Return header column data for given parameters."""
         return EmptyQVariant
 
     def flags(self, index):
         """Return flags that given valid item index is enabled and
         selected."""
         if not index.isValid():
             return 0
-        return QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable
+        return QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
 
     def clear(self):
         """Empty the document list."""
         self.beginResetModel()
         self.documents = []
         self.endResetModel()
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/settings.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """Read and store QSettings for this application."""
 
-from PyQt5 import QtCore
+from PyQt6 import QtCore
 
 
 def save_point(qpoint):
     """Ensure positive X and Y values of point."""
     qpoint.setX(max(0, qpoint.x()))
     qpoint.setY(max(0, qpoint.y()))
     return qpoint
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/statistics.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/statistics.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/syntax.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/syntax.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-from PyQt5 import QtCore, QtGui
+from PyQt6 import QtCore, QtGui
 
 
 def format(color, style=''):
     """Return a QTextCharFormat with the given attributes."""
     format = QtGui.QTextCharFormat()
-    format.setForeground(getattr(QtCore.Qt, color))
+    format.setForeground(getattr(QtCore.Qt.GlobalColor, color))
     if 'bold' in style:
-        format.setFontWeight(QtGui.QFont.Bold)
+        format.setFontWeight(QtGui.QFont.Weight.Bold)
     if 'italic' in style:
         format.setFontItalic(True)
     return format
 
 
 class Highlighter(QtGui.QSyntaxHighlighter):
     """Base class for all highlighters."""
@@ -36,26 +36,23 @@
         super().__init__(document)
         self.rules = []
         self.styles = {}
 
     def highlightBlock(self, text):
         """Highlight a text block."""
         for expression, format in self.rules:
-            # get first match
-            index = expression.indexIn(text)
-            while index >= 0:
-                length = expression.matchedLength()
-                self.setFormat(index, length, format)
-                # jump to next match
-                index = expression.indexIn(text, index + length)
+            i = expression.globalMatch(text)
+            while i.hasNext():
+                match = i.next()
+                self.setFormat(match.capturedStart(), match.capturedLength(), format)
         self.setCurrentBlockState(0)
 
     def addRule(self, pattern, style):
         """Add a rule pattern with given style."""
-        self.rules.append((QtCore.QRegExp(pattern), self.styles[style]))
+        self.rules.append((QtCore.QRegularExpression(pattern), self.styles[style]))
 
 
 class XmlHighlighter(Highlighter):
     """XML syntax highlighter."""
 
     def __init__(self, document):
         """Set XML syntax rules."""
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/updater.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-from PyQt5 import QtCore, QtWidgets
+from PyQt6 import QtCore, QtWidgets
 from linkcheck import updater, configuration
 
 
 class UpdateThread(QtCore.QThread):
     """Thread to check for updated versions."""
 
     def reset(self):
@@ -41,15 +41,15 @@
         self.thread = UpdateThread()
         self.thread.finished.connect(self.update)
 
     def reset(self):
         """Reset dialog and restart update check."""
         self.thread.reset()
         self.thread.start()
-        self.setIcon(QtWidgets.QMessageBox.Information)
+        self.setIcon(QtWidgets.QMessageBox.Icon.Information)
         self.setText(_('Checking for updates...'))
 
     def update(self):
         """Display update thread result (which must be available)."""
         result, value = self.thread.result, self.thread.value
         if result:
             if value is None:
@@ -77,14 +77,14 @@
                     currentversion=configuration.Version,
                 )
         else:
             # value is an error message or None if UpdateThread has been
             # terminated
             if value is None:
                 value = _('update thread has been terminated')
-            self.setIcon(QtWidgets.QMessageBox.Warning)
+            self.setIcon(QtWidgets.QMessageBox.Icon.Warning)
             text = _(
                 'An error occured while checking for an '
                 'update of %(app)s: %(error)s.'
             )
             attrs = dict(error=value, app=configuration.AppName)
         self.setText(text % attrs)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/urlmodel.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/urlmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 import operator
-from PyQt5 import QtCore, QtGui
+from PyQt6 import QtCore, QtGui
 from linkcheck import strformat
 
 
 Headers = [_("Parent"), _("URL"), _("Name"), _("Result")]
 EmptyQVariant = QtCore.QVariant()
 
 
@@ -53,24 +53,24 @@
         raise IndexError("invalid index %d" % key)
 
     def init_display(self):
         """Store formatted display texts from URL data."""
         # result
         if self.url_data.valid:
             if self.url_data.warnings:
-                self.result_color = QtCore.Qt.darkYellow
+                self.result_color = QtCore.Qt.GlobalColor.darkYellow
                 text = "\n".join(x[1] for x in self.url_data.warnings)
                 result = "Warning: %s" % strformat.limit(text, length=25)
             else:
-                self.result_color = QtCore.Qt.darkGreen
+                self.result_color = QtCore.Qt.GlobalColor.darkGreen
                 result = "Valid"
                 if self.url_data.result:
                     result += ": %s" % self.url_data.result
         else:
-            self.result_color = QtCore.Qt.darkRed
+            self.result_color = QtCore.Qt.GlobalColor.darkRed
             result = "Error"
             if self.url_data.result:
                 result += ": %s" % self.url_data.result
         # Parent URL
         if self.url_data.parent_url:
             parent = "{}{}{}".format(
                 self.url_data.parent_url,
@@ -132,42 +132,43 @@
         """Return empty QModelIndex since the URL list is not hierarchical."""
         return QtCore.QModelIndex()
 
     def index(self, row, column, parent=QtCore.QModelIndex()):
         """Return index of URL item in given row and column."""
         return self.createIndex(row, column)
 
-    def data(self, index, role=QtCore.Qt.DisplayRole):
+    def data(self, index, role=QtCore.Qt.ItemDataRole.DisplayRole):
         """Return URL item data at given index for given role."""
         V = QtCore.QVariant
         if not index.isValid() or not (0 <= index.row() < len(self.urls)):
             return EmptyQVariant
         urlitem = self.urls[index.row()]
         column = index.column()
-        if role == QtCore.Qt.DisplayRole:
+        if role == QtCore.Qt.ItemDataRole.DisplayRole:
             return V(urlitem.display[column])
-        elif role == QtCore.Qt.ToolTipRole:
+        elif role == QtCore.Qt.ItemDataRole.ToolTipRole:
             return V(urlitem.tooltips[column])
-        elif role == QtCore.Qt.TextColorRole and column == 3:
+        elif role == QtCore.Qt.ItemDataRole.TextColorRole and column == 3:
             return QtGui.QColor(urlitem.result_color)
         else:
             return EmptyQVariant
 
     def headerData(self, section, orientation, role):
         """Return header column data for given parameters."""
-        if orientation == QtCore.Qt.Horizontal and role == QtCore.Qt.DisplayRole:
+        if (orientation == QtCore.Qt.Orientation.Horizontal
+                and role == QtCore.Qt.ItemDataRole.DisplayRole):
             return Headers[section]
         return EmptyQVariant
 
     def flags(self, index):
         """Return flags that given valid item index is enabled and
         selected."""
         if not index.isValid():
             return 0
-        return QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsSelectable
+        return QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
 
     def clear(self):
         """Empty the URL item list."""
         self.beginResetModel()
         self.urls = []
         self.endResetModel()
 
@@ -181,13 +182,13 @@
 
     def getUrlItem(self, index):
         """Get URL item object at given index."""
         if not index.isValid() or not (0 <= index.row() < len(self.urls)):
             return None
         return self.urls[index.row()]
 
-    def sort(self, column, order=QtCore.Qt.AscendingOrder):
+    def sort(self, column, order=QtCore.Qt.SortOrder.AscendingOrder):
         """Sort URL items by given column and order."""
         self.layoutAboutToBeChanged.emit()
-        reverse = order == QtCore.Qt.DescendingOrder
+        reverse = order == QtCore.Qt.SortOrder.DescendingOrder
         self.urls.sort(key=operator.itemgetter(column), reverse=reverse)
         self.layoutChanged.emit()
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/urlsave.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/urlsave.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-from PyQt5 import QtWidgets
+from PyQt6 import QtWidgets
 
 FilterHtml = _("HTML output (*.html)")
 FilterText = _("Text output (*.txt)")
 FilterXml = _("XML output (*.xml)")
 FilterCsv = _("CSV output (*.csv)")
 
 LoggerFilters = (
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/validator.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """Provide custom validators."""
 
-from PyQt5 import QtGui
+from PyQt6 import QtGui
 import re
 
 
 def check_regex(value):
     """Check if given string value can be compiled with re.compile()."""
     try:
         re.compile(value)
@@ -30,13 +30,13 @@
 
 
 class PyRegexValidator(QtGui.QValidator):
     """Validate input that it is a valid Python regular expression."""
 
     def validate(self, input, pos):
         if check_regex(input):
-            return (QtGui.QValidator.Acceptable, pos)
-        return (QtGui.QValidator.Intermediate, pos)
+            return (QtGui.QValidator.State.Acceptable, pos)
+        return (QtGui.QValidator.State.Intermediate, pos)
 
     def fixup(self, input):
         while not check_regex(input):
             input.chop(1)
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/data/help/lccollection.qhc` & `linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lccollection.qhc`

 * *Files 14% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4,25 +4,25 @@
 INSERT INTO NamespaceTable VALUES(1,'linkchecker.app.linkchecker-gui','lcdoc.qch');
 CREATE TABLE FolderTable (Id INTEGER PRIMARY KEY, NamespaceId INTEGER, Name TEXT );
 INSERT INTO FolderTable VALUES(1,1,'doc');
 CREATE TABLE FilterAttributeTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterNameTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterTable (NameId INTEGER, FilterAttributeId INTEGER );
 CREATE TABLE SettingsTable (Key TEXT PRIMARY KEY, Value BLOB );
-INSERT INTO SettingsTable VALUES('LastRegisterTime','2022-12-05T19:35:48.000');
+INSERT INTO SettingsTable VALUES('LastRegisterTime','2023-04-21T18:37:43.000');
 INSERT INTO SettingsTable VALUES('WindowTitle','LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('LastShownPages','qthelp://linkchecker.app.linkchecker-gui/doc/index.html');
 INSERT INTO SettingsTable VALUES('CacheDirectory','linkchecker/LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('CacheDirRelativeToCollection',0);
 INSERT INTO SettingsTable VALUES('EnableFilterFunctionality',0);
 INSERT INTO SettingsTable VALUES('HideFilterFunctionality',1);
 INSERT INTO SettingsTable VALUES('EnableDocumentationManager',0);
 INSERT INTO SettingsTable VALUES('EnableAddressBar',0);
 INSERT INTO SettingsTable VALUES('HideAddressBar',1);
-INSERT INTO SettingsTable VALUES('CreationTime',1670268948);
+INSERT INTO SettingsTable VALUES('CreationTime',1682102263);
 INSERT INTO SettingsTable VALUES('FullTextSearchFallback',0);
 INSERT INTO SettingsTable VALUES('ApplicationIcon',X'89504e470d0a1a0a0000000d49484452000000100000001008060000001ff3ff6100000006624b474400ff00ff00ffa0bda79300000009704859730000375c0000375c01cbc7a4b9000003af4944415438cb05c15b681c550006e0ff9c33979dd95b92cd65d324dd6ed2b4696252a4d634a285168b979712a1166c51fba214aa0f8a102df8526b0b62147c284aa95044a9a4e08bb7b41830921242adb59590d0682fc9ee26d9cbccecccececccec397e1f99fc6206aa2aa152ae92030787c8537bb7f2b3677ede5628d7f6d782c68e5cdec2ed3bb9e5c0adff162aea6aac4923a11f824a544000d2d2721194803c582c886ac5ef9899593e1b694b1ccd6c69893edab0452eef40ed6c26ccad5b81eb5fae6e981f1a6bc54aefe3bd448d4882ed1a3c4cec9223ea10bd03bb7ba6b5eed421afbd455a63b2c88754747626851c8b408b451489d151cae86116517f322a6e85324a089005b0553bfdd107b3ed035d7bc25434686a92250846fe7e688ab575078a1790dc83a2084c37ac976cd9339c9b3a0f9f093c5e6327dfb9846ddb87decd0cf5bc6ac309e6af7c2eafcdfd8a1e6e92375f1c251d1a274b7913d53a8161d598ef8741e885dd1cb00d2ffc835e987c497605394e34051b2e6785643f6e4507c8955bf7a14a0cfbba2278b6b584ed6995c4123a882cb1788b8e7447e2f58dbca9b378e7e921b92936c1a3aa54957544fb4648ac6f042f8f0d81afdfc3f1b72670fbcf058c3f9186132a585aade3e9914ee2397eb262793fb0fee1f111aa2b272c50114f28786408f264ab8ce75265bc71ee22ea7d8750d7bab070ed2a0c9780c632304a16ca25872574794a8a4615cff242d09a07d751301abd86533bbbf1f1e5ff80fee7b1b5f731d44c0b1b0d1d7a2285a46028e6eb500114cbae47635a6485f0b058b508d1cc799cdb7b01851b27706335444b5b2faa850202db81de9c056551e83290d415e238fea6697a2bf4e6663ccfa8f2bbe217f1de9e2fb9d4d8c467d37de0b111f8a601df09601b35488127ba9a15908668944a36bc7a38abb5c6f3d4bcd384bbff463f39357615633b73e49b69ce57c4313469ba08ac1ae44603d9942632299d1472267fb85a2101879064f6a92e5348f7bf7e01f9a2e81bded58ebfeedaf86afe2051fb86797794139b521151181cd3c1e2aad988e82ab8aa301af0f7a5a43e8706a774bdc407b3d98e49b7e6e1e28fca9a9f7ea51c4d3753574f20d9dd4e0ca6923c224864b730b525e1534adfceee1f3aaf690ac9f4a739dbb73b7eb4bd991c9959a8d8672e85af8535e93bdb323265bbde52a8380ae7752e372cd3df5c99b5efcd9d54d2fddf57560a3477fd5b6198040448d22307cc09cb01ff651ee7e33a3aec1ad20474871c4975060d3444505c05c422082bb40d8ebb9bff4c8500706c4ae07f702bc1c500e2ed86000000227a545874536f667477617265000078da2b2f2fd7cbcccb2e4e4e2c48d5cb2f4a070036d806581053ca5c0000000049454e44ae426082');
 CREATE TABLE FileNameTable (FolderId INTEGER, Name TEXT, FileId INTEGER PRIMARY KEY, Title TEXT);
 INSERT INTO FileNameTable VALUES(1,'index.html',1,'Check websites for broken links');
 INSERT INTO FileNameTable VALUES(1,'pygments.css',2,'pygments.css');
 INSERT INTO FileNameTable VALUES(1,'sphinxdoc.css',3,'sphinxdoc.css');
 INSERT INTO FileNameTable VALUES(1,'logo/64x64/linkchecker-gui.png',4,'linkchecker-gui.png');
@@ -31,11 +31,18 @@
 INSERT INTO ContentsTable VALUES(1,1,X'00000000000000140069006e006400650078002e00680074006d006c00000032004c0069006e006b0043006800650063006b0065007200200064006f00630075006d0065006e0074006100740069006f006e');
 CREATE TABLE FileFilterTable (FilterAttributeId INTEGER, FileId INTEGER);
 CREATE TABLE IndexFilterTable (FilterAttributeId INTEGER, IndexId INTEGER);
 CREATE TABLE ContentsFilterTable (FilterAttributeId INTEGER, ContentsId INTEGER );
 CREATE TABLE FileAttributeSetTable (NamespaceId INTEGER, FilterAttributeSetId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE OptimizedFilterTable (NamespaceId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE TimeStampTable (NamespaceId INTEGER, FolderId INTEGER, FilePath TEXT, Size INTEGER, TimeStamp TEXT);
-INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2022-12-05T19:37:50');
+INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2023-04-21T18:37:43');
 CREATE TABLE VersionTable (NamespaceId INTEGER, Version TEXT);
 INSERT INTO VersionTable VALUES(1,NULL);
+CREATE TABLE Filter (FilterId INTEGER PRIMARY KEY, Name TEXT);
+CREATE TABLE ComponentTable (ComponentId INTEGER PRIMARY KEY, Name TEXT);
+INSERT INTO ComponentTable VALUES(1,'doc');
+CREATE TABLE ComponentMapping (ComponentId INTEGER, NamespaceId INTEGER);
+INSERT INTO ComponentMapping VALUES(1,1);
+CREATE TABLE ComponentFilter (ComponentName TEXT, FilterId INTEGER);
+CREATE TABLE VersionFilter (Version TEXT, FilterId INTEGER);
 COMMIT;
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/data/help/lcdoc.qch` & `linkchecker_gui-10.0.0a3/linkcheck_gui/data/help/lcdoc.qch`

 * *Files 10% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -9,15 +9,15 @@
 CREATE TABLE IndexFilterTable (FilterAttributeId INTEGER, IndexId INTEGER );
 CREATE TABLE ContentsTable (Id INTEGER PRIMARY KEY, NamespaceId INTEGER, Data BLOB );
 INSERT INTO ContentsTable VALUES(1,1,X'00000000000000140069006e006400650078002e00680074006d006c00000032004c0069006e006b0043006800650063006b0065007200200064006f00630075006d0065006e0074006100740069006f006e');
 CREATE TABLE ContentsFilterTable (FilterAttributeId INTEGER, ContentsId INTEGER );
 CREATE TABLE FileAttributeSetTable (Id INTEGER, FilterAttributeId INTEGER );
 CREATE TABLE FileDataTable (Id INTEGER PRIMARY KEY, Data BLOB );
 INSERT INTO FileDataTable VALUES(1,NULL);
-INSERT INTO FileDataTable VALUES(2,X'000020fb789ca55a6b731bb715fdbebf02e5878cdda1b8969ca48d4d716acb4ea2567e8c25c7c99776c05d9044b45c6c00ac48a6ed7fefb917c03e28d9d34e673c1a7217b8b8cf73ee053dffc3ab771737bfbc7f2d367e5b89f71f5f5e5d5e88c9499e7f7a7a91e7af6e5e899f7fbc7973254e674fc48d95b5d35e9b5a5679fefaed241362b2f1be7996e7bbdd6eb67b3a33769ddf7cc8f724ed94b6c78f277eb07756fa72b2c8b2399fb9df56b53b7f40cee977df7d17b663b110f38d92257dc0c7adf252d08e13f55babefce2717a6f6aaf6273787464d4411be9d4fbcdafb9c243c17c5465aa7fc79eb57277f9e883c480ae2bcf6955a5c6c54712b766a093d95132b63c5d29a5b558b4ad7b76e9e8765610b3d125655e713e70f95721ba5fc446cac5ae149b3d1f5be34c5ac706e223c748aaaf0f7fcbf10d11cd65b58e03e2b61ce7b8edf2c32bd5d8b7f8aa5b1a5b2cfc493e7e2dfd93ce7b570380ecd9317e74b531e20a7d47782df9f4f96b2b85d5bd3d6e549612a83fdbb0d5cf15c90fc1359e975fd4c546ae59f8b4696a5aed7cfc4e993661fff7c13ff408bb9974b6817d4389f3c992ce6dee2d4b92f1773a888f39d2dce2795599bfcdbaff7df7e9d93370a8a80b227eb56cf9a7a3d190810b2423cafb0e8222c123f7cbc9ce40b44a54c8237a78bc102987a1a5fe3afa58fa4147d83cd9c7ea78b57a668c9d192329377d0f3b3c54be974215a27d70a4fcfe869b3b831823514527cfc7085acb855622e63c406f9abf672db548a9378b2f8cc8b792e112d2fb413aa36ed7a23bcc9289c625e98522d06fe10477be739af10a6167ea390eddbadac4bca52258c1d0af9cc461d36c28342364da50b367f266e36d066a7ab2ada894519a463b757a2345b898d6615653f6c573ac2aaa2b54edfa9ea30132f20916b286b8cae3d124798d63b5d2a1247aa44e1d22a04da453fab928bf00e99576a0f3997ec2e5a0041ce69ca319f828290a068add90ac4873256ac7445de01eeb870e60a2e531cbb065e257f3d17191dcf2b6bb95562db3a8f8094e4a360e7ac723e59456ea6f58df4142f91f6666e63daaa144b85bd5e5955261fd3614bb34f761ebb7c9e3721b7ae4c212b96e54421ebe005888b8e988977b5f8586b08b2e2ddf5cfc21d9c575bc742dd0109bccfe09aa03149416472d232f726df1e727a3423208c96b0bc4fba2ecd6e2803eecd46322efef565299f3680c75223dade580ddd298251e7692611775d17555b5228d936ceae815d9d03def53959541a5ee4af4199d7087f0a01aab5151be9045c6e7d81340a486dcced56dadb8c8f9989eff12ca6a5d02bf183316b7cbad8203f142591ae9d877ad092ce81d251b14c8613a0803d2012b4246a71593b65fd91a8742e9b9774046c169b8cc2084b5b07095d96924bc02a3b88eaf6bae40500cdbb86f2c20d40a7af702ef0e81c13d6b1bfcb0862aacc62d68d50c9218e033499adb5dfb4cb9936c3a7390e18ad0abc3b78f2e8f4b1c0a21669da302cca451fbdcbe3e84d436d98aa323baebd81bef24eea8ab0f859dcdf5640e54a2f20e843c20d51aac66fba0302390f50853dc9a022da86fcbbc6e33aec9a652f44add628b124473c52eb598ce3c9698cd3e31074553359e97aa56bd05d3a2456e71c5ee9b4fb49d9a5718ad0ab697d6ffd4aa0b5980ad019ab95d08b2069265ea9956c2b862ea8496b4c0dfd95b5c63a86949db4359ce4ee1ff84a2ddb7577ce7b0bf474b0080fd71145a107618d84068db4d25326535987241431099d826f76087c2cef1f55d58893afd6a0f2eb0d1697e19c50d50f6b81bad81ad44424c54e25130a7bf8361865b98d72c4adc0df22982a45d96e9b00b83b020ff6156cc99c378d230e528325517daa64247f194d38ceee98d12893514a0f3f2f2bb3448e03346dee0aab1bef72895ef4f0bbfa0754a71367cd61b2006f288be70895a91c2779c6b418125844a0e70886e25eb5152350a9909606c4f240183f8500c31996e23c407d244c0a3fe194ac0f691197ca8abab1c425b1ad4d5c12b32c4396cdc4f56053a22022bb44747da97e44fefa4d48c68049a43d95343181f47c0c91b1237cc3bb2d1dc8d93ae5a51156b3494825f60e6d6754de9a3b55c6449a1059c555efac2c10cf173df7059169e97d9f5dae6b43367115f5da13cb6fa52f36f48adc10eadeaa755b4952aeb1ca39c69ac4359a24c11f947fb5f11df7641f43f4e0f702c84e36135d53ffe452a0697d4f57a1e753e8552a271e69354b4ef83b3df2e65932e7f1d09e9cf08dd11d63ca4aaf5b1b1c10282301fd6b89726d891728e915280fa9518c3650f60b59dec9baa0f04648454cb25445e4718845fcf1858be97eb5fccf5c608bfb6c608b47dfdce3832c31916318a4e84425bfc01429b58f1cd3953e1c0163438f81a2a30e8f7bb6524bc2d2be438878d631e8b865c361d143f5fdae6240c0ef95a59cc7916ce98089a98be5f4dbc83bee3b1be960a840c2551af024017fb18d02f07990d00a71187657a1dc689b72d3ae3d44f9fcd6aa3676bbf0440d4b614217d4d040f72f5277ce79ca0d8022485b2a6a40c1b7b3fbb4fae3cdcdfbc8968f06ed7b347f3a68e95d7af8b80b59b0239d4f65670695c7a291b677d1d6f094bac60ce6c032b805265a4ceaf00ab5b2640dea9123da3505a155a07e0c11cb5092540a39f96a8721902404c18873aa6beeac8039b2f5e805f5ef9c3c19b30a34050a2022b30c01459a22d1903c8c4e11eb1e1133b5e8b661ac78fa04dd8d76ae553d1e238015b5e4c406c1c87e03f880da4602cc5a9cedf7017799d1fb54a71e94365e07cf87885f5f5f31dae815e120f7a2095ce45a525bca63573076639ca7b104a3cf8a2c2f0d4e264862049cf6ba3a92d3507b107bea11940e878b4783fefe7ea4138e4ef14196dc17713106620815098e232ac6813c99219edde22c8d028734a8756be0cae0325663c424a2ad938069569bfa44edd3c4c6b4aa0b15957fd0cb71caf30177faf9838fe89b3972211438f092862e8358e3e895a13a7ce1c5cf1f4f076d26b3b08c63651a178673ccc8e76f4008e38a1b53c4d0e9f18d883742ce54778af959e29163c267ce01f697c46e1870b2cb30cc8e9e8b151313a5d96e63a025ef6655e9cd2ce3a9887866bc6ddcaafb4dd74944eb529f6e22a05ca4db814e4200b829461a1a8c7942b6449c706be806256108e3f65f840321cf7a675d610ce21e1e2fdffc2c5ebdbda6a8a1e81dc7ac36f4343ca1ace296689a71b20b19db8881b8a09c0eee89ad1204b0c1544fb0ac283013d0deeb3728eb1e586759d81c9631db6ef49a9216a701613ce8475b8276d6ab973f924b42a7c3b66e589949cb1b9408020cd0d4abc3c8957c2c3df8e9c3f7bfa4d12f65af25c0c8e87ea0763b6503a4b0104d001245f427323cd634db9874788e288e32f5fb636a58f5ccf0780466fdca71c6f418762f53826f1363b846154155f2d87d7780d075dd7b208020f7449443890ce29010c6aa8c5f77771f1261396c4deb3a6af3fd5a31a493a3f57fe95b8123a50a60fc5a8d49afc3b9611eeb80dd0920a2116fafae6fba307e2e0637aaaa951f87c1f3b387f022662c3be51e5352ddb292d3e8cea07864942034f1354d01563f045f6fdf1e6745ad76eeb861700f3dac6bdf7c41e97426bb769c1e41453e3a28c8692f059d22e866baa1fb4d208ba6590282ba7c9a0efb82aed508d7819c7841dc3d333fd6ae6d1a633df7f6036b7f957732cc89bd79ca17b38145c8cca3dd4183884ca9fe018a18d1816201a8c45b2356ad652aec66dfa4f9569683492d5efd84ebd744040484eb5aff4e3693e0631ddc68e40f93e3ff3d3177cff3f4b6ad6f6bb3ab5b5bf1d83cfacaa38033ad8dbc1dea758b8a876f0c0df2dd10bbe574fd2b9c7dcdce0e263c3c3c7d4854deb7e42f03c150ffab6afa416274438430987057cfe941e3a927e7572b72b7c3bc6e659521074b1d8614113c9ebe8f9a09f624dd03f02f2b473077135b79be3d86ef43d3334092a3f75dfb11efdca1b30d1d6abc2e758326649abd4c1785a9877b87b15e4ed31d2490f95aaea4d568574677b135dd0164e99a375d19bfb9169f0828822ce0077f4b73d2fb0320fde919c255b6688f8657a5343a1d10d628895950c6fe907e7340e2c571b944c6da706333eaac862d2c4d5199646434756faea01b989ac23ced67b778f1d1edada865a0593ca37d8f39bcd470a281df06648112d449f68ebe1f8c243505c52ac2a5bb4158f0af751870abc0d085742a537b26f9a155a97dc3a35807fd3dc2d1b95bb9d7db76dbb7a5a2a26ba3a043741e9da04a1a94c2ef1d69365665d6914abcc93ce9e49cb09c34f48e7f12e281381061b73e0be7d2189ede1b1a676cf829eac1919c6ec2d43dd5c949350dc08440cb43e2da81e197beb78f0717969f6e65c24f69e8063a9f5360ace18ce3fbbea1c161d70980e60bb61e99923d60ca382c1f0c1a57275eef517c6cda7b6bbc294c0c8ca4466738058404e234cbd2e03afec9abb325c2071c83d4aa5ae9d3bd55a02497593e7be6d30f56640b72d6861b2eca332926b509c74c6281d3c576c476ae1cfa551784524a2f873d0683e45be3e30047c7563c0bd221d4cdf5f35a1f569ac5c2054e448830f7f4b3dd9423f92b7b46b876e9b873b94d4102dca83ddd18fd7174bb32dfd8f4cb37fde65c54a8d6f3c9ca403b3b092f84f8aa30cde1b9b8c05f8bcedb8bb327a76727f8f3ad78092ad2a0b6bf550a91d6a5dc4ee9ed9ff0f6ec4c0c7f197ec1f7019891f8b0f06b2f7d88bf78f37f085864ff0177e656a5');
+INSERT INTO FileDataTable VALUES(2,X'000020fb789ca55a6b731bb715fdbebf02e5878cdda1b8969da48d4d716a4b4ea2567e8c25c7c99776c05d9044b45c6c00ac48a6ed7fefb917c03e28d9d34e673c1a7217b8b8cf73ee053dffc3c5bbf39b5fdebf161bbfadc4fb8fafae2ecfc5e424cf3f3d3bcff38b9b0bf1f38f376faec4e9ec89b8b1b276da6b53cb2acf5fbf9d64424c36de37cff37cb7dbcd76cf66c6aef39b0ff99ea49dd2f6f8f1c40ff6ce4a5f4e165936e733f7dbaa76670fc839fdeebbefc2762c1662be51b2a40ff8b8555e0ada71a27e6bf5ddd9e4dcd45ed5fee4e6d0a88928c2b7b389577b9f938417a2d848eb943f6bfdeae4cf13910749419cd7be528bf38d2a6ec54e2da1a7726265ac585a73ab6a51e9fad6cdf3b02c6ca147c2aaea6ce2fca1526ea3949f888d552b3c6936bade97a69815ce4d84874e5115fe9eff17229ac37a0b0bdc6725cc79cff19b45a6b76bf14fb134b654f6b978f242fc3b9be7bc160ec7a179f2e27c69ca03e494fa4ef0fbb3c95216b76b6bdaba3c294c65b07fb7812b5e08927f222bbdae9f8b4aadfc0bd1c8b2d4f5fab9387dd2ece39f6fe21f6831f77209ed821a67932793c5dc5b9c3af7e5620e1571beb3c5d9a4326b937ffbf5fedbaf73f246411150f664ddea5953af270301425688e715169d8745e2878f97937c81a89449f0e674315800534fe36bfcb5f49194a26fb099d3ef7471618a961c2d293379073d7fba78259d2e44ebe45ae1e9537ada2c6e8c600d85141f3f5c212b6e9598cb18b141feaabddc3695e2249e2c3ef3629e4b44cb0bed84aa4dbbde086f320aa79817a6548b813fc4d1de79ce2b84a985df2864fb762beb92b254096387423eb351878df0a0904d53e982cd9f899b0db4d9e9aa8a76625106e9d8ed9528cd5662a35945d90fdb958eb0aa68add377aa3accc44b48e41aca1aa36b8fc411a6f54e978ac4912a51b8b40a8176d1cfaae422bc43e695da43ce25bb8b164090739a72cca7a02024285a6bb602f1a18c152b5d9177803b2e9cb982cb14c7ae8157c95f2f4446c7f3ca5a6e95d8b6ce232025f928d839ab9c4f56919b697d233dc54ba4bd99db98b62ac55261af575695c9c774d8d2ec939dc72e9fe74dc8ad2b53c88a653951c83a7801e2a22366e25d2d3ed61a82ac7877fdb37007e7d5d6b150774002ef33b826684c5210999cb4ccbdc9b7879c1ecd0808a3252cef93ae4bb31bca807bb3918cf37f7d59caa70de0b1d488b6375643778a60d4799a49c45dd745d596144ab68db36b6057e780777d4e16958617f96b50e635c29f42806a6dc5463a01975b5f208d02521b73bb95f636e36366e27b3c8b6929f44afc60cc1a9fce37c80f4549a46be7a11eb4a473a074542c93e10428600f88042d895a5cd64e597f242a9dcbe6251d019bc526a330c2d2d6414297a5e412b0ca0ea2babd2e790140f3aea1bc7003d0e92b9c0b3c3ac78475ecef3282982ab3987523547288e3004d666bed37ed72a6cdf0698e0346ab02ef0e9e3c3a7d2cb0a8459a360c8b72d147eff2387ad3501ba6aacc8e6b6fa0afbc93ba222c7e1ef7b71550b9d20b08fa90704394aaf19bee8040ce0354614f32a888b621ffaef1b80ebb66d94b51ab354a2cc9118fd47a16e378721ae3f438045dd54c56ba5ee91a74970e89d53987573aed7e5276699c22f46a5adf5bbf12682da60274c66a25f422489a890bb5926dc5d00535698da9a1bfb2d658c790b293b68693dcfd032fd4b25d77e7bcb7404f078bf0701d51147a10d64868d0482b3d6532957548421193d029f86687c0c7f2fe51558d38f96a0d2abfde607119ce0955fdb016a88bad414d4452ec5432a1b0876f835196db2847dc0afc2d82a95294edb60980bb23f0605fc196cc79d338e220355812d5a74a46f297d184e3ec8e198d3219a5f4f0f3b2324be43840d3e6aeb0baf12e97e8450fbfab7f40753a71d61c260bf086b2788e5099ca7192674c8b218145047a8e6028ee555b3102950a6969402c0f84f15308309c6129ce03d447c2a4f0134ec9fa901671a9aca81b4b5c12dbdac42531cb3264d94c5c0f36250a22b24b44d797ea47e4afdf84640c9844da5349131348cfc710193bc237bcdbd2819cad535e1a61359b845462efd07646e5adb953654ca40991555cf5ceca02f17cd9735f109996def7d9e5ba3664135751af3db1fc56fa6243afc80da1eead5ab79524e51aab9c63ac495ca34912fc41f9571bdf714ff631440f7e2f80ec6433d135f54f2e059ad6f774157a3e855ea572e29156b3e484bfd3236f9e27731e0fedc909df18dd31a6acf4bab5c101813212d0bf9628d7967881925e81f2901ac5680365bf90e59dac0b0a6f8454c4244b55441e8758c41f5fb898ee57cbffcc05b6b8cf06b678f4cd3d3ec812133986418a4e54f20b4c9152fbc8315de9c3113036f418283aeaf0b8672bb5242ced3b8488671d838e5b361c163d54dfef2a0604fc5e59ca791cc9960e9898ba584ebf8dbce3beb3910e860a245ca5014f12f017db28009f0709ad1087617715ca8db62937edda4394cf6fad6a63b70b4fd4b0142674410d0d74ff2275e79ca7dc002882b4a5a206147c3bbb4fab3fdedcbc8f6cf968d0be47f3a78396dea5878fbb90053bd2f954766650792c1a697b176d0d4fa96bcc600e2c835b60a2c5a40eaf502b4bd6a01e39a25d53105a05eac710b10c2549a59093af7618024942108c38a7bae6ce0a98235b8f5e50ffcec99331ab4053a0002232cb1050a429120dc9c3e814b1ee1131538b6e1bc68a674fd0dd68e75ad5e3310258514b4e6c108cec37800fa86d24c0acc5d3fd3ee02e337a9fead483d2c6ebe0f910f1ebeb2b461bbd221ce45e34818b5c4b6a4b79ec0ac66e8cf3349660f45991e5a5c1c904498c80d35e5747721a6a0f624f3d82d2e170f168d0dfdf8f74c2d1293ec892fb222ec6400ca122c17144c538902733c4b35b9ca551e09006b56e0d5c195cc66a8c9844b4751230cd6a539fa87d9ad8985675a1a2f20f7a394e793ee04e3f7ff0117d33472e8402075ed2d065106b1cbd3254872fbcf8f9e3e9a0cd64169671ac4ce3c2708e19f9fc0d08615c71638a183a3dbe11f146c899ea4e313f4b3c724cf8cc39c0fe92d80d034e761986d9d173b16262a234db6d0cb4e4ddac2abd99653c1511cf8cb78d5b75bfe93a89685dead34d0494f3743bd049080037c5484383314fc89688136e0ddda0240c61dcfe8b7020e459efac2b8c41dcc3e3e59b9fc5c5db6b8a1a8ade71cc6a434fc313ca2a6e89a61927bb90b18d18880bcae9e09ed82a41001b4cf504cb8a023301edbd7e83b2ee81759685cd6119b3ed46af2969711a10c6837eb4256867bd7af923b924743a6ceb869599b4bc418920c0004dbd3a8c5cc9c7d2839f3e7cff4b1afd52f65a028c8cee076ab75336400a0bd1042051447f22c3634db38d4987e788e22853bf3fa68655cf0c8f4760d6af1c674c8f61f73225f83631866b541154258fdd7707085dd7bd070208724f443994c8200e0961accaf87577f7211196c3d6b4aea336dfaf15433a395aff97be153852aa00c6afd598f43a9c1be6b10ed89d00221af1f6eafaa60be3e76270a3aa5af971183c3f7b082f62c6b253ee3125d52d2b398dee0c8a47460942135fd31460f543f0f5f6ed7156d46ae78e1b06f7d0c3baf6cd17944e67b26bc7e91154e4a383829cf652d029826ea61bbadf04b2689a2520a8cba7e9b02fe85a8d701dc88917c4dd33f363eddaa631d6736f3fb0f6577927c39cd89ba77c311b5884cc3cda1d3488c894ea1fa088111d2816804abc3562d55aa6c26ef64d9a6f653998d4e2d54fb87e4d444040b8aef5ef6433093ed6c18d46fe3039fedf1373f73c4f6fdbfab636bbbab5158fcda3af3c0a38d3dac8dba15eb7a878f8c6d020df0db15b4ed7bfc2d9d7ecec60c2c3c3d38744e57d4bfe2a100cf5bfaaa61f2446374408830977f59c1e349e7a727eb522773bcceb56561972b0d4614811c1e3e9fba899604fd23d00ffb272047337b195e7db63f83e343d0324397adfb51ff1ce1d3adbd0a1c6eb52376842a6d9ab7451987ab87718ebe534dd410299afe54a5a8d766574175bd31d4096ae79d395f19b6bf1898022c8027ef0b73427bd3f00d29f3d45b8ca16edd1f0aa9446a703c21a25310bcad81fd26f0e48bc382e97c8581b6e6c469dd5b085a5292a938c8ca6eecd157403535398a7fdec162f3ebabd15b50c348b67b4ef3187971a4e34f0db802c50823ac9ded1f78391a4a6a05845b87437080bfeb50e036e1518ba904e656acf243fb42ab56f7814eba0bf47383a772bf77adb6efbb65454746d147488cea31354498352f8bd23cdc6aacc3a52893799279d9c13969386def14f423c100722ecd667e15c1ac3d37b43e38c0d3f453d3892d34d98baa73a39a9a60198106879485c3b30fcd2f7f6f1e0c2f2d3ad4cf8290ddd40e7730a8c359c717cdf373438ec3a01d07cc1d62353b2074c1987e58341e3eac4eb3d8a8f4d7b6f8d3785898191d4e80ca78090409c66591a5cc73f7975b644f88063905a552b7dbab70a94e432cb67cf7cfac18a6c41ceda70c3457926c5a436e198492c70bad88ed8ce9543bfea82504ae9e5b0c760907c6b7c1ce0e8d88a67413a84bab97e5eebc34ab358b8c0890811e69e7eb69b72247f65cf08d72e1d772eb72948801bb5a71ba33f8e6e57e61b9b7ef9a6df9c8b0ad57a365919686727e185105f15a639bc10e7f86bd1797bf1f4c9e9d313fcf956bc02156950dbdf2a8548eb526ea7f4f64f78fbf49918fe32fc92ef033023f161e1d75efa107ff1e6ff10b0c8fe03781a56a6');
 INSERT INTO FileDataTable VALUES(3,X'00000c98789c9d56cb6ee23014ddf72b22cdae525303e5d559b53cda6a3aa52a68ba769c4b62e1d891ed50d068fe7d0c4ec001c284093b74ce7d9e7baffd9831efb71760b288a4c87878430413f2defb36371f21de9f2b9f1840f1ef1deaa13efaeecd05d7374aaf19dc7b5463460dd2bbbdf6062249806beffaf6ca072937a6850cc1501be9ca5382d1d0fb361e23f359c2484a21b7f085e306a12e6a166ebe8046b1be37965868493f60fd65cc6e69c2a175b69fc54c529058e7b64972790efecf8c69ca28076b223d8aaf0c7f97904a412cb8f11ffea694472c77a64ef04f3709cd0fe298a64028665b3b51e8d87940fbb23f010749893f04061a6c252330e0aa200bc22849638b968e69b7a33be4aeb3515c2a1d32f954b6b6603f030e4d3d2c9f96f80f47ae5eb802b94bc355440b6d7e65f424d36966251ab94d259d7688faff8cec5d8a24cde9aaa858357caaa528f2c81c6fbd7a75986641ec9642974a71878607c9cd2426b0518a9d2972f150f903c195c6f90c2fc2cb0d0c81306c668f0a6e6df0cb6dbce104546a52b116aa66af80bf2bc84261b1f2726f1f60f4b3ccf5b3704bdc377474e06cb64e6d58ee52699a66b673e02bd566f730ff2d4b02b023509ee72ec20750a392a2c51c57603735f11fb4410699b611f0a0a2305bec6346cd06b34de0252540ef2e685796654b1e30ac94a596562cc261d87671ae5cb82b97f6f63befc56845ecd73477073d34e456f73c7dc435d56bcb8573a518ad08a43b45f2b98bed347b5d70b0e38c933d9495cc368de1f321bde200ecf2e5fcc2929745cff56190adf3f419ce05b4748841d041a57efdc292e220bf33e2abfeb01407d5ff2c4eef57c9cfe6b3c819acb4ff191b69efb349e6b586c51f3381ad9692b81ee31956164febe15fb886281fcb44d4e34c888d4905b5e6d87f340b58d37c092b528f348871be2cc22342f5ebe1c0c8307f81a8663da7439115625050e5f6580c0756468ae07c29aab89ee367901016c1baaddb30c2fa096fda295361474ead8eeef949d244c7c56276cf45b3d56ef57a27191f46335667aa512f41e739a7dcf5df6e74fb8dd34ea6eb24c83309aa4e9ebbd9ddbbb72475a6de59ebcba816e18989207f4d2e692dc6cbf620e4734fd94553e9bfdac7d25f514cd23c');
 INSERT INTO FileDataTable VALUES(4,X'00001506789cd5575973db36107ed7af40e3e9b8f1888c78c83afc525bb6f2d24e3bcd347d8648484403022c08f98827fded0508122240d04edaa74aa303cbc59edf2e16ef2e2e26e0027ca80a4c1f412d9e08aa0b840408025037c49c654014a8448aefefaf78493ec5fa0bc7074c21214f20e3080a9483dd13b8e625a6e037466156200ef68c833f10fff4191d0f53007358b57cef11e30770c321cd4928c5bd9b4c7ec465c5b800474e7e78b38335cec2acaedfbcbd9a4cde5d287b2b784080c0277654e6ffeb57a36cc7f227f03c01f2b56754047b5862f2b406e73f1d339c43f05e5986cea786f001d21afc4e71c634f93da2e81e9e4f1b11d6ebfc23e239a4f219a8e5a6a0461cefaf4eaa6afc19ad4194568f9a48901088077505334c0f6b10ccc25984caf621a62828103e1442ee99cfbed764811e4500093ed035c81095fb357d07b34f07ce8e340f3246185f83b39bed6d749beac72d6d47249ba65430cf1badb35600e339922c5125d1c208cec1198450a6403d2c21972997bcf2e1527d757ff45e99f9e001e7a2588345da50bf4c2639be0f25c48ea5b4b20df8d0c887020b34f48ca0bd18f8854b09837583924c86538aadc38a1ede0e1839aa242cd740ff06277354ee1f38ac2a09d067db3110a78d5f763802dec6ff14942ccb2c79ae2037bae11c952056b2cd97d9cf1169cae7798011850287e9488651ec8584c27b7c800233da0b4a879fb84355eb966095e5549ee7d6f31d1382954396a14904bf1680114bf684a91ce94cfbe4864decbbd868ee8674d5d3d72568ee89aab60ebe669fdaabbf7d85172ee69dc55d5dddddad96d1e598ba75c1ee0dbcba2dc9e67a79b7305b74ffad718e7690db80ecc7cdc7fd55708b944bcd57fbbc2dce3832253b0ca80b3f7f4d7a6d2a9229f05053c7582956155863e26c5c69cf996e47f31bba99e8350f4ff75a5eae96ab9bd1ee78bddd449b74d421831b5b9797db54666b79a042a5b0630c6ec1da94dda24b815b2236f012d5f1c7d4198dad60add0ea2d7bc6844195c7ffbbe46ebb8d6c64f74366ac4b54ab979fe404a78c20a84e13268a411a67e1d2879e1668b6714e8c8dfe2fddc1df34583dbbfce783bf02cf4a975d3ecad83e26a566d7a8cdf562356b1f798b3b4e57d166db3014d1abf5b9681526fe221880fc2c8ae6f3c5468b8fdd8ad262a4b878445c321f9695969578ab3318b72cee1d4a4d62a4b75017be5ec6f632b197a9bd9cdbcb4b170ccda8f29d9e0c21155d7861086956303e6dd49d16497f91f617f3fee2d22c5a6d39ae2b3959ae0165145dd9b9d36f158fc199d1065cffdaf99253d3c0ec16377de387a464484a5dd2a4980fb92e1d92eb1aa6aab5b811d49bac381a523224a52e69d28bace1ba74484ea92c168bd1868c903631938d760ad4b43d05427847f50fecc83304369207fcca999aca6fd19f107c3cea69fd6746997740bfc1a216f2ce520239aac33e3328e58f9ac491a7a3ad4c11b9237b37b14bbbc5f8947bb68fd5fbab462c6b6c4892567498a33aa3b06c62d22c3202ebda501e39da77eadba3b02d73ee90fbf3fd2eb311df55383c05be276dac294ae6d7fa62c5d1ff209173ffdd2beeee5ef694353a7834378431202cd5dbc4c4e97998caab33d64d43e4a13243fa024ed173e6bcd38cf8d7511ea8a7f1f005cd3adf8fdd7d2d9ebf30121a75b1f4cecc2d632eb7a6c8210767afdba15c843b822c9c292e02ab5a26abfbe7f6e4a075bdfdd3132472590afa5f318c57dc8d90fdffc668984bd860757bd287d203e4546e1cdecc2486eca1ae3b38a3d3a9f9edc3e87ea1dede73dab60e54b67d953b6fe8f9dff8ea19aabd523972e41ac89d24a74672da49f648ea2d02810541d3892578f0fcd589e91b2f01beceda0f7f93cc87b6b8778ce4a35971ae0836263c495ea5b3d96c36e01f75d9a372b3d52206ee180e47492ff447a273d823316247bf63e9d68c0cb21cf5ea447d7ba61fa35cf6fc5aaac174cffc57bd172ae2a52e797b7b77bd7581b01cb9a01b038755fa65f20ffe1d35c0');
 INSERT INTO FileDataTable VALUES(5,X'00002621789c012126ded989504e470d0a1a0a0000000d4948445200000040000000400806000000aa6971de00000009704859730000375c0000375c01cbc7a4b900000006624b474400ff00ff00ffa0bda793000025934944415478dab47b09941d5799de77abeaedfbeb7d93ba5badcdad5db264c9b66c636c186ce28031e02140329ee130131cce496012161b863078068719601232c4873301db6c36de101883912d7993b55892d5526b6da9f7edf5f6f6a5aa6ebe7b5fab5b126b02b9477fdf7af5ea55ddfffbf7ff9604fee8633b699a740a6af8421f175d2b9ac5d22509b1637b3b3efcc1adeeabfbfbe5d0d02cfed3bd37408d70dbfd88c703f8a72fdf21fee7375f368e1d1b45a56c4b01c87c2a230b8539c4ea1b2084c0f4f803f8638edf1b0029e56fbd07bfd70b741c17bb7e7a1c4f3ed363dcb87399fb2fdfd92f1d47e29517be042047ca906012a800d06601fc87291b78a900f81d2006815a245bde0621004fc82f9c8a6d4847baa6cf2b0189fc780a9e700053c37f3818e20f60fcd2a199af8e30ba6fc9e0d42b4fc0ce7b017caf76e9f2551b9b9ba29b1389e01aafcfecf078ac3a5e1e725de9755c8972d92913b85ca96c4f4e4fe7cf4f4c667bca65fb9070e5616fd89f722a0e726333d4945a43da2e7cc928c1b0901d9c000c81c90b5ff8ff030099ff6de72d52828cc7f2f972d8340dafcf67e52550dcfdc269df7ffbc7177778bde6bb93c9d0b64432980806bdd2300de14809a511156a4a998cd9b6abb5263595c300cd8200a058a848e9ba42ba7286cf7a1dae7cca75dda70dd31a1364d8f018866bbb5298420a08ecf8fa87b1f7230f61b2ffff1e08f1ff20792fbf6b22e3414aa93c37572cd4d58567fb07664af77cf4fb37b536c73eb3664df30d3c8768d40fb5ceb1c9ac3b3153702b645602a2527144799ef152c9c6990bd3181c9e83c38bc99f849420f34ada864bb4a4e30ad21ccf3d49fa9a15f01c0104788edf13a9452ea87565a486bff8870140067fd3b9b892388f671e7cf047e94f7ff1249c4c1a407ad5f69dabefdfb2b9edcea5ed355e8fdf232bae24eb02e188cf48c68314a214fd23693992ca09ed2f2090ce95d0733a8599b9022c72ae1857927515c3b40f0200c52019e579c720099eb3f9dd13bcfb7dc2304e530b0c05190ca50d0067d8853226fa3eff47054033cff3060198aea9ffa0686ddf24376d68ac397162ec53ebd6b5fcd5ba75cd8160c4ef16ca0eca64dd21f7367f50b25d413e108df8d0da10a1ca3b387e7e1a4313599c1d98452e5f8129a01885acd2c2311956b3242882c792c78e06a2a2c12810842ff3f88172ae580a24c346b03eeaa6de1c84bf3602652a63a7effb0301583c0e080ecef9b7ddfe0d3397ab38d168601b6dfe7f6fdad4b66a497b8d9b2f3b92ff0c9710391092c41950644ba044604ab4f98664101d8d11bc7864187b8f8e21e03100572a661799d79277784e1dab591f4bce1a087eef9271d0a64c5eff0681f830801efa1893e71d1862c1298f9efa2c7edb307f0fe68d79e68b777ff88766d78a154eff8581f7ad59d3f2c4f61d9d4d89ba889d2dd986c3a74bcb84344de15a16c98422c75464003c165e0b93d90a76f78ca3b325862d2bebd03799870d012fbdba308d05320cce8a113deb63f58fb326bd269e7778aa05101f02d047ae8f1996691210c92bb47823b537239bdafd5b34e077abbf78f28903f21fbf79c48cd6d43bfbf71ef8e43d7fb6fdcbabbb9b28751736609069a925cf85ba26491870b800072409d86ed5ebbb9c2f90e1f199028ac50ad6b6c5b0a93d869fee1fc218bdbf5fd96fc5d61aa0256c5f4295c5d921719624a5118e9a49067dc35f535c0f121ad329f2a4025e81268091decffcfe26d0d2f1390c9fefc17f79f9713c702db065e77f378b8ee50c9de9fffc5ffcf98ecf6dddde618f4de54de1a1b40d3e9752a7f435f33c5e04a1aafe0bcca732650ca4f244ac6ae3e96c09f5612fdeda5d87dd3487b34373f00ac02e138405c61799e6394dc27501fe5e3855b3e077ae229a84c5fbfe0d55e3f31030ea3775ba66c887b9b3a3c80dcf60e4c4a77f37006d9d9f43be6883aa84da86284af9b2c9853a8574e19377dfbdf9cbef7af706bb6f68d69455a615f35adda54791852a10246a835d95be0e77ca399e99c851f2361cc504cf050cc0e0dc14f5e28e4d8dd8773285d94c09014b2cf8039bbfb3c97ca150413e5f4286dfcfcce431972e229729a252b2e97808b7e4200e4ec9b65c879a20a0354154530fcc875605c26f0720d1f069f0526d775cb8919e48bbf058ef7fcf7b377defaebb363a45c6e6a96c45185e4b9271b1c0b8579107e0ac411002f457a026925c8cce15151aa8f31b48fa4c843d062529755498cb96314b6db879752dde383b8d237dd3f040aa7a4003055ee71180d704fc96a1894f4589604e33811a1a9d9313e319512a56a405b8d40e939a713780ef83ea00c173127a0cf77cea3703906cfc340c43a040fbcce5ca02a5710984d7dff0b60d7bdffbbecdd1683ce0e6caae915171ce67290d58605af838fb15f9e0109012992f93f1a0014448a0da0a529a89ca64ba84490242c6b56499eb6b667d00deb3a5093f3f3c8a81f10cbcd0e6a0bf67b2bc305332b00084096432ec434dd4a70091a304e15cdf949b4d170c13489b023bc9ce51652d92df572a55539c3cfdd95f1f0502b11b901e4fa398cf00ce3700ca6a59f79627eeba6b53a7e5f738a1b0df9ccddb925e5d334f6faf55df21553c1e547c3eede92920c465196bfc157478ca64348b0bd3599ca0099c992e6134e7206f030a171f57e921f9783ffa35ed23de75750be782d61caf9236856899241eebcfbc1e12c8535013d480fe9139a4a6f3221af6cae5ed49231cf239d3b38500b3cc4dc968e0e1550d417b9ca0bb04d31bf090c7e77f1580dad6cf426a10820844c346c1de2283d1a5f7bdf39d6b3fd0de594b53945638169053b90a99b7aa76cec5b8be007c91109ac2269659797495a7d15198c032378d26a38c8425b13c626243d8c5d6988d4d511b1dfe12c2868d920b646c031557404817b40aa40bb6d6903fd9d08863fdb3d043ea3fd54c91743150198602af0a8e92eef864568c8c676434e4355674d6d885a2dd36349a76ce4de45e642d62246bc372fb962568ee7807ce1e7f1a6a58a80e1d7b25112272c2cda55c42d1bdee9aab3eb1666d336673653314f183cf1065094a4440eaa2c40b7f6e1466df29e6f27d38363d8512d5d420408170188944124d0d0d58ba7409babbbbd11e8b52a54bb8da2ed3c4b2184acde2d8680687a64c9cc97869364028c050399547cf301de3b6567c7fef0504898c74557e2061b80a084d5a9d25cf81b3492d0c08af321171666006c3a3a6b9bc3d8170c8fb899e9e91c7062e4c1fafad0f8bb3e752f23d77ac5d28df0538ea96dc8726bf05b4d7a338953166660b2e6ce7bbef7fffe6bbdb3a6a9d5cd931e3c9900c4503a27fba009a035c7f10e3079ec4c8a19f339d2dea5017f007580045118fc711e11c0c86c01211b333333c0ee0ce3befc4faf51bc0e0059320554af4035313181a1ac6d1e10c5e9d0aa22feb87e9d8f4f605bc6b4bb3f605af9d9844d014ca1f5c91135c795cfd5e32f4303a880a53cfced69819f25bdf0b85fc7f1af09bc6b64d8deec7eeb99e029bc692d61a1817a53f5a7470fae00571fad07977f2c2d496aee5f5ef6d6e49c85cc1366c05b8d0b93d58e468fb4df8a82d27f7219dc9c113882014af85198ac1b67cc83b40890bb1c864546b421ca3a3a378e491473036360a0fcfb3e2d120c46b1bb16ce555b87e750bee6a9ec1ced0104ce1c04b67fab323a3d8d09144632200f56cc39ccf0e4d929eaf3c3634c160fca3d6305537ce0dccc874b6fcbef6d6e88ea0dfe31eed49191fffcc2eb4b524b51698f5ed9fd307fe58007ebfc770bd1e198905feeb75d72ddb1c4d84dcb294460502e1b04fc7f6697aed8dcbeb61966670e2fc107cedeb508e36628eea97e2772333695c60c7e6cce008ce0d8d209bcba3b9a10ecd8d8d348f0ac148a0a3a31dcce62149ae63abf522188e527b6248ca39d4944790713c182f7af9fb22c1a9c3e1be19ed2ca50b40915c243de4af9204840ab653d339937ebbf6070fddfdfd37f6fd00fbf67e173dbda3a8af8b5068899bb41d6466f3626a604256b29596ced58d5fdbb47949a0ac229792bcf2c23e0b0982b48415dd0463f691d13c44a41693634c63cff762767400f99914ca853cec4a09e5720573197afd8141f49e3b8fa6fa5ad425e31a80152b56e86287c06b20481a08afd78b68a2064e6e1693bd2f61ced380813981aefa00425e13fd13590d827bd10f5c3e5f493a99f2792de1f39a6232955bf2f70f7cf18570edcd830f3f76443cbeeb04aebfa61d962e1a2060aaf8128d387eaf757b53532cc9cf4e96b64fe8902bd968a5dd773645f0b337c7315b560b2e63666c006902e02afb4f3440787d10a6a505e490218736ee14b2484fa5f09397f6e33d375d033f7d02c7bc3727015a136cdb6696485f522e23d9d482c6ba043b443d48c7b6e3c59e09bc9b0ef104cb67dab6765e920483343f8bcb499b4bc17671db4dcbc5d9be9473e08dc1e0ae5f9c7ac7330f7ff035009243e73b167870d3d7efc10b9f7cd8754d9d65fd2b55ab2f67a2e20d7a91a15a373646b1b431a2c3d238cf07985f17cb80154a20d1b91609da32c3040443220880144a4a366c6a43696e0ae18921d8a9616a44164b96b42d145d8a6c9a45a150407a2e8db9b93954085c2416c3b61dd7431c3a4ccda2932c46717c388f1dabebf1b3fd8308790c820e0d04e90a40b42f20900e5a9aa2b8fde6e578a0778ccb32717e60e6063e3301608644f32ac3523fd87defb7749ded03ea3c5eefb674be82833d63467777235a5ae268667bebc5a3a358be34090e5dd74bd38740ed12786b5b21297930244a320fed844820835a0b98d0cc4d2377fa201a6acae85cd645ed70b4d99529ed2c93a4de93a770faf4190d8404e80b22686d6dc5c6b5dd686bcbe0e8e01c7a2ecce1c6abaf424d3c846c3aaffd86030e812ad39793ae41de7e43174214229da0e16198cce62b6b1f79ec48d7438f1c38c02c55e4d97bd4262038384b00eb79e71a7fc0e38e4de5442de3f1b64d6d78ad674ce5fb9a2f16603ae990ba000a022667322dd5972496ea0b0b82e121f204271087756e1f6e7bfb2db02c53a939ef51a10472786ddfebd8b3772fd46029afcfa5d3693a643fbad774e39db7dd866b3606e8b454ae71102bc301ec9b0bc2d27c2b127a96240eadfe259a687b6b0c57af6bc2582a0bdb719549b8043ebe77df85f57b9fd97b001aea474100aa91703ebddacc0ba10ace68c46f31adc4f79e3b851a6a802505889a4e8298178070e9a840f38524091330d439cec2ad264afc4b703cf06646b1b33389b59bb7814315595ada070f1cc4b3cf3e8b4c2e4f93b279ff32caa5122bd02c72d48cf1f171163c25dc72ebad587555375adbdab07470000de10c9e3bcdd41be2926ae6a22940cf3b36b6408dc9e982d206b2290880c0442ab70e485dd41d6919aa9ae310ae54f31a0d008fb7ae6f462f7b77e3bc414918ccec5ce4e83482f4c6e3d90201011c539259c0985f854b12b25a490afd4135388ab84e0ee26dd75f8b9ee327505f5b83e6a6461cefe9c1c3dfff218ef49ec5543a8b120180faad7a96d7405b328812c13874e8105be5d3d8baf56a742d5f81ae152b31573e875d74c63082f3bc578110f315e8b2b638da9aa2643ecff2baa8dbf0173b444cd83af857bb61ad75b99119c497374a0340295bec50edea552b92a24829b3ee473419d22a34cd3afcfc5816753521e44732f09349cca7c52e9135303fa4d08c80535978b13c7f063b5736e8adad59667dc70e1fa6e42b78f8b1a7f0fc2b07b8300b160b297f28c86353fd56e70b3345c1b00b546c1bc3c3c3d8b3a788f31706d0d2588b132315cca63288d7b42819e2d2470bce0db52182e7906cccce110029ab91ced075430d90045091070e0e30bc2742983a3e443f6699be86789d8fe16e494b4cbc717a42c5501d730d091d7fd9d246477354abb04b128a79157216a55fede7f1834dd58f96c6f0d64660e98a55ccfd334a9d75bc7ff4f1a7f03386c570240a4f90144ec21b8ac3f404347676912630358669a6d84dbe8af617856201674ef5e2e4d900738b49847cedac5aa3f0d1bf2c2200a8b07de4e484ce0196d10fb0e49e0fb752303384d4dcbf6c0261e7eab7ff332cb5e058531cf1983f30962e873ac9e00455871e13e1b8673ea790bc105a0b4cceb180857cc5d1bd7ce990501d84585dac2b4554f2b8319cc2a60d9ba1102a158ac8d3c11d7cf3185e3e7c929ad580404d13c20d1d8c266d042001c3f2eaae8d4d1fe01febc344ff31446806d1a807857c0e0635e440ef39941c03dd1b5761a05c952c7fb48881acaafbe1de71708b0d91a00780d0661d4ffa41cf1f06b606004f5699bf45296a1561e8b3586f7b6b12419c617dedb15405a6b95f98556b7b72b648fb0ce0cdc1b4f6e82eaa0f17f3644a81926be06a6b04376f5c815032899989711429c1fec1413cf1f397a81d7ed4b4ad44a4ed2a84ebdbe1a1f405230624f4b39c40198261d6613679f2fc6196c893a88b78985a4f617c962576cb4ab42d6d476a586bcc6525b3e2271cf4ea2db6b3ac0a9904eab2598d063af3be0b535e845658a076d7d3540c55c58d0ece62e0e438e251bf8ef1ec06c154d2bd2cadac6ac17996af4b6a826aa12497e72f9203c3a980d528ea2be3b87d651cadcb96a344c931c3e382a6f0f42f5e44fff82c92ad5d88b5af47ac75357cb17a4ade0f21cc0518858a1ce11a449a9623dcb89ce5b18dfdbd2398a03d476a9ad57e3afcac3f5a1be2f4110bd2d7ce2e12f2ea75f3bcb6f972b9baff988c077443658a1de9eecdad58b6bc165e6a8091a1974471107007ec58d45f9e4b972ef2bc207d92ced7a92e189acc6a546b421e862cbbcabced684798ae446130f179475301eb36acd7d960a9506048cbe0a5d70fe285fdc7106f5c8270f34a842879cb1f01602c80a9e7f91ea0418df045eb116d61f2d3be8ee6d28e70ed52feae0bc19aa548e52cb4d6473473f3fbf35a68c9a84f253ee0a10682d2d74e7cd5b25a0c0ccf557d33846aa66ba5b14aacb781c74828f8fdefc8cde4f48fabcc6b201641e01f3054e3c25806ab9a23d8db9b026b0d54e043484e615be887087a5661e7d63b108c8430333545dbcde3d499b3f8c1aedd3083093244b3a0dd5bfe28e63738ab605f0440933ea735239068814173f0451ae154f8a4702d0c7f0d53726695cd71cd3424b4c49ba999c59243b2b5af02a9c0cf4b5b621a8811ae9b3bd6b9a1e199020b2478035e58c077f1933d67055177bef2f53d93dcf15d01406a86352daaba6bbb64d8c4890b33b8e3da76f82dc0b1251c51c107eabf8077ad388849bb1ba59900a62377aaee0c553f85ef3df31ccb6496c52b3793f92e3abc1aadf2aeb3e063385df2acf919f32078230d307d3148db06840501137374c86a84e990b39478888ba98df9b9d93a5905c5e1ba48019f89b5dc817ae195f39226a09e3319af8b39506a90cd4bebde4f7f1b7c8b43309e4bc6c8f30c7bd74242725c267d920e7d1e6547b4c509654bad11bc7cb6823fadff1adedefe06acf84ab48a1226463e8ec1811fa398f8089e79fe00f61e3a8e9ad65508d19efdf12608d3bb28f9c5e7a8e32bcc417fd6c9914920a4a8767505890e597974c4425587b7aeb31e4363696a820373de27721b1e6fb9b603c7094a2657965e435060ee7922537535019f3486e9f169cb425decf75bc7b5462d4afe0a92ea0650377ae3d418ba989a5e1b7c02ef5ef234f246ab72acb43fc66dc7835afb47a8f47e8009cc8f60851b9543a31db7c1f028070ab897ef045fe1502569018845d2a6b208189982cf6360496344833796cae906a91ab97c19375db394213d8773fdd36099af4b7001f48033784852d70ba8fdfc80cf52b1f290f28cb972c5b852fa7a6186ab131fcb90189d35b8fdfc2cee5dfd2d568cb5f007033ac971ed02afcfd36e4d584e0a517f826a7f1d4275cae9c50059b5fbf9452c441a3d692db894f12b8f1735c500b4262e6d8868660f1d1fd71d62aa88fe7cf3f6a57a47e9c0d11104fc9674b87788ea230f81434848351be58a43144dd9dc1046737df82863e814a13224e1ba8c79e7e2ec50cd4c04dd095ceddec79bf3be668c482a09e40942011e83616fcec19e1e0f4ece762256d7042b58b57bf9ebde0370e4e55ab0c8fc6f9c01892c195db3ac0627ce4de91d269ed74d8e3fb9be43dff3c57dfda060b5d9406326a708de511234e402302619d6befd8dbbe4a1de0971ec6c6a8200bc4eb5528b7371c982dcf963e8979a5cdc59f755dcb26606f56c75850226cda858ade438e7f22e0e9f069e39dc882292f0f84280b0164074af507dd22228579a82fe7ca919e835e886c79655caee3348d11f311cea1ec19db7acc02c43f9eecb98d7e2e48cd70dcb9c343c96685ab754636074b2eb7aed6ddf54ad26f54e0e19a83cc3a441abcf95c90ef51bb9921fd7451ec16d2b8f20e3d623acba43a50a1f5a40c49fd71d9ed41cb0ff8c1fa7522d08452230ac20e08a45c6ed4b18be92f15f01465ee68384847eabe4da754d7a8d83048095a4f60377be75398e9d9ac42b870611f42f30bfe06c4199cc6bb431766c006a58e759f29eea9b825278e54d8521765db7bd633a1ef125e70ab6f45ba6508b344db5d1194567700ffe6cfd53686aae81e10d826c31c72fd0211511b44adce71778b587ea77aa196688f97e9cb337022905606bd5bd3473e5b8c217b8580c89f272fba763d25bead7af6f4224e0c173aff5635b77036ed9b6048dcc0176bd780e530cb7217e479bafdeaffa14ae1ed3bcefaef956b10b08fd8571aa2fa5764fb07a75a3dcb8a1d558b7a66998afab3d55970caa1bb92a95e4f5b47b0f426e3fee59f32dd4d68428d508a2618bf57601a6a0f47dccf80a12a95989977ba318ceb52056dbcc18dea41399aab49d052df88dbec0bd342ac87972c97cd5eb5f47c927233e3cb9fb2caeea4860e7a616bde5fec3674f229d29d2db9b3a5249cdbc1e17d5ff29aaffb0414f4913582821ccfcd40b4c2d6fc28cdaad25a55239154b471816ef59d1556b941cd5087174baf5a1555fc31d5b27e109d411b4201756c6e8449e739e8b28e3ccb081578e01cf1e5f0633da8968d34a78a38d3ab78716bebc9c1613204d7271d684458faf25bf7d4d231a689e87a9e6b75eb3046df511edfd77bf3ea013224865a58b110642a803411015221f85c40830ff15af1938f80918985fd74ef6c827b265697173a464bb075910fdb0f7f48458d61a711bd9c1b9bee17179fbfa3ed8462d9476180655bf9047225404dc124102edd1c5c10b2dc8c866846b5a59ebd74308cfa2e3bbd4f66dd2afd5022d7dbd4001a99c1b234a01b76e6dc38d1b9bf5f2af6677f8b52323f8c9de3ed6fb459ded517b480b9297f3ad7257564b85c70c531c24193e694bbba515bceaf2f7035ad6fdbdae96346ed096d2edc0795dfa13a1eb56f5c97b37ff9de86a8fc1311268acf561722acb6e4b8e713e83914997f581c48f5ff360ef85ade8ba6a0bcee69a11af6f53d25f6892fefaa197bbb01857375d75054772106569fba177acc4eaf604f716cea3e74c0a03a3695d88ade9aad1d1802f5aea02ad0ac042b754f2b3704b951ce76dfce2b8e08049680b0efa0ffdc72b768705aabd33cb43415854fdc8f18039fb15af3d76ff5b1bff87dbd6e4337d8108d82c65a4d0b19e5ebf803c6f9629081c3b07bc76ae1563a52876b4746279e30a3cff468a7ec2a33cfc42df0e8b106b29b8d5576834c33cd6c94c5d9cfd02e6f59b56d46927f7fcebfdf8d6933dd5325d003e0a8a92d0d7a6323918f3c04908f002dd01a526a8f7f62cce5f1190c7553ead1792b3c123352e07e03dcdff19b3919bf12f3ff82544e37d2ec63f06041efafafdffe6ab7ff1d68db92647d4ba4c9e0dc7b1197ba97656516f818d4c090c8e4bec3b1d45ff5c13e24dcdf8e5d1123ed419c2b56b3dd87d6808114ad17617bcff82b44d7213f05aba84ad4b04d0521b6251e351098e6e6735d1d9fec32387708c52a7d7e7b5a6360fc77634109621f4bb429caa5ac61455a89b028e5b2c5b94e40156400f40d8305cc30d463dc8a44c0cb4fe07e0c85f5f6e025fe5b970004884c1b80aa35c863b99161fbb6913fe89aacfddf084f078bca250c8209dce31cc64697f0e7afb05f61c11f8c5a98d88376f44cbb28dace35b90af1878ef2dcb5933a47084c5480d9d1705a3b24e46174b2729645e576eb6ebeaeaeef4c0acde73b871738b5ed813bf3cc3c8524190d7d21c16d2609bd7c4c25e6eb4047516e82130304c293c66d58a8a15c3ce1733d48a9dc2718e4070301698536950823875fbe7c9b058d48007ff3d409ef830603405d13f0697a9fdbab76f935f4a2642ac0dc2229af08999d9bccef82c14309d55ed3181e109893dbd4d18cdd540946308e40248f840a95bd8b5a70f6fd9ba046b3a93f8396376900c97c9c8d86449bfdec2ad771dda662845356e60a7e6ba0dcd78fdd828f652733cd5ad3adab97d69aea04d26411349316a993e8f22098bbacf419b974eb1ac2efb4b51718e48aa3efd9eabf38b801fe7ffea93c047c4a20934d702cb9a80777f5630c64abc7414fc8dd7f3e87de56facedf24442e1b0e30b044dd7a948be0821ec321f2ab9e88c40dfb0c40bc7d8674b7720d6d08ab287a9e9948dc1a9142e8ed7588cfcebb7742141357f86898aea347b3dd50d15d621babcdeb1b611376e69d37dfc871e7f93a96d9edae899f70f728171355c12f7267533636eb6cc301bd06d1f9decb29fe7e44b168f3f8562f951d7b44ca74217e8f1c0b080e1c7fe1c68bfdc198b47ef07ea62407d02dc048151b1e1f68fe30bd7ad33ee8bc66276437dd262852867663354a32c8a851ca6d3aee4b5dca834c4a307d6c08dad41ac652dbce16618c203ccd70c8004c5a2df3bbc95d559136dfcb15f9c267825dabd1f1bd8a8d8cad8aebe7feed50b38d33fa34dc332abfe8a63315809e81d5f9b076dcd319a988bd97c459a16631d1b9b64de2dcfe52c1e7fd1199fb9cf8d458c8157ee75c577d280af04f97e86e48725f0c12b0078f26f415556d28031c23ad06361e72d5bf0cbeeaeb0599249b04b2c14d3c3e359667b5939355b11031386ec1f75f1bf7ed12c4fe53718b59deb65a87195f0324a0860be4fa89d9526ca006932bd635d236e6727697c8ae96ad043bb2fe3d5a3c338dd3fab4330b3b82a6e976c7ae2e2bbc2164181506f9debcc7574ba204d9a76856a64942ac2c9140cbe27f8a9fcf9b1bfb31a9346d867b9c6d0381c66872d638f63f7a3e7800f085c3944530d70d346e0bbcf0bdaaa083ff897eecbab3a7ceb03c184db501f330adc412d16327c5046e6734531310bd937023cb6378ca3a9ed58ba7aa3eb69586394bc49c176b8ace8ff2500eda5fd1e53ef213432acb5d50675dbca9100dfe222a0693cfe421fb2943ebb3ada41ba5acd2fd9e656334901e002da81f25a49db170455560a8c73a5b265552ad974aef25186a4479d68446f839ad3193810f00dcea077e441202ef0eb8635b21f38b71fc6973e22dd37cec8bfe9ee34d77bfc61dbf2852d55454ecee4854dc7e7b74a627052c8741ee2cd3e5979fe80bddf881b4b1299585b7757dc6d6cab710321bf418f4c69ea3769f513cbe478265b46ef641e839339b5afa06d7f3d1de3fb6fbf0a433cf7e6f959a5ceca8f910c0d06ae78fb25601a9249aa98a226d1292a5b47d075ac8089233365f1ef6a7de2c87463d2ccbcdeeb2408944d9b365916f7ee23f351fcc6217ef9551836ed9ea9ecad2b96e0673e7f4436352405dfea52afb28952318b52212b33395b0c1180de7e291efa318ebd790e4f5bdee02bb1e51f7f8b3752ff315f2418082442ae8f4ec9f47b0d8540454a650942029a292fd5d84352d0e44b8efedcdd16d3da31c768d0374e80d245bdbd3d9fd6401de8f7a0a4a4269655552602ae63442d51640afc0fe950f86f939140fee4aba78dae6fff5bf7a70d16da03f74338719caf30dbbb16c02be277bd2eefb15effe7cabef656ffe6a1e9a4b37a59c4b4ed32de3c9541670399cf16c5e08490b9a2140f3f87f1c75fc4d314d41e477a5faadffc9dc188f7e47ad788fd8de1f5df66b010b7c23e6906bdac2ba8daec9bebb7b738aac6b1b88f2f25d4bbc43ab36bad0992020a14ed14d3747059e600ec52ab37c2818a232c92c926000d6997e9979f0f0ec923c366c1189fc8cb4098b1291082431f71e20b77022f00f83fad9bcb8b1c5514c6bf73efadae47774d7a1ec4194746cc6444e830082af880a0d9e8220b51916c04c93f212efc17e23a1b570a12302e0c22c6e0441d14e29010216812308d93f8c84c32d3d5d5f5be3767ba2fdd4d6f7c8c077e7c0567519cef1e288a7bce09c2df05bdc60efd740b73ef9d54579e69858b8f2fcf555a43c651c7f09013091df33fbee15d1fa24b3f9becd4c7f882bbef2b41f846436d4a55275dc69acf5acdaebc79ac3e73e46da73e7b5406f560cf04e12912ae32c291869424bb003136d9011833f8246a6de03bc21cf0240225a84644a6a84cdecb29e571b324babfb6f5d72f1f5c5f7bff822227f39b8bb248ba699a6c9576f011387e1c58ff1e7c29817f12ea95a353e2ec7a27b9b0213e2ca1dec97429960ee69a744a3591f09538d04d089dd8e093355ce1e2371c89ab4585bb40e954c56e40c209094eb87de3cced6d9c39e54daf7c1ece3ff782d73cf454ad3ef788f21b9ef0dc413728399cef033136a461b441566aba9d95a64c332a93382de2ed766fa7fd63e7ce0f17f5bdabd700c4caf19660d08deedd8a0018bbb758021ce7cefdfbb5b9301053514fb75657bcb7de38e69f78f270357d683ed5412da7cb37a5294a2d3efbceb43f3a8fb33585aff3129701244cc03498b00fc9a9be9aca6565d0741a0b8b7ef3f0a36eb8f4b0533f38abbc030d590b5ca15c4542da5b2dad8d2ecaaa48d22aeb4465b275378f3637d3dd1bbfa63beddf74a9ef1390917452634c6474d9011059ba4c8fc9f7b338a9ea1e16e2142dd7a1675f7f49befa7cab5a9d9f31980ec1b302e8be7b1a9f9655bff5bfd5067f0290430346d4074a7b66b0119af3da03c0c0efe788eac2f17c215d8f841240ffc72dd75596683e72547abca814102948c46c6a04189b1b125b52a6fccf063443819d483bdc093359a11fcb0bb45697f1f2d34fe045af06f5e525acdfdcc47947e26251e1ba7da1626af6a47d4b30a10cf920b1a72e605c18edb04a6b20d916ae0605500112396b06981446f758136bc64847644c6e8b37fbe9009e031468ffa105171c106121c9b00ce008334d843bac1bc6e09a10881a3e4c270638842d44591ca666997c562348b032c3d003138c3502c518b9a518d3d25231fa7f5d9e1683cb1567aa8e269bf0100ddaba9397f89d739dd087de8d3119641113c871b5d090519831b4a51ad7098c65dff10012e1fd4920ff1247000000227a545874536f667477617265000078da2b2f2fd7cbcccb2e4e4e2c48d5cb2f4a070036d806581053ca5c0000000049454e44ae4260823623a9d9');
 CREATE TABLE FileFilterTable (FilterAttributeId INTEGER, FileId INTEGER );
 CREATE TABLE FileNameTable (FolderId INTEGER, Name TEXT, FileId INTEGER, Title TEXT );
 INSERT INTO FileNameTable VALUES(0,'',1,'');
 INSERT INTO FileNameTable VALUES(1,'index.html',2,'Check websites for broken links');
```

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/containers.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/containers.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/fileutil.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/fileutil.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/chrome.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chrome.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/chromium.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/chromium.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/firefox.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/firefox.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/opera.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/opera.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/safari.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/safari.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/linkcheck_gui/library/bookmarks/winutil.py` & `linkchecker_gui-10.0.0a3/linkcheck_gui/library/bookmarks/winutil.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/tests/__init__.py` & `linkchecker_gui-10.0.0a3/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return check_func
 
 
 @lru_cache(1)
 def has_pyqt():
     """Test if PyQT is installed."""
     try:
-        import PyQt5  # noqa: F401
+        import PyQt6  # noqa: F401
 
         return True
     except ImportError:
         pass
     return False
```

### Comparing `linkchecker_gui-10.0.0a2/tests/test_containers.py` & `linkchecker_gui-10.0.0a3/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/tests/test_gui.py` & `linkchecker_gui-10.0.0a3/tests/test_gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 class TestGui(unittest.TestCase):
     """Test OMT GUI client."""
 
     @need_pyqt
     @need_x11
     def test_gui(self):
-        from PyQt5 import QtCore, QtTest, QtWidgets
+        from PyQt6 import QtCore, QtTest, QtWidgets
         from linkcheck_gui import LinkCheckerMain
 
         app = QtWidgets.QApplication(sys.argv)
         window = LinkCheckerMain()
         window.show()
-        QtTest.QTest.mouseClick(window.controlButton, QtCore.Qt.LeftButton)
+        QtTest.QTest.mouseClick(window.controlButton, QtCore.Qt.MouseButton.LeftButton)
         window.close()
         del window
         del app
```

### Comparing `linkchecker_gui-10.0.0a2/tools/hatch_build.py` & `linkchecker_gui-10.0.0a3/tools/hatch_build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Chris Mayo
+# Copyright (C) 2022-2023 Chris Mayo
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation; either version 2 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -11,14 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from pathlib import Path
+import re
 import shutil
 import subprocess
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 import markdown2
 
 HELP_DIR = ("linkcheck_gui", "data", "help")
@@ -28,27 +29,36 @@
 
 class CustomBuildHook(BuildHookInterface):
     def clean(self, versions):
         Path(*RELEASE_PY).unlink(missing_ok=True)
         shutil.rmtree(str(Path(*HELP_DIR)), ignore_errors=True)
 
     def initialize(self, version, build_data):
-        if not shutil.which("qtchooser"):
-            raise SystemExit("qtchooser not found")
-
         cp = None
         committer_date = committer_year = "unknown"
         try:
             cp = subprocess.run(["git", "log", "-n 1", "HEAD", "--format=%cs"],
                                 capture_output=True, check=True, text=True)
         except (FileNotFoundError, subprocess.CalledProcessError):
             # support building wheel from sdist
             if Path(*RELEASE_PY).is_file():
                 self.app.display_warning("_release.py already exists")
                 return
+
+            try:
+                git_archival = Path(".git_archival.txt").read_text()
+            except FileNotFoundError:
+                self.app.display_warning(".git_archival.txt does not exist")
+            else:
+                rematch = re.search(r"node-date: ((\d{4})-\d{2}-\d{2})", git_archival)
+                if rematch:
+                    committer_date = rematch.group(1)
+                    committer_year = rematch.group(2)
+                else:
+                    self.app.display_warning("node-date not substituted")
         else:
             if cp and cp.stdout:
                 committer_date = cp.stdout.strip()
                 committer_year = committer_date[:4]
 
         Path(*RELEASE_PY).write_text(f"""\
 __app_name__ = "{self.metadata.core.raw_name}"
@@ -60,15 +70,28 @@
 """)
 
         index_html = (Path(*HELP_SRC_DIR, "html.header").read_text()
                       + markdown2.markdown_path(str(Path(*HELP_SRC_DIR, "index.txt")))
                       + Path(*HELP_SRC_DIR, "html.footer").read_text())
         Path(*HELP_SRC_DIR, "index.html").write_text(index_html)
 
-        cp = subprocess.run(["qtchooser", "-run-tool=qhelpgenerator", "-qt=qt5",
-                             "-c", "lccollection.qhcp", "-o", "lccollection.qhc",
-                             ],
-                            cwd=Path(*HELP_SRC_DIR), check=True)
+        cp = subprocess.run(
+            ["pkg-config", "--variable=libexecdir", "Qt6Help"],
+            capture_output=True, text=True)
+        help_exec_dir = cp.stdout.strip()
+        if help_exec_dir:
+            help_generator = Path(help_exec_dir, "qhelpgenerator")
+        else:
+            # Ubuntu 22.04 doesn't provide Qt6Help.pc, 22.10 does but without libexecdir
+            # qhelpgenerator found in bin on 22.04, libexec from 22.10
+            help_generator = shutil.which(
+                "qhelpgenerator",
+                path="/usr/lib/qt6/libexec/:/usr/lib64/qt6/libexec/:"
+                     "/usr/lib/qt6/bin/:/usr/lib64/qt6/bin/")
+
+        cp = subprocess.run(
+            [help_generator, "-c", "lccollection.qhcp", "-o", "lccollection.qhc"],
+            cwd=Path(*HELP_SRC_DIR), check=True)
 
         Path(*HELP_DIR).mkdir(parents=True, exist_ok=True)
         shutil.copy(Path(*HELP_SRC_DIR, "lcdoc.qch"), Path(*HELP_DIR))
         shutil.copy(Path(*HELP_SRC_DIR, "lccollection.qhc"), Path(*HELP_DIR))
```

### Comparing `linkchecker_gui-10.0.0a2/.gitignore` & `linkchecker_gui-10.0.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/LICENSE` & `linkchecker_gui-10.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `linkchecker_gui-10.0.0a2/README.md` & `linkchecker_gui-10.0.0a3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 ## Installation
 
 Python 3.9 or later is needed. Using pip to install LinkChecker-GUI:
 
 `pip3 install linkchecker-gui`
 
 The version in the pip repository may be old, to install the latest code first
-install qtchooser and qhelpgenerator e.g.
+install qhelpgenerator e.g.
 
-`apt install qhelpgenerator-qt5`
+`apt install qt6-documentation-tools`
 
 Then:
 
 `pip3 install git+https://github.com/linkchecker/linkchecker-gui.git`
 
 ## Usage
 
-`$ linkchecker-gui`
+`linkchecker-gui`
 
-A desktop entry is created for compatible environments.
+A freedesktop.org desktop entry is installed for compatible environments.
 
 ## Development
 
 Development is managed on [GitHub](https://github.com/linkchecker/linkchecker-gui).
```

### Comparing `linkchecker_gui-10.0.0a2/pyproject.toml` & `linkchecker_gui-10.0.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,23 @@
     "Programming Language :: Python :: 3.11",
 ]
 
 requires-python = ">=3.9"
 
 dependencies = [
     "linkchecker >= 10.1",
-    "PyQt5",
-    "QScintilla",
+    "PyQt6",
+    "PyQt6-QScintilla",
 ]
 
 [build-system]
 requires = [
     "hatchling >= 1.8.0",
     "hatch-vcs",
+    "setuptools-scm >= 7.1.0",
     "markdown2",
 ]
 build-backend = "hatchling.build"
 
 [project.urls]
 Homepage = "https://github.com/linkchecker/linkchecker-gui"
```

### Comparing `linkchecker_gui-10.0.0a2/PKG-INFO` & `linkchecker_gui-10.0.0a3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: LinkChecker-GUI
-Version: 10.0.0a2
+Version: 10.0.0a3
 Summary: GUI for LinkChecker
 Project-URL: Homepage, https://github.com/linkchecker/linkchecker-gui
 Author: LinkChecker Authors
 Maintainer: LinkChecker Authors
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.9
 Requires-Dist: linkchecker>=10.1
-Requires-Dist: pyqt5
-Requires-Dist: qscintilla
+Requires-Dist: pyqt6
+Requires-Dist: pyqt6-qscintilla
 Description-Content-Type: text/markdown
 
 # LinkChecker-GUI
 
 [![GPL-3](https://img.shields.io/badge/license-GPL3-d49a6a.svg)](https://opensource.org/licenses/GPL-3.0)
 
 This is the GUI client for [LinkChecker](https://linkchecker.github.io/linkchecker/).
@@ -28,24 +28,24 @@
 ## Installation
 
 Python 3.9 or later is needed. Using pip to install LinkChecker-GUI:
 
 `pip3 install linkchecker-gui`
 
 The version in the pip repository may be old, to install the latest code first
-install qtchooser and qhelpgenerator e.g.
+install qhelpgenerator e.g.
 
-`apt install qhelpgenerator-qt5`
+`apt install qt6-documentation-tools`
 
 Then:
 
 `pip3 install git+https://github.com/linkchecker/linkchecker-gui.git`
 
 ## Usage
 
-`$ linkchecker-gui`
+`linkchecker-gui`
 
-A desktop entry is created for compatible environments.
+A freedesktop.org desktop entry is installed for compatible environments.
 
 ## Development
 
 Development is managed on [GitHub](https://github.com/linkchecker/linkchecker-gui).
```

