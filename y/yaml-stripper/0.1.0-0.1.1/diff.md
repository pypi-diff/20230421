# Comparing `tmp/yaml-stripper-0.1.0.tar.gz` & `tmp/yaml-stripper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-0.1.0.tar", last modified: Fri Apr 21 19:02:20 2023, max compression
+gzip compressed data, was "yaml-stripper-0.1.1.tar", last modified: Fri Apr 21 19:13:53 2023, max compression
```

## Comparing `yaml-stripper-0.1.0.tar` & `yaml-stripper-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:02:20.740874 yaml-stripper-0.1.0/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3226 2023-04-21 19:02:20.740743 yaml-stripper-0.1.0/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.0/README.md
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:02:20.740919 yaml-stripper-0.1.0/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      785 2023-04-21 18:57:10.000000 yaml-stripper-0.1.0/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:02:20.740553 yaml-stripper-0.1.0/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3226 2023-04-21 19:02:20.000000 yaml-stripper-0.1.0/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      206 2023-04-21 19:02:20.000000 yaml-stripper-0.1.0/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:02:20.000000 yaml-stripper-0.1.0/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       53 2023-04-21 19:02:20.000000 yaml-stripper-0.1.0/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:02:20.000000 yaml-stripper-0.1.0/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:13:53.379649 yaml-stripper-0.1.1/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:13:53.379508 yaml-stripper-0.1.1/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.1/README.md
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:13:53.379704 yaml-stripper-0.1.1/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1081 2023-04-21 19:13:06.000000 yaml-stripper-0.1.1/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:13:53.379300 yaml-stripper-0.1.1/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      206 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       53 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:13:53.000000 yaml-stripper-0.1.1/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-0.1.0/PKG-INFO` & `yaml-stripper-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
+Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
+Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
+Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
+Project-URL: Homepage, https://github.com/vavasilva/YamlStripper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # YamlStripper
```

### Comparing `yaml-stripper-0.1.0/README.md` & `yaml-stripper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.0/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-0.1.1/yaml_stripper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
+Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
+Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
+Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
+Project-URL: Homepage, https://github.com/vavasilva/YamlStripper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # YamlStripper
```

