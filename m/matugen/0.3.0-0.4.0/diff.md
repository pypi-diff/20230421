# Comparing `tmp/matugen-0.3.0.tar.gz` & `tmp/matugen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matugen-0.3.0.tar", max compression
+gzip compressed data, was "matugen-0.4.0.tar", max compression
```

## Comparing `matugen-0.3.0.tar` & `matugen-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1615 2023-04-17 19:24:00.227213 matugen-0.3.0/README.md
--rw-r--r--   0        0        0      437 2023-04-17 19:08:30.540135 matugen-0.3.0/matugen/__main__.py
--rw-r--r--   0        0        0     5623 2023-04-17 19:08:25.961097 matugen-0.3.0/matugen/util.py
--rw-r--r--   0        0        0      375 2023-04-17 19:28:58.050912 matugen-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 matugen-0.3.0/setup.py
--rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 matugen-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1615 2023-04-17 19:24:00.227213 matugen-0.4.0/README.md
+-rw-r--r--   0        0        0      388 2023-04-18 19:23:03.501766 matugen-0.4.0/matugen/__main__.py
+-rw-r--r--   0        0        0     9157 2023-04-21 18:30:09.147119 matugen-0.4.0/matugen/util.py
+-rw-r--r--   0        0        0      433 2023-04-21 18:31:38.638471 matugen-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2412 1970-01-01 00:00:00.000000 matugen-0.4.0/setup.py
+-rw-r--r--   0        0        0     2041 1970-01-01 00:00:00.000000 matugen-0.4.0/PKG-INFO
```

### Comparing `matugen-0.3.0/README.md` & `matugen-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `matugen-0.3.0/setup.py` & `matugen-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['material-color-utilities-python==0.1.5', 'rich>=12.5.1,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['matugen = matugen.__main__:main']}
 
 setup_kwargs = {
     'name': 'matugen',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': '',
     'long_description': '<div align="center">\n     <img src="https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-4fe9-9ee5-a1a1395d70dc.png" width=140>\n      <h1>Matugen</h1>\n </div>\n    \n<div align="center">\n  <b>A material you color generation tool for linux</b>\n</div>\n\n<div align="center">\n    <a href="#installation">Installation</a>\n    ·\n    <a href="#usage">Usage</a>\n    ·\n    <a href="https://github.com/InioX/matugen/wiki">Wiki</a>\n</div>\n\n## Description\n[Material Design 3](https://m3.material.io/) offers a new color system that allows for more flexible and dynamic use of color. The new system includes a wider range of colors, as well as a range of tints and shades that can be used to create subtle variations in color.\n\n## Installation\n### From Pypi\n>**Note** Assuming you have python with pip installed\n```shell\npip install matugen\n```\n\n### Usage\n```shell\n# Dark theme\nmatugen /path/to/wallpaper/\n# Light theme\nmatugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\nmatugen ~/wall/snow.png -l\n```\n\n### From repo with poetry\n>**Note** Assuming you already have [Poetry](https://python-poetry.org/) installed:\n```shell\ngit clone https://github.com/InioX/matugen && cd matugen\npoetry install\n```\n\n#### Usage\n```shell\n# Dark theme\npoetry run matugen /path/to/wallpaper/\n# Light theme\npoetry run matugen /path/to/wallpaper/ -l\n```\nExample:\n```shell\npoetry run matugen ~/wall/snow.png -l\n```\n\n## Showcase\nShowcase with Hyprland, Waybar, kitty, and fish shell:\n\n>**Warning**\n>The preview and usage may be outdated.\n\n[![](https://markdown-videos.deta.dev/youtube/rMxoORO41rs)](https://youtu.be/rMxoORO41rs)\n',
     'author': 'InioX',
     'author_email': 'justimnix@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['matugen']
 package_data = \ {'': ['*']} install_requires = \ ['material-color-utilities-
 python==0.1.5', 'rich>=12.5.1,<13.0.0'] entry_points = \ {'console_scripts':
 ['matugen = matugen.__main__:main']} setup_kwargs = { 'name': 'matugen',
-'version': '0.3.0', 'description': '', 'long_description': '
+'version': '0.4.0', 'description': '', 'long_description': '
 \n [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                          4fe9-9ee5-a1a1395d70dc.png]\n
                              ****** Matugen ******
                                       \n
 \n \n
               \n A material you color generation tool for linux\n
 \n\n
```

### Comparing `matugen-0.3.0/PKG-INFO` & `matugen-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matugen
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: InioX
 Author-email: justimnix@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: matugen Version: 0.3.0 Summary: Author: InioX
+Metadata-Version: 2.1 Name: matugen Version: 0.4.0 Summary: Author: InioX
 Author-email: justimnix@gmail.com Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 material-color-utilities-python (==0.1.5) Requires-Dist: rich
 (>=12.5.1,<13.0.0) Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/81521595/226138807-db504bdf-4eb5-
                           4fe9-9ee5-a1a1395d70dc.png]
```

