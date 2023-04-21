# Comparing `tmp/pynnacle-1.1.1.tar.gz` & `tmp/pynnacle-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynnacle-1.1.1.tar", last modified: Sat Oct  8 17:25:41 2022, max compression
+gzip compressed data, was "pynnacle-1.1.2.tar", last modified: Fri Apr 21 13:44:46 2023, max compression
```

## Comparing `pynnacle-1.1.1.tar` & `pynnacle-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-10-08 17:25:41.737339 pynnacle-1.1.1/
--rw-rw-rw-   0        0        0      163 2022-08-01 13:42:04.000000 pynnacle-1.1.1/AUTHORS.md
--rw-rw-rw-   0        0        0     1139 2022-10-08 17:25:31.000000 pynnacle-1.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-08-01 13:05:46.000000 pynnacle-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      194 2022-08-01 13:05:46.000000 pynnacle-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9817 2022-10-08 17:25:41.737339 pynnacle-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8544 2022-10-08 17:21:13.000000 pynnacle-1.1.1/README.md
--rw-rw-rw-   0        0        0     2215 2022-10-08 17:08:41.000000 pynnacle-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1611 2022-10-08 17:25:41.738336 pynnacle-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-08-01 13:05:46.000000 pynnacle-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-08 17:25:41.692347 pynnacle-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2022-10-08 17:25:41.726338 pynnacle-1.1.1/src/pynnacle/
--rw-rw-rw-   0        0        0     1430 2022-10-08 17:25:31.000000 pynnacle-1.1.1/src/pynnacle/__init__.py
--rw-rw-rw-   0        0        0      953 2021-07-15 06:06:06.000000 pynnacle-1.1.1/src/pynnacle/config.ini
--rw-rw-rw-   0        0        0     8368 2022-08-01 19:15:14.000000 pynnacle-1.1.1/src/pynnacle/pynnacle.py
-drwxrwxrwx   0        0        0        0 2022-10-08 17:25:41.734349 pynnacle-1.1.1/src/pynnacle.egg-info/
--rw-rw-rw-   0        0        0     9817 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-08 17:25:41.000000 pynnacle-1.1.1/src/pynnacle.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 13:44:46.770288 pynnacle-1.1.2/
+-rw-rw-rw-   0        0        0      157 2023-04-18 15:26:49.000000 pynnacle-1.1.2/AUTHORS.md
+-rw-rw-rw-   0        0        0     2280 2023-04-21 13:44:36.000000 pynnacle-1.1.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1074 2022-08-01 13:05:46.000000 pynnacle-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      194 2022-08-01 13:05:46.000000 pynnacle-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9973 2023-04-21 13:44:46.770288 pynnacle-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8688 2023-04-19 22:07:28.000000 pynnacle-1.1.2/README.md
+-rw-rw-rw-   0        0        0     2215 2022-10-08 17:08:41.000000 pynnacle-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1605 2023-04-21 13:44:46.770288 pynnacle-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      108 2023-04-21 12:34:36.000000 pynnacle-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:44:46.685611 pynnacle-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 13:44:46.754650 pynnacle-1.1.2/src/pynnacle/
+-rw-rw-rw-   0        0        0     1451 2023-04-21 13:44:36.000000 pynnacle-1.1.2/src/pynnacle/__init__.py
+-rw-rw-rw-   0        0        0      953 2021-07-15 06:06:06.000000 pynnacle-1.1.2/src/pynnacle/config.ini
+-rw-rw-rw-   0        0        0     8392 2023-04-21 12:34:36.000000 pynnacle-1.1.2/src/pynnacle/pynnacle.py
+drwxrwxrwx   0        0        0        0 2023-04-21 13:44:46.770288 pynnacle-1.1.2/src/pynnacle.egg-info/
+-rw-rw-rw-   0        0        0     9973 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 13:44:46.000000 pynnacle-1.1.2/src/pynnacle.egg-info/top_level.txt
```

### Comparing `pynnacle-1.1.1/LICENSE` & `pynnacle-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynnacle-1.1.1/PKG-INFO` & `pynnacle-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pynnacle
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utility wrapper class to leverage email transmission
 Home-page: https://github.com/Stephen-RA-King/pynnacle
 Download-URL: https://github.com/Stephen-RA-King/pynnacle/archive/refs/heads/main.zip
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
@@ -22,30 +22,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# pynnacle
+# Pynnacle
 
-> A utility class to simplify sending emails.
+_**A utility class to simplify sending emails.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+
+<!--[![tests][tests-image]][tests-url]
+[![Codecov][codecov-image]][codecov-url] -->
+
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
+[![CodeQl][codeql-image]][codeql-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
@@ -54,51 +58,55 @@
 interface to make sending emails as simple as possible. It abstracts away all the low level details and when
 imported into other modules provides a clean, clutter-free interface.
 
 ![](assets/header.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install pynnacle
 ```
 
 Windows:
 
 ```sh
 pip install pynnacle
 ```
 
 ## Usage example
 
+---
+
 Firstly import the module
 
 ```sh
 from pynnacle.pynnacle import SendEmail
 ```
 
 Pynnacle stores the configuration of email servers in an 'ini' configuration file.
 If a service is already configured then the main class can be instantiated with only 3 arguments e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="gmail"
+    service="gmail",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
 )
 ```
 
 If the service has not been configured, simply pass "custom" as the service and pass the other smtp arguments
 to the initializer e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="custom"
+    service="custom",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
     smtp_server="smtp.abc.com",
     smtp_port=25,
     smtp_authentication="yes",
     smtp_encryption="yes",
 )
@@ -127,14 +135,16 @@
     bcc=["person3@jkl.com", "person4@mno.com"],
     attachments=["path_to_file1", "path_to_file2"]
 )
 ```
 
 ## Further simplifications
 
+---
+
 ### Storing and Reusing SMTP
 
 Additional setting can be saved in the "ini" file as and when you like.
 
 e.g.config.ini
 
 ```sh
@@ -160,55 +170,63 @@
 user_pass = keyring.get_password(service, "service_password")
 ```
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## A Note on gmail authentication
 
+---
+
 As of 30/05/2022 Google will no longer support the use of third-party apps or devices that only ask for your username and password.
 The "Less secure app access" setting has now been turned off.
 The application now has to be assigned a 16 byte code which can be configured from your account as follows:
 
 - 1 Log onto your account: https://myaccount.google.com
 - 2 Goto security
 - 3 Enable 2-step verification
 - 4 click "App password" to generate the key
 
 Then simply use this along with the account email address to authenticate
 
 ## Documentation
 
-### - [**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/?)
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/pynnacle/wiki)
+- [**Example Usage**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynnacle.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynnacle.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynnacle/)
+[![](assets/pypi.png)](https://pypi.org/project/pynnacle)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
-
-Stephen R A King : stephen.ra.king@gmail.com
+[![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Distributed under the MIT license. See [license][license-url] for more information.
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-[https://github.com/Stephen-RA-King/pynnacle](https://github.com/Stephen-RA-King/pynnacle)
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.0
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynnacle/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynnacle/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynnacle
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle
 [codeql-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/codeql-analysis.yml/badge.svg
@@ -218,30 +236,30 @@
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynnacle/?ref=repository-badge
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynnacle?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynnacle
 [format-image]: https://img.shields.io/pypi/format/pynnacle
+[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/context:python
 [license-image]: https://img.shields.io/pypi/l/pynnacle
 [license-url]: https://github.com/Stephen-RA-King/pynnacle/blob/main/license
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynnacle/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynnacle/main
 [pypi-url]: https://pypi.org/project/pynnacle/
 [pypi-image]: https://img.shields.io/pypi/v/pynnacle.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynnacle
 [readthedocs-image]: https://readthedocs.org/projects/pynnacle/badge/?version=latest
 [readthedocs-url]: https://pynnacle.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/pynnacle.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynnacle/wiki
```

### Comparing `pynnacle-1.1.1/README.md` & `pynnacle-1.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-# pynnacle
+# Pynnacle
 
-> A utility class to simplify sending emails.
+_**A utility class to simplify sending emails.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+
+<!--[![tests][tests-image]][tests-url]
+[![Codecov][codecov-image]][codecov-url] -->
+
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
+[![CodeQl][codeql-image]][codeql-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
@@ -26,51 +30,55 @@
 interface to make sending emails as simple as possible. It abstracts away all the low level details and when
 imported into other modules provides a clean, clutter-free interface.
 
 ![](assets/header.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install pynnacle
 ```
 
 Windows:
 
 ```sh
 pip install pynnacle
 ```
 
 ## Usage example
 
+---
+
 Firstly import the module
 
 ```sh
 from pynnacle.pynnacle import SendEmail
 ```
 
 Pynnacle stores the configuration of email servers in an 'ini' configuration file.
 If a service is already configured then the main class can be instantiated with only 3 arguments e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="gmail"
+    service="gmail",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
 )
 ```
 
 If the service has not been configured, simply pass "custom" as the service and pass the other smtp arguments
 to the initializer e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="custom"
+    service="custom",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
     smtp_server="smtp.abc.com",
     smtp_port=25,
     smtp_authentication="yes",
     smtp_encryption="yes",
 )
@@ -99,14 +107,16 @@
     bcc=["person3@jkl.com", "person4@mno.com"],
     attachments=["path_to_file1", "path_to_file2"]
 )
 ```
 
 ## Further simplifications
 
+---
+
 ### Storing and Reusing SMTP
 
 Additional setting can be saved in the "ini" file as and when you like.
 
 e.g.config.ini
 
 ```sh
@@ -132,55 +142,63 @@
 user_pass = keyring.get_password(service, "service_password")
 ```
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## A Note on gmail authentication
 
+---
+
 As of 30/05/2022 Google will no longer support the use of third-party apps or devices that only ask for your username and password.
 The "Less secure app access" setting has now been turned off.
 The application now has to be assigned a 16 byte code which can be configured from your account as follows:
 
 - 1 Log onto your account: https://myaccount.google.com
 - 2 Goto security
 - 3 Enable 2-step verification
 - 4 click "App password" to generate the key
 
 Then simply use this along with the account email address to authenticate
 
 ## Documentation
 
-### - [**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/?)
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/pynnacle/wiki)
+- [**Example Usage**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynnacle.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynnacle.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynnacle/)
+[![](assets/pypi.png)](https://pypi.org/project/pynnacle)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
-
-Stephen R A King : stephen.ra.king@gmail.com
+[![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Distributed under the MIT license. See [license][license-url] for more information.
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-[https://github.com/Stephen-RA-King/pynnacle](https://github.com/Stephen-RA-King/pynnacle)
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.0
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynnacle/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynnacle/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynnacle
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle
 [codeql-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/codeql-analysis.yml/badge.svg
@@ -190,30 +208,30 @@
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynnacle/?ref=repository-badge
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynnacle?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynnacle
 [format-image]: https://img.shields.io/pypi/format/pynnacle
+[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/context:python
 [license-image]: https://img.shields.io/pypi/l/pynnacle
 [license-url]: https://github.com/Stephen-RA-King/pynnacle/blob/main/license
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynnacle/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynnacle/main
 [pypi-url]: https://pypi.org/project/pynnacle/
 [pypi-image]: https://img.shields.io/pypi/v/pynnacle.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynnacle
 [readthedocs-image]: https://readthedocs.org/projects/pynnacle/badge/?version=latest
 [readthedocs-url]: https://pynnacle.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/pynnacle.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynnacle/wiki
```

### Comparing `pynnacle-1.1.1/pyproject.toml` & `pynnacle-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynnacle-1.1.1/setup.cfg` & `pynnacle-1.1.2/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796e 6e61 636c 650d 0a76 6572   = pynnacle..ver
 00000020: 7369 6f6e 203d 2061 7474 723a 2070 796e  sion = attr: pyn
 00000030: 6e61 636c 652e 5f5f 7665 7273 696f 6e5f  nacle.__version_
 00000040: 5f0d 0a61 7574 686f 7220 3d20 5374 6570  _..author = Step
 00000050: 6865 6e20 5220 4120 4b69 6e67 0d0a 6175  hen R A King..au
-00000060: 7468 6f72 5f65 6d61 696c 203d 2073 7465  thor_email = ste
-00000070: 7068 656e 2e72 612e 6b69 6e67 4067 6d61  phen.ra.king@gma
-00000080: 696c 2e63 6f6d 0d0a 6d61 696e 7461 696e  il.com..maintain
-00000090: 6572 203d 2053 7465 7068 656e 2052 2041  er = Stephen R A
-000000a0: 204b 696e 670d 0a6d 6169 6e74 6169 6e65   King..maintaine
-000000b0: 725f 656d 6169 6c20 3d20 7374 6570 6865  r_email = stephe
-000000c0: 6e2e 7261 2e6b 696e 6740 676d 6169 6c2e  n.ra.king@gmail.
-000000d0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
-000000e0: 203d 2055 7469 6c69 7479 2077 7261 7070   = Utility wrapp
-000000f0: 6572 2063 6c61 7373 2074 6f20 6c65 7665  er class to leve
-00000100: 7261 6765 2065 6d61 696c 2074 7261 6e73  rage email trans
-00000110: 6d69 7373 696f 6e0d 0a6c 6f6e 675f 6465  mission..long_de
-00000120: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-00000130: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-00000140: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000150: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000160: 742f 6d61 726b 646f 776e 0d0a 6b65 7977  t/markdown..keyw
-00000170: 6f72 6473 203d 2075 7469 6c69 7479 2c0d  ords = utility,.
-00000180: 0a70 6c61 7466 6f72 6d73 203d 2041 6e79  .platforms = Any
-00000190: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-000001a0: 6769 7468 7562 2e63 6f6d 2f53 7465 7068  github.com/Steph
-000001b0: 656e 2d52 412d 4b69 6e67 2f70 796e 6e61  en-RA-King/pynna
-000001c0: 636c 650d 0a64 6f77 6e6c 6f61 645f 7572  cle..download_ur
-000001d0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
-000001e0: 7562 2e63 6f6d 2f53 7465 7068 656e 2d52  ub.com/Stephen-R
-000001f0: 412d 4b69 6e67 2f70 796e 6e61 636c 652f  A-King/pynnacle/
-00000200: 6172 6368 6976 652f 7265 6673 2f68 6561  archive/refs/hea
-00000210: 6473 2f6d 6169 6e2e 7a69 700d 0a6c 6963  ds/main.zip..lic
-00000220: 656e 7365 203d 204d 4954 0d0a 636c 6173  ense = MIT..clas
-00000230: 7369 6669 6572 7320 3d20 0d0a 0944 6576  sifiers = ...Dev
-00000240: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
-00000250: 3a3a 2035 202d 2050 726f 6475 6374 696f  :: 5 - Productio
-00000260: 6e2f 5374 6162 6c65 0d0a 0945 6e76 6972  n/Stable...Envir
-00000270: 6f6e 6d65 6e74 203a 3a20 436f 6e73 6f6c  onment :: Consol
-00000280: 650d 0a09 496e 7465 6e64 6564 2041 7564  e...Intended Aud
-00000290: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
-000002a0: 6572 730d 0a09 4f70 6572 6174 696e 6720  ers...Operating 
-000002b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000002c0: 6570 656e 6465 6e74 0d0a 094e 6174 7572  ependent...Natur
-000002d0: 616c 204c 616e 6775 6167 6520 3a3a 2045  al Language :: E
-000002e0: 6e67 6c69 7368 0d0a 0950 726f 6772 616d  nglish...Program
-000002f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000300: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
-00000310: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000320: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000330: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
-00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000360: 2e38 0d0a 0950 726f 6772 616d 6d69 6e67  .8...Programming
-00000370: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000380: 686f 6e20 3a3a 2033 2e39 0d0a 0950 726f  hon :: 3.9...Pro
-00000390: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000003a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000003b0: 2e31 300d 0a0d 0a5b 6f70 7469 6f6e 735d  .10....[options]
-000003c0: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-000003d0: 0d0a 093d 7372 630d 0a70 6163 6b61 6765  ...=src..package
-000003e0: 7320 3d20 6669 6e64 3a0d 0a70 726f 6a65  s = find:..proje
-000003f0: 6374 5f75 726c 7320 3d20 0d0a 696e 636c  ct_urls = ..incl
-00000400: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000410: 203d 2054 7275 650d 0a70 7974 686f 6e5f   = True..python_
-00000420: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
-00000430: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-00000440: 6573 203d 200d 0a09 636c 6963 6b0d 0a0d  es = ...click...
-00000450: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000460: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000470: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
-00000480: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000490: 0a70 796e 6e61 636c 6520 3d20 0d0a 0963  .pynnacle = ...c
-000004a0: 6f6e 6669 672e 696e 690d 0a0d 0a5b 6f70  onfig.ini....[op
-000004b0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000004c0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-000004d0: 6970 7473 203d 200d 0a09 7079 6e6e 6163  ipts = ...pynnac
-000004e0: 6c65 203d 2070 796e 6e61 636c 652e 7079  le = pynnacle.py
-000004f0: 6e6e 6163 6c65 5f63 6c69 3a63 6c69 0d0a  nnacle_cli:cli..
-00000500: 0d0a 5b66 6c61 6b65 385d 0d0a 646f 6373  ..[flake8]..docs
-00000510: 7472 696e 672d 636f 6e76 656e 7469 6f6e  tring-convention
-00000520: 203d 206e 756d 7079 0d0a 6d61 782d 636f   = numpy..max-co
-00000530: 6d70 6c65 7869 7479 203d 2031 380d 0a6d  mplexity = 18..m
-00000540: 6178 2d6c 696e 652d 6c65 6e67 7468 203d  ax-line-length =
-00000550: 2038 380d 0a73 656c 6563 7420 3d20 422c   88..select = B,
-00000560: 2042 392c 2043 2c20 442c 2045 2c20 462c   B9, C, D, E, F,
-00000570: 204e 2c20 570d 0a65 7863 6c75 6465 203d   N, W..exclude =
-00000580: 2074 6573 7473 2f2a 2c2e 746f 782f 2a2c   tests/*,.tox/*,
-00000590: 2e6e 6f78 2f2a 2c64 6f63 732f 2a2c 2e67  .nox/*,docs/*,.g
-000005a0: 6974 2f2a 2c2e 6769 7468 7562 2f2a 0d0a  it/*,.github/*..
-000005b0: 6967 6e6f 7265 203d 200d 0a09 4532 3033  ignore = ...E203
-000005c0: 2c0d 0a09 5735 3033 2c0d 0a70 6572 2d66  ,...W503,..per-f
-000005d0: 696c 652d 6967 6e6f 7265 7320 3d20 0d0a  ile-ignores = ..
-000005e0: 095f 5f69 6e69 745f 5f2e 7079 3a46 3430  .__init__.py:F40
-000005f0: 310d 0a09 7061 7468 6d61 6769 632e 7079  1...pathmagic.py
-00000600: 3a46 3430 310d 0a09 7465 7374 5f70 796e  :F401...test_pyn
-00000610: 6e61 636c 652e 7079 3a46 3430 310d 0a0d  nacle.py:F401...
-00000620: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000630: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000640: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000060: 7468 6f72 5f65 6d61 696c 203d 2073 6b69  thor_email = ski
+00000070: 6e67 2e67 6974 6875 6240 676d 6169 6c2e  ng.github@gmail.
+00000080: 636f 6d0d 0a6d 6169 6e74 6169 6e65 7220  com..maintainer 
+00000090: 3d20 5374 6570 6865 6e20 5220 4120 4b69  = Stephen R A Ki
+000000a0: 6e67 0d0a 6d61 696e 7461 696e 6572 5f65  ng..maintainer_e
+000000b0: 6d61 696c 203d 2073 6b69 6e67 2e67 6974  mail = sking.git
+000000c0: 6875 6240 676d 6169 6c2e 636f 6d0d 0a64  hub@gmail.com..d
+000000d0: 6573 6372 6970 7469 6f6e 203d 2055 7469  escription = Uti
+000000e0: 6c69 7479 2077 7261 7070 6572 2063 6c61  lity wrapper cla
+000000f0: 7373 2074 6f20 6c65 7665 7261 6765 2065  ss to leverage e
+00000100: 6d61 696c 2074 7261 6e73 6d69 7373 696f  mail transmissio
+00000110: 6e0d 0a6c 6f6e 675f 6465 7363 7269 7074  n..long_descript
+00000120: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000130: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000140: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000150: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000160: 646f 776e 0d0a 6b65 7977 6f72 6473 203d  down..keywords =
+00000170: 2075 7469 6c69 7479 2c0d 0a70 6c61 7466   utility,..platf
+00000180: 6f72 6d73 203d 2041 6e79 0d0a 7572 6c20  orms = Any..url 
+00000190: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001a0: 2e63 6f6d 2f53 7465 7068 656e 2d52 412d  .com/Stephen-RA-
+000001b0: 4b69 6e67 2f70 796e 6e61 636c 650d 0a64  King/pynnacle..d
+000001c0: 6f77 6e6c 6f61 645f 7572 6c20 3d20 6874  ownload_url = ht
+000001d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001e0: 2f53 7465 7068 656e 2d52 412d 4b69 6e67  /Stephen-RA-King
+000001f0: 2f70 796e 6e61 636c 652f 6172 6368 6976  /pynnacle/archiv
+00000200: 652f 7265 6673 2f68 6561 6473 2f6d 6169  e/refs/heads/mai
+00000210: 6e2e 7a69 700d 0a6c 6963 656e 7365 203d  n.zip..license =
+00000220: 204d 4954 0d0a 636c 6173 7369 6669 6572   MIT..classifier
+00000230: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
+00000240: 6e74 2053 7461 7475 7320 3a3a 2035 202d  nt Status :: 5 -
+00000250: 2050 726f 6475 6374 696f 6e2f 5374 6162   Production/Stab
+00000260: 6c65 0d0a 0945 6e76 6972 6f6e 6d65 6e74  le...Environment
+00000270: 203a 3a20 436f 6e73 6f6c 650d 0a09 496e   :: Console...In
+00000280: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000290: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+000002a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000002b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000002c0: 6e74 0d0a 094e 6174 7572 616c 204c 616e  nt...Natural Lan
+000002d0: 6775 6167 6520 3a3a 2045 6e67 6c69 7368  guage :: English
+000002e0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000002f0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000300: 6e20 3a3a 2033 0d0a 0950 726f 6772 616d  n :: 3...Program
+00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000320: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
+00000330: 4f6e 6c79 0d0a 0950 726f 6772 616d 6d69  Only...Programmi
+00000340: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000350: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
+00000360: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000370: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000380: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000390: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000003a0: 7974 686f 6e20 3a3a 2033 2e31 300d 0a0d  ython :: 3.10...
+000003b0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
+000003c0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+000003d0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
+000003e0: 6e64 3a0d 0a70 726f 6a65 6374 5f75 726c  nd:..project_url
+000003f0: 7320 3d20 0d0a 696e 636c 7564 655f 7061  s = ..include_pa
+00000400: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+00000410: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
+00000420: 6573 203d 203e 3d33 2e38 0d0a 696e 7374  es = >=3.8..inst
+00000430: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000440: 0a09 636c 6963 6b0d 0a0d 0a5b 6f70 7469  ..click....[opti
+00000450: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000460: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000470: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000480: 6167 655f 6461 7461 5d0d 0a70 796e 6e61  age_data]..pynna
+00000490: 636c 6520 3d20 0d0a 0963 6f6e 6669 672e  cle = ...config.
+000004a0: 696e 690d 0a0d 0a5b 6f70 7469 6f6e 732e  ini....[options.
+000004b0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+000004c0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+000004d0: 200d 0a09 7079 6e6e 6163 6c65 203d 2070   ...pynnacle = p
+000004e0: 796e 6e61 636c 652e 7079 6e6e 6163 6c65  ynnacle.pynnacle
+000004f0: 5f63 6c69 3a63 6c69 0d0a 0d0a 5b66 6c61  _cli:cli....[fla
+00000500: 6b65 385d 0d0a 646f 6373 7472 696e 672d  ke8]..docstring-
+00000510: 636f 6e76 656e 7469 6f6e 203d 206e 756d  convention = num
+00000520: 7079 0d0a 6d61 782d 636f 6d70 6c65 7869  py..max-complexi
+00000530: 7479 203d 2031 380d 0a6d 6178 2d6c 696e  ty = 18..max-lin
+00000540: 652d 6c65 6e67 7468 203d 2038 380d 0a73  e-length = 88..s
+00000550: 656c 6563 7420 3d20 422c 2042 392c 2043  elect = B, B9, C
+00000560: 2c20 442c 2045 2c20 462c 204e 2c20 570d  , D, E, F, N, W.
+00000570: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
+00000580: 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a  /*,.tox/*,.nox/*
+00000590: 2c64 6f63 732f 2a2c 2e67 6974 2f2a 2c2e  ,docs/*,.git/*,.
+000005a0: 6769 7468 7562 2f2a 0d0a 6967 6e6f 7265  github/*..ignore
+000005b0: 203d 200d 0a09 4532 3033 2c0d 0a09 5735   = ...E203,...W5
+000005c0: 3033 2c0d 0a70 6572 2d66 696c 652d 6967  03,..per-file-ig
+000005d0: 6e6f 7265 7320 3d20 0d0a 095f 5f69 6e69  nores = ...__ini
+000005e0: 745f 5f2e 7079 3a46 3430 310d 0a09 7061  t__.py:F401...pa
+000005f0: 7468 6d61 6769 632e 7079 3a46 3430 310d  thmagic.py:F401.
+00000600: 0a09 7465 7374 5f70 796e 6e61 636c 652e  ..test_pynnacle.
+00000610: 7079 3a46 3430 310d 0a0d 0a5b 6567 675f  py:F401....[egg_
+00000620: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000630: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000640: 300d 0a0d 0a                             0....
```

### Comparing `pynnacle-1.1.1/src/pynnacle/__init__.py` & `pynnacle-1.1.2/src/pynnacle/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+#!/usr/bin/env python3
 """Top-level package for pynnacle."""
 # Core Library modules
 import configparser
 import json
 import logging.config
 from importlib import resources
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynnacle"
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 __author__ = "Stephen R A King"
 __description__ = "Utiltiy wrapper class to leverage email transmission"
-__email__ = "stephen.ra.king@gmail.com"
+__email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022 Stephen R A King"
 
 LOGGING_CONFIG = """
 version: 1
 disable_existing_loggers: False
 handlers:
```

### Comparing `pynnacle-1.1.1/src/pynnacle/config.ini` & `pynnacle-1.1.2/src/pynnacle/config.ini`

 * *Files identical despite different names*

### Comparing `pynnacle-1.1.1/src/pynnacle/pynnacle.py` & `pynnacle-1.1.2/src/pynnacle/pynnacle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 """A utility class to simplify the sending of emails."""
 # Core Library modules
 import mimetypes
 import re
 import smtplib
 from email.message import EmailMessage
 from pathlib import Path
```

### Comparing `pynnacle-1.1.1/src/pynnacle.egg-info/PKG-INFO` & `pynnacle-1.1.2/src/pynnacle.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pynnacle
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utility wrapper class to leverage email transmission
 Home-page: https://github.com/Stephen-RA-King/pynnacle
 Download-URL: https://github.com/Stephen-RA-King/pynnacle/archive/refs/heads/main.zip
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
@@ -22,30 +22,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# pynnacle
+# Pynnacle
 
-> A utility class to simplify sending emails.
+_**A utility class to simplify sending emails.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
-[![Requirements][requirements-status-image]][requirements-status-url]
-[![Lgtm alerts][lgtm-alerts-image]][lgtm-alerts-url]
-[![Lgtm quality][lgtm-quality-image]][lgtm-quality-url]
-[![CodeQl][codeql-image]][codeql-url]
-[![readthedocs][readthedocs-image]][readthedocs-url]
+
+<!--[![tests][tests-image]][tests-url]
+[![Codecov][codecov-image]][codecov-url] -->
+
 [![pre-commit][pre-commit-image]][pre-commit-url]
 [![pre-commit.ci status][pre-commit.ci-image]][pre-commit.ci-url]
+[![CodeFactor][codefactor-image]][codefactor-url]
+[![Codeclimate][codeclimate-image]][codeclimate-url]
+[![CodeQl][codeql-image]][codeql-url]
+[![readthedocs][readthedocs-image]][readthedocs-url]
+[![Imports: isort][isort-image]][isort-url]
 [![Code style: black][black-image]][black-url]
 [![Checked with mypy][mypy-image]][mypy-url]
 [![security: bandit][bandit-image]][bandit-url]
 [![Commitizen friendly][commitizen-image]][commitizen-url]
 [![Conventional Commits][conventional-commits-image]][conventional-commits-url]
 [![DeepSource][deepsource-image]][deepsource-url]
 [![license][license-image]][license-url]
@@ -54,51 +58,55 @@
 interface to make sending emails as simple as possible. It abstracts away all the low level details and when
 imported into other modules provides a clean, clutter-free interface.
 
 ![](assets/header.png)
 
 ## Installation
 
+---
+
 OS X & Linux:
 
 ```sh
 pip3 install pynnacle
 ```
 
 Windows:
 
 ```sh
 pip install pynnacle
 ```
 
 ## Usage example
 
+---
+
 Firstly import the module
 
 ```sh
 from pynnacle.pynnacle import SendEmail
 ```
 
 Pynnacle stores the configuration of email servers in an 'ini' configuration file.
 If a service is already configured then the main class can be instantiated with only 3 arguments e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="gmail"
+    service="gmail",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
 )
 ```
 
 If the service has not been configured, simply pass "custom" as the service and pass the other smtp arguments
 to the initializer e.g.:
 
 ```sh
 mailer = SendEmail(
-    service="custom"
+    service="custom",
     user_id="jsmith",
     user_pass="P@zzw0rd1",
     smtp_server="smtp.abc.com",
     smtp_port=25,
     smtp_authentication="yes",
     smtp_encryption="yes",
 )
@@ -127,14 +135,16 @@
     bcc=["person3@jkl.com", "person4@mno.com"],
     attachments=["path_to_file1", "path_to_file2"]
 )
 ```
 
 ## Further simplifications
 
+---
+
 ### Storing and Reusing SMTP
 
 Additional setting can be saved in the "ini" file as and when you like.
 
 e.g.config.ini
 
 ```sh
@@ -160,55 +170,63 @@
 user_pass = keyring.get_password(service, "service_password")
 ```
 
 _For more examples and usage, please refer to the [Wiki][wiki]._
 
 ## A Note on gmail authentication
 
+---
+
 As of 30/05/2022 Google will no longer support the use of third-party apps or devices that only ask for your username and password.
 The "Less secure app access" setting has now been turned off.
 The application now has to be assigned a 16 byte code which can be configured from your account as follows:
 
 - 1 Log onto your account: https://myaccount.google.com
 - 2 Goto security
 - 3 Enable 2-step verification
 - 4 click "App password" to generate the key
 
 Then simply use this along with the account email address to authenticate
 
 ## Documentation
 
-### - [**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/)
+---
+
+[**Read the Docs**](https://pynnacle.readthedocs.io/en/latest/?)
 
-### - [**Wiki**](https://github.com/Stephen-RA-King/pynnacle/wiki)
+- [**Example Usage**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Credits**](https://pynnacle.readthedocs.io/en/latest/example.html)
+- [**Changelog**](https://pynnacle.readthedocs.io/en/latest/changelog.html)
+- [**API Reference**](https://pynnacle.readthedocs.io/en/latest/autoapi/index.html)
+
+[**Wiki**][wiki]
 
 ## Meta
 
-[![](assets/linkedin.png)](https://linkedin.com/in/stephen-k-3a4644210)
+---
+
+[![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
-[![](assets/pypi.png)](https://pypi.org/project/pynnacle/)
+[![](assets/pypi.png)](https://pypi.org/project/pynnacle)
 [![](assets/www.png)](https://www.justpython.tech)
-[![](assets/email.png)](mailto:stephen.ra.king@gmail.com)
-[![](assets/cv.png)](https://www.justpython.tech/cv)
-
-Stephen R A King : stephen.ra.king@gmail.com
+[![](assets/email.png)](mailto:sking.github@gmail.com)
 
-Distributed under the MIT license. See [license][license-url] for more information.
+Stephen R A King : [sking.github@gmail.com](mailto:sking.github@gmail.com)
 
-[https://github.com/Stephen-RA-King/pynnacle](https://github.com/Stephen-RA-King/pynnacle)
+Distributed under the MIT license. See [![][license-image]][license-url] for more information.
 
-Created with Cookiecutter template: [**cc_template**][cc_template-url] version 1.2.0
+Created with Cookiecutter template: [**pydough**][pydough-url] version 1.2.1
 
 <!-- Markdown link & img dfn's -->
 
 [bandit-image]: https://img.shields.io/badge/security-bandit-yellow.svg
 [bandit-url]: https://github.com/PyCQA/bandit
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-url]: https://github.com/psf/black
-[cc_template-url]: https://github.com/Stephen-RA-King/cc_template
+[pydough-url]: https://github.com/Stephen-RA-King/pydough
 [codeclimate-image]: https://api.codeclimate.com/v1/badges/7fc352185512a1dab75d/maintainability
 [codeclimate-url]: https://codeclimate.com/github/Stephen-RA-King/pynnacle/maintainability
 [codecov-image]: https://codecov.io/gh/Stephen-RA-King/pynnacle/branch/main/graph/badge.svg
 [codecov-url]: https://app.codecov.io/gh/Stephen-RA-King/pynnacle
 [codefactor-image]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle/badge
 [codefactor-url]: https://www.codefactor.io/repository/github/Stephen-RA-King/pynnacle
 [codeql-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/codeql-analysis.yml/badge.svg
@@ -218,30 +236,30 @@
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square
 [conventional-commits-url]: https://conventionalcommits.org
 [deepsource-image]: https://static.deepsource.io/deepsource-badge-light-mini.svg
 [deepsource-url]: https://deepsource.io/gh/Stephen-RA-King/pynnacle/?ref=repository-badge
 [downloads-image]: https://static.pepy.tech/personalized-badge/pynnacle?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
 [downloads-url]: https://pepy.tech/project/pynnacle
 [format-image]: https://img.shields.io/pypi/format/pynnacle
+[isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynnacle.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynnacle/context:python
 [license-image]: https://img.shields.io/pypi/l/pynnacle
 [license-url]: https://github.com/Stephen-RA-King/pynnacle/blob/main/license
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
-[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/gitwatch/main.svg
-[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/gitwatch/main
+[pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynnacle/main.svg
+[pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynnacle/main
 [pypi-url]: https://pypi.org/project/pynnacle/
 [pypi-image]: https://img.shields.io/pypi/v/pynnacle.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynnacle
 [readthedocs-image]: https://readthedocs.org/projects/pynnacle/badge/?version=latest
 [readthedocs-url]: https://pynnacle.readthedocs.io/en/latest/?badge=latest
-[requirements-status-image]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements.svg?branch=main
-[requirements-status-url]: https://requires.io/github/Stephen-RA-King/pynnacle/requirements/?branch=main
 [status-image]: https://img.shields.io/pypi/status/pynnacle.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynnacle/actions/workflows/tests.yml
 [wiki]: https://github.com/Stephen-RA-King/pynnacle/wiki
```

