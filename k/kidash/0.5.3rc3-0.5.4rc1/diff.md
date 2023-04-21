# Comparing `tmp/kidash-0.5.3rc3.tar.gz` & `tmp/kidash-0.5.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidash-0.5.3rc3.tar", max compression
+gzip compressed data, was "kidash-0.5.4rc1.tar", max compression
```

## Comparing `kidash-0.5.3rc3.tar` & `kidash-0.5.4rc1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      300 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/LICENSE
--rw-r--r--   0        0        0     1054 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/NEWS
--rw-r--r--   0        0        0     2525 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/README.md
--rw-r--r--   0        0        0      894 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/kidash/__init__.py
--rw-r--r--   0        0        0       91 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/kidash/_version.py
--rwxr-xr-x   0        0        0     4355 2023-02-01 08:41:12.779456 kidash-0.5.3rc3/kidash/bin/kidash.py
--rwxr-xr-x   0        0        0    59367 2023-02-01 08:41:12.783455 kidash-0.5.3rc3/kidash/kidash.py
--rw-r--r--   0        0        0     1307 2023-02-01 08:41:12.783455 kidash-0.5.3rc3/pyproject.toml
--rw-r--r--   0        0        0    54328 2023-02-01 08:41:12.783455 kidash-0.5.3rc3/tests/data/overview-with-index-patterns.json
--rwxr-xr-x   0        0        0     1166 2023-02-01 08:41:12.783455 kidash-0.5.3rc3/tests/run_tests.py
--rw-r--r--   0        0        0     2131 2023-02-01 08:41:12.783455 kidash-0.5.3rc3/tests/test_export.py
--rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 kidash-0.5.3rc3/setup.py
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 kidash-0.5.3rc3/PKG-INFO
+-rw-r--r--   0        0        0      300 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/LICENSE
+-rw-r--r--   0        0        0     1132 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/NEWS
+-rw-r--r--   0        0        0     2525 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/README.md
+-rw-r--r--   0        0        0      894 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/_version.py
+-rwxr-xr-x   0        0        0     4355 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/bin/kidash.py
+-rwxr-xr-x   0        0        0    59367 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/kidash/kidash.py
+-rw-r--r--   0        0        0     1307 2023-04-20 14:54:08.673520 kidash-0.5.4rc1/pyproject.toml
+-rw-r--r--   0        0        0    54328 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/data/overview-with-index-patterns.json
+-rwxr-xr-x   0        0        0     1166 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     2131 2023-04-20 14:54:08.677521 kidash-0.5.4rc1/tests/test_export.py
+-rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 kidash-0.5.4rc1/PKG-INFO
```

### Comparing `kidash-0.5.3rc3/LICENSE` & `kidash-0.5.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/NEWS` & `kidash-0.5.4rc1/NEWS`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## kidash 0.5.3 - (2023-02-01)
+  
+  * Update Poetry's package dependencies
+
   ## kidash 0.5.2 - (2022-10-31)
   
   * Update Poetry's package dependencies
 
 ## kidash 0.5.1 - (2022-09-26)
 
 **Others:**
```

### Comparing `kidash-0.5.3rc3/README.md` & `kidash-0.5.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/kidash/__init__.py` & `kidash-0.5.4rc1/kidash/__init__.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/kidash/bin/kidash.py` & `kidash-0.5.4rc1/kidash/bin/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/kidash/kidash.py` & `kidash-0.5.4rc1/kidash/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/pyproject.toml` & `kidash-0.5.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kidash"
-version = "0.5.3-rc.3"
+version = "0.5.4-rc.1"
 description = "GrimoireLab script to manage Kibana dashboards from the command line"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `kidash-0.5.3rc3/tests/data/overview-with-index-patterns.json` & `kidash-0.5.4rc1/tests/data/overview-with-index-patterns.json`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/tests/run_tests.py` & `kidash-0.5.4rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/tests/test_export.py` & `kidash-0.5.4rc1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.3rc3/setup.py` & `kidash-0.5.4rc1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: kidash
+Version: 0.5.4rc1
+Summary: GrimoireLab script to manage Kibana dashboards from the command line
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.7.0,<3.0.0)
+Requires-Dist: urllib3 (>=1.26,<2.0)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-kidash/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-kidash
+Description-Content-Type: text/markdown
+
+# Kidash [![Build Status](https://github.com/chaoss/grimoirelab-kidash/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-kidash/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-kidash.svg)](https://coveralls.io/r/chaoss/grimoirelab-kidash?branch=master) [![PyPI version](https://badge.fury.io/py/kidash.svg)](https://badge.fury.io/py/kidash)
+
+Kidash is a tool for managing Kibana-related dashboards from the command line. The standard GrimoireLab dashboards
+are available in the [Sigils](https://github.com/chaoss/grimoirelab-sigils) repository.
+
+## Requirements
+
+ * Python >= 3.7
+
+You will also need some other libraries for running the tool, you can find the
+whole list of dependencies in [pyproject.toml](pyproject.toml) file.
+
+## Installation
+
+There are several ways to install Kidash on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI:
+
+Kidash can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install kidash
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-kidash
+$ cd grimoirelab-kidash
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install kidash in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install kidash and the dependencies:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
+## Usage
+
+- Get a list of all options with:
+```
+$ kidash --help
+```
+
+- Import a dashboard:
+```buildoutcfg
+kidash -g -e <elasticsearch-url>:<port> --import <local-file-path>
+example: kidash -g -e https://admin:admin@localhost:9200 --import ./overview.json
+```
+
+- Export a dashboard:
+```buildoutcfg
+kidash -g -e <elasticsearch-url> --dashboard <dashboard-id>* --export <local-file-path> --split-index-pattern
+example: kidash -g -e https://admin:admin@localhost:9200 --dashboard overview --export overview.json
+```
 
-packages = \
-['kidash', 'kidash.bin', 'tests']
+## License
 
-package_data = \
-{'': ['*'], 'tests': ['data/*']}
+Licensed under GNU General Public License (GPL), version 3 or later.
 
-install_requires = \
-['python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.7.0,<3.0.0',
- 'urllib3>=1.26,<2.0']
-
-entry_points = \
-{'console_scripts': ['kidash = kidash.bin.kidash:main']}
-
-setup_kwargs = {
-    'name': 'kidash',
-    'version': '0.5.3rc3',
-    'description': 'GrimoireLab script to manage Kibana dashboards from the command line',
-    'long_description': '# Kidash [![Build Status](https://github.com/chaoss/grimoirelab-kidash/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-kidash/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-kidash.svg)](https://coveralls.io/r/chaoss/grimoirelab-kidash?branch=master) [![PyPI version](https://badge.fury.io/py/kidash.svg)](https://badge.fury.io/py/kidash)\n\nKidash is a tool for managing Kibana-related dashboards from the command line. The standard GrimoireLab dashboards\nare available in the [Sigils](https://github.com/chaoss/grimoirelab-sigils) repository.\n\n## Requirements\n\n * Python >= 3.7\n\nYou will also need some other libraries for running the tool, you can find the\nwhole list of dependencies in [pyproject.toml](pyproject.toml) file.\n\n## Installation\n\nThere are several ways to install Kidash on your system: packages or source \ncode using Poetry or pip.\n\n### PyPI:\n\nKidash can be installed using pip, a tool for installing Python packages. \nTo do it, run the next command:\n```\n$ pip install kidash\n```\n\n### Source code\n\nTo install from the source code you will need to clone the repository first:\n```\n$ git clone https://github.com/chaoss/grimoirelab-kidash\n$ cd grimoirelab-kidash\n```\n\nThen use pip or Poetry to install the package along with its dependencies.\n\n#### Pip\nTo install the package from local directory run the following command:\n```\n$ pip install .\n```\nIn case you are a developer, you should install kidash in editable mode:\n```\n$ pip install -e .\n```\n\n#### Poetry\nWe use [poetry](https://python-poetry.org/) for dependency management and \npackaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).\nOnce you have installed it, you can install kidash and the dependencies:\n```\n$ poetry install\n```\nTo spaw a new shell within the virtual environment use:\n```\n$ poetry shell\n```\n\n## Usage\n\n- Get a list of all options with:\n```\n$ kidash --help\n```\n\n- Import a dashboard:\n```buildoutcfg\nkidash -g -e <elasticsearch-url>:<port> --import <local-file-path>\nexample: kidash -g -e https://admin:admin@localhost:9200 --import ./overview.json\n```\n\n- Export a dashboard:\n```buildoutcfg\nkidash -g -e <elasticsearch-url> --dashboard <dashboard-id>* --export <local-file-path> --split-index-pattern\nexample: kidash -g -e https://admin:admin@localhost:9200 --dashboard overview --export overview.json\n```\n\n## License\n\nLicensed under GNU General Public License (GPL), version 3 or later.\n',
-    'author': 'GrimoireLab Developers',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://chaoss.github.io/grimoirelab/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

