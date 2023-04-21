# Comparing `tmp/kolo-2.6.2.tar.gz` & `tmp/kolo-2.7.0.tar.gz`

## Comparing `kolo-2.6.2.tar` & `kolo-2.7.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.6.2/rust/Cargo.toml
--rw-rw-r--   0     1000     1001       54 2023-04-18 16:24:50.000000 kolo-2.6.2/rust/build.rs
--rw-rw-r--   0     1000     1001    35236 2023-04-18 16:24:50.000000 kolo-2.6.2/rust/src/lib.rs
--rw-rw-r--   0     1000     1001     2106 2023-04-18 16:24:50.000000 kolo-2.6.2/pyproject.toml
--rw-rw-r--   0     1000     1001    11199 2023-04-18 16:25:15.000000 kolo-2.6.2/rust/Cargo.lock
--rw-rw-r--   0     1000     1001     3681 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/serialize.py
--rw-rw-r--   0     1000     1001     3400 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/requests.py
--rw-rw-r--   0     1000     1001      348 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/kolo.py
--rw-rw-r--   0     1000     1001     1322 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/unittest.py
--rw-rw-r--   0     1000     1001     4355 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/exception.py
--rw-rw-r--   0     1000     1001     1457 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/pytest.py
--rw-rw-r--   0     1000     1001     4345 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/sql.py
--rw-rw-r--   0     1000     1001     2262 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/celery.py
--rw-rw-r--   0     1000     1001     3157 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/urllib.py
--rw-rw-r--   0     1000     1001     4055 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/django.py
--rw-rw-r--   0     1000     1001     1778 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/logging.py
--rw-rw-r--   0     1000     1001     5180 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/core.py
--rw-rw-r--   0     1000     1001      809 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/attrs.py
--rw-rw-r--   0     1000     1001     3707 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/urllib3.py
--rw-rw-r--   0     1000     1001      141 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/pypy.py
--rw-rw-r--   0     1000     1001        0 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/__init__.py
--rw-rw-r--   0     1000     1001     2921 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/huey.py
--rw-rw-r--   0     1000     1001     2640 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/middleware.py
--rw-rw-r--   0     1000     1001      951 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/templates/django_request_test.py.j2
--rw-rw-r--   0     1000     1001    13710 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/profiler.py
--rw-rw-r--   0     1000     1001      169 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/version.py
--rw-rw-r--   0     1000     1001     3210 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/generate_tests.py
--rw-rw-r--   0     1000     1001     6765 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/__main__.py
--rw-rw-r--   0     1000     1001     3556 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/db.py
--rw-rw-r--   0     1000     1001      473 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/git.py
--rw-rw-r--   0     1000     1001      228 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/pytest_plugin.py
--rw-rw-r--   0     1000     1001      108 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/__init__.py
--rw-rw-r--   0     1000     1001     2881 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/config.py
--rw-rw-r--   0     1000     1001      228 2023-04-18 16:24:50.000000 kolo-2.6.2/README.md
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.7.0/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-04-21 15:48:20.000000 kolo-2.7.0/rust/build.rs
+-rw-rw-r--   0     1000     1001    35236 2023-04-21 15:48:20.000000 kolo-2.7.0/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2106 2023-04-21 15:48:20.000000 kolo-2.7.0/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-04-21 15:48:50.000000 kolo-2.7.0/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     2039 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/django_schema.py
+-rw-rw-r--   0     1000     1001     3798 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3400 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4355 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4055 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001      951 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/version.py
+-rw-rw-r--   0     1000     1001     3210 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001     7537 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     4450 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-04-21 15:48:20.000000 kolo-2.7.0/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-04-21 15:48:20.000000 kolo-2.7.0/README.md
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.7.0/PKG-INFO
```

### Comparing `kolo-2.6.2/rust/Cargo.toml` & `kolo-2.7.0/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/rust/src/lib.rs` & `kolo-2.7.0/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/pyproject.toml` & `kolo-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.6.2"
+version = "2.7.0"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
```

### Comparing `kolo-2.6.2/rust/Cargo.lock` & `kolo-2.7.0/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
```

### Comparing `kolo-2.6.2/src/kolo/serialize.py` & `kolo-2.7.0/src/kolo/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import gzip
 import json
 import logging
 import os
 import types
 from cgi import parse_header
+from datetime import date, datetime
 from typing import Any, Dict, TypeVar, TYPE_CHECKING
 
 
 logger = logging.getLogger("kolo")
 
 
 if TYPE_CHECKING:
@@ -63,14 +64,16 @@
         return json.dumps(data, skipkeys=True, cls=KoloJSONEncoder)
     finally:
         IN_KOLO_PROFILER = False
 
 
 class KoloJSONEncoder(json.JSONEncoder):
     def default(self, obj):
+        if isinstance(obj, (datetime, date)):
+            return obj.isoformat()
         try:
             return repr(obj)
         except Exception:
             return "SerializationError"
 
 
 def decode_header_value(bytes_or_str: bytes | str) -> str:
```

### Comparing `kolo-2.6.2/src/kolo/filters/requests.py` & `kolo-2.7.0/src/kolo/filters/requests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/unittest.py` & `kolo-2.7.0/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/exception.py` & `kolo-2.7.0/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/pytest.py` & `kolo-2.7.0/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/sql.py` & `kolo-2.7.0/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/celery.py` & `kolo-2.7.0/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/urllib.py` & `kolo-2.7.0/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/django.py` & `kolo-2.7.0/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/logging.py` & `kolo-2.7.0/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/core.py` & `kolo-2.7.0/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/attrs.py` & `kolo-2.7.0/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/urllib3.py` & `kolo-2.7.0/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/filters/huey.py` & `kolo-2.7.0/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/middleware.py` & `kolo-2.7.0/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/templates/django_request_test.py.j2` & `kolo-2.7.0/src/kolo/templates/django_request_test.py.j2`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/profiler.py` & `kolo-2.7.0/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/generate_tests.py` & `kolo-2.7.0/src/kolo/generate_tests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/src/kolo/__main__.py` & `kolo-2.7.0/src/kolo/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 import json
 import sqlite3
 import sys
 from runpy import run_module, run_path
 
 import click
 
+from . import django_schema
 from .config import load_config
 from .db import (
+    create_schema_table,
+    db_cursor,
     delete_traces_from_db,
     list_traces_from_db,
     load_trace_from_db,
     save_invocation_in_sqlite,
+    save_schema,
     setup_db,
 )
 from .profiler import KoloProfiler
 from .serialize import monkeypatch_queryset_repr
 
 
 DATETIME_FORMATS = click.DateTime(
@@ -242,9 +246,34 @@
 
     if file:
         file.write(test_code)
     else:
         click.echo(test_code)
 
 
+DJANGO_SETTINGS_ERROR = """Django settings not found.
+Use `--settings` or set the `DJANGO_SETTINGS_MODULE` environment variable."""
+
+
+@cli.command()
+@click.option("--settings", default="")
+def store_django_model_schema(settings):
+    import os
+    import django
+
+    if not os.environ.setdefault("DJANGO_SETTINGS_MODULE", settings):
+        raise click.ClickException(DJANGO_SETTINGS_ERROR)
+
+    django.setup()
+
+    schema = django_schema.get_schema()
+
+    db_config = load_config()
+    wal_mode = db_config.get("wal_mode", True)
+    db_path = setup_db(db_config)
+    with db_cursor(db_path, wal_mode) as cursor:
+        create_schema_table(cursor)
+        save_schema(cursor, schema)
+
+
 if __name__ == "__main__":
     cli()  # pragma: no cover
```

### Comparing `kolo-2.6.2/src/kolo/db.py` & `kolo-2.7.0/src/kolo/db.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import json
 import sqlite3
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
-from typing import Any, MutableMapping
+from typing import Any, Dict, MutableMapping, Tuple
 
 from .config import create_kolo_directory
 
 
 @contextmanager
 def db_cursor(db_path, wal_mode=True):
     """
@@ -119,7 +120,38 @@
         cursor.execute("SELECT changes()")
         data = cursor.fetchone()
 
     if vacuum:
         with db_cursor(db_path, wal_mode=False) as cursor:
             cursor.execute("VACUUM")
     return data[0]
+
+
+def create_schema_table(cursor) -> None:
+    create_table_query = """
+    CREATE TABLE IF NOT EXISTS schemas (
+        id integer PRIMARY KEY,
+        created_at TEXT DEFAULT (STRFTIME('%Y-%m-%d %H:%M:%f', 'NOW')) NOT NULL,
+        git_commit TEXT NULL,
+        data text NOT NULL
+    );
+    """
+
+    cursor.execute(create_table_query)
+
+
+def save_schema(cursor, schema) -> None:
+    from .git import COMMIT_SHA
+
+    insert_sql = 'INSERT INTO schemas("data", "git_commit") VALUES(?, ?)'
+    cursor.execute(insert_sql, (json.dumps(schema), COMMIT_SHA))
+
+
+def load_schema(db_path: Path, wal_mode: bool = True) -> Tuple[Dict[str, Any], str]:
+    load_sql = "SELECT data, git_commit FROM schemas LIMIT 1"
+
+    with db_cursor(db_path) as cursor:
+        cursor.execute(load_sql)
+        data, commit = cursor.fetchone()
+
+    data = json.loads(data)
+    return data, commit
```

### Comparing `kolo-2.6.2/src/kolo/config.py` & `kolo-2.7.0/src/kolo/config.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.2/PKG-INFO` & `kolo-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.6.2
+Version: 2.7.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -35,17 +35,17 @@
 Requires-Dist: jinja2>=3.0.0; extra == 'test_generation'
 Provides-Extra: test_generation
 Summary: See everything happening in your running Django app
 Author-email: Wilhelm Klopp <team@kolo.app>, Lily Foote <lily@kolo.app>
 License: © Kolo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/kolofordjango/kolo
-Project-URL: Homepage, https://kolo.app
 Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
+Project-URL: Homepage, https://kolo.app
+Project-URL: Repository, https://github.com/kolofordjango/kolo
 
 # Kolo
 
 See everything happening in your running Django app
 
 More information: https://kolo.app
```

