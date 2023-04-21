# Comparing `tmp/luigi-tools-0.3.3.tar.gz` & `tmp/luigi-tools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luigi-tools-0.3.3.tar", last modified: Wed Mar  8 16:01:39 2023, max compression
+gzip compressed data, was "luigi-tools-0.3.4.tar", last modified: Fri Apr 21 13:15:06 2023, max compression
```

## Comparing `luigi-tools-0.3.3.tar` & `luigi-tools-0.3.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.384675 luigi-tools-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.auto-changelog
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.auto-changelog-template.hbs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.codespellignorelines
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.376675 luigi-tools-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.376675 luigi-tools-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.github/workflows/commitlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-03-08 16:01:39.384675 luigi-tools-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.376675 luigi-tools-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.376675 luigi-tools-0.3.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.380675 luigi-tools-0.3.3/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/_ext/luigi_move.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.380675 luigi-tools-0.3.3/luigi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/luigi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/luigi_tools/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/luigi_tools/target.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/luigi_tools/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/luigi_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.380675 luigi-tools-0.3.3/luigi_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-03-08 16:01:39.000000 luigi-tools-0.3.3/luigi_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-08 16:01:39.000000 luigi-tools-0.3.3/luigi_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:01:39.000000 luigi-tools-0.3.3/luigi_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-08 16:01:39.000000 luigi-tools-0.3.3/luigi_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-08 16:01:39.000000 luigi-tools-0.3.3/luigi_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 16:01:39.384675 luigi-tools-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:01:39.384675 luigi-tools-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39874 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tests/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-08 16:01:26.000000 luigi-tools-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.767520 luigi-tools-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.auto-changelog
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.auto-changelog-template.hbs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.codespellignorelines
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.github/workflows/commitlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-21 13:15:06.767520 luigi-tools-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/_ext/luigi_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/luigi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/luigi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/luigi_tools/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/luigi_tools/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/luigi_tools/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16489 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/luigi_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.763520 luigi-tools-0.3.4/luigi_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-21 13:15:06.000000 luigi-tools-0.3.4/luigi_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-21 13:15:06.000000 luigi-tools-0.3.4/luigi_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:15:06.000000 luigi-tools-0.3.4/luigi_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-21 13:15:06.000000 luigi-tools-0.3.4/luigi_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 13:15:06.000000 luigi-tools-0.3.4/luigi_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:15:06.767520 luigi-tools-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:15:06.767520 luigi-tools-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39874 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37825 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tests/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-21 13:14:57.000000 luigi-tools-0.3.4/tox.ini
```

### Comparing `luigi-tools-0.3.3/.auto-changelog` & `luigi-tools-0.3.4/.auto-changelog`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.auto-changelog-template.hbs` & `luigi-tools-0.3.4/.auto-changelog-template.hbs`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.copier-answers.yml` & `luigi-tools-0.3.4/.copier-answers.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Changes here will be overwritten by Copier
 
-_commit: 0.1.38
+_commit: 0.1.42
 _src_path: git@bbpgitlab.epfl.ch:neuromath/python-template.git
 author_email: ''
 author_name: Blue Brain Project, EPFL
 copyright_license: Apache License 2.0
 copyright_year: '2022'
 distribution_name: luigi-tools
 download_url: git@github.com:BlueBrain/luigi-tools.git
```

### Comparing `luigi-tools-0.3.3/.github/dependabot.yml` & `luigi-tools-0.3.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.github/workflows/codeql.yml` & `luigi-tools-0.3.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.github/workflows/commitlint.yml` & `luigi-tools-0.3.4/.github/workflows/commitlint.yml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.github/workflows/publish-sdist.yml` & `luigi-tools-0.3.4/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.github/workflows/run-tox.yml` & `luigi-tools-0.3.4/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/.pre-commit-config.yaml` & `luigi-tools-0.3.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,30 +9,30 @@
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/alessandrojcm/commitlint-pre-commit-hook
-    rev: v9.4.0
+    rev: v9.5.0
     hooks:
         - id: commitlint
           stages:
             - commit-msg
           additional_dependencies: ['conventional-changelog-conventionalcommits']
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-x", ".codespellignorelines"]
   - repo: https://github.com/PyCQA/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
```

### Comparing `luigi-tools-0.3.3/.pylintrc` & `luigi-tools-0.3.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/CHANGELOG.md` & `luigi-tools-0.3.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [0.3.4](https://github.com/BlueBrain/luigi-tools/compare/0.3.3..0.3.4)
+
+> 21 April 2023
+
+### Chores And Housekeeping
+
+- Bump copier template (Adrien Berchet - [#87](https://github.com/BlueBrain/luigi-tools/pull/87))
+
+### Refactoring and Updates
+
+- Filter warnings when registering missing files in register_templates() (Adrien Berchet - [#86](https://github.com/BlueBrain/luigi-tools/pull/86))
+
 ## [0.3.3](https://github.com/BlueBrain/luigi-tools/compare/0.3.2..0.3.3)
 
 > 8 March 2023
 
 ### New Features
 
 - Add function to convert luigi config file into a dict (Adrien Berchet - [#83](https://github.com/BlueBrain/luigi-tools/pull/83))
```

### Comparing `luigi-tools-0.3.3/CONTRIBUTING.md` & `luigi-tools-0.3.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/LICENSE.txt` & `luigi-tools-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/PKG-INFO` & `luigi-tools-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools to work with luigi.
 Home-page: https://luigi-tools.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/luigi-tools/issues
 Project-URL: Source, https://github.com/BlueBrain/luigi-tools
 Classifier: Development Status :: 4 - Beta
```

### Comparing `luigi-tools-0.3.3/README.md` & `luigi-tools-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/commitlint.config.js` & `luigi-tools-0.3.4/commitlint.config.js`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/docs/Makefile` & `luigi-tools-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/docs/source/_ext/luigi_move.py` & `luigi-tools-0.3.4/docs/source/_ext/luigi_move.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/docs/source/conf.py` & `luigi-tools-0.3.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/luigi_tools/__init__.py` & `luigi-tools-0.3.4/luigi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/luigi_tools/parameter.py` & `luigi-tools-0.3.4/luigi_tools/parameter.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/luigi_tools/target.py` & `luigi-tools-0.3.4/luigi_tools/target.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/luigi_tools/task.py` & `luigi-tools-0.3.4/luigi_tools/task.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/luigi_tools/util.py` & `luigi-tools-0.3.4/luigi_tools/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """This module provides some functions to work with luigi tasks."""
 import configparser
 import logging
 import os
 import re
+import warnings
 from configparser import ConfigParser
 from pathlib import Path
 
 import luigi
 from luigi.parameter import _no_value as PARAM_NO_VALUE
 
 L = logging.getLogger(__name__)
@@ -376,18 +377,20 @@
 
     template = (template_path / template_name).with_suffix(".cfg")
     if not template.exists():
         raise ValueError(f"The template '{template}' could not be found.")
 
     luigi.configuration.add_config_path(template)
     if hierarchy_end:
-        luigi.configuration.add_config_path("luigi.cfg")
-        env_cfg = os.environ.get("LUIGI_CONFIG_PATH")
-        if env_cfg is not None:
-            luigi.configuration.add_config_path(env_cfg)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="Config file does not exist.*")
+            luigi.configuration.add_config_path("luigi.cfg")
+            env_cfg = os.environ.get("LUIGI_CONFIG_PATH")
+            if env_cfg is not None:
+                luigi.configuration.add_config_path(env_cfg)
 
 
 class set_luigi_config:
     """Context manager to set current luigi config.
 
     Args:
         params (dict): The parameters to load into the luigi configuration.
```

### Comparing `luigi-tools-0.3.3/luigi_tools.egg-info/PKG-INFO` & `luigi-tools-0.3.4/luigi_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luigi-tools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools to work with luigi.
 Home-page: https://luigi-tools.readthedocs.io
 Author: Blue Brain Project, EPFL
 License: Apache License 2.0
 Project-URL: Tracker, https://github.com/BlueBrain/luigi-tools/issues
 Project-URL: Source, https://github.com/BlueBrain/luigi-tools
 Classifier: Development Status :: 4 - Beta
```

### Comparing `luigi-tools-0.3.3/luigi_tools.egg-info/SOURCES.txt` & `luigi-tools-0.3.4/luigi_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/package.json` & `luigi-tools-0.3.4/package.json`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/pyproject.toml` & `luigi-tools-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/setup.py` & `luigi-tools-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/__init__.py` & `luigi-tools-0.3.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/conftest.py` & `luigi-tools-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/test_parameter.py` & `luigi-tools-0.3.4/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/test_target.py` & `luigi-tools-0.3.4/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/test_task.py` & `luigi-tools-0.3.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/test_util.py` & `luigi-tools-0.3.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `luigi-tools-0.3.3/tests/tools.py` & `luigi-tools-0.3.4/tests/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 def create_empty_file(filename):
     """Create an empty file."""
     with open(filename, "w", encoding="utf-8"):
         pass
 
 
 def check_empty_file(filename):
-    """Checck that a file is empty."""
+    """Check that a file is empty."""
     with open(filename, encoding="utf-8") as f:
         return f.read() == ""
 
 
 def create_not_empty_file(filename):
     """Create a not empty file."""
     with open(filename, "w", encoding="utf-8") as f:
         f.write("NOT EMPTY")
 
 
 def check_not_empty_file(filename):
-    """Checck that a file is not empty."""
+    """Check that a file is not empty."""
     with open(filename, encoding="utf-8") as f:
         return f.read() == "NOT EMPTY"
```

### Comparing `luigi-tools-0.3.3/tox.ini` & `luigi-tools-0.3.4/tox.ini`

 * *Files identical despite different names*

