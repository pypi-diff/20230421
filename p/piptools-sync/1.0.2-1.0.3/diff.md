# Comparing `tmp/piptools_sync-1.0.2.tar.gz` & `tmp/piptools_sync-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piptools_sync-1.0.2.tar", last modified: Sat Apr  8 12:38:29 2023, max compression
+gzip compressed data, was "piptools_sync-1.0.3.tar", last modified: Fri Apr 21 13:48:26 2023, max compression
```

## Comparing `piptools_sync-1.0.2.tar` & `piptools_sync-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:38:29.641249 piptools_sync-1.0.2/
--rw-rw-rw-   0        0        0      163 2022-08-23 11:18:38.000000 piptools_sync-1.0.2/AUTHORS.md
--rw-rw-rw-   0        0        0     2954 2023-04-08 12:38:19.000000 piptools_sync-1.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-08-23 11:11:28.000000 piptools_sync-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      194 2022-08-23 11:11:28.000000 piptools_sync-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    13240 2023-04-08 12:38:29.641249 piptools_sync-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    12258 2023-04-08 12:38:19.000000 piptools_sync-1.0.2/README.md
--rw-rw-rw-   0        0        0     2241 2022-10-07 21:51:55.000000 piptools_sync-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1699 2023-04-08 12:38:29.643248 piptools_sync-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-08-23 11:11:28.000000 piptools_sync-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:38:29.493249 piptools_sync-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 12:38:29.554250 piptools_sync-1.0.2/src/piptools_sync/
--rw-rw-rw-   0        0        0     1685 2023-04-08 12:38:19.000000 piptools_sync-1.0.2/src/piptools_sync/__init__.py
--rw-rw-rw-   0        0        0      167 2023-04-07 17:19:25.000000 piptools_sync-1.0.2/src/piptools_sync/config.toml
--rw-rw-rw-   0        0        0     7645 2023-04-08 11:56:30.000000 piptools_sync-1.0.2/src/piptools_sync/mapping.json
--rw-rw-rw-   0        0        0    17374 2023-04-08 11:58:05.000000 piptools_sync-1.0.2/src/piptools_sync/piptools_sync.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:38:29.568250 piptools_sync-1.0.2/src/piptools_sync.egg-info/
--rw-rw-rw-   0        0        0    13240 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-08 12:38:29.000000 piptools_sync-1.0.2/src/piptools_sync.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 12:38:29.639256 piptools_sync-1.0.2/tests/
--rw-rw-rw-   0        0        0      583 2022-09-04 19:08:21.000000 piptools_sync-1.0.2/tests/test__utility_find_file_path.py
--rw-rw-rw-   0        0        0      541 2022-08-26 17:02:45.000000 piptools_sync-1.0.2/tests/test__utility_remove_vee.py
--rw-rw-rw-   0        0        0      529 2022-08-28 18:06:52.000000 piptools_sync-1.0.2/tests/test_find_requirements_file.py
--rw-rw-rw-   0        0        0      348 2022-08-27 18:08:46.000000 piptools_sync-1.0.2/tests/test_find_yaml_config_file.py
--rw-rw-rw-   0        0        0      555 2022-09-20 15:51:26.000000 piptools_sync-1.0.2/tests/test_generate_db.py
--rw-rw-rw-   0        0        0      411 2022-08-28 17:54:33.000000 piptools_sync-1.0.2/tests/test_get_installed_version.py
--rw-rw-rw-   0        0        0      358 2022-08-26 17:04:02.000000 piptools_sync-1.0.2/tests/test_get_precommit_repos.py
--rw-rw-rw-   0        0        0      575 2022-08-28 17:54:33.000000 piptools_sync-1.0.2/tests/test_get_requirement_versions.py
--rw-rw-rw-   0        0        0      693 2022-08-28 15:02:33.000000 piptools_sync-1.0.2/tests/test_update_yaml.py
--rw-rw-rw-   0        0        0      465 2022-08-28 14:26:16.000000 piptools_sync-1.0.2/tests/test_yaml_to_dict.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.528265 piptools_sync-1.0.3/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:46.000000 piptools_sync-1.0.3/AUTHORS.md
+-rw-rw-rw-   0        0        0     3830 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1074 2022-08-23 11:11:28.000000 piptools_sync-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      194 2022-08-23 11:11:28.000000 piptools_sync-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    13543 2023-04-21 13:48:26.533795 piptools_sync-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    12567 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/README.md
+-rw-rw-rw-   0        0        0     2241 2022-10-07 21:51:55.000000 piptools_sync-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1693 2023-04-21 13:48:26.533795 piptools_sync-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      108 2023-04-21 12:31:49.000000 piptools_sync-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.433761 piptools_sync-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.497008 piptools_sync-1.0.3/src/piptools_sync/
+-rw-rw-rw-   0        0        0     1706 2023-04-21 13:48:16.000000 piptools_sync-1.0.3/src/piptools_sync/__init__.py
+-rw-rw-rw-   0        0        0      167 2023-04-07 17:19:25.000000 piptools_sync-1.0.3/src/piptools_sync/config.toml
+-rw-rw-rw-   0        0        0     7645 2023-04-08 11:56:30.000000 piptools_sync-1.0.3/src/piptools_sync/mapping.json
+-rw-rw-rw-   0        0        0    17398 2023-04-21 12:31:49.000000 piptools_sync-1.0.3/src/piptools_sync/piptools_sync.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.497008 piptools_sync-1.0.3/src/piptools_sync.egg-info/
+-rw-rw-rw-   0        0        0    13543 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13231 2023-04-18 15:26:46.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO.rum-bak
+-rw-rw-rw-   0        0        0      838 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-21 13:48:26.000000 piptools_sync-1.0.3/src/piptools_sync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:48:26.528265 piptools_sync-1.0.3/tests/
+-rw-rw-rw-   0        0        0      583 2022-09-04 19:08:21.000000 piptools_sync-1.0.3/tests/test__utility_find_file_path.py
+-rw-rw-rw-   0        0        0      541 2022-08-26 17:02:45.000000 piptools_sync-1.0.3/tests/test__utility_remove_vee.py
+-rw-rw-rw-   0        0        0      529 2022-08-28 18:06:52.000000 piptools_sync-1.0.3/tests/test_find_requirements_file.py
+-rw-rw-rw-   0        0        0      348 2022-08-27 18:08:46.000000 piptools_sync-1.0.3/tests/test_find_yaml_config_file.py
+-rw-rw-rw-   0        0        0      555 2022-09-20 15:51:26.000000 piptools_sync-1.0.3/tests/test_generate_db.py
+-rw-rw-rw-   0        0        0      411 2022-08-28 17:54:33.000000 piptools_sync-1.0.3/tests/test_get_installed_version.py
+-rw-rw-rw-   0        0        0      358 2022-08-26 17:04:02.000000 piptools_sync-1.0.3/tests/test_get_precommit_repos.py
+-rw-rw-rw-   0        0        0      575 2022-08-28 17:54:33.000000 piptools_sync-1.0.3/tests/test_get_requirement_versions.py
+-rw-rw-rw-   0        0        0      693 2022-08-28 15:02:33.000000 piptools_sync-1.0.3/tests/test_update_yaml.py
+-rw-rw-rw-   0        0        0      465 2022-08-28 14:26:16.000000 piptools_sync-1.0.3/tests/test_yaml_to_dict.py
```

### Comparing `piptools_sync-1.0.2/CHANGELOG.md` & `piptools_sync-1.0.3/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.3 (2023-04-21)
+### Fix
+* Shebang for version 3 env ([`b1442d8`](https://github.com/Stephen-RA-King/piptools-sync/commit/b1442d88028386ffacdba39dfe5ae04c30ac534d))
+
+### Documentation
+* Update email link ([`cf67f5f`](https://github.com/Stephen-RA-King/piptools-sync/commit/cf67f5f16c366f0567c4d90667b77cb4ffe9ad34))
+* Update author email ([`9cfd29f`](https://github.com/Stephen-RA-King/piptools-sync/commit/9cfd29fd3e845b16e55b6a0c8eb4f9963ee6bd18))
+* Rename base cookiecutter name ([`7254956`](https://github.com/Stephen-RA-King/piptools-sync/commit/725495639051e3c5f94d9871bb6a888675f73da9))
+* Update meta ([`642778b`](https://github.com/Stephen-RA-King/piptools-sync/commit/642778b1c0c6c7fc482b88c3045359d1feaffd0a))
+* Add pre-commit.ci badge ([`b65ae6c`](https://github.com/Stephen-RA-King/piptools-sync/commit/b65ae6cbba56ad1c6e7fefe32c7b4ce99737c507))
+
 ## v1.0.2 (2023-04-08)
 ### Documentation
 * Fix spelling ([`156aeb5`](https://github.com/Stephen-RA-King/piptools-sync/commit/156aeb5dc43958e9d250a5f434271efee7d1404f))
 
 ## v1.0.0 (2022-10-07)
 ### Fix
 * Correct path for PSR version ([`7f25a18`](https://github.com/Stephen-RA-King/piptools-sync/commit/7f25a187ba6df98be5684a52b09b88f0c1037af1))
```

### Comparing `piptools_sync-1.0.2/LICENSE` & `piptools_sync-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/PKG-INFO` & `piptools_sync-1.0.3/src/piptools_sync.egg-info/PKG-INFO.rum-bak`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: piptools_sync
+Name: piptools-sync
 Version: 1.0.2
 Summary: A piptools pre-commit version sync utility
 Home-page: https://github.com/Stephen-RA-King/piptools-sync
 Download-URL: https://github.com/Stephen-RA-King/piptools_sync/archive/refs/heads/main.zip
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -220,15 +220,15 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/piptools-sync)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : stephen.ra.king@gmail.com
+Stephen R A King : sking.github@gmail.com
 
 Distributed under the MIT license. See [license][license-url] for more information.
 
 [https://github.com/Stephen-RA-King/piptools-sync](https://github.com/Stephen-RA-King/piptools-sync)
 
 Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.1
```

### Comparing `piptools_sync-1.0.2/README.md` & `piptools_sync-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# piptools-sync
+# Piptools-sync
 
 ---
 
-> A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools..
+_**A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -172,17 +173,22 @@
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## Documentation
 
 ---
 
-### - [**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/)
+[**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/?)
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
+- [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
 
 ## Future Enhancements
 
 ---
 
 - Move some global variables into a separate settings file (toml).
 - Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
@@ -194,29 +200,27 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/piptools-sync)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : stephen.ra.king@gmail.com
-
-Distributed under the MIT license. See [license][license-url] for more information.
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-[https://github.com/Stephen-RA-King/piptools-sync](https://github.com/Stephen-RA-King/piptools-sync)
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.1
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/9543c409696e9976a987/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/piptools-sync/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/piptools-sync/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/piptools-sync
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/piptools-sync/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/piptools-sync
 [codeql-image]: https://github.com/Stephen-RA-King/piptools-sync/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `piptools_sync-1.0.2/pyproject.toml` & `piptools_sync-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/setup.cfg` & `piptools_sync-1.0.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,106 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6970 746f 6f6c 735f 7379 6e63   = piptools_sync
 00000020: 0d0a 7665 7273 696f 6e20 3d20 6174 7472  ..version = attr
 00000030: 3a20 7069 7074 6f6f 6c73 5f73 796e 632e  : piptools_sync.
 00000040: 5f5f 7665 7273 696f 6e5f 5f0d 0a61 7574  __version__..aut
 00000050: 686f 7220 3d20 5374 6570 6865 6e20 5220  hor = Stephen R 
 00000060: 4120 4b69 6e67 0d0a 6175 7468 6f72 5f65  A King..author_e
-00000070: 6d61 696c 203d 2073 7465 7068 656e 2e72  mail = stephen.r
-00000080: 612e 6b69 6e67 4067 6d61 696c 2e63 6f6d  a.king@gmail.com
-00000090: 0d0a 6d61 696e 7461 696e 6572 203d 2053  ..maintainer = S
-000000a0: 7465 7068 656e 2052 2041 204b 696e 670d  tephen R A King.
-000000b0: 0a6d 6169 6e74 6169 6e65 725f 656d 6169  .maintainer_emai
-000000c0: 6c20 3d20 7374 6570 6865 6e2e 7261 2e6b  l = stephen.ra.k
-000000d0: 696e 6740 676d 6169 6c2e 636f 6d0d 0a64  ing@gmail.com..d
-000000e0: 6573 6372 6970 7469 6f6e 203d 2041 2070  escription = A p
-000000f0: 6970 746f 6f6c 7320 7072 652d 636f 6d6d  iptools pre-comm
-00000100: 6974 2076 6572 7369 6f6e 2073 796e 6320  it version sync 
-00000110: 7574 696c 6974 790d 0a6c 6f6e 675f 6465  utility..long_de
-00000120: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-00000130: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-00000140: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000150: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000160: 742f 6d61 726b 646f 776e 0d0a 6b65 7977  t/markdown..keyw
-00000170: 6f72 6473 203d 2075 7469 6c69 7479 2c0d  ords = utility,.
-00000180: 0a70 6c61 7466 6f72 6d73 203d 2041 6e79  .platforms = Any
-00000190: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-000001a0: 6769 7468 7562 2e63 6f6d 2f53 7465 7068  github.com/Steph
-000001b0: 656e 2d52 412d 4b69 6e67 2f70 6970 746f  en-RA-King/pipto
-000001c0: 6f6c 732d 7379 6e63 0d0a 646f 776e 6c6f  ols-sync..downlo
-000001d0: 6164 5f75 726c 203d 2068 7474 7073 3a2f  ad_url = https:/
-000001e0: 2f67 6974 6875 622e 636f 6d2f 5374 6570  /github.com/Step
-000001f0: 6865 6e2d 5241 2d4b 696e 672f 7069 7074  hen-RA-King/pipt
-00000200: 6f6f 6c73 5f73 796e 632f 6172 6368 6976  ools_sync/archiv
-00000210: 652f 7265 6673 2f68 6561 6473 2f6d 6169  e/refs/heads/mai
-00000220: 6e2e 7a69 700d 0a6c 6963 656e 7365 203d  n.zip..license =
-00000230: 204d 4954 0d0a 6c69 6365 6e73 655f 6669   MIT..license_fi
-00000240: 6c65 203d 204c 4943 454e 5345 0d0a 636c  le = LICENSE..cl
-00000250: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
-00000260: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-00000270: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
-00000280: 696f 6e2f 5374 6162 6c65 0d0a 0945 6e76  ion/Stable...Env
-00000290: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
-000002a0: 6f6c 650d 0a09 496e 7465 6e64 6564 2041  ole...Intended A
-000002b0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
-000002c0: 6f70 6572 730d 0a09 4f70 6572 6174 696e  opers...Operatin
-000002d0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-000002e0: 6e64 6570 656e 6465 6e74 0d0a 094e 6174  ndependent...Nat
-000002f0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
-00000300: 2045 6e67 6c69 7368 0d0a 0950 726f 6772   English...Progr
-00000310: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000320: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-00000330: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000340: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000350: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 0950  :: 3 :: Only...P
-00000360: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000370: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000380: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
-00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000003a0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a0d  ython :: 3.10...
-000003b0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-000003c0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
-000003d0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
-000003e0: 6e64 3a0d 0a70 726f 6a65 6374 5f75 726c  nd:..project_url
-000003f0: 7320 3d20 0d0a 696e 636c 7564 655f 7061  s = ..include_pa
-00000400: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000410: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
-00000420: 6573 203d 203e 3d33 2e38 0d0a 696e 7374  es = >=3.8..inst
-00000430: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000440: 0a09 6169 6f68 7474 700d 0a09 636c 6963  ..aiohttp...clic
-00000450: 6b0d 0a09 6769 7470 7974 686f 6e0d 0a09  k...gitpython...
-00000460: 7079 7961 6d6c 0d0a 0972 6571 7565 7374  pyyaml...request
-00000470: 730d 0a09 746f 6d6c 0d0a 0974 7164 6d0d  s...toml...tqdm.
-00000480: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000490: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000004a0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
-000004b0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000004c0: 5d0d 0a70 6970 746f 6f6c 735f 7379 6e63  ]..piptools_sync
-000004d0: 203d 200d 0a09 636f 6e66 6967 2e74 6f6d   = ...config.tom
-000004e0: 6c0d 0a09 6d61 7070 696e 672e 6a73 6f6e  l...mapping.json
-000004f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000500: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-00000510: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-00000520: 0970 6970 746f 6f6c 735f 7379 6e63 203d  .piptools_sync =
-00000530: 2070 6970 746f 6f6c 735f 7379 6e63 2e70   piptools_sync.p
-00000540: 6970 746f 6f6c 735f 7379 6e63 3a6d 6169  iptools_sync:mai
-00000550: 6e0d 0a0d 0a5b 666c 616b 6538 5d0d 0a64  n....[flake8]..d
-00000560: 6f63 7374 7269 6e67 2d63 6f6e 7665 6e74  ocstring-convent
-00000570: 696f 6e20 3d20 6e75 6d70 790d 0a6d 6178  ion = numpy..max
-00000580: 2d63 6f6d 706c 6578 6974 7920 3d20 3138  -complexity = 18
-00000590: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
-000005a0: 6820 3d20 3838 0d0a 7365 6c65 6374 203d  h = 88..select =
-000005b0: 2042 2c20 4239 2c20 432c 2044 2c20 452c   B, B9, C, D, E,
-000005c0: 2046 2c20 4e2c 2057 0d0a 6578 636c 7564   F, N, W..exclud
-000005d0: 6520 3d20 7465 7374 732f 2a2c 2e74 6f78  e = tests/*,.tox
-000005e0: 2f2a 2c2e 6e6f 782f 2a2c 646f 6373 2f2a  /*,.nox/*,docs/*
-000005f0: 2c2e 6769 742f 2a2c 2e67 6974 6875 622f  ,.git/*,.github/
-00000600: 2a0d 0a69 676e 6f72 6520 3d20 0d0a 0945  *..ignore = ...E
-00000610: 3230 332c 0d0a 0957 3530 332c 0d0a 7065  203,...W503,..pe
-00000620: 722d 6669 6c65 2d69 676e 6f72 6573 203d  r-file-ignores =
-00000630: 200d 0a09 5f5f 696e 6974 5f5f 2e70 793a   ...__init__.py:
-00000640: 4634 3031 0d0a 0970 6174 686d 6167 6963  F401...pathmagic
-00000650: 2e70 793a 4634 3031 0d0a 0974 6573 745f  .py:F401...test_
-00000660: 7069 7074 6f6f 6c73 5f73 796e 632e 7079  piptools_sync.py
-00000670: 3a46 3430 310d 0a0d 0a5b 6567 675f 696e  :F401....[egg_in
-00000680: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000690: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000006a0: 0a0d 0a                                  ...
+00000070: 6d61 696c 203d 2073 6b69 6e67 2e67 6974  mail = sking.git
+00000080: 6875 6240 676d 6169 6c2e 636f 6d0d 0a6d  hub@gmail.com..m
+00000090: 6169 6e74 6169 6e65 7220 3d20 5374 6570  aintainer = Step
+000000a0: 6865 6e20 5220 4120 4b69 6e67 0d0a 6d61  hen R A King..ma
+000000b0: 696e 7461 696e 6572 5f65 6d61 696c 203d  intainer_email =
+000000c0: 2073 6b69 6e67 2e67 6974 6875 6240 676d   sking.github@gm
+000000d0: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
+000000e0: 7469 6f6e 203d 2041 2070 6970 746f 6f6c  tion = A piptool
+000000f0: 7320 7072 652d 636f 6d6d 6974 2076 6572  s pre-commit ver
+00000100: 7369 6f6e 2073 796e 6320 7574 696c 6974  sion sync utilit
+00000110: 790d 0a6c 6f6e 675f 6465 7363 7269 7074  y..long_descript
+00000120: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000130: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000140: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000150: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000160: 646f 776e 0d0a 6b65 7977 6f72 6473 203d  down..keywords =
+00000170: 2075 7469 6c69 7479 2c0d 0a70 6c61 7466   utility,..platf
+00000180: 6f72 6d73 203d 2041 6e79 0d0a 7572 6c20  orms = Any..url 
+00000190: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001a0: 2e63 6f6d 2f53 7465 7068 656e 2d52 412d  .com/Stephen-RA-
+000001b0: 4b69 6e67 2f70 6970 746f 6f6c 732d 7379  King/piptools-sy
+000001c0: 6e63 0d0a 646f 776e 6c6f 6164 5f75 726c  nc..download_url
+000001d0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000001e0: 622e 636f 6d2f 5374 6570 6865 6e2d 5241  b.com/Stephen-RA
+000001f0: 2d4b 696e 672f 7069 7074 6f6f 6c73 5f73  -King/piptools_s
+00000200: 796e 632f 6172 6368 6976 652f 7265 6673  ync/archive/refs
+00000210: 2f68 6561 6473 2f6d 6169 6e2e 7a69 700d  /heads/main.zip.
+00000220: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
+00000230: 6c69 6365 6e73 655f 6669 6c65 203d 204c  license_file = L
+00000240: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
+00000250: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
+00000260: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
+00000270: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
+00000280: 6162 6c65 0d0a 0945 6e76 6972 6f6e 6d65  able...Environme
+00000290: 6e74 203a 3a20 436f 6e73 6f6c 650d 0a09  nt :: Console...
+000002a0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000002b0: 6520 3a3a 2044 6576 656c 6f70 6572 730d  e :: Developers.
+000002c0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000002d0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000002e0: 6465 6e74 0d0a 094e 6174 7572 616c 204c  dent...Natural L
+000002f0: 616e 6775 6167 6520 3a3a 2045 6e67 6c69  anguage :: Engli
+00000300: 7368 0d0a 0950 726f 6772 616d 6d69 6e67  sh...Programming
+00000310: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000320: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
+00000330: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000340: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
+00000350: 3a20 4f6e 6c79 0d0a 0950 726f 6772 616d  : Only...Program
+00000360: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000370: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
+00000380: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000390: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003a0: 3a3a 2033 2e31 300d 0a0d 0a5b 6f70 7469  :: 3.10....[opti
+000003b0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+000003c0: 7220 3d20 0d0a 093d 7372 630d 0a70 6163  r = ...=src..pac
+000003d0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+000003e0: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+000003f0: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000400: 6461 7461 203d 2054 7275 650d 0a70 7974  data = True..pyt
+00000410: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000420: 3d33 2e38 0d0a 696e 7374 616c 6c5f 7265  =3.8..install_re
+00000430: 7175 6972 6573 203d 200d 0a09 6169 6f68  quires = ...aioh
+00000440: 7474 700d 0a09 636c 6963 6b0d 0a09 6769  ttp...click...gi
+00000450: 7470 7974 686f 6e0d 0a09 7079 7961 6d6c  tpython...pyyaml
+00000460: 0d0a 0972 6571 7565 7374 730d 0a09 746f  ...requests...to
+00000470: 6d6c 0d0a 0974 7164 6d0d 0a0d 0a5b 6f70  ml...tqdm....[op
+00000480: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000490: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000004a0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+000004b0: 636b 6167 655f 6461 7461 5d0d 0a70 6970  ckage_data]..pip
+000004c0: 746f 6f6c 735f 7379 6e63 203d 200d 0a09  tools_sync = ...
+000004d0: 636f 6e66 6967 2e74 6f6d 6c0d 0a09 6d61  config.toml...ma
+000004e0: 7070 696e 672e 6a73 6f6e 0d0a 0d0a 5b6f  pping.json....[o
+000004f0: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+00000500: 6e74 735d 0d0a 636f 6e73 6f6c 655f 7363  nts]..console_sc
+00000510: 7269 7074 7320 3d20 0d0a 0970 6970 746f  ripts = ...pipto
+00000520: 6f6c 735f 7379 6e63 203d 2070 6970 746f  ols_sync = pipto
+00000530: 6f6c 735f 7379 6e63 2e70 6970 746f 6f6c  ols_sync.piptool
+00000540: 735f 7379 6e63 3a6d 6169 6e0d 0a0d 0a5b  s_sync:main....[
+00000550: 666c 616b 6538 5d0d 0a64 6f63 7374 7269  flake8]..docstri
+00000560: 6e67 2d63 6f6e 7665 6e74 696f 6e20 3d20  ng-convention = 
+00000570: 6e75 6d70 790d 0a6d 6178 2d63 6f6d 706c  numpy..max-compl
+00000580: 6578 6974 7920 3d20 3138 0d0a 6d61 782d  exity = 18..max-
+00000590: 6c69 6e65 2d6c 656e 6774 6820 3d20 3838  line-length = 88
+000005a0: 0d0a 7365 6c65 6374 203d 2042 2c20 4239  ..select = B, B9
+000005b0: 2c20 432c 2044 2c20 452c 2046 2c20 4e2c  , C, D, E, F, N,
+000005c0: 2057 0d0a 6578 636c 7564 6520 3d20 7465   W..exclude = te
+000005d0: 7374 732f 2a2c 2e74 6f78 2f2a 2c2e 6e6f  sts/*,.tox/*,.no
+000005e0: 782f 2a2c 646f 6373 2f2a 2c2e 6769 742f  x/*,docs/*,.git/
+000005f0: 2a2c 2e67 6974 6875 622f 2a0d 0a69 676e  *,.github/*..ign
+00000600: 6f72 6520 3d20 0d0a 0945 3230 332c 0d0a  ore = ...E203,..
+00000610: 0957 3530 332c 0d0a 7065 722d 6669 6c65  .W503,..per-file
+00000620: 2d69 676e 6f72 6573 203d 200d 0a09 5f5f  -ignores = ...__
+00000630: 696e 6974 5f5f 2e70 793a 4634 3031 0d0a  init__.py:F401..
+00000640: 0970 6174 686d 6167 6963 2e70 793a 4634  .pathmagic.py:F4
+00000650: 3031 0d0a 0974 6573 745f 7069 7074 6f6f  01...test_piptoo
+00000660: 6c73 5f73 796e 632e 7079 3a46 3430 310d  ls_sync.py:F401.
+00000670: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000680: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000690: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `piptools_sync-1.0.2/src/piptools_sync/__init__.py` & `piptools_sync-1.0.3/src/piptools_sync/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+#!/usr/bin/env python3
 """Top-level package for piptools_sync."""
 # Core Library modules
 import logging.config
 from importlib.resources import as_file, files
 from pathlib import Path
 
 # Third party modules
 import git
 import toml  # type: ignore
 import yaml  # type: ignore
 
 __title__ = "piptools-sync"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Stephen R A King"
 __description__ = "A piptools pre-commit version sync utility"
-__email__ = "stephen.ra.king@gmail.com"
+__email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 Stephen R A King"
 
 
 ROOT_DIR = Path(git.Repo(".", search_parent_directories=True).working_tree_dir)
 
 LOGGING_CONFIG = """
```

### Comparing `piptools_sync-1.0.2/src/piptools_sync/mapping.json` & `piptools_sync-1.0.3/src/piptools_sync/mapping.json`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/src/piptools_sync/piptools_sync.py` & `piptools_sync-1.0.3/src/piptools_sync/piptools_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 """A pre-commit utility plugin to verify requirement versions determined by
 pip-tools are utilized by pre-commit
 """
 
 # Core Library modules
 import json
 import os
```

### Comparing `piptools_sync-1.0.2/src/piptools_sync.egg-info/PKG-INFO` & `piptools_sync-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: piptools-sync
-Version: 1.0.2
+Name: piptools_sync
+Version: 1.0.3
 Summary: A piptools pre-commit version sync utility
 Home-page: https://github.com/Stephen-RA-King/piptools-sync
 Download-URL: https://github.com/Stephen-RA-King/piptools_sync/archive/refs/heads/main.zip
 Author: Stephen R A King
-Author-email: stephen.ra.king@gmail.com
+Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
-Maintainer-email: stephen.ra.king@gmail.com
+Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -20,27 +20,28 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# piptools-sync
+# Piptools-sync
 
 ---
 
-> A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools..
+_**A pre-commit plugin to align pre-commit repository versions with those derived by pip-tools.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
 [![tests][tests-image]][tests-url]
 [![Codecov][codecov-image]][codecov-url]
+[![pre-commit.ci][pre-commit.ci-image]][pre-commit.ci-url]
 [![CodeFactor][codefactor-image]][codefactor-url]
 [![Codeclimate][codeclimate-image]][codeclimate-url]
 [![CodeQl][codeql-image]][codeql-url]
 [![readthedocs][readthedocs-image]][readthedocs-url]
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
@@ -198,17 +199,22 @@
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## Documentation
 
 ---
 
-### - [**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/)
+[**Read the Docs**](https://piptools-sync.readthedocs.io/en/latest/?)
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
+- [**Example Usage**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://piptools-sync.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://piptools-sync.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://piptools-sync.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**](https://github.com/Stephen-RA-King/piptools-sync/wiki)
 
 ## Future Enhancements
 
 ---
 
 - Move some global variables into a separate settings file (toml).
 - Settings configurable from the command line (and therefore configurable from the pre-commit.yaml file).
@@ -220,29 +226,27 @@
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/piptools-sync)
 [![](assets/www.png)](https://www.justpython.tech)
 [![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Stephen R A King : stephen.ra.king@gmail.com
-
-Distributed under the MIT license. See [license][license-url] for more information.
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-[https://github.com/Stephen-RA-King/piptools-sync](https://github.com/Stephen-RA-King/piptools-sync)
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.1
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/9543c409696e9976a987/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/piptools-sync/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/piptools-sync/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/piptools-sync
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/piptools-sync/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/piptools-sync
 [codeql-image]: https://github.com/Stephen-RA-King/piptools-sync/actions/workflows/github-code-scanning/codeql/badge.svg
```

### Comparing `piptools_sync-1.0.2/src/piptools_sync.egg-info/SOURCES.txt` & `piptools_sync-1.0.3/src/piptools_sync.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 src/piptools_sync/__init__.py
 src/piptools_sync/config.toml
 src/piptools_sync/mapping.json
 src/piptools_sync/piptools_sync.py
 src/piptools_sync.egg-info/PKG-INFO
+src/piptools_sync.egg-info/PKG-INFO.rum-bak
 src/piptools_sync.egg-info/SOURCES.txt
 src/piptools_sync.egg-info/dependency_links.txt
 src/piptools_sync.egg-info/entry_points.txt
 src/piptools_sync.egg-info/requires.txt
 src/piptools_sync.egg-info/top_level.txt
 tests/test__utility_find_file_path.py
 tests/test__utility_remove_vee.py
```

### Comparing `piptools_sync-1.0.2/tests/test__utility_find_file_path.py` & `piptools_sync-1.0.3/tests/test__utility_find_file_path.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/tests/test__utility_remove_vee.py` & `piptools_sync-1.0.3/tests/test__utility_remove_vee.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/tests/test_find_requirements_file.py` & `piptools_sync-1.0.3/tests/test_find_requirements_file.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/tests/test_generate_db.py` & `piptools_sync-1.0.3/tests/test_generate_db.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/tests/test_get_requirement_versions.py` & `piptools_sync-1.0.3/tests/test_get_requirement_versions.py`

 * *Files identical despite different names*

### Comparing `piptools_sync-1.0.2/tests/test_update_yaml.py` & `piptools_sync-1.0.3/tests/test_update_yaml.py`

 * *Files identical despite different names*

