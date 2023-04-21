# Comparing `tmp/lsptrain-0.0.43.tar.gz` & `tmp/lsptrain-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.43.tar", last modified: Fri Apr 21 02:59:27 2023, max compression
+gzip compressed data, was "lsptrain-0.0.44.tar", last modified: Fri Apr 21 03:35:32 2023, max compression
```

## Comparing `lsptrain-0.0.43.tar` & `lsptrain-0.0.44.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.653886 lsptrain-0.0.43/
--rw-rw-rw-   0        0        0      434 2023-04-21 02:59:27.652886 lsptrain-0.0.43/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.43/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.635885 lsptrain-0.0.43/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.43/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.646886 lsptrain-0.0.43/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.43/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6690 2023-04-21 01:57:35.000000 lsptrain-0.0.43/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.650886 lsptrain-0.0.43/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.43/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-04-21 02:59:24.000000 lsptrain-0.0.43/lsptrain/utils/init_args.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.643887 lsptrain-0.0.43/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      434 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 02:59:27.653886 lsptrain-0.0.43/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-21 02:59:24.000000 lsptrain-0.0.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:35:32.849207 lsptrain-0.0.44/
+-rw-rw-rw-   0        0        0      434 2023-04-21 03:35:32.848205 lsptrain-0.0.44/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.44/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 03:35:32.835205 lsptrain-0.0.44/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.44/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:35:32.844205 lsptrain-0.0.44/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.44/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6690 2023-04-21 01:57:35.000000 lsptrain-0.0.44/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:35:32.846205 lsptrain-0.0.44/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.44/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-04-21 02:59:24.000000 lsptrain-0.0.44/lsptrain/utils/init_args.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:35:32.841205 lsptrain-0.0.44/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-21 03:35:32.000000 lsptrain-0.0.44/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-21 03:35:32.000000 lsptrain-0.0.44/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:35:32.000000 lsptrain-0.0.44/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-21 03:35:32.000000 lsptrain-0.0.44/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 03:35:32.000000 lsptrain-0.0.44/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 03:35:32.849207 lsptrain-0.0.44/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-21 03:35:02.000000 lsptrain-0.0.44/setup.py
```

### Comparing `lsptrain-0.0.43/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.44/lsptrain/nlp_classfication/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.43/lsptrain/utils/init_args.py` & `lsptrain-0.0.44/lsptrain/utils/init_args.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.43/setup.py` & `lsptrain-0.0.44/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.43',
+      version='0.0.44',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
-      install_requires=['torch>=1.10',
+      install_requires=['torch>=1.11.0',
                         'transformers>=4.20.1',
                         'scikit-learn>=1.1.0',
                         'tqdm'],
       python_requires='>=3.7',
       license='BSD License',
       packages=find_packages(),
       platforms=['all'],
```

