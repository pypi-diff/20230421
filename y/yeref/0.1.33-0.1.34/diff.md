# Comparing `tmp/yeref-0.1.33.tar.gz` & `tmp/yeref-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.33.tar", last modified: Fri Apr 21 17:01:36 2023, max compression
+gzip compressed data, was "yeref-0.1.34.tar", last modified: Fri Apr 21 17:52:57 2023, max compression
```

## Comparing `yeref-0.1.33.tar` & `yeref-0.1.34.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.162832 yeref-0.1.33/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:01:36.162977 yeref-0.1.33/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 17:01:36.163552 yeref-0.1.33/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-04-21 16:53:09.000000 yeref-0.1.33/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.156404 yeref-0.1.33/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       21 2022-09-17 12:40:01.000000 yeref-0.1.33/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.33/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.162447 yeref-0.1.33/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      167 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.555632 yeref-0.1.34/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:52:57.555881 yeref-0.1.34/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 17:52:57.556519 yeref-0.1.34/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1125 2023-04-21 17:52:14.000000 yeref-0.1.34/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.549806 yeref-0.1.34/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.34/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1243 2023-04-21 17:51:37.000000 yeref-0.1.34/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.34/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:52:57.555014 yeref-0.1.34/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 17:52:57.000000 yeref-0.1.34/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.33/setup.py` & `yeref-0.1.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.33',
+      version='0.1.34',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -31,12 +31,14 @@
 #       packages=find_packages(),
 #       scripts=['yeref.py']
 # )
 #
 # python setup.py sdist
 # python setup.py install
 # python setup.py develop
+
+# python -m build
 # twine upload dist/*
 # python3 -m pip install --upgrade yeref
 
 # python setup.py bdist_wheel
 # python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.33-py3-none-any.whl
```

### Comparing `yeref-0.1.33/yeref/yeref.py` & `yeref-0.1.34/yeref/yeref.py`

 * *Files identical despite different names*

