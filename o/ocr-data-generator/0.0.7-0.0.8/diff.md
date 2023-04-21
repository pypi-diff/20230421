# Comparing `tmp/ocr_data_generator-0.0.7.tar.gz` & `tmp/ocr_data_generator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_data_generator-0.0.7.tar", last modified: Tue Apr 18 19:13:53 2023, max compression
+gzip compressed data, was "ocr_data_generator-0.0.8.tar", last modified: Fri Apr 21 17:22:23 2023, max compression
```

## Comparing `ocr_data_generator-0.0.7.tar` & `ocr_data_generator-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/ocr_data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/background_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/font_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/foreground_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/painter.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/sample_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 19:13:41.000000 ocr_data_generator-0.0.7/src/ocr_data_generator/word_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:13:53.894967 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 19:13:53.000000 ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:22:23.261281 ocr_data_generator-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-21 17:22:23.261281 ocr_data_generator-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-21 17:22:23.261281 ocr_data_generator-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:22:23.257281 ocr_data_generator-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:22:23.261281 ocr_data_generator-0.0.8/src/ocr_data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/background_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/font_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/foreground_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/painter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/random_layout_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/sample_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-21 17:22:12.000000 ocr_data_generator-0.0.8/src/ocr_data_generator/word_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:22:23.261281 ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-21 17:22:23.000000 ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-21 17:22:23.000000 ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:22:23.000000 ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 17:22:23.000000 ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/top_level.txt
```

### Comparing `ocr_data_generator-0.0.7/LICENSE` & `ocr_data_generator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/PKG-INFO` & `ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocr_data_generator
-Version: 0.0.7
+Name: ocr-data-generator
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: baiyigali
 Author-email: 1304646911@qq.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ocr_data_generator-0.0.7/setup.cfg` & `ocr_data_generator-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/setup.py` & `ocr_data_generator-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/background_generator.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/background_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/drawer.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/drawer.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/font_generator.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/font_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/foreground_generator.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/foreground_generator.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/painter.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/painter.py`

 * *Files identical despite different names*

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator/sample_generator.py` & `ocr_data_generator-0.0.8/src/ocr_data_generator/sample_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from .background_generator import BackgroundGenerator
 from .foreground_generator import ForegroundGenerator
+from ocr_data_generator.random_layout_generator import RandomLayoutGenerator
 from .painter import Painter
 from .drawer import Drawer
 
 class SampleGenerator:
-    def __init__(self, back_cfg, fore_cfg, paint_cfg, draw_cfg):
+    def __init__(self, back_cfg, fore_cfg, paint_cfg, draw_cfg, cfg={}):
         self.background_generator = BackgroundGenerator(back_cfg)
-        self.foreground_generator = ForegroundGenerator(fore_cfg)
+
+        layout_generator = cfg.get('layout_generator', None)
+        if layout_generator=='RandomLayoutGenerator':
+            self.foreground_generator = RandomLayoutGenerator(fore_cfg)
+        else:
+            self.foreground_generator = ForegroundGenerator(fore_cfg)
         self.painter = Painter(paint_cfg)
         self.drawer = Drawer(draw_cfg)
 
     def generate_raw(self):
         background = self.background_generator.generate()
         foreground = self.foreground_generator.generate()
         background, foreground = self.painter.paint(background, foreground)
```

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/PKG-INFO` & `ocr_data_generator-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocr-data-generator
-Version: 0.0.7
+Name: ocr_data_generator
+Version: 0.0.8
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: baiyigali
 Author-email: 1304646911@qq.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ocr_data_generator-0.0.7/src/ocr_data_generator.egg-info/SOURCES.txt` & `ocr_data_generator-0.0.8/src/ocr_data_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 setup.py
 src/ocr_data_generator/__init__.py
 src/ocr_data_generator/background_generator.py
 src/ocr_data_generator/drawer.py
 src/ocr_data_generator/font_generator.py
 src/ocr_data_generator/foreground_generator.py
 src/ocr_data_generator/painter.py
+src/ocr_data_generator/random_layout_generator.py
 src/ocr_data_generator/sample_generator.py
 src/ocr_data_generator/word_generator.py
 src/ocr_data_generator.egg-info/PKG-INFO
 src/ocr_data_generator.egg-info/SOURCES.txt
 src/ocr_data_generator.egg-info/dependency_links.txt
 src/ocr_data_generator.egg-info/top_level.txt
```

