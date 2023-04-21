# Comparing `tmp/django-mapper-1.1.8.tar.gz` & `tmp/django-mapper-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.8.tar", last modified: Fri Apr 21 06:24:22 2023, max compression
+gzip compressed data, was "django-mapper-1.1.9.tar", last modified: Fri Apr 21 07:25:49 2023, max compression
```

## Comparing `django-mapper-1.1.8.tar` & `django-mapper-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 06:24:22.155055 django-mapper-1.1.8/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.8/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.8/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     5026 2023-04-21 06:20:41.000000 django-mapper-1.1.8/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-21 06:24:22.155055 django-mapper-1.1.8/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-21 06:21:15.000000 django-mapper-1.1.8/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 07:25:49.284927 django-mapper-1.1.9/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 07:25:49.284927 django-mapper-1.1.9/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.9/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 07:25:49.284927 django-mapper-1.1.9/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.9/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     5026 2023-04-21 07:18:38.000000 django-mapper-1.1.9/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 07:25:49.284927 django-mapper-1.1.9/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 07:25:49.000000 django-mapper-1.1.9/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-21 07:25:49.000000 django-mapper-1.1.9/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-21 07:25:49.000000 django-mapper-1.1.9/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-21 07:25:49.000000 django-mapper-1.1.9/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-21 07:25:49.000000 django-mapper-1.1.9/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-21 07:25:49.284927 django-mapper-1.1.9/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-21 07:25:44.000000 django-mapper-1.1.9/setup.py
```

### Comparing `django-mapper-1.1.8/PKG-INFO` & `django-mapper-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.8
+Version: 1.1.9
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.8/django_mapper/mapper.py` & `django-mapper-1.1.9/django_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `django-mapper-1.1.8/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.9/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.8
+Version: 1.1.9
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.8/setup.py` & `django-mapper-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.8',
+    version='1.1.9',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

