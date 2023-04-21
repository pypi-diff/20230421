# Comparing `tmp/resotoeventlog-3.3.2.tar.gz` & `tmp/resotoeventlog-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoeventlog-3.3.2.tar", last modified: Fri Apr 14 16:14:13 2023, max compression
+gzip compressed data, was "resotoeventlog-3.3.3.tar", last modified: Fri Apr 21 14:37:43 2023, max compression
```

## Comparing `resotoeventlog-3.3.2.tar` & `resotoeventlog-3.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/resotoeventlog/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/resotoeventlog/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/logs/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/resotoeventlog/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/resotoeventlog/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/resotoeventlog/web/directives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:14:13.756357 resotoeventlog-3.3.2/resotoeventlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:14:13.000000 resotoeventlog-3.3.2/resotoeventlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-14 16:14:13.760357 resotoeventlog-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 16:12:48.000000 resotoeventlog-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/resotoeventlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/resotoeventlog/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/logs/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/resotoeventlog/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/resotoeventlog/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/resotoeventlog/web/directives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/resotoeventlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 14:37:43.000000 resotoeventlog-3.3.3/resotoeventlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-21 14:37:43.166362 resotoeventlog-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-21 14:35:51.000000 resotoeventlog-3.3.3/setup.py
```

### Comparing `resotoeventlog-3.3.2/resotoeventlog/__main__.py` & `resotoeventlog-3.3.3/resotoeventlog/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/resotoeventlog/logs/log_handler.py` & `resotoeventlog-3.3.3/resotoeventlog/logs/log_handler.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/resotoeventlog/model.py` & `resotoeventlog-3.3.3/resotoeventlog/model.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/resotoeventlog/web/api.py` & `resotoeventlog-3.3.3/resotoeventlog/web/api.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/resotoeventlog/web/directives.py` & `resotoeventlog-3.3.3/resotoeventlog/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/resotoeventlog.egg-info/SOURCES.txt` & `resotoeventlog-3.3.3/resotoeventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/setup.cfg` & `resotoeventlog-3.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `resotoeventlog-3.3.2/setup.py` & `resotoeventlog-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return [str(requirement) for requirement in pkg_resources.parse_requirements(read(fname))]
 
 
 setup_requirements = ["pytest-runner"]
 
 setup(
     name="resotoeventlog",
-    version="3.3.2",
+    version="3.3.3",
     description="Event log aggregator for resoto.",
     python_requires=">=3.5",
     classifiers=["Programming Language :: Python :: 3"],
     entry_points={"console_scripts": ["resotoeventlog=resotoeventlog.__main__:main"]},
     install_requires=read_requirements("requirements.txt"),
     license="Apache Software License 2.0",
     long_description=read("README.md"),
```

