# Comparing `tmp/django-viewers-counts-middleware-0.0.1.tar.gz` & `tmp/django-viewers-counts-middleware-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-viewers-counts-middleware-0.0.1.tar", last modified: Fri Apr 21 17:23:18 2023, max compression
+gzip compressed data, was "django-viewers-counts-middleware-0.0.2.tar", last modified: Fri Apr 21 18:13:08 2023, max compression
```

## Comparing `django-viewers-counts-middleware-0.0.1.tar` & `django-viewers-counts-middleware-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 17:23:18.140155 django-viewers-counts-middleware-0.0.1/
--rw-rw-r--   0 noob      (1000) noob      (1000)      633 2023-04-21 17:23:18.136159 django-viewers-counts-middleware-0.0.1/PKG-INFO
--rw-rw-r--   0 noob      (1000) noob      (1000)      590 2023-04-21 16:57:18.000000 django-viewers-counts-middleware-0.0.1/README.md
-drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 17:23:18.136159 django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/
--rw-rw-r--   0 noob      (1000) noob      (1000)      633 2023-04-21 17:23:17.000000 django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 noob      (1000) noob      (1000)      242 2023-04-21 17:23:17.000000 django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 17:23:17.000000 django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 17:23:17.000000 django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/top_level.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)       38 2023-04-21 17:23:18.140155 django-viewers-counts-middleware-0.0.1/setup.cfg
--rw-rw-r--   0 noob      (1000) noob      (1000)      966 2023-04-21 17:22:36.000000 django-viewers-counts-middleware-0.0.1/setup.py
+drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:13:08.624064 django-viewers-counts-middleware-0.0.2/
+-rw-rw-r--   0 noob      (1000) noob      (1000)      633 2023-04-21 18:13:08.624064 django-viewers-counts-middleware-0.0.2/PKG-INFO
+-rw-rw-r--   0 noob      (1000) noob      (1000)      590 2023-04-21 16:57:18.000000 django-viewers-counts-middleware-0.0.2/README.md
+drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:13:08.624064 django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/
+-rw-rw-r--   0 noob      (1000) noob      (1000)      633 2023-04-21 18:13:08.000000 django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 noob      (1000) noob      (1000)      242 2023-04-21 18:13:08.000000 django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:13:08.000000 django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:13:08.000000 django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/top_level.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)       38 2023-04-21 18:13:08.624064 django-viewers-counts-middleware-0.0.2/setup.cfg
+-rw-rw-r--   0 noob      (1000) noob      (1000)      966 2023-04-21 18:12:27.000000 django-viewers-counts-middleware-0.0.2/setup.py
```

### Comparing `django-viewers-counts-middleware-0.0.1/PKG-INFO` & `django-viewers-counts-middleware-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-viewers-counts-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django Viewers Count Middleware get from user request
 Home-page: https://github.com/ittamil/django-viewers-counts-middleware
 Author: Hariharan
 Author-email: hari@ittamil.in
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,django,viewers count middleware,viewers count,middleware,django plugin
```

### Comparing `django-viewers-counts-middleware-0.0.1/README.md` & `django-viewers-counts-middleware-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-viewers-counts-middleware-0.0.1/django_viewers_counts_middleware.egg-info/PKG-INFO` & `django-viewers-counts-middleware-0.0.2/django_viewers_counts_middleware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-viewers-counts-middleware
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django Viewers Count Middleware get from user request
 Home-page: https://github.com/ittamil/django-viewers-counts-middleware
 Author: Hariharan
 Author-email: hari@ittamil.in
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,django,viewers count middleware,viewers count,middleware,django plugin
```

### Comparing `django-viewers-counts-middleware-0.0.1/setup.py` & `django-viewers-counts-middleware-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Django Viewers Count Middleware get from user request'
 
 # Setting up
 setup(
     name="django-viewers-counts-middleware",
     version=VERSION,
     author="Hariharan",
```

