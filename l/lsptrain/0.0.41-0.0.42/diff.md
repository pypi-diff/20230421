# Comparing `tmp/lsptrain-0.0.41.tar.gz` & `tmp/lsptrain-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.41.tar", last modified: Thu Apr 20 15:17:15 2023, max compression
+gzip compressed data, was "lsptrain-0.0.42.tar", last modified: Fri Apr 21 02:57:13 2023, max compression
```

## Comparing `lsptrain-0.0.41.tar` & `lsptrain-0.0.42.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.009638 lsptrain-0.0.41/
--rw-rw-rw-   0        0        0      434 2023-04-20 15:17:15.008638 lsptrain-0.0.41/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.41/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 15:17:14.995638 lsptrain-0.0.41/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.41/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.006638 lsptrain-0.0.41/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.41/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     8524 2023-04-20 14:56:41.000000 lsptrain-0.0.41/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:17:15.002638 lsptrain-0.0.41/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      434 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 15:17:14.000000 lsptrain-0.0.41/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 15:17:15.009638 lsptrain-0.0.41/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-20 15:16:29.000000 lsptrain-0.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.915957 lsptrain-0.0.42/
+-rw-rw-rw-   0        0        0      434 2023-04-21 02:57:13.914956 lsptrain-0.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.42/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.901956 lsptrain-0.0.42/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.42/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.910956 lsptrain-0.0.42/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.42/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6690 2023-04-21 01:57:35.000000 lsptrain-0.0.42/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.912956 lsptrain-0.0.42/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.42/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-04-21 02:56:08.000000 lsptrain-0.0.42/lsptrain/utils/init_args.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.907957 lsptrain-0.0.42/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 02:57:13.915957 lsptrain-0.0.42/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-21 02:57:03.000000 lsptrain-0.0.42/setup.py
```

### Comparing `lsptrain-0.0.41/setup.py` & `lsptrain-0.0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.41',
+      version='0.0.42',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.10',
                         'transformers>=4.20.1',
```

