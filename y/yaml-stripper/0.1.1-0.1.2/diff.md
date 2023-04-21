# Comparing `tmp/yaml-stripper-0.1.1.tar.gz` & `tmp/yaml-stripper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-0.1.1.tar", last modified: Fri Apr 21 19:13:53 2023, max compression
+gzip compressed data, was "yaml-stripper-0.1.2.tar", last modified: Fri Apr 21 19:19:10 2023, max compression
```

## Comparing `yaml-stripper-0.1.1.tar` & `yaml-stripper-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:13:53.379649 yaml-stripper-0.1.1/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:13:53.379508 yaml-stripper-0.1.1/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.1/README.md
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:13:53.379704 yaml-stripper-0.1.1/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1081 2023-04-21 19:13:06.000000 yaml-stripper-0.1.1/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:13:53.379300 yaml-stripper-0.1.1/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      206 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       53 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:19:10.519307 yaml-stripper-0.1.2/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:19:10.519182 yaml-stripper-0.1.2/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.2/README.md
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:19:10.519349 yaml-stripper-0.1.2/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1081 2023-04-21 19:18:49.000000 yaml-stripper-0.1.2/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:19:10.519002 yaml-stripper-0.1.2/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:19:10.000000 yaml-stripper-0.1.2/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      206 2023-04-21 19:19:10.000000 yaml-stripper-0.1.2/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:19:10.000000 yaml-stripper-0.1.2/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       53 2023-04-21 19:19:10.000000 yaml-stripper-0.1.2/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:19:10.000000 yaml-stripper-0.1.2/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-0.1.1/PKG-INFO` & `yaml-stripper-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

### Comparing `yaml-stripper-0.1.1/README.md` & `yaml-stripper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.1/setup.py` & `yaml-stripper-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yaml-stripper",
-    version="0.1.1",
+    version="0.1.2",
     author="Wagner Silva",
     author_email="wra.silva@gmail.com",
     description="A command-line tool for removing specified fields from YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your_username/yaml-stripper",
     packages=setuptools.find_packages(),
```

### Comparing `yaml-stripper-0.1.1/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-0.1.2/yaml_stripper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

