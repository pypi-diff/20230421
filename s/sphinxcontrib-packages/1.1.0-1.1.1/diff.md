# Comparing `tmp/sphinxcontrib-packages-1.1.0.tar.gz` & `tmp/sphinxcontrib-packages-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-packages-1.1.0.tar", last modified: Tue Nov 29 12:36:03 2022, max compression
+gzip compressed data, was "sphinxcontrib-packages-1.1.1.tar", last modified: Fri Apr 21 14:52:33 2023, max compression
```

## Comparing `sphinxcontrib-packages-1.1.0.tar` & `sphinxcontrib-packages-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,20 @@
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.952001 sphinxcontrib-packages-1.1.0/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.920001 sphinxcontrib-packages-1.1.0/.github/
--rw-r--r--   0 louis     (1000) louis     (1000)      160 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 louis     (1000) louis     (1000)      103 2022-01-31 16:27:08.000000 sphinxcontrib-packages-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 louis     (1000) louis     (1000)      196 2022-11-29 07:14:05.000000 sphinxcontrib-packages-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 louis     (1000) louis     (1000)      101 2022-11-29 08:18:41.000000 sphinxcontrib-packages-1.1.0/.pylintrc
--rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/AUTHORS
--rw-r--r--   0 louis     (1000) louis     (1000)     1312 2022-11-29 11:13:12.000000 sphinxcontrib-packages-1.1.0/CHANGELOG.md
--rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/LICENSE
--rw-r--r--   0 louis     (1000) louis     (1000)     3020 2022-11-29 12:36:03.952001 sphinxcontrib-packages-1.1.0/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)     1576 2021-05-21 17:49:20.000000 sphinxcontrib-packages-1.1.0/README.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      143 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/TODO.md
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.936001 sphinxcontrib-packages-1.1.0/doc/
--rw-r--r--   0 louis     (1000) louis     (1000)        8 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/.gitignore
--rw-r--r--   0 louis     (1000) louis     (1000)     7417 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/Makefile
--rw-r--r--   0 louis     (1000) louis     (1000)      233 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/bin.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      335 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/c.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     9343 2022-11-29 11:11:39.000000 sphinxcontrib-packages-1.1.0/doc/conf.py
--rw-r--r--   0 louis     (1000) louis     (1000)      227 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/deb.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     1622 2021-05-22 16:34:26.000000 sphinxcontrib-packages-1.1.0/doc/index.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      210 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/latex.rst
--rw-r--r--   0 louis     (1000) louis     (1000)     7248 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/make.bat
--rw-r--r--   0 louis     (1000) louis     (1000)      170 2022-01-31 21:32:40.000000 sphinxcontrib-packages-1.1.0/doc/platform.rst
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.936001 sphinxcontrib-packages-1.1.0/doc/python/
--rw-r--r--   0 louis     (1000) louis     (1000)      258 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/python/python2.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      258 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/python/python3.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      577 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/python.rst
--rw-r--r--   0 louis     (1000) louis     (1000)      193 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.0/doc/pyversions.rst
--rw-r--r--   0 louis     (1000) louis     (1000)       41 2022-03-06 12:51:38.000000 sphinxcontrib-packages-1.1.0/doc/requirements.txt
--rw-r--r--   0 louis     (1000) louis     (1000)      257 2022-11-29 09:51:40.000000 sphinxcontrib-packages-1.1.0/pyproject.toml
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2022-01-31 21:18:40.000000 sphinxcontrib-packages-1.1.0/requirements.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       64 2022-11-29 12:36:03.952001 sphinxcontrib-packages-1.1.0/setup.cfg
--rw-r--r--   0 louis     (1000) louis     (1000)     2742 2022-11-29 12:33:40.000000 sphinxcontrib-packages-1.1.0/setup.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.888001 sphinxcontrib-packages-1.1.0/sphinxcontrib/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.936001 sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/
--rw-r--r--   0 louis     (1000) louis     (1000)    14193 2022-11-29 11:11:39.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/__init__.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.892001 sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/data/
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.940001 sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/data/bin/
--rw-r--r--   0 louis     (1000) louis     (1000)     2412 2022-11-29 11:11:39.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/data/bin/list_modules.py
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.948001 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/
--rw-r--r--   0 louis     (1000) louis     (1000)     3020 2022-11-29 12:36:03.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/PKG-INFO
--rw-r--r--   0 louis     (1000) louis     (1000)      820 2022-11-29 12:36:03.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-11-29 12:36:03.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2017-12-30 15:11:23.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/not-zip-safe
--rw-r--r--   0 louis     (1000) louis     (1000)       14 2022-11-29 12:36:03.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/requires.txt
--rw-r--r--   0 louis     (1000) louis     (1000)        1 2022-11-29 12:36:03.000000 sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/top_level.txt
--rw-r--r--   0 louis     (1000) louis     (1000)       68 2020-06-21 10:56:25.000000 sphinxcontrib-packages-1.1.0/stdeb.cfg
-drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2022-11-29 12:36:03.948001 sphinxcontrib-packages-1.1.0/test/
--rw-r--r--   0 louis     (1000) louis     (1000)     1226 2022-01-31 20:51:08.000000 sphinxcontrib-packages-1.1.0/test/__init__.py
--rw-r--r--   0 louis     (1000) louis     (1000)     1541 2022-01-31 20:51:08.000000 sphinxcontrib-packages-1.1.0/test/test_doctests.py
--rw-r--r--   0 louis     (1000) louis     (1000)      841 2022-11-29 09:51:40.000000 sphinxcontrib-packages-1.1.0/tox.ini
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/
+-rw-r--r--   0 louis     (1000) louis     (1000)       17 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.1/AUTHORS
+-rw-r--r--   0 louis     (1000) louis     (1000)    34520 2020-06-21 10:56:24.000000 sphinxcontrib-packages-1.1.1/LICENSE
+-rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)     1576 2021-05-21 17:49:20.000000 sphinxcontrib-packages-1.1.1/README.rst
+-rw-r--r--   0 louis     (1000) louis     (1000)      257 2023-04-21 13:09:34.000000 sphinxcontrib-packages-1.1.1/pyproject.toml
+-rw-r--r--   0 louis     (1000) louis     (1000)     1538 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/setup.cfg
+-rw-r--r--   0 louis     (1000) louis     (1000)       93 2023-04-21 09:24:16.000000 sphinxcontrib-packages-1.1.1/setup.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.093986 sphinxcontrib-packages-1.1.1/sphinxcontrib/
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/
+-rw-r--r--   0 louis     (1000) louis     (1000)    14193 2023-04-21 14:49:13.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/__init__.py
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/
+-rw-r--r--   0 louis     (1000) louis     (1000)     3091 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (1000) louis     (1000)      387 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/requires.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)       14 2023-04-21 14:52:33.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/top_level.txt
+-rw-r--r--   0 louis     (1000) louis     (1000)        1 2023-04-21 14:52:32.000000 sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/zip-safe
+drwxr-xr-x   0 louis     (1000) louis     (1000)        0 2023-04-21 14:52:33.097986 sphinxcontrib-packages-1.1.1/test/
+-rw-r--r--   0 louis     (1000) louis     (1000)     1541 2022-01-31 20:51:08.000000 sphinxcontrib-packages-1.1.1/test/test_doctests.py
```

### Comparing `sphinxcontrib-packages-1.1.0/LICENSE` & `sphinxcontrib-packages-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-packages-1.1.0/PKG-INFO` & `sphinxcontrib-packages-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-packages
-Version: 1.1.0
+Version: 1.1.1
 Summary: This packages contains the Packages sphinx extension, which provides directives to display packages installed on the host machine
-Home-page: https://git.framasoft.org/spalax/sphinxcontrib-packages
+Home-page: https://framagit.org/spalax/sphinxcontrib-packages
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://packages.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/sphinxcontrib-packages
 Project-URL: Tracker, https://framagit.org/spalax/sphinxcontrib-packages/issues
-Keywords: sphinx packages system
+Keywords: sphinx package system
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 `sphinxcontrib-packages` 📦 Display a list of tools available on the host machine
 =================================================================================
```

### Comparing `sphinxcontrib-packages-1.1.0/README.rst` & `sphinxcontrib-packages-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-packages-1.1.0/sphinxcontrib/packages/__init__.py` & `sphinxcontrib-packages-1.1.1/sphinxcontrib/packages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright Louis Paternault 2015-2022
+# Copyright Louis Paternault 2015-2023
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -32,15 +32,15 @@
 import pkg_resources
 from docutils import nodes
 from docutils.parsers.rst import Directive, directives
 from docutils.parsers.rst.directives import flag, unchanged
 from docutils.statemachine import StringList
 from sphinx.util.nodes import nested_parse_with_titles
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 def node_or_str(text):
     """Return argument, converted to a node if necessary."""
     if isinstance(text, str):
         return nodes.paragraph(text=text)
     return text
```

### Comparing `sphinxcontrib-packages-1.1.0/sphinxcontrib_packages.egg-info/PKG-INFO` & `sphinxcontrib-packages-1.1.1/sphinxcontrib_packages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-packages
-Version: 1.1.0
+Version: 1.1.1
 Summary: This packages contains the Packages sphinx extension, which provides directives to display packages installed on the host machine
-Home-page: https://git.framasoft.org/spalax/sphinxcontrib-packages
+Home-page: https://framagit.org/spalax/sphinxcontrib-packages
 Author: Louis Paternault
 Author-email: spalax@gresille.org
 License: AGPLv3 or any later version
 Project-URL: Documentation, http://packages.readthedocs.io
 Project-URL: Source, https://framagit.org/spalax/sphinxcontrib-packages
 Project-URL: Tracker, https://framagit.org/spalax/sphinxcontrib-packages/issues
-Keywords: sphinx packages system
+Keywords: sphinx package system
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 `sphinxcontrib-packages` 📦 Display a list of tools available on the host machine
 =================================================================================
```

### Comparing `sphinxcontrib-packages-1.1.0/test/test_doctests.py` & `sphinxcontrib-packages-1.1.1/test/test_doctests.py`

 * *Files identical despite different names*

