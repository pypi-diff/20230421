# Comparing `tmp/alibabacloud_ecd20200930_py2-2.0.14.tar.gz` & `tmp/alibabacloud_ecd20200930_py2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ecd20200930_py2-2.0.14.tar", last modified: Fri Apr 21 03:48:39 2023, max compression
+gzip compressed data, was "dist/alibabacloud_ecd20200930_py2-2.0.7.tar", last modified: Tue Jul 12 07:46:05 2022, max compression
```

## Comparing `alibabacloud_ecd20200930_py2-2.0.14.tar` & `alibabacloud_ecd20200930_py2-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2473 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)   368297 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930/client.py
--rw-r--r--   0 root         (0) root         (0)  1390492 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2473 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-21 03:48:39.000000 alibabacloud_ecd20200930_py2-2.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      134 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   221019 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930/client.py
+-rw-r--r--   0 root         (0) root         (0)   871598 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2022-07-12 07:46:05.000000 alibabacloud_ecd20200930_py2-2.0.7/setup.py
```

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/LICENSE` & `alibabacloud_ecd20200930_py2-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/PKG-INFO` & `alibabacloud_ecd20200930_py2-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ecd20200930_py2
-Version: 2.0.14
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/README-CN.md` & `alibabacloud_ecd20200930_py2-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/README.md` & `alibabacloud_ecd20200930_py2-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/alibabacloud_ecd20200930_py2.egg-info/PKG-INFO` & `alibabacloud_ecd20200930_py2-2.0.7/alibabacloud_ecd20200930_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ecd20200930-py2
-Version: 2.0.14
+Version: 2.0.7
 Summary: Alibaba Cloud ecd (20200930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ecd20200930_py2-2.0.14/setup.py` & `alibabacloud_ecd20200930_py2-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ecd20200930_py2.
 
-Created on 21/04/2023
+Created on 12/07/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ecd20200930"
 NAME = "alibabacloud_ecd20200930_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ecd (20200930) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

