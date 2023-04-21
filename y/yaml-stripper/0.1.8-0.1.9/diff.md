# Comparing `tmp/yaml-stripper-0.1.8.tar.gz` & `tmp/yaml-stripper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-0.1.8.tar", last modified: Fri Apr 21 19:47:55 2023, max compression
+gzip compressed data, was "yaml-stripper-0.1.9.tar", last modified: Fri Apr 21 19:48:10 2023, max compression
```

## Comparing `yaml-stripper-0.1.8.tar` & `yaml-stripper-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:47:55.247413 yaml-stripper-0.1.8/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:47:55.247218 yaml-stripper-0.1.8/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.8/README.md
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:47:55.245449 yaml-stripper-0.1.8/YamlStripper/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-0.1.8/YamlStripper/__init__.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      847 2023-04-21 19:47:42.000000 yaml-stripper-0.1.8/YamlStripper/cli.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1161 2023-04-21 19:16:58.000000 yaml-stripper-0.1.8/YamlStripper/yaml_stripper.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:47:55.247467 yaml-stripper-0.1.8/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1173 2023-04-21 19:47:51.000000 yaml-stripper-0.1.8/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:47:55.245686 yaml-stripper-0.1.8/test/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1711 2023-04-21 19:47:42.000000 yaml-stripper-0.1.8/test/test_yaml_stripper.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:47:55.246888 yaml-stripper-0.1.8/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      344 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       66 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       27 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/requires.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       13 2023-04-21 19:47:55.000000 yaml-stripper-0.1.8/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.743608 yaml-stripper-0.1.9/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:48:10.743422 yaml-stripper-0.1.9/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.9/README.md
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.742205 yaml-stripper-0.1.9/YamlStripper/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-0.1.9/YamlStripper/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      847 2023-04-21 19:47:42.000000 yaml-stripper-0.1.9/YamlStripper/cli.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1161 2023-04-21 19:16:58.000000 yaml-stripper-0.1.9/YamlStripper/yaml_stripper.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:48:10.743652 yaml-stripper-0.1.9/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1173 2023-04-21 19:47:59.000000 yaml-stripper-0.1.9/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.742417 yaml-stripper-0.1.9/test/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1711 2023-04-21 19:47:42.000000 yaml-stripper-0.1.9/test/test_yaml_stripper.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.743245 yaml-stripper-0.1.9/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      344 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       66 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       27 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/requires.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       13 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-0.1.8/PKG-INFO` & `yaml-stripper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

### Comparing `yaml-stripper-0.1.8/README.md` & `yaml-stripper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.8/YamlStripper/cli.py` & `yaml-stripper-0.1.9/YamlStripper/cli.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.8/YamlStripper/yaml_stripper.py` & `yaml-stripper-0.1.9/YamlStripper/yaml_stripper.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.8/setup.py` & `yaml-stripper-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yaml-stripper",
-    version="0.1.8",
+    version="0.1.9",
     author="Wagner Silva",
     author_email="wra.silva@gmail.com",
     description="A command-line tool for removing specified fields from YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your_username/yaml-stripper",
     packages=setuptools.find_packages(),
```

### Comparing `yaml-stripper-0.1.8/test/test_yaml_stripper.py` & `yaml-stripper-0.1.9/test/test_yaml_stripper.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.8/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-0.1.9/yaml_stripper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

