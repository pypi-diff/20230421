# Comparing `tmp/collective.z3cform.jsonwidget-1.1.0.tar.gz` & `tmp/collective.z3cform.jsonwidget-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.z3cform.jsonwidget-1.1.0.tar", last modified: Mon Jul 18 15:23:07 2022, max compression
+gzip compressed data, was "collective.z3cform.jsonwidget-1.1.1.tar", last modified: Fri Apr 21 08:41:25 2023, max compression
```

## Comparing `collective.z3cform.jsonwidget-1.1.0.tar` & `collective.z3cform.jsonwidget-1.1.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.370334 collective.z3cform.jsonwidget-1.1.0/
--rw-r--r--   0 cekk       (501) staff       (20)      376 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/.eslintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      278 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/.prettierrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      131 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/.stylelintrc.json
--rw-r--r--   0 cekk       (501) staff       (20)      821 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       70 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      673 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      234 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     6510 2022-07-18 15:23:07.370501 collective.z3cform.jsonwidget-1.1.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     2967 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/constraints_plone51.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.353619 collective.z3cform.jsonwidget-1.1.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7935 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)      110 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)     3013 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      256 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/postcss.config.js
--rw-r--r--   0 cekk       (501) staff       (20)       50 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      321 2022-07-18 15:23:07.370986 collective.z3cform.jsonwidget-1.1.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2603 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.344532 collective.z3cform.jsonwidget-1.1.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.353872 collective.z3cform.jsonwidget-1.1.0/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.356353 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.358591 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/
--rw-r--r--   0 cekk       (501) staff       (20)      146 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.359618 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      847 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      366 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/json_widget_input.pt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.345483 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.345336 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.361125 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/
--rw-r--r--   0 cekk       (501) staff       (20)     2520 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css
--rw-r--r--   0 cekk       (501) staff       (20)     2879 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map
--rw-r--r--   0 cekk       (501) staff       (20)   330364 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js
--rw-r--r--   0 cekk       (501) staff       (20)      198 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.361389 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.361656 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/
--rw-r--r--   0 cekk       (501) staff       (20)      494 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.362296 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1380 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.362515 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     3839 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.363054 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     4726 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)     1006 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.364979 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/
--rw-r--r--   0 cekk       (501) staff       (20)     2790 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js
--rw-r--r--   0 cekk       (501) staff       (20)      370 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.less
--rw-r--r--   0 cekk       (501) staff       (20)     8758 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js
--rw-r--r--   0 cekk       (501) staff       (20)     1335 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less
--rw-r--r--   0 cekk       (501) staff       (20)     1324 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js
--rw-r--r--   0 cekk       (501) staff       (20)      354 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextAreaField.js
--rw-r--r--   0 cekk       (501) staff       (20)      920 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js
--rw-r--r--   0 cekk       (501) staff       (20)      767 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.365533 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/utils/
--rw-r--r--   0 cekk       (501) staff       (20)      953 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js
--rw-r--r--   0 cekk       (501) staff       (20)      274 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/utils/widgetContext.js
--rw-r--r--   0 cekk       (501) staff       (20)     2482 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/widget.py
--rw-r--r--   0 cekk       (501) staff       (20)     1432 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      277 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.367055 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1328 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.346786 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.367584 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      988 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1541 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po
--rw-r--r--   0 cekk       (501) staff       (20)     1027 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1701 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      543 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      260 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.347185 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.369077 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      212 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)     1084 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.369641 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      139 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      478 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/uninstall/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      630 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1724 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.370107 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2678 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-07-18 15:23:07.356096 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     6510 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3950 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      154 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       30 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      173 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2022-07-18 15:23:07.000000 collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/top_level.txt
--rw-r--r--   0 cekk       (501) staff       (20)     2795 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/webpack.config.js
--rw-r--r--   0 cekk       (501) staff       (20)   471705 2022-07-18 15:23:06.000000 collective.z3cform.jsonwidget-1.1.0/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672797 collective.z3cform.jsonwidget-1.1.1/
+-rw-r--r--   0 cekk       (501) staff       (20)      376 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.eslintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.prettierrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      131 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/.stylelintrc.json
+-rw-r--r--   0 cekk       (501) staff       (20)      895 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       70 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      673 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      234 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     6632 2023-04-21 08:41:25.673022 collective.z3cform.jsonwidget-1.1.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2967 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints_plone51.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.657861 collective.z3cform.jsonwidget-1.1.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7935 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)      110 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)     3013 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      256 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/postcss.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2023-04-21 08:41:25.673479 collective.z3cform.jsonwidget-1.1.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2603 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.648833 collective.z3cform.jsonwidget-1.1.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.658110 collective.z3cform.jsonwidget-1.1.1/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.660573 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.662167 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/
+-rw-r--r--   0 cekk       (501) staff       (20)      146 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.663119 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      847 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      366 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/json_widget_input.pt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.649751 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.649612 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.664465 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)     2520 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css
+-rw-r--r--   0 cekk       (501) staff       (20)     2879 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)   330486 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)      198 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.664760 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665010 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/ArrayFieldContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665514 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1523 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.665708 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     3839 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.666197 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     4726 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1006 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.667954 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/
+-rw-r--r--   0 cekk       (501) staff       (20)     2790 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      370 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     8758 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js
+-rw-r--r--   0 cekk       (501) staff       (20)     1335 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less
+-rw-r--r--   0 cekk       (501) staff       (20)     1324 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      354 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextAreaField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      961 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js
+-rw-r--r--   0 cekk       (501) staff       (20)      767 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.668436 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)      953 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js
+-rw-r--r--   0 cekk       (501) staff       (20)      274 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/widgetContext.js
+-rw-r--r--   0 cekk       (501) staff       (20)     2482 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/widget.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1432 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      277 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.669830 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1328 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.651121 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.670317 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      988 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     1541 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1027 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1701 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      543 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      260 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.651538 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.671559 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      212 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1084 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672086 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      139 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      478 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      630 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1724 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.672509 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2678 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-04-21 08:41:25.660332 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     6632 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3950 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      154 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       30 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      173 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/top_level.txt
+-rw-r--r--   0 cekk       (501) staff       (20)     2795 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/webpack.config.js
+-rw-r--r--   0 cekk       (501) staff       (20)   471705 2023-04-21 08:41:25.000000 collective.z3cform.jsonwidget-1.1.1/yarn.lock
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/CHANGES.rst` & `collective.z3cform.jsonwidget-1.1.1/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+1.1.1 (2023-04-21)
+------------------
+
+- Handle integer fields.
+  [cekk]
+
 1.1.0 (2022-07-18)
 ------------------
 
 - Force vocabularies batch size to 1000 to get all of possible values.
   [cekk]
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/DEVELOP.rst` & `collective.z3cform.jsonwidget-1.1.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/LICENSE.GPL` & `collective.z3cform.jsonwidget-1.1.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/LICENSE.rst` & `collective.z3cform.jsonwidget-1.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/PKG-INFO` & `collective.z3cform.jsonwidget-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.z3cform.jsonwidget
-Version: 1.1.0
+Version: 1.1.1
 Summary: Custom widget to manage complex json data stored into a text field
 Home-page: https://github.com/collective/collective.z3cform.jsonwidget
 Author: Andrea Cecchi
 Author-email: andrea.cecchi85@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.z3cform.jsonwidget
 Project-URL: Source, https://github.com/collective/collective.z3cform.jsonwidget
@@ -140,14 +140,20 @@
         - Andrea Cecchi, andrea.cecchi85@gmail.com
         
         
         Changelog
         =========
         
         
+        1.1.1 (2023-04-21)
+        ------------------
+        
+        - Handle integer fields.
+          [cekk]
+        
         1.1.0 (2022-07-18)
         ------------------
         
         - Force vocabularies batch size to 1000 to get all of possible values.
           [cekk]
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/README.rst` & `collective.z3cform.jsonwidget-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/docs/conf.py` & `collective.z3cform.jsonwidget-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/package.json` & `collective.z3cform.jsonwidget-1.1.1/package.json`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/setup.py` & `collective.z3cform.jsonwidget-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name='collective.z3cform.jsonwidget',
-    version='1.1.0',
+    version='1.1.1',
     description="Custom widget to manage complex json data stored into a text field",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/configure.zcml` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.css.map`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/dist/prod/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9752,51 +9752,54 @@
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
     var U = function(e) {
         var t = e.value,
             n = e.id,
             i = e.row,
-            a = Object(r.useContext)(R).updateField,
-            l = F(Object(r.useState)({
+            a = e.type,
+            l = void 0 === a ? "text" : a,
+            u = Object(r.useContext)(R).updateField,
+            s = F(Object(r.useState)({
                 text: "",
                 timeout: 0
             }), 2),
-            u = l[0],
-            s = l[1];
+            c = s[0],
+            f = s[1];
         return Object(r.useEffect)((function() {
-            s({
+            f({
                 text: t,
                 timeout: 0
             })
         }), [t]), o.a.createElement("input", {
-            type: "text",
-            value: u.text,
+            type: l,
+            value: c.text,
             onChange: function(e) {
                 return function(e) {
-                    u.timeout && clearInterval(u.timeout);
+                    c.timeout && clearInterval(c.timeout);
                     var t = setTimeout((function() {
-                        a({
+                        u({
                             row: i,
                             id: n,
                             value: e
                         })
                     }), 1e3);
-                    s({
+                    f({
                         text: e,
                         timeout: t
                     })
                 }(e.target.value)
             }
         })
     };
     U.propTypes = {
         value: u.a.string,
         id: u.a.string,
-        row: u.a.number
+        row: u.a.number,
+        type: u.a.string
     };
     var V = U;
     n(37), n(39), n(40), n(44), n(48);
 
     function H(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
@@ -14472,18 +14475,20 @@
             n = Object(r.useContext)(R).schema.fields[t],
             i = n.type,
             a = n.widgetOptions,
             l = n.title,
             u = n.description,
             s = n.vocabulary,
             c = n.items,
-            f = null;
+            f = o.a.createElement(V, e);
         return "array" === i ? f = a ? o.a.createElement(er, tr({}, e, {
             items: c
-        })) : o.a.createElement(L, e) : "string" === i && (f = s ? o.a.createElement(Fn, e) : o.a.createElement(V, e)), o.a.createElement("div", {
+        })) : o.a.createElement(L, e) : "string" === i ? f = s ? o.a.createElement(Fn, e) : o.a.createElement(V, e) : "integer" === i && (f = o.a.createElement(V, tr({}, e, {
+            type: "number"
+        }))), o.a.createElement("div", {
             className: "column block"
         }, o.a.createElement("label", null, l), o.a.createElement("p", {
             className: "discreet"
         }, u), f)
     };
     nr.propTypes = {
         value: u.a.oneOfType([u.a.string, u.a.array]),
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/EntryColumnContainer/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,17 @@
         type,
         widgetOptions,
         title,
         description,
         vocabulary,
         items,
     } = schema.fields[id];
-    let Field = null;
+    let Field = < TextLineField {
+        ...props
+    } > < /TextLineField>;
     if (type === 'array') {
         if (!widgetOptions) {
             Field = < LinesField {
                 ...props
             } > < /LinesField>;
         } else {
             Field = ( <
@@ -46,14 +48,19 @@
                 ...props
             } > < /SelectField>;
         } else {
             Field = < TextLineField {
                 ...props
             } > < /TextLineField>;
         }
+    } else if (type === 'integer') {
+        Field = < TextLineField {
+            ...props
+        }
+        type = "number" > < /TextLineField>;
     }
     return ( <
         div className = "column block" >
         <
         label > {
             title
         } < /label> <
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetContainer/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/WidgetDataContainer/index.less`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/LinesField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/ReferenceField.less`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/SelectField.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/fields/TextLineField.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,16 @@
 } from 'react';
 import PropTypes from 'prop-types';
 import WidgetContext from '../utils/widgetContext';
 
 const TextLineField = ({
     value,
     id,
-    row
+    row,
+    type = 'text'
 }) => {
     const {
         updateField
     } = useContext(WidgetContext);
     const [data, setData] = useState({
         text: '',
         timeout: 0
@@ -40,24 +41,27 @@
         setData({
             text: value,
             timeout: 0
         });
     }, [value]);
 
     return ( <
-        input type = "text"
+        input type = {
+            type
+        }
         value = {
             data.text
         }
         onChange = {
             e => updateText(e.target.value)
         }
         />
     );
 };
 TextLineField.propTypes = {
     value: PropTypes.string,
     id: PropTypes.string,
     row: PropTypes.number,
+    type: PropTypes.string,
 };
 
 export default TextLineField;
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/index.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/index.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/static/js/utils/i18n.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/browser/widget.py` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/browser/widget.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/configure.zcml` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/README.rst` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/collective.z3cform.jsonwidget.pot`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.mo`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/it/LC_MESSAGES/collective.z3cform.jsonwidget.po`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/manual.pot` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/update.py` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/locales/update.sh` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/profiles/default/registry.xml` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/setuphandlers.py` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/testing.py` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/testing.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective/z3cform/jsonwidget/tests/test_setup.py` & `collective.z3cform.jsonwidget-1.1.1/src/collective/z3cform/jsonwidget/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO` & `collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.z3cform.jsonwidget
-Version: 1.1.0
+Version: 1.1.1
 Summary: Custom widget to manage complex json data stored into a text field
 Home-page: https://github.com/collective/collective.z3cform.jsonwidget
 Author: Andrea Cecchi
 Author-email: andrea.cecchi85@gmail.com
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.z3cform.jsonwidget
 Project-URL: Source, https://github.com/collective/collective.z3cform.jsonwidget
@@ -140,14 +140,20 @@
         - Andrea Cecchi, andrea.cecchi85@gmail.com
         
         
         Changelog
         =========
         
         
+        1.1.1 (2023-04-21)
+        ------------------
+        
+        - Handle integer fields.
+          [cekk]
+        
         1.1.0 (2022-07-18)
         ------------------
         
         - Force vocabularies batch size to 1000 to get all of possible values.
           [cekk]
```

### Comparing `collective.z3cform.jsonwidget-1.1.0/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt` & `collective.z3cform.jsonwidget-1.1.1/src/collective.z3cform.jsonwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/webpack.config.js` & `collective.z3cform.jsonwidget-1.1.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `collective.z3cform.jsonwidget-1.1.0/yarn.lock` & `collective.z3cform.jsonwidget-1.1.1/yarn.lock`

 * *Files identical despite different names*

