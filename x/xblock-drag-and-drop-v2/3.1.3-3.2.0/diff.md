# Comparing `tmp/xblock-drag-and-drop-v2-3.1.3.tar.gz` & `tmp/xblock-drag-and-drop-v2-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-drag-and-drop-v2-3.1.3.tar", last modified: Tue Apr 18 10:23:45 2023, max compression
+gzip compressed data, was "xblock-drag-and-drop-v2-3.2.0.tar", last modified: Fri Apr 21 09:16:14 2023, max compression
```

## Comparing `xblock-drag-and-drop-v2-3.1.3.tar` & `xblock-drag-and-drop-v2-3.2.0.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (122)    13122 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    35236 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21924 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/default_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    53365 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/drag_and_drop_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/
--rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop.css
--rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/
--rw-r--r--   0 runner    (1001) docker     (122)    34942 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/
--rw-r--r--   0 runner    (1001) docker     (122)    86843 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop.js
--rw-r--r--   0 runner    (1001) docker     (122)    41638 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    39006 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/
--rw-r--r--   0 runner    (1001) docker     (122)    18357 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3578 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/
--rw-r--r--   0 runner    (1001) docker     (122)    64209 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    20270 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    19590 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     6854 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     7058 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    21316 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)    22577 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/
--rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/
--rw-r--r--   0 runner    (1001) docker     (122)    16851 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    18514 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)    37990 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/
--rw-r--r--   0 runner    (1001) docker     (122)     5079 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)    84693 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
--rw-r--r--   0 runner    (1001) docker     (122)    16608 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/apros.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop.html
--rw-r--r--   0 runner    (1001) docker     (122)    16156 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/js_templates.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19892 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28625 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16505 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24470 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32171 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38531 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25388 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16671 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24859 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18883 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25607 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11388 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22806 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18941 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15579 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23406 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23285 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15801 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24322 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16196 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24372 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26457 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18165 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20913 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    11732 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    35236 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.061090 xblock-drag-and-drop-v2-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    13313 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    35427 2023-04-21 09:16:14.061090 xblock-drag-and-drop-v2-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21924 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/default_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52992 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/drag_and_drop_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/css/drag_and_drop.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/css/drag_and_drop_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/img/
+-rw-r--r--   0 runner    (1001) docker     (122)    34942 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/img/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    86843 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/drag_and_drop.js
+-rw-r--r--   0 runner    (1001) docker     (122)    41638 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/drag_and_drop_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    39006 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/de/
+-rw-r--r--   0 runner    (1001) docker     (122)    18357 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/de/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3578 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/eo/
+-rw-r--r--   0 runner    (1001) docker     (122)    64209 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/eo/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.037090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    20270 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    19590 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     6854 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     7058 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    21316 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)    22577 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/nl/
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/nl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pl/
+-rw-r--r--   0 runner    (1001) docker     (122)    16851 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    18514 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)    37990 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/tr/
+-rw-r--r--   0 runner    (1001) docker     (122)     5079 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/tr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.041090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)    84693 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16608 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/themes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/themes/apros.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/drag_and_drop.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16156 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/js_templates.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19892 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28625 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16505 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24470 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.025090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32171 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    38531 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.045090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25388 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16671 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24859 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18883 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25607 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11388 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22806 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18941 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.049090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.053090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    15579 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23406 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.029090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.053090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.053090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23285 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.053090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    15801 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24322 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.057090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16196 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24372 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.057090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26457 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.057090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18165 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.057090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.033090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.057090 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    20913 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11732 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.061090 xblock-drag-and-drop-v2-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 09:16:14.061090 xblock-drag-and-drop-v2-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-04-21 09:16:08.000000 xblock-drag-and-drop-v2-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 09:16:14.061090 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    35427 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-21 09:16:14.000000 xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/top_level.txt
```

### Comparing `xblock-drag-and-drop-v2-3.1.3/Changelog.md` & `xblock-drag-and-drop-v2-3.2.0/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.2.0 (2023-04-20)
+---------------------------
+
+* Use the `replace_urls` service instead of a runtime property.
+
+  BREAKING CHANGE: This version is no longer compatible with Maple. 
+
 Version 3.1.3 (2023-04-15)
 --------------------------
 
 * Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
   * `conf/locale` directory is now the source of truth for translations.
   * `translations` directory is now a symbolic link for backwards compatibility.
   * `locale` symbolic link is deleted to avoid too many symbolic links.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_z8qm0nb0_/tmpb08l2ffo_TarContainer/0/1.md", line 343, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_z8qm0nb0_/tmpb08l2ffo_TarContainer/0/1.md", line 343, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,15 @@
-Drag and Drop XBlock changelog ============================== Version 3.1.3
-(2023-04-15) -------------------------- * Prepare repository for upcoming
-changes related to [openedx-translations](https://github.com/openedx/openedx-
-translations). * `conf/locale` directory is now the source of truth for
-translations. * `translations` directory is now a symbolic link for backwards
-compatibility. * `locale` symbolic link is deleted to avoid too many symbolic
-links. * `en` translations are now extracted into `django.po` instead of
-`text.po`. * `en` `text.po` is now a symbolic link to `django.po` for backwards
-compatibility. Version 3.1.0 (2023-01-31) -------------------------- * Upgrade
-to be compatible with `bleach==6.0.0` and `bleach<6.0.0` * Make the dependency
-on the `css` extras explicit. Version 3.0.0 (2022-11-18) ----------------------
------ * Sanitize HTML tags to prevent XSS vulnerabilities. BREAKING CHANGE:
-Disallowed HTML tags (e.g. `
+Drag and Drop XBlock changelog ============================== Version 3.2.0
+(2023-04-20) --------------------------- * Use the `replace_urls` service
+instead of a runtime property. BREAKING CHANGE: This version is no longer
+compatible with Maple. Version 3.1.3 (2023-04-15) -------------------------- *
+Prepare repository for upcoming changes related to [openedx-translations]
+(https://github.com/openedx/openedx-translations). * `conf/locale` directory is
+now the source of truth for translations. * `translations` directory is now a
+symbolic link for backwards compatibility. * `locale` symbolic link is deleted
+to avoid too many symbolic links. * `en` translations are now extracted into
+`django.po` instead of `text.po`. * `en` `text.po` is now a symbolic link to
+`django.po` for backwards compatibility. Version 3.1.0 (2023-01-31) -----------
+--------------- * Upgrade to be compatible with `bleach==6.0.0` and
+`bleach<6.0.0` * Make the dependency on the `css` extras explicit. Version
+3.0.0 (2022-11-18) --------------------------- * Sanitize HTML tags to prevent
+XSS vulnerabilities. BREAKING CHANGE: Disallowed HTML tags (e.g. `
```

### Comparing `xblock-drag-and-drop-v2-3.1.3/LICENSE` & `xblock-drag-and-drop-v2-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/PKG-INFO` & `xblock-drag-and-drop-v2-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 3.1.3
+Version: 3.2.0
 Summary: XBlock - Drag-and-Drop v2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Drag and Drop XBlock v2
 =======================
@@ -589,14 +589,21 @@
 -------------------------------------
 To release a new version, update .travis.yml and setup.py to point to your new intended version number and create a new release with that version tag via Github.
 
 
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.2.0 (2023-04-20)
+---------------------------
+
+* Use the `replace_urls` service instead of a runtime property.
+
+  BREAKING CHANGE: This version is no longer compatible with Maple. 
+
 Version 3.1.3 (2023-04-15)
 --------------------------
 
 * Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
   * `conf/locale` directory is now the source of truth for translations.
   * `translations` directory is now a symbolic link for backwards compatibility.
   * `locale` symbolic link is deleted to avoid too many symbolic links.
```

### Comparing `xblock-drag-and-drop-v2-3.1.3/README.md` & `xblock-drag-and-drop-v2-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/compat.py` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/compat.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/default_data.py` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/default_data.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/drag_and_drop_v2.py` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/drag_and_drop_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,24 +653,16 @@
             )
 
         answer = self._get_correct_state()
 
         if explanation := (self.data.get('explanation') or '').strip():
             if replace_urls_service := self.runtime.service(self, 'replace_urls'):
                 explanation = replace_urls_service.replace_urls(explanation)
-
-            # pylint: disable=fixme
-            # TODO: No longer needed after Maple.
             else:
-                try:
-                    explanation = self.runtime.replace_urls(explanation)
-                    explanation = self.runtime.replace_course_urls(explanation)
-                    explanation = self.runtime.replace_jump_to_id_urls(explanation)
-                except (TypeError, AttributeError):
-                    logger.debug('Unable to perform URL substitution on the explanation: %s', explanation)
+                logger.debug('Unable to perform URL substitution on the explanation: %s', explanation)
 
             answer['explanation'] = sanitize_html(explanation)
         return answer
 
     @XBlock.json_handler
     def expand_static_url(self, url, suffix=''):
         """ AJAX-accessible handler for expanding URLs to static [image] files """
@@ -1052,16 +1044,16 @@
     def _expand_static_url(self, url):
         """
         This is required to make URLs like '/static/dnd-test-image.png' work (note: that is the
         only portable URL format for static files that works across export/import and reruns).
         This method is unfortunately a bit hackish since XBlock does not provide a low-level API
         for this.
         """
-        if hasattr(self.runtime, 'replace_urls'):
-            url = self.runtime.replace_urls(u'"{}"'.format(url))[1:-1]
+        if replace_urls_service := self.runtime.service(self, 'replace_urls'):
+            url = replace_urls_service.replace_urls(f'"{url}"')[1:-1]
         elif hasattr(self.runtime, 'course_id'):
             # edX Studio uses a different runtime for 'studio_view' than 'student_view',
             # and the 'studio_view' runtime doesn't provide the replace_urls API.
             try:
                 from common.djangoapps.static_replace import replace_static_urls  # pylint: disable=import-error
                 url = replace_static_urls(u'"{}"'.format(url), None, course_id=self.runtime.course_id)[1:-1]
             except ImportError:
```

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop.css` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/css/drag_and_drop.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop_edit.css` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/css/drag_and_drop_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/triangle.png` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/img/triangle.png`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/drag_and_drop.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop_edit.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/drag_and_drop_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/de/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/eo/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/nl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/tr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/text.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/apros.css` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/public/themes/apros.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop_edit.html` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/drag_and_drop_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/js_templates.html` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/templates/html/js_templates.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/config.yaml` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/settings.py` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/utils.py` & `xblock-drag-and-drop-v2-3.2.0/drag_and_drop_v2/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/requirements/constraints.txt` & `xblock-drag-and-drop-v2-3.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/setup.py` & `xblock-drag-and-drop-v2-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/PKG-INFO` & `xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 3.1.3
+Version: 3.2.0
 Summary: XBlock - Drag-and-Drop v2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Drag and Drop XBlock v2
 =======================
@@ -589,14 +589,21 @@
 -------------------------------------
 To release a new version, update .travis.yml and setup.py to point to your new intended version number and create a new release with that version tag via Github.
 
 
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.2.0 (2023-04-20)
+---------------------------
+
+* Use the `replace_urls` service instead of a runtime property.
+
+  BREAKING CHANGE: This version is no longer compatible with Maple. 
+
 Version 3.1.3 (2023-04-15)
 --------------------------
 
 * Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
   * `conf/locale` directory is now the source of truth for translations.
   * `translations` directory is now a symbolic link for backwards compatibility.
   * `locale` symbolic link is deleted to avoid too many symbolic links.
```

### Comparing `xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/SOURCES.txt` & `xblock-drag-and-drop-v2-3.2.0/xblock_drag_and_drop_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

