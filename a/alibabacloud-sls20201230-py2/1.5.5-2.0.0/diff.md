# Comparing `tmp/alibabacloud_sls20201230_py2-1.5.5.tar.gz` & `tmp/alibabacloud_sls20201230_py2-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sls20201230_py2-1.5.5.tar", last modified: Fri Apr 21 06:35:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_sls20201230_py2-2.0.0.tar", last modified: Fri Apr 21 07:04:18 2023, max compression
```

## Comparing `alibabacloud_sls20201230_py2-1.5.5.tar` & `alibabacloud_sls20201230_py2-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/
--rw-r--r--   0 root         (0) root         (0)     1237 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98538 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/client.py
--rw-r--r--   0 root         (0) root         (0)   258545 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2960 2023-04-21 06:35:51.000000 alibabacloud_sls20201230_py2-1.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98538 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/client.py
+-rw-r--r--   0 root         (0) root         (0)   258545 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2960 2023-04-21 07:04:18.000000 alibabacloud_sls20201230_py2-2.0.0/setup.py
```

### Comparing `alibabacloud_sls20201230_py2-1.5.5/ChangeLog.md` & `alibabacloud_sls20201230_py2-2.0.0/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-21 Version: 1.5.5
+- Incompatible changes update. 
+
 2023-03-23 Version: 1.5.4
 - Fix project api head.
 
 2023-02-22 Version: 1.5.3
 - Fix api pathname.
 
 2022-10-20 Version: 1.5.2
```

### Comparing `alibabacloud_sls20201230_py2-1.5.5/LICENSE` & `alibabacloud_sls20201230_py2-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-1.5.5/PKG-INFO` & `alibabacloud_sls20201230_py2-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sls20201230_py2
-Version: 1.5.5
+Version: 2.0.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230_py2-1.5.5/README-CN.md` & `alibabacloud_sls20201230_py2-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-1.5.5/README.md` & `alibabacloud_sls20201230_py2-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/client.py` & `alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230/models.py` & `alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sls20201230_py2-1.5.5/alibabacloud_sls20201230_py2.egg-info/PKG-INFO` & `alibabacloud_sls20201230_py2-2.0.0/alibabacloud_sls20201230_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sls20201230-py2
-Version: 1.5.5
+Version: 2.0.0
 Summary: Alibaba Cloud Log Service (20201230) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sls20201230_py2-1.5.5/setup.py` & `alibabacloud_sls20201230_py2-2.0.0/setup.py`

 * *Files identical despite different names*

