# Comparing `tmp/pynball-1.5.4.tar.gz` & `tmp/pynball-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball-1.5.4.tar", last modified: Mon Apr 17 18:23:42 2023, max compression
+gzip compressed data, was "pynball-1.5.5.tar", last modified: Fri Apr 21 13:35:21 2023, max compression
```

## Comparing `pynball-1.5.4.tar` & `pynball-1.5.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.413279 pynball-1.5.4/
--rw-rw-rw-   0        0        0      155 2022-07-17 14:14:50.000000 pynball-1.5.4/AUTHORS.md
--rw-rw-rw-   0        0        0     7122 2023-04-17 18:23:29.000000 pynball-1.5.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.4/LICENSE
--rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0    12584 2023-04-17 18:23:42.413279 pynball-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0    11247 2023-04-17 14:12:33.000000 pynball-1.5.4/README.md
--rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0     1550 2023-04-17 18:23:42.415290 pynball-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-05-31 13:06:01.000000 pynball-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.298413 pynball-1.5.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.339531 pynball-1.5.4/src/pynball/
--rw-rw-rw-   0        0        0      269 2023-04-17 18:23:29.000000 pynball-1.5.4/src/pynball/__init__.py
--rw-rw-rw-   0        0        0    31282 2023-04-17 18:18:09.000000 pynball-1.5.4/src/pynball/pynball.py
-drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.347532 pynball-1.5.4/src/pynball.egg-info/
--rw-rw-rw-   0        0        0    12584 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 18:23:42.000000 pynball-1.5.4/src/pynball.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 18:23:42.411280 pynball-1.5.4/tests/
--rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.4/tests/test__check_pyenv.py
--rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.4/tests/test__check_virtual_env.py
--rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.4/tests/test__execute.py
--rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.4/tests/test__get_pynball.py
--rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.4/tests/test__message.py
--rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.4/tests/test__set_get_del_env.py
--rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.4/tests/test__set_pynball.py
--rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.4/tests/test_add.py
--rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.4/tests/test_delete.py
--rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.4/tests/test_lsproject.py
--rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.4/tests/test_mkproject.py
--rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.4/tests/test_rmproject.py
--rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.4/tests/test_version.py
--rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.4/tests/test_versions.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.403856 pynball-1.5.5/
+-rw-rw-rw-   0        0        0      140 2023-04-19 21:02:11.000000 pynball-1.5.5/AUTHORS.md
+-rw-rw-rw-   0        0        0     7570 2023-04-21 13:35:11.000000 pynball-1.5.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-04-09 16:05:23.000000 pynball-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    12613 2023-04-21 13:35:21.403856 pynball-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11282 2023-04-19 21:46:58.000000 pynball-1.5.5/README.md
+-rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1571 2023-04-21 13:35:21.403856 pynball-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 12:30:25.000000 pynball-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.225375 pynball-1.5.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.256684 pynball-1.5.5/src/pynball/
+-rw-rw-rw-   0        0        0      293 2023-04-21 13:35:11.000000 pynball-1.5.5/src/pynball/__init__.py
+-rw-rw-rw-   0        0        0    31204 2023-04-21 12:24:49.000000 pynball-1.5.5/src/pynball/pynball.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.272291 pynball-1.5.5/src/pynball.egg-info/
+-rw-rw-rw-   0        0        0    12613 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 13:35:21.000000 pynball-1.5.5/src/pynball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:35:21.403856 pynball-1.5.5/tests/
+-rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.5/tests/test__check_pyenv.py
+-rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.5/tests/test__check_virtual_env.py
+-rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.5/tests/test__execute.py
+-rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.5/tests/test__get_pynball.py
+-rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.5/tests/test__message.py
+-rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.5/tests/test__set_get_del_env.py
+-rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.5/tests/test__set_pynball.py
+-rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.5/tests/test_add.py
+-rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.5/tests/test_delete.py
+-rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.5/tests/test_lsproject.py
+-rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.5/tests/test_mkproject.py
+-rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.5/tests/test_rmproject.py
+-rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.5/tests/test_version.py
+-rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.5/tests/test_versions.py
```

### Comparing `pynball-1.5.4/CHANGELOG.md` & `pynball-1.5.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.5 (2023-04-21)
+### Fix
+* Shebang for version 3 env ([`57d4c92`](https://github.com/Stephen-RA-King/pynball/commit/57d4c927521b73c715f5f574fe208b2f9966f878))
+
+### Documentation
+* Update email link ([`39fba7a`](https://github.com/Stephen-RA-King/pynball/commit/39fba7adc7058d786735e65daab3f8c7d979aaee))
+* Update email address ([`736bb43`](https://github.com/Stephen-RA-King/pynball/commit/736bb432ab7501c58c9bab0813b560e6316cae22))
+
 ## v1.5.4 (2023-04-17)
 ### Fix
 * File open encoding error ([`4304034`](https://github.com/Stephen-RA-King/pynball/commit/4304034b56d81cb34ffce552294a20a07fd55ea7))
 
 ### Documentation
 * Rename base cookiecutter ([`9db5538`](https://github.com/Stephen-RA-King/pynball/commit/9db5538bfecb24210b138997f4efaeb7f3ffef34))
 * Update meta ([`5275172`](https://github.com/Stephen-RA-King/pynball/commit/52751725028692807284dc65ac8101781bd30e50))
```

### Comparing `pynball-1.5.4/LICENSE` & `pynball-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/PKG-INFO` & `pynball-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.4
+Version: 1.5.5
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
@@ -25,15 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pynball
 
-> Centralized management and utilization of all your Python versions, installations and virtual environments.
+_**Centralized management and utilization of all your Python versions, installations and virtual environments.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
@@ -249,27 +249,27 @@
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
 - [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
 - [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
-- [**Wiki**][wiki]
+[**Wiki**][wiki]
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : sking.github@gmail.com
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
```

### Comparing `pynball-1.5.4/README.md` & `pynball-1.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pynball
 
-> Centralized management and utilization of all your Python versions, installations and virtual environments.
+_**Centralized management and utilization of all your Python versions, installations and virtual environments.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
@@ -220,27 +220,27 @@
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
 - [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
 - [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
-- [**Wiki**][wiki]
+[**Wiki**][wiki]
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : sking.github@gmail.com
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
```

### Comparing `pynball-1.5.4/pyproject.toml` & `pynball-1.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/setup.cfg` & `pynball-1.5.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796e 6261 6c6c 0d0a 7665 7273   = pynball..vers
 00000020: 696f 6e20 3d20 6174 7472 3a20 7079 6e62  ion = attr: pynb
 00000030: 616c 6c2e 5f5f 7665 7273 696f 6e5f 5f0d  all.__version__.
 00000040: 0a61 7574 686f 7220 3d20 5374 6570 6865  .author = Stephe
 00000050: 6e20 5220 4120 4b69 6e67 0d0a 6175 7468  n R A King..auth
-00000060: 6f72 5f65 6d61 696c 203d 2073 7465 7068  or_email = steph
-00000070: 656e 2e72 612e 6b69 6e67 4067 6d61 696c  en.ra.king@gmail
-00000080: 2e63 6f6d 0d0a 6d61 696e 7461 696e 6572  .com..maintainer
-00000090: 203d 2053 7465 7068 656e 2052 2041 204b   = Stephen R A K
-000000a0: 696e 670d 0a6d 6169 6e74 6169 6e65 725f  ing..maintainer_
-000000b0: 656d 6169 6c20 3d20 7374 6570 6865 6e2e  email = stephen.
-000000c0: 7261 2e6b 696e 6740 676d 6169 6c2e 636f  ra.king@gmail.co
-000000d0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
-000000e0: 2055 7469 6c69 7479 2063 6f6d 6d61 6e64   Utility command
-000000f0: 206c 696e 6520 746f 6f6c 2074 6f20 6d61   line tool to ma
-00000100: 6e61 6765 2070 7974 686f 6e20 7665 7273  nage python vers
-00000110: 696f 6e73 0d0a 6c6f 6e67 5f64 6573 6372  ions..long_descr
-00000120: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-00000130: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-00000140: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-00000150: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-00000160: 6172 6b64 6f77 6e0d 0a6b 6579 776f 7264  arkdown..keyword
-00000170: 7320 3d20 7574 696c 6974 792c 0d0a 706c  s = utility,..pl
-00000180: 6174 666f 726d 7320 3d20 7769 6e64 6f77  atforms = window
-00000190: 730d 0a75 726c 203d 2068 7474 7073 3a2f  s..url = https:/
-000001a0: 2f67 6974 6875 622e 636f 6d2f 7374 6570  /github.com/step
-000001b0: 6865 6e2d 7261 2d6b 696e 672f 7079 6e62  hen-ra-king/pynb
-000001c0: 616c 6c0d 0a64 6f77 6e6c 6f61 645f 7572  all..download_ur
-000001d0: 6c20 3d20 0d0a 6c69 6365 6e73 6520 3d20  l = ..license = 
-000001e0: 4d49 540d 0a63 6c61 7373 6966 6965 7273  MIT..classifiers
-000001f0: 203d 200d 0a09 4465 7665 6c6f 706d 656e   = ...Developmen
-00000200: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
-00000210: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
-00000220: 650d 0a09 456e 7669 726f 6e6d 656e 7420  e...Environment 
-00000230: 3a3a 2043 6f6e 736f 6c65 0d0a 0949 6e74  :: Console...Int
-00000240: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-00000250: 3a20 4465 7665 6c6f 7065 7273 0d0a 094f  : Developers...O
-00000260: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000270: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
-00000280: 5769 6e64 6f77 730d 0a09 546f 7069 6320  Windows...Topic 
-00000290: 3a3a 2053 7973 7465 6d20 3a3a 2049 6e73  :: System :: Ins
-000002a0: 7461 6c6c 6174 696f 6e2f 5365 7475 700d  tallation/Setup.
-000002b0: 0a09 4e61 7475 7261 6c20 4c61 6e67 7561  ..Natural Langua
-000002c0: 6765 203a 3a20 456e 676c 6973 680d 0a09  ge :: English...
-000002d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002f0: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
-00000300: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000310: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-00000320: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
-00000330: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000340: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000350: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000360: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000370: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000380: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000390: 6f6e 203a 3a20 332e 3130 0d0a 0d0a 5b6f  on :: 3.10....[o
-000003a0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-000003b0: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
-000003c0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-000003d0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-000003e0: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
-000003f0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000400: 203e 3d33 2e38 0d0a 696e 7374 616c 6c5f   >=3.8..install_
-00000410: 7265 7175 6972 6573 203d 200d 0a09 636c  requires = ...cl
-00000420: 6963 6b3e 3d38 2e31 2e33 2c3c 382e 322e  ick>=8.1.3,<8.2.
-00000430: 300d 0a09 7079 7468 6f6e 2d6d 6167 6963  0...python-magic
-00000440: 2d62 696e 3d3d 302e 342e 3134 0d0a 0d0a  -bin==0.4.14....
-00000450: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000460: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000470: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
-00000480: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000490: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-000004a0: 3d20 0d0a 0970 796e 6261 6c6c 203d 2070  = ...pynball = p
-000004b0: 796e 6261 6c6c 2e70 796e 6261 6c6c 3a63  ynball.pynball:c
-000004c0: 6c69 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  li....[flake8]..
-000004d0: 646f 6373 7472 696e 672d 636f 6e76 656e  docstring-conven
-000004e0: 7469 6f6e 203d 206e 756d 7079 0d0a 6d61  tion = numpy..ma
-000004f0: 782d 636f 6d70 6c65 7869 7479 203d 2031  x-complexity = 1
-00000500: 380d 0a6d 6178 2d6c 696e 652d 6c65 6e67  8..max-line-leng
-00000510: 7468 203d 2038 380d 0a73 656c 6563 7420  th = 88..select 
-00000520: 3d20 422c 2042 392c 2043 2c20 442c 2045  = B, B9, C, D, E
-00000530: 2c20 462c 204e 2c20 570d 0a65 7863 6c75  , F, N, W..exclu
-00000540: 6465 203d 2074 6573 7473 2f2a 2c2e 746f  de = tests/*,.to
-00000550: 782f 2a2c 2e6e 6f78 2f2a 2c64 6f63 732f  x/*,.nox/*,docs/
-00000560: 2a2c 2e67 6974 2f2a 2c2e 6769 7468 7562  *,.git/*,.github
-00000570: 2f2a 0d0a 6967 6e6f 7265 203d 200d 0a09  /*..ignore = ...
-00000580: 4532 3033 2c0d 0a09 5735 3033 2c0d 0a70  E203,...W503,..p
-00000590: 6572 2d66 696c 652d 6967 6e6f 7265 7320  er-file-ignores 
-000005a0: 3d20 0d0a 095f 5f69 6e69 745f 5f2e 7079  = ...__init__.py
-000005b0: 3a46 3430 310d 0a09 7061 7468 6d61 6769  :F401...pathmagi
-000005c0: 632e 7079 3a46 3430 310d 0a09 7465 7374  c.py:F401...test
-000005d0: 5f70 796e 6261 6c6c 2e70 793a 4634 3031  _pynball.py:F401
-000005e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000005f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000600: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000060: 6f72 5f65 6d61 696c 203d 2073 6b69 6e67  or_email = sking
+00000070: 2e67 6974 6875 6240 676d 6169 6c2e 636f  .github@gmail.co
+00000080: 6d0d 0a6d 6169 6e74 6169 6e65 7220 3d20  m..maintainer = 
+00000090: 5374 6570 6865 6e20 5220 4120 4b69 6e67  Stephen R A King
+000000a0: 0d0a 6d61 696e 7461 696e 6572 5f65 6d61  ..maintainer_ema
+000000b0: 696c 203d 2073 6b69 6e67 2e67 6974 6875  il = sking.githu
+000000c0: 6240 676d 6169 6c2e 636f 6d0d 0a64 6573  b@gmail.com..des
+000000d0: 6372 6970 7469 6f6e 203d 2055 7469 6c69  cription = Utili
+000000e0: 7479 2063 6f6d 6d61 6e64 206c 696e 6520  ty command line 
+000000f0: 746f 6f6c 2074 6f20 6d61 6e61 6765 2070  tool to manage p
+00000100: 7974 686f 6e20 7665 7273 696f 6e73 0d0a  ython versions..
+00000110: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000120: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000130: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+00000140: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000150: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000160: 6e0d 0a6b 6579 776f 7264 7320 3d20 7574  n..keywords = ut
+00000170: 696c 6974 792c 0d0a 706c 6174 666f 726d  ility,..platform
+00000180: 7320 3d20 7769 6e64 6f77 730d 0a75 726c  s = windows..url
+00000190: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000001a0: 622e 636f 6d2f 7374 6570 6865 6e2d 7261  b.com/stephen-ra
+000001b0: 2d6b 696e 672f 7079 6e62 616c 6c0d 0a64  -king/pynball..d
+000001c0: 6f77 6e6c 6f61 645f 7572 6c20 3d20 0d0a  ownload_url = ..
+000001d0: 6c69 6365 6e73 6520 3d20 4d49 540d 0a63  license = MIT..c
+000001e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000200: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
+00000210: 7469 6f6e 2f53 7461 626c 650d 0a09 456e  tion/Stable...En
+00000220: 7669 726f 6e6d 656e 7420 3a3a 2043 6f6e  vironment :: Con
+00000230: 736f 6c65 0d0a 0949 6e74 656e 6465 6420  sole...Intended 
+00000240: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000250: 6c6f 7065 7273 0d0a 094f 7065 7261 7469  lopers...Operati
+00000260: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
+00000270: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
+00000280: 730d 0a09 546f 7069 6320 3a3a 2053 7973  s...Topic :: Sys
+00000290: 7465 6d20 3a3a 2049 6e73 7461 6c6c 6174  tem :: Installat
+000002a0: 696f 6e2f 5365 7475 700d 0a09 4e61 7475  ion/Setup...Natu
+000002b0: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+000002c0: 456e 676c 6973 680d 0a09 5072 6f67 7261  English...Progra
+000002d0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002e0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+000002f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000300: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000310: 3a20 3320 3a3a 204f 6e6c 790d 0a09 5072  : 3 :: Only...Pr
+00000320: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000330: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000340: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+00000350: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000360: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
+00000370: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000380: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000390: 332e 3130 0d0a 0d0a 5b6f 7074 696f 6e73  3.10....[options
+000003a0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+000003b0: 200d 0a09 3d73 7263 0d0a 7061 636b 6167   ...=src..packag
+000003c0: 6573 203d 2066 696e 643a 0d0a 696e 636c  es = find:..incl
+000003d0: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
+000003e0: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
+000003f0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+00000400: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+00000410: 6573 203d 200d 0a09 636c 6963 6b3e 3d38  es = ...click>=8
+00000420: 2e31 2e33 2c3c 382e 322e 300d 0a09 7079  .1.3,<8.2.0...py
+00000430: 7468 6f6e 2d6d 6167 6963 2d62 696e 3d3d  thon-magic-bin==
+00000440: 302e 342e 3134 3b70 6c61 7466 6f72 6d5f  0.4.14;platform_
+00000450: 7379 7374 656d 3d3d 2757 696e 646f 7773  system=='Windows
+00000460: 270d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  '....[options.pa
+00000470: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000480: 6572 6520 3d20 7372 630d 0a0d 0a5b 6f70  ere = src....[op
+00000490: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
+000004a0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
+000004b0: 6970 7473 203d 200d 0a09 7079 6e62 616c  ipts = ...pynbal
+000004c0: 6c20 3d20 7079 6e62 616c 6c2e 7079 6e62  l = pynball.pynb
+000004d0: 616c 6c3a 636c 690d 0a0d 0a5b 666c 616b  all:cli....[flak
+000004e0: 6538 5d0d 0a64 6f63 7374 7269 6e67 2d63  e8]..docstring-c
+000004f0: 6f6e 7665 6e74 696f 6e20 3d20 6e75 6d70  onvention = nump
+00000500: 790d 0a6d 6178 2d63 6f6d 706c 6578 6974  y..max-complexit
+00000510: 7920 3d20 3138 0d0a 6d61 782d 6c69 6e65  y = 18..max-line
+00000520: 2d6c 656e 6774 6820 3d20 3838 0d0a 7365  -length = 88..se
+00000530: 6c65 6374 203d 2042 2c20 4239 2c20 432c  lect = B, B9, C,
+00000540: 2044 2c20 452c 2046 2c20 4e2c 2057 0d0a   D, E, F, N, W..
+00000550: 6578 636c 7564 6520 3d20 7465 7374 732f  exclude = tests/
+00000560: 2a2c 2e74 6f78 2f2a 2c2e 6e6f 782f 2a2c  *,.tox/*,.nox/*,
+00000570: 646f 6373 2f2a 2c2e 6769 742f 2a2c 2e67  docs/*,.git/*,.g
+00000580: 6974 6875 622f 2a0d 0a69 676e 6f72 6520  ithub/*..ignore 
+00000590: 3d20 0d0a 0945 3230 332c 0d0a 0957 3530  = ...E203,...W50
+000005a0: 332c 0d0a 7065 722d 6669 6c65 2d69 676e  3,..per-file-ign
+000005b0: 6f72 6573 203d 200d 0a09 5f5f 696e 6974  ores = ...__init
+000005c0: 5f5f 2e70 793a 4634 3031 0d0a 0970 6174  __.py:F401...pat
+000005d0: 686d 6167 6963 2e70 793a 4634 3031 0d0a  hmagic.py:F401..
+000005e0: 0974 6573 745f 7079 6e62 616c 6c2e 7079  .test_pynball.py
+000005f0: 3a46 3430 310d 0a0d 0a5b 6567 675f 696e  :F401....[egg_in
+00000600: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000610: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000620: 0a0d 0a                                  ...
```

### Comparing `pynball-1.5.4/src/pynball/pynball.py` & `pynball-1.5.5/src/pynball/pynball.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # TODO: implement conditional imports based on OS
 import winreg
 from pathlib import Path
 from typing import Any
 
 # Third party modules
 import click
-
-# TODO: replace 3rd party libmagic library with standard mimetypes library
 import magic
 
 #: Specifies the operating system to which the module is installed
 _PLATFORM = sys.platform
 if _PLATFORM != "win32":
     print(
         "Your Operating system is not supported yet."
```

### Comparing `pynball-1.5.4/src/pynball.egg-info/PKG-INFO` & `pynball-1.5.5/src/pynball.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.4
+Version: 1.5.5
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
@@ -25,15 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # Pynball
 
-> Centralized management and utilization of all your Python versions, installations and virtual environments.
+_**Centralized management and utilization of all your Python versions, installations and virtual environments.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
@@ -249,27 +249,27 @@
 [**Read the Docs**](https://pynball.readthedocs.io/en/latest/?)
 
 - [**Example Usage**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Credits**](https://pynball.readthedocs.io/en/latest/example.html)
 - [**Changelog**](https://pynball.readthedocs.io/en/latest/changelog.html)
 - [**API Reference**](https://pynball.readthedocs.io/en/latest/autoapi/index.html)
 
-- [**Wiki**][wiki]
+[**Wiki**][wiki]
 
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynball)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : sking.github@gmail.com
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
 Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
 Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
```

### Comparing `pynball-1.5.4/src/pynball.egg-info/SOURCES.txt` & `pynball-1.5.5/src/pynball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test__check_pyenv.py` & `pynball-1.5.5/tests/test__check_pyenv.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test__check_virtual_env.py` & `pynball-1.5.5/tests/test__check_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test__get_pynball.py` & `pynball-1.5.5/tests/test__get_pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test__message.py` & `pynball-1.5.5/tests/test__message.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test__set_get_del_env.py` & `pynball-1.5.5/tests/test__set_get_del_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_add.py` & `pynball-1.5.5/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_delete.py` & `pynball-1.5.5/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_lsproject.py` & `pynball-1.5.5/tests/test_lsproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_mkproject.py` & `pynball-1.5.5/tests/test_mkproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_rmproject.py` & `pynball-1.5.5/tests/test_rmproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.4/tests/test_versions.py` & `pynball-1.5.5/tests/test_versions.py`

 * *Files identical despite different names*

