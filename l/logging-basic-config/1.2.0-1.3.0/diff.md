# Comparing `tmp/logging_basic_config-1.2.0.tar.gz` & `tmp/logging_basic_config-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logging_basic_config-1.2.0.tar", last modified: Thu Apr 20 21:42:03 2023, max compression
+gzip compressed data, was "dist/logging_basic_config-1.3.0.tar", last modified: Thu Apr 20 23:04:37 2023, max compression
```

## Comparing `logging_basic_config-1.2.0.tar` & `logging_basic_config-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/
--rw-r--r--   0 msantino  (1000) msantino  (1000)     1073 2023-04-20 20:50:29.000000 logging_basic_config-1.2.0/LICENSE
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/PKG-INFO
--rw-r--r--   0 msantino  (1000) msantino  (1000)      536 2023-04-20 21:02:37.000000 logging_basic_config-1.2.0/README.md
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config/
--rw-r--r--   0 msantino  (1000) msantino  (1000)       26 2023-04-20 20:55:50.000000 logging_basic_config-1.2.0/logging_basic_config/__init__.py
--rw-r--r--   0 msantino  (1000) msantino  (1000)     1240 2023-04-20 21:41:53.000000 logging_basic_config-1.2.0/logging_basic_config/config.py
-drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/PKG-INFO
--rw-rw-r--   0 msantino  (1000) msantino  (1000)      309 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/SOURCES.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/dependency_links.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/not-zip-safe
--rw-rw-r--   0 msantino  (1000) msantino  (1000)       21 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/logging_basic_config.egg-info/top_level.txt
--rw-rw-r--   0 msantino  (1000) msantino  (1000)       38 2023-04-20 21:42:03.000000 logging_basic_config-1.2.0/setup.cfg
--rw-r--r--   0 msantino  (1000) msantino  (1000)      893 2023-04-20 21:39:34.000000 logging_basic_config-1.2.0/setup.py
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/
+-rw-r--r--   0 msantino  (1000) msantino  (1000)     1073 2023-04-20 20:50:29.000000 logging_basic_config-1.3.0/LICENSE
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/PKG-INFO
+-rw-r--r--   0 msantino  (1000) msantino  (1000)      536 2023-04-20 21:02:37.000000 logging_basic_config-1.3.0/README.md
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config/
+-rw-r--r--   0 msantino  (1000) msantino  (1000)       26 2023-04-20 20:55:50.000000 logging_basic_config-1.3.0/logging_basic_config/__init__.py
+-rw-r--r--   0 msantino  (1000) msantino  (1000)     1267 2023-04-20 23:04:29.000000 logging_basic_config-1.3.0/logging_basic_config/config.py
+drwxrwxr-x   0 msantino  (1000) msantino  (1000)        0 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      997 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/PKG-INFO
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)      309 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)        1 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/not-zip-safe
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)       21 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/logging_basic_config.egg-info/top_level.txt
+-rw-rw-r--   0 msantino  (1000) msantino  (1000)       38 2023-04-20 23:04:37.000000 logging_basic_config-1.3.0/setup.cfg
+-rw-r--r--   0 msantino  (1000) msantino  (1000)      893 2023-04-20 23:04:35.000000 logging_basic_config-1.3.0/setup.py
```

### Comparing `logging_basic_config-1.2.0/LICENSE` & `logging_basic_config-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_basic_config-1.2.0/PKG-INFO` & `logging_basic_config-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging_basic_config
-Version: 1.2.0
+Version: 1.3.0
 Summary: Basic logging configurations to easily use in many projects
 Home-page: https://github.com/msantino/logging-basic-config
 Author: Marcelo Santino
 Author-email: marcelo@santino.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logging_basic_config-1.2.0/README.md` & `logging_basic_config-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `logging_basic_config-1.2.0/logging_basic_config.egg-info/PKG-INFO` & `logging_basic_config-1.3.0/logging_basic_config.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-basic-config
-Version: 1.2.0
+Version: 1.3.0
 Summary: Basic logging configurations to easily use in many projects
 Home-page: https://github.com/msantino/logging-basic-config
 Author: Marcelo Santino
 Author-email: marcelo@santino.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `logging_basic_config-1.2.0/setup.py` & `logging_basic_config-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='logging_basic_config',  
-    version='1.2.0',
+    version='1.3.0',
     author="Marcelo Santino",
     author_email="marcelo@santino.dev",
     description="Basic logging configurations to easily use in many projects",
     url='https://github.com/msantino/logging-basic-config',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```

