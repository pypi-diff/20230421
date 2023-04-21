# Comparing `tmp/databudgie-2.7.2.tar.gz` & `tmp/databudgie-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.7.2.tar", max compression
+gzip compressed data, was "databudgie-2.7.4.tar", max compression
```

## Comparing `databudgie-2.7.2.tar` & `databudgie-2.7.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     5139 2023-01-12 17:17:37.819760 databudgie-2.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-01-12 17:17:37.819760 databudgie-2.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-01-12 17:17:37.819760 databudgie-2.7.2/LICENSE
--rw-r--r--   0        0        0     1292 2023-01-12 17:17:37.819760 databudgie-2.7.2/README.md
--rw-r--r--   0        0        0     2867 2023-01-12 17:17:37.823760 databudgie-2.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     6597 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    10464 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     9487 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     2709 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     4649 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     1481 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/cli/config.py
--rw-r--r--   0        0        0      456 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/cli/setup.py
--rw-r--r--   0        0        0     1112 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/compression.py
--rw-r--r--   0        0        0    10174 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/match.py
--rw-r--r--   0        0        0     1502 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/py.typed
--rw-r--r--   0        0        0    13195 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/restore.py
--rw-r--r--   0        0        0     1891 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/s3.py
--rw-r--r--   0        0        0     4551 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2986 2023-01-12 17:17:37.823760 databudgie-2.7.2/src/databudgie/utils.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 databudgie-2.7.2/setup.py
--rw-r--r--   0        0        0     2652 1970-01-01 00:00:00.000000 databudgie-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-04-21 18:37:32.911767 databudgie-2.7.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-04-21 18:37:32.911767 databudgie-2.7.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-04-21 18:37:32.911767 databudgie-2.7.4/LICENSE
+-rw-r--r--   0        0        0     1292 2023-04-21 18:37:32.911767 databudgie-2.7.4/README.md
+-rw-r--r--   0        0        0     2879 2023-04-21 18:37:32.911767 databudgie-2.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7162 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    10638 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     7361 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     2896 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     6458 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     1473 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0      456 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/setup.py
+-rw-r--r--   0        0        0     1112 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11862 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8408 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11806 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/storage.py
+-rw-r--r--   0        0        0     4586 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2320 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 databudgie-2.7.4/setup.py
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 databudgie-2.7.4/PKG-INFO
```

### Comparing `databudgie-2.7.2/CHANGELOG.md` & `databudgie-2.7.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/CONTRIBUTING.md` & `databudgie-2.7.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/LICENSE` & `databudgie-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/README.md` & `databudgie-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/pyproject.toml` & `databudgie-2.7.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.7.2"
+version = "2.7.4"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
@@ -38,42 +38,38 @@
 importlib-metadata = {version = "*", python = "<3.8"}
 
 boto3 = { version = "*", optional = true }
 sentry-sdk = { version = "*", optional = true }
 psycopg2 = { version = ">=2.7", optional = true }
 psycopg2-binary = { version = ">=2.7", optional = true }
 
+[tool.poetry.extras]
+sentry = ["sentry-sdk"]
+s3 = ["boto3"]
+psycopg2 = ["psycopg2"]
+psycopg2-binary = ["psycopg2-binary"]
+
 [tool.poetry.dev-dependencies]
 boto3 = "^1.16.10,<1.17.72"
-bandit = "^1.6.2"
 black = "22.3.0"
 boto3-stubs = {extras = ["s3"], version = "^1.18.38"}
 coverage = ">=5"
-flake8 = ">=5"
 freezegun = "*"
-isort = ">=5"
 mypy = "^0.991"
-ptpython = "^2.0.6"
-pydocstyle = {version = "^6.1.1", extras = ['toml']}
 pytest = ">=6.2.4"
 pytest-mock-resources = {version = ">=2.1.10", extras = ["docker"]}
 responses = "^0.10.9"
+ruff = "0.0.254"
 types-freezegun = "^0.1.3"
 types-requests = "^0.1.11"
 faker = "^8.12.1"
 moto = {extras = ["s3"], version = "^2.2.6"}
 sqlalchemy-model-factory = "^0.4.5"
 types-click = "^7.1.5"
 
-[tool.poetry.extras]
-sentry = ["sentry-sdk"]
-s3 = ["boto3"]
-psycopg2 = ["psycopg2"]
-psycopg2-binary = ["psycopg2-binary"]
-
 [tool.black]
 line_length = 120
 
 [tool.isort]
 profile = 'black'
 known_first_party = 'databudgie,tests'
 line_length = 120
@@ -106,12 +102,14 @@
 
 [tool.pytest.ini_options]
 doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
 addopts = "--doctest-modules -vv --ff --strict-markers"
 norecursedirs = ".* build dist *.egg migrations bin"
 filterwarnings = [
     "ignore::sqlalchemy.exc.SAWarning",
+    "ignore::sqlalchemy.exc.SADeprecationWarning",
+    "ignore:ssl.PROTOCOL_TLS is deprecated:DeprecationWarning",
 ]
 
 [build-system]
 requires = ["poetry_core==1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `databudgie-2.7.2/src/databudgie/adapter/base.py` & `databudgie-2.7.4/src/databudgie/adapter/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from __future__ import annotations
+
+import contextlib
 import csv
 import io
 import warnings
-from dataclasses import dataclass, replace
-from typing import Any, cast, Dict, Generator, List, Optional, Sequence
+from dataclasses import dataclass, field, replace
+from typing import Any, cast, Generator, Sequence
 
 import sqlalchemy
 from sqlalchemy import inspect, MetaData, Table, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session
 
 from databudgie.output import Console, default_console
 from databudgie.table_op import TableOp
-from databudgie.utils import join_paths, parse_table
+from databudgie.utils import join_paths, parse_table, wrap_buffer
 
 
 @dataclass
 class Adapter:
     """Root class designating a shared interface for operating on different databases.
 
     Any database-agnostic functionality should live here, while more optimized
@@ -24,15 +27,15 @@
 
     Uses native Python CSV methods with a lightweight/naive type conversion on insert.
     """
 
     session: Session
 
     @classmethod
-    def get_adapter(cls, session: Session, dialect: Optional[str] = None) -> "Adapter":
+    def get_adapter(cls, session: Session, dialect: str | None = None) -> Adapter:
         """Determine an interface based on the dialect name from the Session (or an explicit string).
 
         Examples:
             >>> from databudgie.adapter.postgres import PostgresAdapter
             >>> adapter = Adapter.get_adapter(None, "postgres")
             >>> isinstance(adapter, PostgresAdapter)
             True
@@ -45,37 +48,43 @@
         if dialect is None:
             dialect = session.get_bind().dialect.name
 
         if dialect in ("postgres", "postgresql"):
             from databudgie.adapter.postgres import PostgresAdapter
 
             return PostgresAdapter(session)
-        else:
-            return cls(session)
 
-    def export_query(self, query: str, dest: io.StringIO):
+        return cls(session)
+
+    def export_query(self, query: str) -> QueryResult:
         def query_database(session: Session, query: str) -> Generator[Sequence[Any], None, None]:
             cursor = session.execute(text(query))
 
             columns: Sequence[str] = list(cursor.keys())
             yield columns
 
-            for row in cursor:
-                yield row
+            yield from cursor
+
+        result = QueryResult()
+        with result.text_buffer() as text_buffer:
+            writer = csv.writer(text_buffer, quoting=csv.QUOTE_MINIMAL)
+
+            i = 0
+            for i, row in enumerate(query_database(self.session, query), start=1):
+                writer.writerow(row)
 
-        writer = csv.writer(dest, quoting=csv.QUOTE_MINIMAL)
-        for row in query_database(self.session, query):
-            writer.writerow(row)
+        result.row_count = i
+        return result
 
     def import_csv(self, csv_file: io.TextIOBase, table: str):
         reader = csv.DictReader(csv_file, quoting=csv.QUOTE_MINIMAL)
 
-        prepared_rows: List[dict] = []
+        prepared_rows: list[dict] = []
         for row in reader:
-            new_row: Dict[str, Any] = dict(row)
+            new_row: dict[str, Any] = dict(row)
             for key, value in new_row.items():
                 if value.lower() == "true":
                     new_row[key] = True
                 elif value.lower() == "false":
                     new_row[key] = False
                 elif value == "":
                     new_row[key] = None
@@ -113,15 +122,15 @@
         the temp database.
 
         This method suffers from being rather prone to failure, but is better
         than nothing!
         """
         raise NotImplementedError()
 
-    def collect_existing_tables(self) -> List[str]:
+    def collect_existing_tables(self) -> list[str]:
         """Find the set of all user-defined tables in a database."""
         connection = self.session.connection()
 
         metadata = MetaData()
         insp = inspect(connection)
         for schema in insp.get_schema_names():
             # Seems to be a generally cross-database compatible filter.
@@ -130,32 +139,32 @@
 
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 metadata.reflect(bind=connection, schema=schema)
 
         return [table.fullname for table in metadata.sorted_tables]
 
-    def collect_table_dependencies(self, table_op: TableOp, console: Console = default_console) -> List[str]:
+    def collect_table_dependencies(self, table_op: TableOp, console: Console = default_console) -> list[str]:
         raise NotImplementedError()
 
-    def collect_table_sequences(self) -> Dict[str, List[str]]:
+    def collect_table_sequences(self) -> dict[str, list[str]]:
         raise NotImplementedError()
 
     def collect_sequence_value(self, sequence_name: str) -> int:
         raise NotImplementedError()
 
     def restore_sequence_value(self, sequence_name: str, value: int) -> int:
         raise NotImplementedError()
 
     def materialize_table_dependencies(
         self,
-        table_ops: List[TableOp],
+        table_ops: list[TableOp],
         reverse: bool = False,
         console: Console = default_console,
-    ) -> List[TableOp]:
+    ) -> list[TableOp]:
         tables = set()
         dependent_table_ops = []
         for table_op in table_ops:
             tables.add(table_op.full_name)
 
             if not table_op.raw_conf.follow_foreign_keys:
                 continue
@@ -173,7 +182,23 @@
         if reverse:
             # The original `table_ops` list comes to us already reverse
             # ordered, so we need to preserve it's original order, and
             # just invert the net-new tables and put them first.
             return list(reversed(dependent_table_ops)) + table_ops
 
         return table_ops + dependent_table_ops
+
+
+@dataclass
+class QueryResult:
+    buffer: io.BytesIO = field(default_factory=io.BytesIO)
+    row_count: int = 0
+
+    @contextlib.contextmanager
+    def binary_buffer(self):
+        yield self.buffer
+        self.buffer.seek(0)
+
+    @contextlib.contextmanager
+    def text_buffer(self):
+        with wrap_buffer(self.buffer) as text_buffer:
+            yield text_buffer
```

### Comparing `databudgie-2.7.2/src/databudgie/adapter/postgres.py` & `databudgie-2.7.4/src/databudgie/adapter/postgres.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import contextlib
 import io
 import os
 import shlex
 import shutil
 import subprocess  # nosec
 from typing import cast, Dict, List
 
-import psycopg2.errors
+from psycopg2._psycopg import cursor
 from sqlalchemy import text
 from sqlalchemy.engine import create_engine, Engine
 from sqlalchemy.engine.url import URL
 
-from databudgie.adapter.base import Adapter
+from databudgie.adapter.base import Adapter, QueryResult
 from databudgie.output import Console, default_console
 from databudgie.table_op import TableOp
 
 
 def update_url(url, database=None):
     try:
         return url.set(database=database)
@@ -26,49 +27,48 @@
             host=url.host,
             port=url.port,
             database=database or url.database,
         )
 
 
 class PostgresAdapter(Adapter):
-    def export_query(self, query: str, dest: io.StringIO):
+    def export_query(self, query: str) -> QueryResult:
         engine: Engine = cast(Engine, self.session.get_bind())
-        conn = engine.raw_connection()
-        cursor: psycopg2.cursor = conn.cursor()
 
-        copy = "COPY ({}) TO STDOUT CSV HEADER".format(query)
-        cursor.copy_expert(copy, dest)
-        cursor.close()
-        conn.close()
+        result = QueryResult()
+        with result.binary_buffer() as buffer:
+            with contextlib.closing(engine.raw_connection()) as conn:
+                with cast(cursor, conn.cursor()) as cursor_:
+                    copy = f"COPY ({query}) TO STDOUT CSV HEADER"
+
+                    cursor_.copy_expert(copy, buffer)
+                    result.row_count = cursor_.rowcount
+
+        return result
 
     def import_csv(self, csv_file: io.TextIOBase, table: str):
         engine: Engine = cast(Engine, self.session.get_bind())
-        conn = engine.raw_connection()
-        cursor: psycopg2.cursor = conn.cursor()
 
         # Reading the header line from the buffer removes it for the ingest
         columns: List[str] = [f'"{c}"' for c in csv_file.readline().strip().split(",")]
-
         copy = "COPY {table} ({columns}) FROM STDIN CSV".format(table=table, columns=",".join(columns))
-        cursor.copy_expert(copy, csv_file)
-        cursor.close()
-        conn.commit()
-        conn.close()
+
+        with contextlib.closing(engine.raw_connection()) as conn:
+            with cast(cursor, conn.cursor()) as cursor_:
+                cursor_.copy_expert(copy, csv_file)
+                conn.commit()
 
     def export_schema_ddl(self, name: str, console: Console = default_console) -> bytes:
         if not shutil.which("pg_dump"):
             console.warn("Could not find pg_dump, falling back to SQLAlchemy implementation.")
             return super().export_schema_ddl(name)
 
         url = self.session.connection().engine.url
         result = pg_dump(url, f"--schema-only --schema={name} --exclude-table={name}.*")
-        result = result.replace(
-            f"CREATE SCHEMA {name};".encode("utf-8"), f"CREATE SCHEMA IF NOT EXISTS {name};".encode("utf-8")
-        )
-        return result
+        return result.replace(f"CREATE SCHEMA {name};".encode(), f"CREATE SCHEMA IF NOT EXISTS {name};".encode())
 
     def export_table_ddl(self, table_name: str, console: Console = default_console):
         if not shutil.which("pg_dump"):
             console.warn("Could not find pg_dump, falling back to SQLAlchemy implementation.")
             return super().export_table_ddl(table_name)
 
         url = self.session.connection().engine.url
@@ -192,15 +192,15 @@
             from all_tables at
             where last_table_row = 1
             order by level;
             """
         )
 
         results = self.session.execute(
-            collect_tables, params=dict(schema=table_op.schema, table_name=table_op.table_name)
+            collect_tables, params={"schema": table_op.schema, "table_name": table_op.table_name}
         )
 
         return [row[0] for row in results]
 
     def collect_table_sequences(self) -> Dict[str, List[str]]:
         sequences = self.session.execute(
             text(
@@ -222,15 +222,15 @@
         )
         result: Dict = {}
         for sequence in sequences:
             result.setdefault(sequence.fq_table_name, []).append(sequence.fq_sequence_name)
         return result
 
     def collect_sequence_value(self, sequence_name: str) -> int:
-        return cast(int, self.session.execute(text(f"SELECT last_value from {sequence_name}")).scalar())  # nosec
+        return cast(int, self.session.execute(text(f"SELECT last_value from {sequence_name}")).scalar())  # noqa: S608
 
     def restore_sequence_value(self, sequence_name: str, value: int) -> int:
         return cast(int, self.session.execute(text(f"SELECT setval('{sequence_name}', {value})")).scalar())
 
 
 def pg_dump(url: URL, rest: str = "", no_comments=True) -> bytes:
     parts = [f"pg_dump -h {url.host} -p {url.port} -U {url.username} -d {url.database} --no-password"]
```

### Comparing `databudgie-2.7.2/src/databudgie/compression.py` & `databudgie-2.7.4/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/src/databudgie/config.py` & `databudgie-2.7.4/src/databudgie/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import abc
 import typing
-from dataclasses import asdict, dataclass, field
-from typing import Any, Optional, Union
+from dataclasses import dataclass, field, fields
+from typing import Any
 
 from databudgie.utils import join_paths
 
 T = typing.TypeVar("T", "BackupTableConfig", "RestoreTableConfig")
 F = typing.TypeVar("F")
 
 
 class ConfigError(ValueError):
     """Raise for invalid or incomplete config."""
 
 
 class ConfigStack:
     def __init__(self, *configs: dict):
-        self.configs: typing.Tuple[dict, ...] = configs
+        self.configs: tuple[dict, ...] = configs
 
     def __getitem__(self, key):
         for config in self.configs:
             if config and key in config:
                 return config[key]
         raise KeyError(key)
 
@@ -39,15 +39,28 @@
 
     def push(self, config: dict):
         return ConfigStack(config, *self.configs)
 
 
 class Config(metaclass=abc.ABCMeta):
     def to_dict(self) -> dict:
-        return asdict(self)
+        result = {}
+        for f in fields(self):
+            v = getattr(self, f.name)
+            if isinstance(v, Config):
+                value: Any = v.to_dict()
+            elif isinstance(v, list):
+                value = [v.to_dict() if isinstance(v, Config) else v for v in v]
+            elif isinstance(v, dict):
+                value = {k: v.to_dict() if isinstance(v, Config) else v for k, v in v.items()}
+            else:
+                value = v
+
+            result[f.name] = value
+        return result
 
 
 def from_partial(cls: typing.Callable[..., F], **kwargs) -> F:
     """Create a new instance of cls with the given kwargs.
 
     This is useful for creating a new instance of a class with only some of the
     fields set.
@@ -60,26 +73,26 @@
 # Optional Configs which have default values built-in
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 @dataclass
 class DDLConfig(Config):
     enabled: bool = False
-    location: str = "ddl"
+    location: str = "backups/ddl"
     clean: bool = False
     strategy: str = "use_latest_filename"
 
     @classmethod
-    def from_dict(cls, ddl_config: Union[dict, bool], root_location: Optional[str] = None):
+    def from_dict(cls, ddl_config: dict | bool, root_location: str | None = None):
         if isinstance(ddl_config, bool):
             expanded_ddl_config: dict[str, Any] = {"enabled": ddl_config}
         else:
             expanded_ddl_config = ddl_config
 
-        location = join_paths(root_location, expanded_ddl_config.get("location"))
+        location = compose_root_location(root_location, expanded_ddl_config.get("location"), default="backups/ddl")
 
         # Splat into a new dict so we can override `location` without mutating
         # the original input (which may be re-read later in config parsing)
         final_ddl_config = {**expanded_ddl_config, "location": location}
 
         return from_partial(cls, **final_ddl_config)
 
@@ -87,16 +100,16 @@
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # Core configuration models
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 @dataclass
 class RootConfig(Config):
-    backup: Optional[BackupConfig] = None
-    restore: Optional[RestoreConfig] = None
+    backup: BackupConfig
+    restore: RestoreConfig
 
     @classmethod
     def from_dict(cls, raw_config: dict):
         config = ConfigStack(raw_config)
         return cls.from_stack(config)
 
     @classmethod
@@ -104,103 +117,136 @@
         backup_config = stack.get("backup", {})
         backup = BackupConfig.from_stack(stack.push(backup_config))
 
         restore_config = stack.get("restore", {})
         restore = RestoreConfig.from_stack(stack.push(restore_config))
         return cls(backup=backup, restore=restore)
 
-    def to_dict(self) -> dict:
-        return {
-            "backup": self.backup.to_dict() if self.backup else None,
-            "restore": self.restore.to_dict() if self.restore else None,
-        }
-
 
 @dataclass
 class TableParentConfig(typing.Generic[T], Config):
-    url: typing.Union[str, dict]
-    tables: typing.List[T]
-
+    tables: list[T]
+    connections: dict[str, Connection]
     ddl: DDLConfig
-    manifest: Optional[str] = None
 
-    s3: Optional[S3Config] = None
-    sentry: Optional[SentryConfig] = None
-    root_location: Optional[str] = None
-    adapter: Optional[str] = None
+    connection: Connection | None = None
+    manifest: str | None = None
+
+    s3: S3Config | None = None
+    sentry: SentryConfig | None = None
+    root_location: str | None = None
+    adapter: str | None = None
 
     @classmethod
     @abc.abstractmethod
     def get_child_class(cls):
         pass
 
     @classmethod
     def from_stack(cls, stack: ConfigStack):
-        url: str = stack.get("url")
+        connection = Connection.from_raw(stack.get("url") or stack.get("connection"), name="default")
         root_location = stack.get("root_location")
 
         tables_config: list = normalize_table_config(stack.get("tables", []))
         table_class = cls.get_child_class()
         tables = [table_class.from_stack(stack.push(tbl_conf), root_location) for tbl_conf in tables_config]
 
         # manifest defauls to None
-        manifest: Optional[str] = stack.get("manifest")
+        manifest: str | None = stack.get("manifest")
 
         ddl = DDLConfig.from_dict(stack.get("ddl", {}), root_location)
 
         # Optional integration configs
         s3 = S3Config.from_dict(stack.get("s3"))
         sentry = SentryConfig.from_dict(stack.get("sentry"))
 
         adapter = stack.get("adapter")
 
+        connections = Connection.from_collection(stack.get("connections"))
+
         return cls(
-            url=url,
+            connection=connection,
             tables=tables,
             manifest=manifest,
             s3=s3,
             sentry=sentry,
             ddl=ddl,
             root_location=root_location,
             adapter=adapter,
+            connections=connections,
         )
 
-    def to_dict(self) -> dict:
-        return {
-            "url": self.url,
-            "tables": [table.to_dict() for table in self.tables],
-            "manifest": self.manifest,
-            "ddl": self.ddl.to_dict(),
-            "s3": self.s3.to_dict() if self.s3 else None,
-            "sentry": self.sentry.to_dict() if self.sentry else None,
-            "root_location": self.root_location,
-            "adapter": self.adapter,
-        }
+
+@dataclass
+class Connection(Config):
+    name: str
+    url: str | dict
+
+    @classmethod
+    def from_raw(cls, raw: str | dict | None, *, name: str | None = None):
+        if raw is None:
+            return None
+
+        if isinstance(raw, str):
+            if name is None:
+                raise ConfigError(f"Connection '{raw}' requires a name")
+            return cls(name="default", url=raw)
+
+        if name is None:
+            raise ConfigError(f"Connection '{raw}' requires a name")
+
+        if "url" in raw:
+            url = raw["url"]
+        else:
+            url = {k: v for k, v in raw.items() if k != "name"}
+
+        return cls(name=name or "default", url=url)
+
+    @classmethod
+    def from_collection(cls, collection: list | dict | None) -> dict[str, Connection]:
+        if collection is None:
+            return {}
+
+        if isinstance(collection, list):
+            connections = []
+            names = set()
+            for c in collection:
+                connection = Connection.from_raw(c, name=c.get("name"))
+                assert connection is not None
+
+                if connection.name in names:
+                    raise ConfigError(f"Detected more than one connection with the same name: {connection.name}")
+                names.add(connection.name)
+                connections.append(connection)
+
+            return {c.name: c for c in connections}
+
+        return {k: Connection.from_raw(c, name=k) for k, c in collection.items()}
 
 
 @dataclass
 class BackupTableConfig(Config):
     name: str
     location: str = "backups/{table}"
     query: str = "select * from {table}"
-    compression: Optional[str] = None
+    compression: str | None = None
     exclude: list = field(default_factory=list)
     ddl: bool = True
     sequences: bool = True
     data: bool = True
     follow_foreign_keys: bool = False
     strict: bool = False
 
     @classmethod
-    def from_stack(cls, stack: ConfigStack, root_location: Optional[str] = None):
+    def from_stack(cls, stack: ConfigStack, root_location: str | None = None):
         ddl = stack.get("ddl", True)
         if isinstance(ddl, dict):
             ddl = ddl["enabled"]
 
-        location = join_paths(root_location, stack.get("location")) or None
+        location = compose_root_location(root_location, stack.get("location"), default="backups/{table}")
 
         return from_partial(
             cls,
             name=stack.get("name"),
             location=location,
             query=stack.get("query"),
             compression=stack.get("compression"),
@@ -221,30 +267,30 @@
 
 
 @dataclass
 class RestoreTableConfig(Config):
     name: str
     location: str = "backups/{table}"
     strategy: str = "use_latest_filename"
-    compression: Optional[str] = None
+    compression: str | None = None
     exclude: list = field(default_factory=list)
     ddl: bool = True
     sequences: bool = True
     truncate: bool = False
     data: bool = True
     follow_foreign_keys: bool = False
     strict: bool = False
 
     @classmethod
-    def from_stack(cls, stack: ConfigStack, root_location: Optional[str] = None):
+    def from_stack(cls, stack: ConfigStack, root_location: str | None = None):
         ddl = stack.get("ddl", True)
         if isinstance(ddl, dict):
             ddl = ddl["enabled"]
 
-        location = join_paths(root_location, stack.get("location"))
+        location = compose_root_location(root_location, stack.get("location"), default="backups/{table}")
 
         return from_partial(
             cls,
             name=stack.get("name"),
             location=location,
             strategy=stack.get("strategy"),
             truncate=stack.get("truncate"),
@@ -261,28 +307,29 @@
 @dataclass
 class RestoreConfig(TableParentConfig[RestoreTableConfig]):
     @classmethod
     def get_child_class(cls):
         return RestoreTableConfig
 
 
-def normalize_table_config(tables_config: typing.Union[list, dict]) -> list:
+def normalize_table_config(tables_config: list | dict) -> list:
     """Convert the dict-style table declaration into list style.
 
     from: {"name": {"location": "backups/{table}"}}
     to: [{"name": "blah", "location": "backups/{table}"}]
 
     alternatively:
     from: ["name1", "name2"]
     to: [{"name": "name1"}, {"name": "name2"}]
     """
     if isinstance(tables_config, dict):
-        tables_config = [{"name": k, **v} for k, v in tables_config.items()]
-    elif isinstance(tables_config, list):
-        tables_config = [{"name": c} if isinstance(c, str) else c for c in tables_config]
+        return [{"name": k, **v} for k, v in tables_config.items()]
+
+    if isinstance(tables_config, list):
+        return [{"name": c} if isinstance(c, str) else c for c in tables_config]
 
     return tables_config
 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # Optional Integration configs which do NOT have default values built-in
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
@@ -291,40 +338,47 @@
 @dataclass
 class SentryConfig(Config):
     """Configuration for Sentry integration.
 
     SentryConfig does not inherit keys from the root config.
     """
 
-    dsn: Optional[str] = None
-    environment: Optional[str] = None
-    version: Optional[str] = None
+    dsn: str | None = None
+    environment: str | None = None
+    version: str | None = None
 
     @classmethod
-    def from_dict(cls, sentry_config: Optional[dict]) -> Optional[SentryConfig]:
+    def from_dict(cls, sentry_config: dict | None) -> SentryConfig | None:
         if sentry_config is None:
             return None
 
         return cls(
             dsn=sentry_config.get("dsn"),
             environment=sentry_config.get("environment"),
             version=sentry_config.get("version"),
         )
 
 
 @dataclass
 class S3Config(Config):
-    aws_access_key_id: Optional[str] = None
-    aws_secret_access_key: Optional[str] = None
-    region: Optional[str] = None
-    profile: Optional[str] = None
+    aws_access_key_id: str | None = None
+    aws_secret_access_key: str | None = None
+    region: str | None = None
+    profile: str | None = None
 
     @classmethod
-    def from_dict(cls, s3_config: Optional[dict]) -> Optional[S3Config]:
+    def from_dict(cls, s3_config: dict | None) -> S3Config | None:
         if s3_config is None:
             return None
         return cls(
             aws_access_key_id=s3_config.get("aws_access_key_id"),
             aws_secret_access_key=s3_config.get("aws_secret_access_key"),
             region=s3_config.get("region"),
             profile=s3_config.get("profile"),
         )
+
+
+def compose_root_location(root_location, location, *, default):
+    if root_location is None:
+        return location or default
+
+    return join_paths(root_location, location or default)
```

### Comparing `databudgie-2.7.2/src/databudgie/manifest/manager.py` & `databudgie-2.7.4/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.7.4/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/src/databudgie/match.py` & `databudgie-2.7.4/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.2/src/databudgie/output.py` & `databudgie-2.7.4/src/databudgie/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from rich import console, progress
+from rich.table import Table
 from rich.theme import Theme
 from rich.traceback import Traceback
 
 
 class Console(console.Console):
     theme = Theme({"trace": "white", "info": "blue", "warn": "yellow", "error": "bold red"})
 
     def __init__(self, verbosity=0):
         super().__init__(theme=self.theme, log_time=True)
         self.verbosity = verbosity
 
     def trace(self, message):
         if self.verbosity >= 1:
             return self.log(message, style="trace")
+        return None
 
     def info(self, message):
         return self.log(message, style="info")
 
     def warn(self, message):
         return self.log(message, style="warn")
 
@@ -46,8 +48,9 @@
 
 
 __all__ = [
     "Console",
     "default_console",
     "Progress",
     "Traceback",
+    "Table",
 ]
```

### Comparing `databudgie-2.7.2/src/databudgie/s3.py` & `databudgie-2.7.4/src/databudgie/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from __future__ import annotations
 
 import urllib.parse
-from typing import Optional, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from mypy_boto3_s3 import S3ServiceResource
 
     from databudgie.config import BackupConfig, RestoreConfig, S3Config
 
 
-def optional_s3_resource(config: Union[BackupConfig, RestoreConfig]) -> Optional["S3ServiceResource"]:
-    if config_uses_s3(config) and config.s3:
+def optional_s3_resource(config: BackupConfig | RestoreConfig) -> S3ServiceResource | None:
+    if config_uses_s3(config):
         return s3_resource(config.s3)
     return None
 
 
-def s3_resource(config: S3Config) -> "S3ServiceResource":
+def s3_resource(config: S3Config | None = None) -> S3ServiceResource:
     try:
         import boto3
     except ImportError:
         raise RuntimeError('Use of S3 requires the "s3" python extra')
 
     # Boto loads all config as environment variables by default, this config
     # section can be entirely optional.
-    session = boto3.session.Session(
-        aws_access_key_id=config.aws_access_key_id,
-        aws_secret_access_key=config.aws_secret_access_key,
-        profile_name=config.profile,
-        region_name=config.region,
-    )
+    if not config:
+        session = boto3.session.Session()
+    else:
+        session = boto3.session.Session(
+            aws_access_key_id=config.aws_access_key_id,
+            aws_secret_access_key=config.aws_secret_access_key,
+            profile_name=config.profile,
+            region_name=config.region,
+        )
 
-    s3: "S3ServiceResource" = session.resource("s3")
+    s3: S3ServiceResource = session.resource("s3")
     return s3
 
 
-def config_uses_s3(config: Union[BackupConfig, RestoreConfig]):
+def config_uses_s3(config: BackupConfig | RestoreConfig):
     if config.root_location and is_s3_path(config.root_location):
         return True
 
     for table_config in config.tables:
         if is_s3_path(table_config.location):
             return True
     return False
```

### Comparing `databudgie-2.7.2/src/databudgie/table_op.py` & `databudgie-2.7.4/src/databudgie/table_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Dict, Generic, List, Optional, Sequence, TypeVar
+from typing import Generic, Sequence, TYPE_CHECKING, TypeVar
 
 from sqlalchemy import inspect
 from sqlalchemy.orm import Session
 
 from databudgie.config import BackupTableConfig, RestoreTableConfig
-from databudgie.manifest.manager import Manifest
 from databudgie.match import expand_table_globs
 from databudgie.output import Console, default_console
 from databudgie.utils import parse_table
 
+if TYPE_CHECKING:
+    from databudgie.storage import StorageBackend
+
 T = TypeVar("T", BackupTableConfig, RestoreTableConfig)
 
 
 @dataclass
 class SchemaOp(Generic[T]):
     name: str
     raw_conf: T
@@ -60,48 +64,47 @@
     def schema_op(self) -> SchemaOp:
         return SchemaOp(self.schema, self.raw_conf)
 
 
 def expand_table_ops(
     session: Session,
     tables: Sequence[T],
-    existing_tables: List[str],
+    existing_tables: list[str],
+    storage: StorageBackend,
     *,
     console: Console = default_console,
-    manifest: Optional[Manifest] = None,
     warn_for_unused_tables: bool = False,
-) -> List[TableOp[T]]:
+) -> list[TableOp[T]]:
     """Produce a full list of table operations to be performed.
 
     tables in the set of `tables` may be globbed and produce more concrete
     tables than initially specified in the input set.
 
     Additionally, tables may be filtered, either by the pre-existence of
     manifest data or explicit table exclusions.
     """
-
     # Avoid hardcoding things like "public", we hardcode this elsewhere, this
     # should probably be moved upstream.
     insp = inspect(session.connection())
     default_schema_name = insp.default_schema_name
 
     # expand table globs into fully qualified mappings to the config.
-    matching_tables: Dict[str, List[T]] = {}
+    matching_tables: dict[str, list[T]] = {}
     for table_conf in tables:
         pattern = table_conf.name
         if "." not in pattern:
             pattern = f"{default_schema_name}.{pattern}"
 
         expanded_tables = expand_table_globs(existing_tables, pattern)
         if warn_for_unused_tables and not expanded_tables:
             console.warn(f"Skipping table definition `{pattern}` which did not match any tables.")
             continue
 
         for table_name in expanded_tables:
-            if manifest and table_name in manifest:
+            if storage.check_manifest(table_name):
                 console.trace(f"Skipping {table_name}...")
                 continue
 
             for exclusion_pattern in table_conf.exclude:
                 exclusions = set(expand_table_globs(existing_tables, exclusion_pattern))
                 if table_name in exclusions:
                     break
```

### Comparing `databudgie-2.7.2/src/databudgie/utils.py` & `databudgie-2.7.4/src/databudgie/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,15 @@
 import contextlib
 import io
 import os
-from datetime import datetime
 from typing import Optional, Tuple
 
-from databudgie.compression import Compressor
 from databudgie.output import Console, default_console
 from databudgie.s3 import is_s3_path, S3Location
 
-DATETIME_FORMAT = r"%Y-%m-%dT%H:%M:%S"
-FILENAME_FORMAT = "{DATETIME_FORMAT}.csv"
-
-
-def generate_filename(timestamp=None, *, filetype="csv", compression=None):
-    if timestamp is None:
-        timestamp = datetime.now()
-
-    filetype = Compressor.get_with_name(compression).compose_filetype(filetype)
-    return timestamp.strftime(f"{DATETIME_FORMAT}.{filetype}")
-
-
-def restore_filename(timestamp, *, filetype="csv", compression=None):
-    filetype = Compressor.get_with_name(compression).compose_filetype(filetype)
-    return datetime.strptime(timestamp, f"{DATETIME_FORMAT}.{filetype}")
-
 
 @contextlib.contextmanager
 def capture_failures(ignore=(), strict=False, console: Console = default_console):
     """Prevent exceptions from interrupting execution.
 
     Examples:
         This exception is captured and not propogated:
```

### Comparing `databudgie-2.7.2/setup.py` & `databudgie-2.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'sentry': ['sentry-sdk']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.7.2',
+    'version': '2.7.4',
     'description': 'Ergonomic and flexible tool for database backup and restore',
     'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and restore\nof database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified config)\nis as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
```

### Comparing `databudgie-2.7.2/PKG-INFO` & `databudgie-2.7.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.7.2
+Version: 2.7.4
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving :: Backup
 Provides-Extra: psycopg2
 Provides-Extra: psycopg2-binary
 Provides-Extra: s3
 Provides-Extra: sentry
 Requires-Dist: boto3; extra == "s3"
 Requires-Dist: click (>=7.0.0)
```

