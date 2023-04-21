# Comparing `tmp/xbox-sdk-0.0.5.tar.gz` & `tmp/xbox-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox-sdk-0.0.5.tar", last modified: Fri Apr 21 08:32:42 2023, max compression
+gzip compressed data, was "xbox-sdk-0.0.6.tar", last modified: Fri Apr 21 08:56:28 2023, max compression
```

## Comparing `xbox-sdk-0.0.5.tar` & `xbox-sdk-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/
--rw-rw-rw-   0        0        0     1095 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      645 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-21 08:32:21.000000 xbox-sdk-0.0.5/README.md
--rw-rw-rw-   0        0        0      535 2023-04-21 08:32:21.000000 xbox-sdk-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0     1031 2023-04-21 08:32:42.909068 xbox-sdk-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.897488 xbox-sdk-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.902549 xbox-sdk-0.0.5/src/xbox_sdk/
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/main.py
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/
--rw-rw-rw-   0        0        0      645 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:56:28.840297 xbox-sdk-0.0.6/
+-rw-rw-rw-   0        0        0     1095 2023-04-21 08:10:04.000000 xbox-sdk-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-04-21 08:56:28.840297 xbox-sdk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-21 08:32:21.000000 xbox-sdk-0.0.6/README.md
+-rw-rw-rw-   0        0        0      535 2023-04-21 08:32:21.000000 xbox-sdk-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1031 2023-04-21 08:56:28.841802 xbox-sdk-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 08:56:28.815601 xbox-sdk-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:56:28.830118 xbox-sdk-0.0.6/src/xbox_sdk/
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.6/src/xbox_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-04-21 08:54:11.000000 xbox-sdk-0.0.6/src/xbox_sdk/client.py
+-rw-rw-rw-   0        0        0      839 2023-04-21 08:54:11.000000 xbox-sdk-0.0.6/src/xbox_sdk/gamer.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.6/src/xbox_sdk/main.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.6/src/xbox_sdk/py.typed
+-rw-rw-rw-   0        0        0     4622 2023-04-21 08:55:34.000000 xbox-sdk-0.0.6/src/xbox_sdk/scraper.py
+-rw-rw-rw-   0        0        0     1046 2023-04-21 08:48:10.000000 xbox-sdk-0.0.6/src/xbox_sdk/timeout.py
+-rw-rw-rw-   0        0        0     8673 2023-04-21 08:48:10.000000 xbox-sdk-0.0.6/src/xbox_sdk/user.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:56:28.839297 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-04-21 08:56:28.000000 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-04-21 08:56:28.000000 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:56:28.000000 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-21 08:56:28.000000 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 08:56:28.000000 xbox-sdk-0.0.6/src/xbox_sdk.egg-info/top_level.txt
```

### Comparing `xbox-sdk-0.0.5/LICENSE` & `xbox-sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.5/PKG-INFO` & `xbox-sdk-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: This application accesses the Xbox Live system.
 Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `xbox-sdk-0.0.5/pyproject.toml` & `xbox-sdk-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.5/setup.cfg` & `xbox-sdk-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2078 626f 782d 7364 6b0d 0a76 6572   = xbox-sdk..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 7465  sion = 0.0.5..te
+00000020: 7369 6f6e 203d 2030 2e30 2e36 0d0a 7465  sion = 0.0.6..te
 00000030: 7374 5f76 6572 7369 6f6e 203d 2030 2e30  st_version = 0.0
-00000040: 2e33 0d0a 7072 6f64 7563 7469 6f6e 5f76  .3..production_v
-00000050: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
+00000040: 2e36 0d0a 7072 6f64 7563 7469 6f6e 5f76  .6..production_v
+00000050: 6572 7369 6f6e 203d 2030 2e30 2e36 0d0a  ersion = 0.0.6..
 00000060: 6175 7468 6f72 203d 204d 6175 7269 6369  author = Maurici
 00000070: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000080: 3d20 6465 762e 6d61 7572 6963 696f 2e6c  = dev.mauricio.l
 00000090: 6f6d 656c 6940 676d 6169 6c2e 636f 6d0d  omeli@gmail.com.
 000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 000000b0: 6869 7320 6170 706c 6963 6174 696f 6e20  his application 
 000000c0: 6163 6365 7373 6573 2074 6865 2058 626f  accesses the Xbo
```

### Comparing `xbox-sdk-0.0.5/src/xbox_sdk.egg-info/PKG-INFO` & `xbox-sdk-0.0.6/src/xbox_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: This application accesses the Xbox Live system.
 Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

