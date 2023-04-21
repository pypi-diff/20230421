# Comparing `tmp/xbox-sdk-0.0.4.tar.gz` & `tmp/xbox-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbox-sdk-0.0.4.tar", last modified: Fri Apr 21 08:26:42 2023, max compression
+gzip compressed data, was "xbox-sdk-0.0.5.tar", last modified: Fri Apr 21 08:32:42 2023, max compression
```

## Comparing `xbox-sdk-0.0.4.tar` & `xbox-sdk-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:26:42.973444 xbox-sdk-0.0.4/
--rw-rw-rw-   0        0        0     1095 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      648 2023-04-21 08:26:42.974442 xbox-sdk-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/README.md
--rw-rw-rw-   0        0        0      536 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0     1034 2023-04-21 08:26:42.974442 xbox-sdk-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 08:26:42.963355 xbox-sdk-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:26:42.968930 xbox-sdk-0.0.4/src/xbox_live/
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/src/xbox_live/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/src/xbox_live/main.py
--rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.4/src/xbox_live/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-21 08:26:42.973444 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/
--rw-rw-rw-   0        0        0      648 2023-04-21 08:26:42.000000 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-21 08:26:42.000000 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:26:42.000000 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-04-21 08:26:42.000000 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 08:26:42.000000 xbox-sdk-0.0.4/src/xbox_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/
+-rw-rw-rw-   0        0        0     1095 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      645 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-21 08:32:21.000000 xbox-sdk-0.0.5/README.md
+-rw-rw-rw-   0        0        0      535 2023-04-21 08:32:21.000000 xbox-sdk-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1031 2023-04-21 08:32:42.909068 xbox-sdk-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.897488 xbox-sdk-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.902549 xbox-sdk-0.0.5/src/xbox_sdk/
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/main.py
+-rw-rw-rw-   0        0        0        0 2023-04-21 08:10:04.000000 xbox-sdk-0.0.5/src/xbox_sdk/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-21 08:32:42.907554 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/
+-rw-rw-rw-   0        0        0      645 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 08:32:42.000000 xbox-sdk-0.0.5/src/xbox_sdk.egg-info/top_level.txt
```

### Comparing `xbox-sdk-0.0.4/LICENSE` & `xbox-sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xbox-sdk-0.0.4/PKG-INFO` & `xbox-sdk-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: This application accesses the Xbox Live system.
-Home-page: https://github.com/mjlomeli/Xbox_Live
+Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
-Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_Live/issues
+Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# Xbox Live
+# Xbox SDK
```

### Comparing `xbox-sdk-0.0.4/pyproject.toml` & `xbox-sdk-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
-addopts = "--cov=arkdriver"
+addopts = "--cov=xbox-sdk"
 testpaths = [
     "tests",
 ]
 
 [too.mypy]
 mypy_path = "src"
 check_untyped_defs = true
```

### Comparing `xbox-sdk-0.0.4/setup.cfg` & `xbox-sdk-0.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2078 626f 782d 7364 6b0d 0a76 6572   = xbox-sdk..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 7465  sion = 0.0.4..te
+00000020: 7369 6f6e 203d 2030 2e30 2e35 0d0a 7465  sion = 0.0.5..te
 00000030: 7374 5f76 6572 7369 6f6e 203d 2030 2e30  st_version = 0.0
-00000040: 2e32 0d0a 7072 6f64 7563 7469 6f6e 5f76  .2..production_v
-00000050: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
+00000040: 2e33 0d0a 7072 6f64 7563 7469 6f6e 5f76  .3..production_v
+00000050: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
 00000060: 6175 7468 6f72 203d 204d 6175 7269 6369  author = Maurici
 00000070: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
 00000080: 3d20 6465 762e 6d61 7572 6963 696f 2e6c  = dev.mauricio.l
 00000090: 6f6d 656c 6940 676d 6169 6c2e 636f 6d0d  omeli@gmail.com.
 000000a0: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 000000b0: 6869 7320 6170 706c 6963 6174 696f 6e20  his application 
 000000c0: 6163 6365 7373 6573 2074 6865 2058 626f  accesses the Xbo
@@ -15,51 +15,51 @@
 000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000f0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000100: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000110: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 00000120: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
 00000130: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
 00000140: 2f67 6974 6875 622e 636f 6d2f 6d6a 6c6f  /github.com/mjlo
-00000150: 6d65 6c69 2f58 626f 785f 4c69 7665 0d0a  meli/Xbox_Live..
-00000160: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-00000170: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-00000180: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000190: 6f6d 2f6d 6a6c 6f6d 656c 692f 5862 6f78  om/mjlomeli/Xbox
-000001a0: 5f4c 6976 652f 6973 7375 6573 0d0a 706c  _Live/issues..pl
-000001b0: 6174 666f 726d 7320 3d20 7769 6e33 320d  atforms = win32.
-000001c0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-000001d0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001e0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001f0: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000200: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000210: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000220: 0d0a 090d 0a09 4c69 6365 6e73 6520 3a3a  ......License ::
-00000230: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000240: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000250: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000260: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000270: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000280: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000290: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-000002a0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-000002b0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-000002c0: 390d 0a69 6e73 7461 6c6c 5f72 6571 7569  9..install_requi
-000002d0: 7265 7320 3d20 0d0a 0977 6865 656c 0d0a  res = ...wheel..
-000002e0: 0972 6571 7565 7374 733e 3d32 2e32 382e  .requests>=2.28.
-000002f0: 310d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  1....[options.pa
-00000300: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000310: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
-00000320: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-00000330: 7569 7265 5d0d 0a74 6573 7469 6e67 203d  uire]..testing =
-00000340: 200d 0a09 7079 7465 7374 3e3d 362e 300d   ...pytest>=6.0.
-00000350: 0a09 7079 7465 7374 2d63 6f76 3e3d 322e  ..pytest-cov>=2.
-00000360: 300d 0a09 6d79 7079 3e3d 302e 3937 310d  0...mypy>=0.971.
-00000370: 0a09 666c 616b 6538 3e3d 332e 390d 0a09  ..flake8>=3.9...
-00000380: 746f 783e 3d33 2e32 340d 0a0d 0a5b 6f70  tox>=3.24....[op
-00000390: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-000003a0: 7461 5d0d 0a78 626f 785f 6c69 7665 203d  ta]..xbox_live =
-000003b0: 2070 792e 7479 7065 640d 0a0d 0a5b 666c   py.typed....[fl
-000003c0: 616b 6538 5d0d 0a6d 6178 2d6c 696e 652d  ake8]..max-line-
-000003d0: 6c65 6e67 7468 203d 2031 3630 0d0a 0d0a  length = 160....
-000003e0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-000003f0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000400: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000150: 6d65 6c69 2f58 626f 785f 5344 4b0d 0a70  meli/Xbox_SDK..p
+00000160: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000170: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000190: 6d2f 6d6a 6c6f 6d65 6c69 2f58 626f 785f  m/mjlomeli/Xbox_
+000001a0: 5344 4b2f 6973 7375 6573 0d0a 706c 6174  SDK/issues..plat
+000001b0: 666f 726d 7320 3d20 7769 6e33 320d 0a63  forms = win32..c
+000001c0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001f0: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+00000200: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000210: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000220: 090d 0a09 4c69 6365 6e73 6520 3a3a 204f  ....License :: O
+00000230: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000240: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000250: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000260: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000270: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+00000280: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000290: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
+000002a0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000002b0: 6571 7569 7265 7320 3d20 3e3d 332e 390d  equires = >=3.9.
+000002c0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000002d0: 7320 3d20 0d0a 0977 6865 656c 0d0a 0972  s = ...wheel...r
+000002e0: 6571 7565 7374 733e 3d32 2e32 382e 310d  equests>=2.28.1.
+000002f0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000300: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000310: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
+00000320: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+00000330: 7265 5d0d 0a74 6573 7469 6e67 203d 200d  re]..testing = .
+00000340: 0a09 7079 7465 7374 3e3d 362e 300d 0a09  ..pytest>=6.0...
+00000350: 7079 7465 7374 2d63 6f76 3e3d 322e 300d  pytest-cov>=2.0.
+00000360: 0a09 6d79 7079 3e3d 302e 3937 310d 0a09  ..mypy>=0.971...
+00000370: 666c 616b 6538 3e3d 332e 390d 0a09 746f  flake8>=3.9...to
+00000380: 783e 3d33 2e32 340d 0a0d 0a5b 6f70 7469  x>=3.24....[opti
+00000390: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+000003a0: 5d0d 0a78 626f 785f 7364 6b20 3d20 7079  ]..xbox_sdk = py
+000003b0: 2e74 7970 6564 0d0a 0d0a 5b66 6c61 6b65  .typed....[flake
+000003c0: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
+000003d0: 6774 6820 3d20 3136 300d 0a0d 0a5b 6567  gth = 160....[eg
+000003e0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000003f0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000400: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `xbox-sdk-0.0.4/src/xbox_sdk.egg-info/PKG-INFO` & `xbox-sdk-0.0.5/src/xbox_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xbox-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: This application accesses the Xbox Live system.
-Home-page: https://github.com/mjlomeli/Xbox_Live
+Home-page: https://github.com/mjlomeli/Xbox_SDK
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
-Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_Live/issues
+Project-URL: Bug Tracker, https://github.com/mjlomeli/Xbox_SDK/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# Xbox Live
+# Xbox SDK
```

