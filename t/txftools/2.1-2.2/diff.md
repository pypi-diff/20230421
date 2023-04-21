# Comparing `tmp/txftools-2.1.tar.gz` & `tmp/txftools-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txftools-2.1.tar", last modified: Mon Jul 25 12:19:26 2022, max compression
+gzip compressed data, was "txftools-2.2.tar", last modified: Fri Apr 21 01:44:32 2023, max compression
```

## Comparing `txftools-2.1.tar` & `txftools-2.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-07-25 12:19:26.855872 txftools-2.1/
--rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.1/LICENSE
--rw-rw-rw-   0        0        0      427 2022-07-25 12:19:26.855872 txftools-2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-07-25 12:19:26.855872 txftools-2.1/setup.cfg
--rw-rw-rw-   0        0        0      878 2022-07-25 12:17:56.000000 txftools-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-25 12:19:26.824633 txftools-2.1/txftools/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.1/txftools/__init__.py
--rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.1/txftools/currency_sorted.py
--rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.1/txftools/execute_redis.py
--rw-rw-rw-   0        0        0    21749 2022-07-05 10:56:21.000000 txftools-2.1/txftools/format_data.py
--rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.1/txftools/province.py
--rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.1/txftools/send_emals.py
--rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.1/txftools/ssh_online.py
--rw-rw-rw-   0        0        0    13082 2022-07-15 05:24:00.000000 txftools-2.1/txftools/timer.py
-drwxrwxrwx   0        0        0        0 2022-07-25 12:19:26.855872 txftools-2.1/txftools.egg-info/
--rw-rw-rw-   0        0        0      427 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.1/txftools.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.419455 txftools-2.2/
+-rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.2/LICENSE
+-rw-rw-rw-   0        0        0      427 2023-04-21 01:44:32.419455 txftools-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:44:32.419455 txftools-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-04-21 01:44:11.000000 txftools-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.403497 txftools-2.2/txftools/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.2/txftools/__init__.py
+-rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.2/txftools/currency_sorted.py
+-rw-rw-rw-   0        0        0     9164 2023-04-21 01:42:35.000000 txftools-2.2/txftools/encryption.py
+-rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.2/txftools/execute_redis.py
+-rw-rw-rw-   0        0        0    23966 2023-01-14 06:53:46.000000 txftools-2.2/txftools/format_data.py
+-rw-rw-rw-   0        0        0     4800 2022-11-21 03:28:29.000000 txftools-2.2/txftools/lazy_test.py
+-rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.2/txftools/province.py
+-rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.2/txftools/send_emals.py
+-rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.2/txftools/ssh_online.py
+-rw-rw-rw-   0        0        0    13082 2022-07-15 05:24:00.000000 txftools-2.2/txftools/timer.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.418458 txftools-2.2/txftools.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.2/txftools.egg-info/zip-safe
```

### Comparing `txftools-2.1/LICENSE` & `txftools-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `txftools-2.1/setup.py` & `txftools-2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(name='txftools',  # 名字
-      version='2.1',  # 版本
+      version='2.2',  # 版本
       long_description_content_type="text/markdown",
       long_description='README',
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
       ],
       url='https://github.com/txf402066270/txf_tools',  # git的目录
       author='wu-di-tian-ge-ge',  # 作者
       author_email='402066270@qq.com',  # 邮箱方便交流
       license='NEU',  #
       packages=find_packages(),  # 默认
       zip_safe=True,  # 默认
-      install_requires=['django_redis', 'python-dateutil']  # 需要的包
+      install_requires=['django_redis', 'python-dateutil', 'pycryptodomex', 'rsa']  # 需要的包
       )
```

### Comparing `txftools-2.1/txftools/__init__.py` & `txftools-2.2/txftools/__init__.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/currency_sorted.py` & `txftools-2.2/txftools/currency_sorted.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/execute_redis.py` & `txftools-2.2/txftools/execute_redis.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/province.py` & `txftools-2.2/txftools/province.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/send_emals.py` & `txftools-2.2/txftools/send_emals.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/ssh_online.py` & `txftools-2.2/txftools/ssh_online.py`

 * *Files identical despite different names*

### Comparing `txftools-2.1/txftools/timer.py` & `txftools-2.2/txftools/timer.py`

 * *Files identical despite different names*

