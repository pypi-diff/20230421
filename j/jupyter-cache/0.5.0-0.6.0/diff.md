# Comparing `tmp/jupyter-cache-0.5.0.tar.gz` & `tmp/jupyter-cache-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-cache-0.5.0.tar", last modified: Tue Jan 25 11:43:08 2022, max compression
+gzip compressed data, was "jupyter-cache-0.6.0.tar", last modified: Fri Apr 21 12:50:18 2023, max compression
```

## Comparing `jupyter-cache-0.5.0.tar` & `jupyter-cache-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11366 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache/cache/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15116 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cache/db.py
--rw-r--r--   0 runner    (1001) docker     (121)    19736 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cache/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     6516 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache/executors/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3977 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/executors/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/executors/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/readers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3988 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/jupyter_cache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/jupyter_cache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 11:43:08.000000 jupyter-cache-0.5.0/jupyter_cache.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-01-25 11:43:08.323172 jupyter-cache-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-01-25 11:42:57.000000 jupyter-cache-0.5.0/setup.py
+-rw-r--r--   0        0        0      529 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2175 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1886 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.gitignore
+-rw-r--r--   0        0        0      821 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      193 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0     5581 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3552 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/README.md
+-rw-r--r--   0        0        0      162 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/codecov.yml
+-rw-r--r--   0        0        0      309 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/__init__.py
+-rw-r--r--   0        0        0    11366 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/base.py
+-rw-r--r--   0        0        0        0 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/__init__.py
+-rw-r--r--   0        0        0    15069 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/db.py
+-rw-r--r--   0        0        0    19736 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cache/main.py
+-rw-r--r--   0        0        0     1294 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cli/__init__.py
+-rw-r--r--   0        0        0     1188 2023-04-21 12:50:13.630891 jupyter-cache-0.6.0/jupyter_cache/cli/arguments.py
+-rw-r--r--   0        0        0      182 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6373 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_cache.py
+-rw-r--r--   0        0        0      392 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_main.py
+-rw-r--r--   0        0        0     6516 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_notebook.py
+-rw-r--r--   0        0        0     2539 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_project.py
+-rw-r--r--   0        0        0     4301 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/options.py
+-rw-r--r--   0        0        0      530 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/cli/utils.py
+-rw-r--r--   0        0        0     1466 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/entry_points.py
+-rw-r--r--   0        0        0       87 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/__init__.py
+-rw-r--r--   0        0        0     3977 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/base.py
+-rw-r--r--   0        0        0     8363 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/basic.py
+-rw-r--r--   0        0        0     3649 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/executors/utils.py
+-rw-r--r--   0        0        0     1286 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/readers.py
+-rw-r--r--   0        0        0     3988 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/jupyter_cache/utils.py
+-rw-r--r--   0        0        0     2773 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1205 2023-04-21 12:50:13.634891 jupyter-cache-0.6.0/tox.ini
+-rw-r--r--   0        0        0     5805 1970-01-01 00:00:00.000000 jupyter-cache-0.6.0/PKG-INFO
```

### Comparing `jupyter-cache-0.5.0/LICENSE` & `jupyter-cache-0.6.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 ExecutableBookProject
+Copyright (c) 2022 ExecutableBookProject
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jupyter-cache-0.5.0/PKG-INFO` & `jupyter-cache-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: jupyter-cache
-Version: 0.5.0
-Summary: A defined interface for working with a cache of jupyter notebooks.
-Home-page: https://github.com/executablebooks/jupyter-cache
-Author: Chris Sewell
-Author-email: chrisj_sewell@hotmail.com
-License: MIT
-Project-URL: Documentation, https://jupyter-cache.readthedocs.io
-Keywords: sphinx extension material design web components
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Sphinx :: Extension
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: cli
-Provides-Extra: code_style
-Provides-Extra: rtd
-Provides-Extra: testing
-License-File: LICENSE
-
 # jupyter-cache
 
 [![Github-CI][github-ci]][github-link]
 [![Coverage Status][codecov-badge]][codecov-link]
 [![Documentation Status][rtd-badge]][rtd-link]
 [![Code style: black][black-badge]][black-link]
 [![PyPI][pypi-badge]][pypi-link]
@@ -115,9 +85,7 @@
 [codecov-link]: https://codecov.io/gh/executablebooks/jupyter-cache
 [rtd-badge]: https://readthedocs.org/projects/jupyter-cache/badge/?version=latest
 [rtd-link]: https://jupyter-cache.readthedocs.io/en/latest/?badge=latest
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [pypi-badge]: https://img.shields.io/pypi/v/jupyter-cache.svg
 [pypi-link]: https://pypi.org/project/jupyter-cache
 [black-link]: https://github.com/ambv/black
-
-
```

### Comparing `jupyter-cache-0.5.0/jupyter_cache/base.py` & `jupyter-cache-0.6.0/jupyter_cache/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cache/db.py` & `jupyter-cache-0.6.0/jupyter_cache/cache/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from sqlalchemy import JSON, Column, DateTime, Integer, String, Text
 from sqlalchemy.engine import Engine, create_engine
 from sqlalchemy.exc import IntegrityError, OperationalError
-from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.orm import Session, sessionmaker, validates
+from sqlalchemy.orm import declarative_base, sessionmaker, validates
 from sqlalchemy.sql.expression import desc
 
 from jupyter_cache import __version__
 from jupyter_cache.utils import shorten_path
 
 OrmBase = declarative_base()
 DB_NAME = "global.db"
```

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cache/main.py` & `jupyter-cache-0.6.0/jupyter_cache/cache/main.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/__init__.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/arguments.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_cache.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
             click.secho("Artifact is not a file", fg="red")
             raise click.Abort()
         text = artifact_path.read_text(encoding="utf8")
     click.echo(text)
 
 
 def cache_file(db, nbpath, validate, overwrite, artifact_paths=()):
-
     from jupyter_cache.base import NbValidityError
 
     click.echo(f"Caching: {nbpath}")
     try:
         db.cache_notebook_file(
             nbpath,
             artifacts=artifact_paths,
```

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_notebook.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_notebook.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/commands/cmd_project.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/commands/cmd_project.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/options.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/options.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/cli/utils.py` & `jupyter-cache-0.6.0/jupyter_cache/cli/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/entry_points.py` & `jupyter-cache-0.6.0/jupyter_cache/entry_points.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/executors/base.py` & `jupyter-cache-0.6.0/jupyter_cache/executors/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/executors/basic.py` & `jupyter-cache-0.6.0/jupyter_cache/executors/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     def log_info(self, msg: str):
         self.logger.info(msg)
 
     def execute(self, project_nb: ProjectNb, data: ProcessData) -> ExecutionResult:
         raise NotImplementedError
 
     def __call__(self, data: ProcessData) -> Tuple[int, str]:
-
         try:
             project_nb = data.cache.get_project_notebook(data.pk)
         except Exception:
             self.logger.error(
                 "Failed Retrieving: %s" % data.uri,
                 exc_info=True,
             )
```

### Comparing `jupyter-cache-0.5.0/jupyter_cache/executors/utils.py` & `jupyter-cache-0.6.0/jupyter_cache/executors/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/readers.py` & `jupyter-cache-0.6.0/jupyter_cache/readers.py`

 * *Files identical despite different names*

### Comparing `jupyter-cache-0.5.0/jupyter_cache/utils.py` & `jupyter-cache-0.6.0/jupyter_cache/utils.py`

 * *Files identical despite different names*

