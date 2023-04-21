# Comparing `tmp/yeref-0.1.30.tar.gz` & `tmp/yeref-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.30.tar", last modified: Thu Mar 23 15:21:32 2023, max compression
+gzip compressed data, was "yeref-0.1.31.tar", last modified: Fri Apr 21 16:33:32 2023, max compression
```

## Comparing `yeref-0.1.30.tar` & `yeref-0.1.31.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-23 15:21:32.817544 yeref-0.1.30/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-03-23 15:21:32.820052 yeref-0.1.30/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-03-23 15:21:32.822251 yeref-0.1.30/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1105 2023-03-23 15:21:30.000000 yeref-0.1.30/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-23 15:21:32.804787 yeref-0.1.30/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       21 2022-09-17 12:40:01.000000 yeref-0.1.30/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   140705 2023-03-22 10:58:20.000000 yeref-0.1.30/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-23 15:21:32.816797 yeref-0.1.30/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-03-23 15:21:32.000000 yeref-0.1.30/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      167 2023-03-23 15:21:32.000000 yeref-0.1.30/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-03-23 15:21:32.000000 yeref-0.1.30/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-03-23 15:21:32.000000 yeref-0.1.30/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.155248 yeref-0.1.31/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 16:33:32.155480 yeref-0.1.31/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 16:33:32.156654 yeref-0.1.31/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-04-21 16:33:19.000000 yeref-0.1.31/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.145733 yeref-0.1.31/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       21 2022-09-17 12:40:01.000000 yeref-0.1.31/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   241961 2023-04-20 14:54:58.000000 yeref-0.1.31/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.154456 yeref-0.1.31/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      167 2023-04-21 16:33:32.000000 yeref-0.1.31/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.30/setup.py` & `yeref-0.1.31/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.30',
+      version='0.1.31',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -15,14 +15,15 @@
       #       "oauth2client>=4.1.3",
       #       "google-api-python-client>=2.61.0",
       #       "telegraph>=2.1.0",
       #       "setuptools>=65.3.0",
       # ]
 )
 
+
 # from distutils.core import setup
 # from setuptools import setup, find_packages
 # setup(
 #       name='yeref',
 #       version='0.0.1',
 #       description='desc-f',
 #       author='john smith',
@@ -34,8 +35,8 @@
 # python setup.py sdist
 # python setup.py install
 # python setup.py develop
 # twine upload dist/*
 # python3 -m pip install --upgrade yeref
 
 # python setup.py bdist_wheel
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.29-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.31-py3-none-any.whl
```

