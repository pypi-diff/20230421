# Comparing `tmp/alibabacloud_sls20201230-1.5.8.tar.gz` & `tmp/alibabacloud_sls20201230-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sls20201230-1.5.8.tar", last modified: Wed Feb  8 03:35:22 2023, max compression
+gzip compressed data, was "dist/alibabacloud_sls20201230-1.5.9.tar", last modified: Wed Feb  8 04:01:46 2023, max compression
```

## Comparing `alibabacloud_sls20201230-1.5.8.tar` & `alibabacloud_sls20201230-1.5.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2336 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/__init__.py
--rw-r--r--   0 root         (0) root         (0)   279653 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/client.py
--rw-r--r--   0 root         (0) root         (0)   326964 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2336 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-08 03:35:22.000000 alibabacloud_sls20201230-1.5.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2663 2023-02-08 03:35:21.000000 alibabacloud_sls20201230-1.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   279653 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/client.py
+-rw-r--r--   0 root         (0) root         (0)   326964 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2336 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      193 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-02-08 04:01:46.000000 alibabacloud_sls20201230-1.5.9/setup.py
```

### Comparing `alibabacloud_sls20201230-1.5.8/ChangeLog.md` & `alibabacloud_sls20201230-1.5.9/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-02-08 Version: 1.5.8
+- Add productType to logstore API.
+
 2023-02-07 Version: 1.5.7
 - Add productType to logstore API.
 
 2023-02-06 Version: 1.5.6
 - Add productType to logstore API.
 
 2023-02-03 Version: 1.5.5
```

### Comparing `alibabacloud_sls20201230-1.5.8/LICENSE` & `alibabacloud_sls20201230-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-1.5.8/PKG-INFO` & `alibabacloud_sls20201230-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sls20201230
-Version: 1.5.8
+Version: 1.5.9
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230-1.5.8/README-CN.md` & `alibabacloud_sls20201230-1.5.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-1.5.8/README.md` & `alibabacloud_sls20201230-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/client.py` & `alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230/models.py` & `alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230-1.5.8/alibabacloud_sls20201230.egg-info/PKG-INFO` & `alibabacloud_sls20201230-1.5.9/alibabacloud_sls20201230.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sls20201230
-Version: 1.5.8
+Version: 1.5.9
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230-1.5.8/setup.py` & `alibabacloud_sls20201230-1.5.9/setup.py`

 * *Files identical despite different names*

