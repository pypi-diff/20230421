# Comparing `tmp/lsptrain-0.0.42.tar.gz` & `tmp/lsptrain-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.42.tar", last modified: Fri Apr 21 02:57:13 2023, max compression
+gzip compressed data, was "lsptrain-0.0.43.tar", last modified: Fri Apr 21 02:59:27 2023, max compression
```

## Comparing `lsptrain-0.0.42.tar` & `lsptrain-0.0.43.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.915957 lsptrain-0.0.42/
--rw-rw-rw-   0        0        0      434 2023-04-21 02:57:13.914956 lsptrain-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.42/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.901956 lsptrain-0.0.42/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.42/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.910956 lsptrain-0.0.42/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.42/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6690 2023-04-21 01:57:35.000000 lsptrain-0.0.42/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.912956 lsptrain-0.0.42/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.42/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2142 2023-04-21 02:56:08.000000 lsptrain-0.0.42/lsptrain/utils/init_args.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:57:13.907957 lsptrain-0.0.42/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      434 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 02:57:13.000000 lsptrain-0.0.42/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 02:57:13.915957 lsptrain-0.0.42/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-21 02:57:03.000000 lsptrain-0.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.653886 lsptrain-0.0.43/
+-rw-rw-rw-   0        0        0      434 2023-04-21 02:59:27.652886 lsptrain-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.43/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.635885 lsptrain-0.0.43/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.43/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.646886 lsptrain-0.0.43/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0        0 2023-04-20 13:11:48.000000 lsptrain-0.0.43/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6690 2023-04-21 01:57:35.000000 lsptrain-0.0.43/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.650886 lsptrain-0.0.43/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.43/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-04-21 02:59:24.000000 lsptrain-0.0.43/lsptrain/utils/init_args.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:59:27.643887 lsptrain-0.0.43/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 02:59:27.000000 lsptrain-0.0.43/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 02:59:27.653886 lsptrain-0.0.43/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-04-21 02:59:24.000000 lsptrain-0.0.43/setup.py
```

### Comparing `lsptrain-0.0.42/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.43/lsptrain/nlp_classfication/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.42/lsptrain/utils/init_args.py` & `lsptrain-0.0.43/lsptrain/utils/init_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                         help="预训练模型名称")
     parser.add_argument("-lr", "--learning_rate", default=0.0001,
                         type=float, help="学习率")
     parser.add_argument("-o", "--optimizer", choices=["adam", "sgd"], default="adam", type=str,
                         help="模型优化函数")
     parser.add_argument("-b", "--batch_size", default=64, type=int,
                         help="训练批次大小，如果报错提示out of memory，可以适当调小")
-    parser.add_argument("-s", "save_dir", default="checkpoint", type=str,
+    parser.add_argument("-s", "--save_dir", default="checkpoint", type=str,
                         help="训练checkpoint保存路径")
     parser.add_argument("--label_file_name", default="catalog_label.txt", type=str,
                         help="保存标签路径")
     parser.add_argument("--save_best", default=False, type=bool,
                         help="是否只保存最优模型")
     parser.add_argument("--max_length", default=64, type=int,
                         help="序列最大长度，超过部分会被自动截断")
```

### Comparing `lsptrain-0.0.42/setup.py` & `lsptrain-0.0.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.42',
+      version='0.0.43',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.10',
                         'transformers>=4.20.1',
```

