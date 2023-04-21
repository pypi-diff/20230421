# Comparing `tmp/yeref-0.1.34.tar.gz` & `tmp/yeref-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.34.tar", last modified: Fri Apr 21 17:52:57 2023, max compression
+gzip compressed data, was "yeref-0.1.35.tar", last modified: Fri Apr 21 18:25:49 2023, max compression
```

## Comparing `yeref-0.1.34.tar` & `yeref-0.1.35.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.555632 yeref-0.1.34/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:52:57.555881 yeref-0.1.34/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 17:52:57.556519 yeref-0.1.34/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1125 2023-04-21 17:52:14.000000 yeref-0.1.34/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.549806 yeref-0.1.34/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.34/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1243 2023-04-21 17:51:37.000000 yeref-0.1.34/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.34/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.555014 yeref-0.1.34/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.983016 yeref-0.1.35/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 18:25:49.983313 yeref-0.1.35/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 18:25:49.984854 yeref-0.1.35/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1125 2023-04-21 18:25:30.000000 yeref-0.1.35/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.979365 yeref-0.1.35/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.35/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)    40958 2023-04-21 18:21:56.000000 yeref-0.1.35/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.35/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 18:25:49.982370 yeref-0.1.35/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 18:25:49.000000 yeref-0.1.35/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.34/setup.py` & `yeref-0.1.35/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.34',
+      version='0.1.35',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -37,8 +37,8 @@
 # python setup.py develop
 
 # python -m build
 # twine upload dist/*
 # python3 -m pip install --upgrade yeref
 
 # python setup.py bdist_wheel
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.33-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.34-py3-none-any.whl
```

### Comparing `yeref-0.1.34/yeref/yeref.py` & `yeref-0.1.35/yeref/yeref.py`

 * *Files identical despite different names*

