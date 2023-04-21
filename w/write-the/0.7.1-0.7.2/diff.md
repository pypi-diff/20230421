# Comparing `tmp/write_the-0.7.1.tar.gz` & `tmp/write_the-0.7.2.tar.gz`

## Comparing `write_the-0.7.1.tar` & `write_the-0.7.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.1/mkdocs.yml
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.7.1/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.7.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/README.md
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.7.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/CNAME
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/cli.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/cst.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/docs.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/mkdocs.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/tests.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.1/docs/reference/utils.md
--rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.7.1/images/docs-help.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.1/images/logo-black.svg
--rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.1/images/mkdocs-help.png
--rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.1/images/multiply-docs-tests.png
--rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.1/images/tests-help.png
--rw-r--r--   0        0        0  3549604 2020-02-02 00:00:00.000000 write_the-0.7.1/images/untitled.blend
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.1/images/write-the-icon.svg
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.1/images/write-the.svg
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cli_main.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_docstring_adder.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_docstring_remover.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_function_and_class_collector.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_node_extractor.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_node_remover.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_cst_utils.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/test_utils.py
--rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/data/expected.dat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/data/multiply.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.1/tests/data/multiply_docstring.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/__main__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cli/__init__.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cli/main.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/node_remover.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/docs/__init__.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/docs/chain.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/docs/write.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/mkdocs/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/mkdocs/write.py
--rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/tests/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/tests/chain.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 write_the-0.7.1/write_the/tests/write.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.7.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 write_the-0.7.1/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 write_the-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 write_the-0.7.2/mkdocs.yml
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 write_the-0.7.2/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 write_the-0.7.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    11065 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 write_the-0.7.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/CNAME
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/tests.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.2/docs/reference/utils.md
+-rw-r--r--   0        0        0   123108 2020-02-02 00:00:00.000000 write_the-0.7.2/images/docs-help.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 write_the-0.7.2/images/logo-black.svg
+-rw-r--r--   0        0        0    84667 2020-02-02 00:00:00.000000 write_the-0.7.2/images/mkdocs-help.png
+-rw-r--r--   0        0        0  1092197 2020-02-02 00:00:00.000000 write_the-0.7.2/images/multiply-docs-tests.png
+-rw-r--r--   0        0        0   139626 2020-02-02 00:00:00.000000 write_the-0.7.2/images/tests-help.png
+-rw-r--r--   0        0        0  3549604 2020-02-02 00:00:00.000000 write_the-0.7.2/images/untitled.blend
+-rw-r--r--   0        0        0   464261 2020-02-02 00:00:00.000000 write_the-0.7.2/images/write-the-docs.gif
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 write_the-0.7.2/images/write-the-icon.svg
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 write_the-0.7.2/images/write-the.svg
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cli_main.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_docstring_adder.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_docstring_remover.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_function_and_class_collector.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_node_extractor.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_node_remover.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_cst_utils.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/test_utils.py
+-rw-r--r--   0        0        0    98897 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/data/expected.dat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/data/multiply.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 write_the-0.7.2/tests/data/multiply_docstring.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/mkdocs/write.py
+-rwxr-xr-x   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/tests/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/tests/chain.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 write_the-0.7.2/write_the/tests/write.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 write_the-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.7.2/LICENSE.txt
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 write_the-0.7.2/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 write_the-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 write_the-0.7.2/PKG-INFO
```

### Comparing `write_the-0.7.1/mkdocs.yml` & `write_the-0.7.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/.github/workflows/tests.yml` & `write_the-0.7.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/.pytest_cache/v/cache/lastfailed` & `write_the-0.7.2/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/.pytest_cache/v/cache/nodeids` & `write_the-0.7.2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/docs/index.md` & `write_the-0.7.2/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,36 +10,31 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
------
-
-**Table of Contents**
-
-- [Features](#Features)
-- [Requirements](#Requirements)
-- [Installation](#Installation)
-- [Usage](#Usage)
-- [Roadmap](#Roadmap)
-- [Contributing](#Contributing)
-- [License](#License)
+## Real-world examples
 
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
+- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
+
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
@@ -50,36 +45,30 @@
 ### Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/docs-help.png)
 
-Real-world examples:
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 
 ### Mkdocs:
 ```bash
 write-the mkdocs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/mkdocs-help.png)
 
-Real-world examples:
-- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 
 ### Tests:
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
-Real-world examples:
-- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
 For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline.
```

### Comparing `write_the-0.7.1/images/docs-help.png` & `write_the-0.7.2/images/docs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/logo-black.svg` & `write_the-0.7.2/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/mkdocs-help.png` & `write_the-0.7.2/images/mkdocs-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/multiply-docs-tests.png` & `write_the-0.7.2/images/multiply-docs-tests.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/tests-help.png` & `write_the-0.7.2/images/tests-help.png`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/untitled.blend` & `write_the-0.7.2/images/untitled.blend`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/write-the-icon.svg` & `write_the-0.7.2/images/write-the-icon.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/images/write-the.svg` & `write_the-0.7.2/images/write-the.svg`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cli_main.py` & `write_the-0.7.2/tests/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_docstring_adder.py` & `write_the-0.7.2/tests/test_cst_docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_docstring_remover.py` & `write_the-0.7.2/tests/test_cst_docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_function_and_class_collector.py` & `write_the-0.7.2/tests/test_cst_function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_node_extractor.py` & `write_the-0.7.2/tests/test_cst_node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_node_remover.py` & `write_the-0.7.2/tests/test_cst_node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_cst_utils.py` & `write_the-0.7.2/tests/test_cst_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/test_utils.py` & `write_the-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/tests/data/expected.dat` & `write_the-0.7.2/tests/data/expected.dat`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/utils.py` & `write_the-0.7.2/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cli/main.py` & `write_the-0.7.2/write_the/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     nodes: List[str] = typer.Option(
         None,
         "--node",
         "-n",
         help="Generate docs for specific nodes (functions and classes).",
     ),
     save: bool = typer.Option(
-        False, "--save/--print", "-s", help="Save the tests to the tests directory or print to stdout."
+        False, "--save/--print", "-s", help="Save the docstrings to file or print to stdout."
     ),
     context: bool = typer.Option(
         False, "--context/--no-context", "-c", help="Send context with nodes."
     ),
     pretty: bool = typer.Option(
         False, "--pretty/--plain", "-p", help="Syntax highlight the output."
     ),
```

### Comparing `write_the-0.7.1/write_the/cst/docstring_adder.py` & `write_the-0.7.2/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cst/docstring_remover.py` & `write_the-0.7.2/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cst/function_and_class_collector.py` & `write_the-0.7.2/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cst/node_extractor.py` & `write_the-0.7.2/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cst/node_remover.py` & `write_the-0.7.2/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/cst/utils.py` & `write_the-0.7.2/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/docs/chain.py` & `write_the-0.7.2/write_the/docs/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/docs/write.py` & `write_the-0.7.2/write_the/docs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/mkdocs/write.py` & `write_the-0.7.2/write_the/mkdocs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/tests/chain.py` & `write_the-0.7.2/write_the/tests/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/write_the/tests/write.py` & `write_the-0.7.2/write_the/tests/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/LICENSE.txt` & `write_the-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/README.md` & `write_the-0.7.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,31 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
------
-
-**Table of Contents**
-
-- [Features](#Features)
-- [Requirements](#Requirements)
-- [Installation](#Installation)
-- [Usage](#Usage)
-- [Roadmap](#Roadmap)
-- [Contributing](#Contributing)
-- [License](#License)
+## Real-world examples
 
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
+- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
+
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
@@ -47,36 +42,30 @@
 ### Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/docs-help.png)
 
-Real-world examples:
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 
 ### Mkdocs:
 ```bash
 write-the mkdocs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/mkdocs-help.png)
 
-Real-world examples:
-- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 
 ### Tests:
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
-Real-world examples:
-- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
 For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline.
```

### Comparing `write_the-0.7.1/pyproject.toml` & `write_the-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `write_the-0.7.1/PKG-INFO` & `write_the-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.7.1
+Version: 0.7.2
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -35,36 +35,31 @@
 [![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 [![write-the - test](https://badgen.net/badge/write-the/tests/green?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://github.com/Wytamma/write-the/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/Wytamma/write-the/branch/master/graph/badge.svg?token=yEDn56L76k)](https://app.codecov.io/gh/Wytamma/write-the/tree/master)
 
 
 Write-the is an AI-powered documentation and test generation tool that leverages GPTs to automatically write tests, generate documentation, and refactor code. It is designed to streamline the development process, improve code quality, and increase productivity.
 
-![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/multiply-docs-tests.png)
+![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-docs.gif)
 
------
-
-**Table of Contents**
-
-- [Features](#Features)
-- [Requirements](#Requirements)
-- [Installation](#Installation)
-- [Usage](#Usage)
-- [Roadmap](#Roadmap)
-- [Contributing](#Contributing)
-- [License](#License)
+## Real-world examples
 
+- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
+- [`write-the docs` and `write-the mkdocs` to build documenation for `hyperspec` 🤖](https://github.com/smutch/hyperspec/pull/1)
+- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 ## Installation
 ```console
 pip install write-the
 ```
 ## Features
 
 Write-the offers the following AI-driven features:
+
 - Write-the Docs: Automatically generate documentation for your codebase, including class and function descriptions, parameter explanations, and examples.
 - Write-the Tests: Create test cases for your code, ensuring thorough test coverage and better code quality.
 - Write-the Refactor: Receive refactoring suggestions, reduce code complexity, optimize performance, and fix bugs (TBD).
 
 ## Requirements
 - Python 3.9 or higher  
 - OpenAI API key
@@ -75,36 +70,30 @@
 ### Docs:
 ```bash
 write-the docs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/docs-help.png)
 
-Real-world examples:
-- [`write-the docs` to write the docs for the `write-the docs` command 🤖](https://github.com/Wytamma/write-the/blob/master/write_the/docs/write.py#L14)
 
 ### Mkdocs:
 ```bash
 write-the mkdocs [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/mkdocs-help.png)
 
-Real-world examples:
-- [`write-the docs` and `write-the mkdocs` to build documenation for `autoresearcher` 🤖](https://github.com/eimenhmdt/autoresearcher/pull/17)
 
 ### Tests:
 ```bash
 write-the tests [OPTIONS] [PATH_TO_SOURCE_CODE]
 ```
 
 ![](https://raw.githubusercontent.com/Wytamma/write-the/master/images/tests-help.png)
 
-Real-world examples:
-- [`write-the tests` to write tests for `write-the docs` 🤖](https://github.com/Wytamma/write-the/commit/6b6c8a08d7991e07e4972281c471f7842c04dda0)
 
 For detailed information on available options and parameters, refer to the official (`write-the` generated) [documentation](https://write-the.wytamma.com/).
 
 ## Roadmap
 
 For a detailed project roadmap, including planned features, improvements, and milestones, please see our Project Timeline.
```

