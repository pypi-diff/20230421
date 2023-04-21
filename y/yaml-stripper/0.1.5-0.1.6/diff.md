# Comparing `tmp/yaml-stripper-0.1.5.tar.gz` & `tmp/yaml-stripper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-0.1.5.tar", last modified: Fri Apr 21 19:39:36 2023, max compression
+gzip compressed data, was "yaml-stripper-0.1.6.tar", last modified: Fri Apr 21 19:43:06 2023, max compression
```

## Comparing `yaml-stripper-0.1.5.tar` & `yaml-stripper-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:39:36.859598 yaml-stripper-0.1.5/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:39:36.859418 yaml-stripper-0.1.5/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.5/README.md
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:39:36.859640 yaml-stripper-0.1.5/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1095 2023-04-21 19:39:32.000000 yaml-stripper-0.1.5/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:39:36.858016 yaml-stripper-0.1.5/test/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1717 2023-04-21 19:34:30.000000 yaml-stripper-0.1.5/test/test_yaml_stripper.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:39:36.858531 yaml-stripper-0.1.5/yaml_stripper/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-0.1.5/yaml_stripper/__init__.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      851 2023-04-21 19:32:46.000000 yaml-stripper-0.1.5/yaml_stripper/cli.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1161 2023-04-21 19:16:58.000000 yaml-stripper-0.1.5/yaml_stripper/yaml_stripper.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:39:36.859228 yaml-stripper-0.1.5/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:39:36.000000 yaml-stripper-0.1.5/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      311 2023-04-21 19:39:36.000000 yaml-stripper-0.1.5/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:39:36.000000 yaml-stripper-0.1.5/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       67 2023-04-21 19:39:36.000000 yaml-stripper-0.1.5/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       14 2023-04-21 19:39:36.000000 yaml-stripper-0.1.5/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:43:06.911917 yaml-stripper-0.1.6/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:43:06.911615 yaml-stripper-0.1.6/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.6/README.md
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:43:06.912759 yaml-stripper-0.1.6/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1174 2023-04-21 19:42:46.000000 yaml-stripper-0.1.6/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:43:06.908366 yaml-stripper-0.1.6/test/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1717 2023-04-21 19:34:30.000000 yaml-stripper-0.1.6/test/test_yaml_stripper.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:43:06.908918 yaml-stripper-0.1.6/yaml_stripper/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-0.1.6/yaml_stripper/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      851 2023-04-21 19:32:46.000000 yaml-stripper-0.1.6/yaml_stripper/cli.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1161 2023-04-21 19:16:58.000000 yaml-stripper-0.1.6/yaml_stripper/yaml_stripper.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:43:06.911008 yaml-stripper-0.1.6/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      347 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       67 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       27 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/requires.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       14 2023-04-21 19:43:06.000000 yaml-stripper-0.1.6/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-0.1.5/PKG-INFO` & `yaml-stripper-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

### Comparing `yaml-stripper-0.1.5/README.md` & `yaml-stripper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.5/setup.py` & `yaml-stripper-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yaml-stripper",
-    version="0.1.5",
+    version="0.1.6",
     author="Wagner Silva",
     author_email="wra.silva@gmail.com",
     description="A command-line tool for removing specified fields from YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/your_username/yaml-stripper",
     packages=setuptools.find_packages(),
@@ -18,14 +18,18 @@
         "Documentation": "https://github.com/vavasilva/YamlStripper",
         "Source Code": "https://github.com/vavasilva/YamlStripper",
         "Homepage": "https://github.com/vavasilva/YamlStripper"
     },
     entry_points={
         'console_scripts': ['yaml-stripper=yaml_stripper.yaml_stripper:main'],
     },
+    install_requires=[
+        'PyYAML>=5.3.1',
+        'click>=8.0.0',
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `yaml-stripper-0.1.5/test/test_yaml_stripper.py` & `yaml-stripper-0.1.6/test/test_yaml_stripper.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.5/yaml_stripper/cli.py` & `yaml-stripper-0.1.6/yaml_stripper/cli.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.5/yaml_stripper/yaml_stripper.py` & `yaml-stripper-0.1.6/yaml_stripper/yaml_stripper.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.5/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-0.1.6/yaml_stripper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/your_username/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

