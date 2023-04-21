# Comparing `tmp/django-viewers-counts-middleware-0.0.3.tar.gz` & `tmp/django-viewers-counts-middleware-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-viewers-counts-middleware-0.0.3.tar", last modified: Fri Apr 21 18:22:49 2023, max compression
+gzip compressed data, was "django-viewers-counts-middleware-0.0.4.tar", last modified: Fri Apr 21 18:26:10 2023, max compression
```

## Comparing `django-viewers-counts-middleware-0.0.3.tar` & `django-viewers-counts-middleware-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:22:49.423133 django-viewers-counts-middleware-0.0.3/
--rw-rw-r--   0 noob      (1000) noob      (1000)      681 2023-04-21 18:22:49.423133 django-viewers-counts-middleware-0.0.3/PKG-INFO
--rw-rw-r--   0 noob      (1000) noob      (1000)      590 2023-04-21 16:57:18.000000 django-viewers-counts-middleware-0.0.3/README.md
-drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:22:49.423133 django-viewers-counts-middleware-0.0.3/django_viewers_counts_middleware.egg-info/
--rw-rw-r--   0 noob      (1000) noob      (1000)      681 2023-04-21 18:22:49.000000 django-viewers-counts-middleware-0.0.3/django_viewers_counts_middleware.egg-info/PKG-INFO
--rw-rw-r--   0 noob      (1000) noob      (1000)      242 2023-04-21 18:22:49.000000 django-viewers-counts-middleware-0.0.3/django_viewers_counts_middleware.egg-info/SOURCES.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:22:49.000000 django-viewers-counts-middleware-0.0.3/django_viewers_counts_middleware.egg-info/dependency_links.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:22:49.000000 django-viewers-counts-middleware-0.0.3/django_viewers_counts_middleware.egg-info/top_level.txt
--rw-rw-r--   0 noob      (1000) noob      (1000)       38 2023-04-21 18:22:49.423133 django-viewers-counts-middleware-0.0.3/setup.cfg
--rw-rw-r--   0 noob      (1000) noob      (1000)     1061 2023-04-21 18:17:56.000000 django-viewers-counts-middleware-0.0.3/setup.py
+drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:26:10.612249 django-viewers-counts-middleware-0.0.4/
+-rw-rw-r--   0 noob      (1000) noob      (1000)     1584 2023-04-21 18:26:10.608249 django-viewers-counts-middleware-0.0.4/PKG-INFO
+-rw-rw-r--   0 noob      (1000) noob      (1000)      590 2023-04-21 16:57:18.000000 django-viewers-counts-middleware-0.0.4/README.md
+drwxrwxr-x   0 noob      (1000) noob      (1000)        0 2023-04-21 18:26:10.608249 django-viewers-counts-middleware-0.0.4/django_viewers_counts_middleware.egg-info/
+-rw-rw-r--   0 noob      (1000) noob      (1000)     1584 2023-04-21 18:26:10.000000 django-viewers-counts-middleware-0.0.4/django_viewers_counts_middleware.egg-info/PKG-INFO
+-rw-rw-r--   0 noob      (1000) noob      (1000)      242 2023-04-21 18:26:10.000000 django-viewers-counts-middleware-0.0.4/django_viewers_counts_middleware.egg-info/SOURCES.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:26:10.000000 django-viewers-counts-middleware-0.0.4/django_viewers_counts_middleware.egg-info/dependency_links.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)        1 2023-04-21 18:26:10.000000 django-viewers-counts-middleware-0.0.4/django_viewers_counts_middleware.egg-info/top_level.txt
+-rw-rw-r--   0 noob      (1000) noob      (1000)       38 2023-04-21 18:26:10.612249 django-viewers-counts-middleware-0.0.4/setup.cfg
+-rw-rw-r--   0 noob      (1000) noob      (1000)     1148 2023-04-21 18:25:52.000000 django-viewers-counts-middleware-0.0.4/setup.py
```

### Comparing `django-viewers-counts-middleware-0.0.3/README.md` & `django-viewers-counts-middleware-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-viewers-counts-middleware-0.0.3/setup.py` & `django-viewers-counts-middleware-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Django Viewers Count Middleware get from user request'
+with open("README.md", "r", encoding = "utf-8") as fh:
+    long_description = fh.read()
 
 # Setting up
 setup(
     name="django-viewers-counts-middleware",
     version=VERSION,
     author="Hariharan",
     author_email="hari@ittamil.in",
     description=DESCRIPTION,
-    long_description = "file: README.md",
+    long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/ittamil/django-viewers-counts-middleware",
     packages=find_packages(),
     keywords=['python', 'django', 'viewers count middleware', 'viewers count', 'middleware', 'django plugin'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

