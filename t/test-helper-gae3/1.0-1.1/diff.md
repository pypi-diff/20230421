# Comparing `tmp/test_helper_gae3-1.0.tar.gz` & `tmp/test_helper_gae3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_gae3-1.0.tar", last modified: Tue Apr 18 12:32:56 2023, max compression
+gzip compressed data, was "test_helper_gae3-1.1.tar", last modified: Fri Apr 21 10:39:12 2023, max compression
```

## Comparing `test_helper_gae3-1.0.tar` & `test_helper_gae3-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 12:32:56.187333 test_helper_gae3-1.0/
--rw-rw-rw-   0        0        0     1094 2023-04-17 15:55:38.000000 test_helper_gae3-1.0/LICENSE
--rw-rw-rw-   0        0        0       64 2023-04-17 15:59:00.000000 test_helper_gae3-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2735 2023-04-18 12:32:56.187333 test_helper_gae3-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1787 2023-04-18 12:32:10.000000 test_helper_gae3-1.0/README.md
--rw-rw-rw-   0        0        0      110 2023-02-11 14:05:41.000000 test_helper_gae3-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      655 2023-04-18 12:32:56.187333 test_helper_gae3-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 12:32:56.156082 test_helper_gae3-1.0/test_helper_gae3/
--rw-rw-rw-   0        0        0     1251 2023-04-18 11:24:42.000000 test_helper_gae3-1.0/test_helper_gae3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 12:32:56.187333 test_helper_gae3-1.0/test_helper_gae3.egg-info/
--rw-rw-rw-   0        0        0     2735 2023-04-18 12:32:56.000000 test_helper_gae3-1.0/test_helper_gae3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-18 12:32:56.000000 test_helper_gae3-1.0/test_helper_gae3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 12:32:56.000000 test_helper_gae3-1.0/test_helper_gae3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 12:32:56.000000 test_helper_gae3-1.0/test_helper_gae3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-17 15:55:38.000000 test_helper_gae3-1.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2023-04-18 12:37:07.000000 test_helper_gae3-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2735 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1787 2023-04-18 12:32:10.000000 test_helper_gae3-1.1/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-18 12:37:07.000000 test_helper_gae3-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      655 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.854644 test_helper_gae3-1.1/test_helper_gae3/
+-rw-rw-rw-   0        0        0     4497 2023-04-21 10:35:40.000000 test_helper_gae3-1.1/test_helper_gae3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/test_helper_gae3.egg-info/
+-rw-rw-rw-   0        0        0     2735 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/top_level.txt
```

### Comparing `test_helper_gae3-1.0/LICENSE` & `test_helper_gae3-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `test_helper_gae3-1.0/PKG-INFO` & `test_helper_gae3-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_helper_gae3
-Version: 1.0
+Version: 1.1
 Summary: Class for autotests GoogleAppEngine python3 app.
 Home-page: https://github.com/vb64/test.helper.gae3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.gae3/issues
 Description: # Class for autotests GoogleAppEngine Python3 app.
```

### Comparing `test_helper_gae3-1.0/README.md` & `test_helper_gae3-1.1/README.md`

 * *Files identical despite different names*

### Comparing `test_helper_gae3-1.0/setup.cfg` & `test_helper_gae3-1.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f67   = test_helper_g
 00000020: 6165 330d 0a76 6572 7369 6f6e 203d 2031  ae3..version = 1
-00000030: 2e30 0d0a 6175 7468 6f72 203d 2056 6974  .0..author = Vit
+00000030: 2e31 0d0a 6175 7468 6f72 203d 2056 6974  .1..author = Vit
 00000040: 616c 7920 426f 676f 6d6f 6c6f 760d 0a61  aly Bogomolov..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6d61  uthor_email = ma
 00000060: 696c 4076 6974 616c 792d 626f 676f 6d6f  il@vitaly-bogomo
 00000070: 6c6f 762e 7275 0d0a 6465 7363 7269 7074  lov.ru..descript
 00000080: 696f 6e20 3d20 436c 6173 7320 666f 7220  ion = Class for 
 00000090: 6175 746f 7465 7374 7320 476f 6f67 6c65  autotests Google
 000000a0: 4170 7045 6e67 696e 6520 7079 7468 6f6e  AppEngine python
```

### Comparing `test_helper_gae3-1.0/test_helper_gae3.egg-info/PKG-INFO` & `test_helper_gae3-1.1/test_helper_gae3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-helper-gae3
-Version: 1.0
+Version: 1.1
 Summary: Class for autotests GoogleAppEngine python3 app.
 Home-page: https://github.com/vb64/test.helper.gae3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.gae3/issues
 Description: # Class for autotests GoogleAppEngine Python3 app.
```

