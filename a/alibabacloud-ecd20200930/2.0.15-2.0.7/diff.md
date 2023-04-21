# Comparing `tmp/alibabacloud_ecd20200930-2.0.15.tar.gz` & `tmp/alibabacloud_ecd20200930-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecd20200930-2.0.15.tar", last modified: Fri Apr 21 03:48:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ecd20200930-2.0.7.tar", last modified: Tue Jul 12 07:46:30 2022, max compression
```

## Comparing `alibabacloud_ecd20200930-2.0.15.tar` & `alibabacloud_ecd20200930-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2329 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)   847511 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930/client.py
--rw-r--r--   0 root         (0) root         (0)  1381942 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2329 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-04-21 03:48:48.000000 alibabacloud_ecd20200930-2.0.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      233 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526955 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/client.py
+-rw-r--r--   0 root         (0) root         (0)   865360 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-07-12 07:46:30.000000 alibabacloud_ecd20200930-2.0.7/setup.py
```

### Comparing `alibabacloud_ecd20200930-2.0.15/LICENSE` & `alibabacloud_ecd20200930-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.15/PKG-INFO` & `alibabacloud_ecd20200930-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ecd20200930
-Version: 2.0.15
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930-2.0.15/README-CN.md` & `alibabacloud_ecd20200930-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.15/README.md` & `alibabacloud_ecd20200930-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930-2.0.15/alibabacloud_ecd20200930.egg-info/PKG-INFO` & `alibabacloud_ecd20200930-2.0.7/alibabacloud_ecd20200930.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ecd20200930
-Version: 2.0.15
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930-2.0.15/setup.py` & `alibabacloud_ecd20200930-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecd20200930.
 
-Created on 21/04/2023
+Created on 12/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecd20200930"
 NAME = "alibabacloud_ecd20200930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ecd (20200930) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
+    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

