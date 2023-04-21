# Comparing `tmp/kaiju_db-2.0.10-py3-none-any.whl.zip` & `tmp/kaiju_db-2.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 21698 bytes, number of entries: 16
--rw-r--r--  2.0 unx      205 b- defN 23-Feb-27 22:16 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Feb-27 22:16 kaiju_db/functions.py
--rw-r--r--  2.0 unx      204 b- defN 23-Feb-27 22:16 kaiju_db/ltree.py
--rw-r--r--  2.0 unx     4522 b- defN 23-Feb-27 22:16 kaiju_db/migrations.py
--rw-r--r--  2.0 unx      148 b- defN 23-Feb-27 22:16 kaiju_db/services.py
--rw-r--r--  2.0 unx    39624 b- defN 23-Feb-27 22:16 kaiju_db/sql_service.py
--rw-r--r--  2.0 unx     9697 b- defN 23-Feb-27 22:16 kaiju_db/transport.py
--rw-r--r--  2.0 unx      206 b- defN 23-Feb-27 22:16 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-27 22:16 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3568 b- defN 23-Feb-27 22:16 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx    13643 b- defN 23-Feb-27 22:16 kaiju_db/tests/test_services.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Feb-27 22:17 kaiju_db-2.0.10.dist-info/LICENSE
--rw-r--r--  2.0 unx     2941 b- defN 23-Feb-27 22:17 kaiju_db-2.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-27 22:17 kaiju_db-2.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Feb-27 22:17 kaiju_db-2.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1260 b- defN 23-Feb-27 22:17 kaiju_db-2.0.10.dist-info/RECORD
-16 files, 80394 bytes uncompressed, 19634 bytes compressed:  75.6%
+Zip file size: 21714 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      205 b- defN 23-Apr-21 14:50 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3665 b- defN 23-Apr-21 14:50 kaiju_db/functions.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Apr-21 14:50 kaiju_db/ltree.py
+-rw-r--r--  2.0 unx     4522 b- defN 23-Apr-21 14:50 kaiju_db/migrations.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Apr-21 14:50 kaiju_db/services.py
+-rw-r--r--  2.0 unx    39624 b- defN 23-Apr-21 14:50 kaiju_db/sql_service.py
+-rw-r--r--  2.0 unx     9697 b- defN 23-Apr-21 14:50 kaiju_db/transport.py
+-rw-r--r--  2.0 unx      206 b- defN 23-Apr-21 14:50 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 14:50 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3568 b- defN 23-Apr-21 14:50 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx    13643 b- defN 23-Apr-21 14:50 kaiju_db/tests/test_services.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Apr-21 14:51 kaiju_db-2.0.11.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2994 b- defN 23-Apr-21 14:51 kaiju_db-2.0.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 14:51 kaiju_db-2.0.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-21 14:51 kaiju_db-2.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1260 b- defN 23-Apr-21 14:51 kaiju_db-2.0.11.dist-info/RECORD
+16 files, 80447 bytes uncompressed, 19650 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_services.py
 Comment: 
 
-Filename: kaiju_db-2.0.10.dist-info/LICENSE
+Filename: kaiju_db-2.0.11.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.0.10.dist-info/METADATA
+Filename: kaiju_db-2.0.11.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.0.10.dist-info/WHEEL
+Filename: kaiju_db-2.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.0.10.dist-info/top_level.txt
+Filename: kaiju_db-2.0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.0.10.dist-info/RECORD
+Filename: kaiju_db-2.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,9 +1,9 @@
 from .types import *
 from .ltree import *
 from .functions import *
 from .services import *
 
-__version__ = '2.0.10'
+__version__ = '2.0.11'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## Comparing `kaiju_db-2.0.10.dist-info/LICENSE` & `kaiju_db-2.0.11.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.0.10.dist-info/METADATA` & `kaiju_db-2.0.11.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.0.10
+Version: 2.0.11
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,31 +15,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: asyncpg (>=0.27)
-Requires-Dist: greenlet (>=2.0)
-Requires-Dist: sqlalchemy[asyncio] (>=2.0)
-Requires-Dist: sqlalchemy-utils (>=0.40)
-Requires-Dist: kaiju-tools (<3.0,>=2.0.19)
+Requires-Dist: greenlet (>=2.0.2)
+Requires-Dist: sqlalchemy[asyncio] (>=2.0.9)
+Requires-Dist: sqlalchemy-utils (>=0.41)
+Requires-Dist: kaiju-tools (<3,>=2.0.49)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
 Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
 Requires-Dist: pydocstyle (>=6.3) ; extra == 'dev'
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
+Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.2) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
 Requires-Dist: docker (>=6.0) ; extra == 'test'
```

