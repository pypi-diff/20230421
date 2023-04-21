# Comparing `tmp/asyncpg_trek-0.3.0.tar.gz` & `tmp/asyncpg_trek-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpg_trek-0.3.0.tar", max compression
+gzip compressed data, was "asyncpg_trek-0.3.1.tar", max compression
```

## Comparing `asyncpg_trek-0.3.0.tar` & `asyncpg_trek-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1063 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2054 2022-12-23 09:10:11.295529 asyncpg_trek-0.3.0/README.md
--rw-r--r--   0        0        0      246 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/__init__.py
--rw-r--r--   0        0        0     1655 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_backend.py
--rw-r--r--   0        0        0     2103 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_collect.py
--rw-r--r--   0        0        0     1972 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_run.py
--rw-r--r--   0        0        0     1929 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_solver.py
--rw-r--r--   0        0        0      580 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_types.py
--rw-r--r--   0        0        0      298 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/_typing.py
--rw-r--r--   0        0        0     2151 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/asyncpg_trek/asyncpg.py
--rw-r--r--   0        0        0     2085 2022-12-23 09:09:47.743305 asyncpg_trek-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 asyncpg_trek-0.3.0/setup.py
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 asyncpg_trek-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-21 17:59:59.793441 asyncpg_trek-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2054 2023-04-21 18:00:31.225432 asyncpg_trek-0.3.1/README.md
+-rw-r--r--   0        0        0      246 2023-04-21 17:59:59.793441 asyncpg_trek-0.3.1/asyncpg_trek/__init__.py
+-rw-r--r--   0        0        0     1655 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_backend.py
+-rw-r--r--   0        0        0     2103 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_collect.py
+-rw-r--r--   0        0        0     1972 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_run.py
+-rw-r--r--   0        0        0     1929 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_solver.py
+-rw-r--r--   0        0        0      580 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_types.py
+-rw-r--r--   0        0        0      298 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/_typing.py
+-rw-r--r--   0        0        0     2423 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/asyncpg_trek/asyncpg.py
+-rw-r--r--   0        0        0     2085 2023-04-21 17:59:59.797441 asyncpg_trek-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 asyncpg_trek-0.3.1/PKG-INFO
```

### Comparing `asyncpg_trek-0.3.0/LICENSE.txt` & `asyncpg_trek-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/README.md` & `asyncpg_trek-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 ```
 
 You could make this an entrypoint in a docker image, an admin endpoint in your API or a helper function in your tests (or all of the above).
 How you run your migrations depends on the complexity of your system.
 For example, for simple systems it may be easy to run migrations on app startup based on a hardcoded revision.
 For more complex systems you may want to run migrations manually or via an admin API.
 
-See this release on GitHub: [v0.3.0](https://github.com/adriangb/asyncpg-trek/releases/tag/0.3.0)
+See this release on GitHub: [v0.3.1](https://github.com/adriangb/asyncpg-trek/releases/tag/0.3.1)
```

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/_backend.py` & `asyncpg_trek-0.3.1/asyncpg_trek/_backend.py`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/_collect.py` & `asyncpg_trek-0.3.1/asyncpg_trek/_collect.py`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/_run.py` & `asyncpg_trek-0.3.1/asyncpg_trek/_run.py`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/_solver.py` & `asyncpg_trek-0.3.1/asyncpg_trek/_solver.py`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/_types.py` & `asyncpg_trek-0.3.1/asyncpg_trek/_types.py`

 * *Files identical despite different names*

### Comparing `asyncpg_trek-0.3.0/asyncpg_trek/asyncpg.py` & `asyncpg_trek-0.3.1/asyncpg_trek/asyncpg.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,65 +3,67 @@
 from typing import AsyncContextManager, AsyncIterator, Optional
 
 import asyncpg  # type: ignore
 
 from asyncpg_trek._types import Operation
 
 CREATE_TABLE = """\
-CREATE TABLE IF NOT EXISTS migrations (
+CREATE SCHEMA IF NOT EXISTS "{schema}";
+CREATE TABLE IF NOT EXISTS "{schema}".migrations (
     id SERIAL PRIMARY KEY,
     from_revision TEXT,
     to_revision TEXT,
     timestamp TIMESTAMP NOT NULL DEFAULT current_timestamp
 );
-CREATE INDEX ON migrations(timestamp);
+CREATE INDEX ON "{schema}".migrations(timestamp);
 """
 
-
 GET_CURRENT_REVISION = """\
 SELECT to_revision
-FROM migrations
+FROM "{schema}".migrations
 ORDER BY id DESC
 LIMIT 1;
 """
 
 RECORD_REVISION = """\
-INSERT INTO migrations(from_revision, to_revision)
+INSERT INTO "{schema}".migrations(from_revision, to_revision)
 VALUES ($1, $2)
 """
 
 
 class AsyncpgExecutor:
-    def __init__(self, connection: asyncpg.Connection) -> None:
+    def __init__(self, connection: asyncpg.Connection, schema: str) -> None:
         self.connection = connection
+        self.schema = schema
 
     async def create_table_idempotent(self) -> None:
-        await self.connection.execute(CREATE_TABLE)  # type: ignore
+        await self.connection.execute(CREATE_TABLE.format(schema=self.schema))  # type: ignore
 
     async def get_current_revision(self) -> Optional[str]:
-        return await self.connection.fetchval(GET_CURRENT_REVISION)  # type: ignore
+        return await self.connection.fetchval(GET_CURRENT_REVISION.format(schema=self.schema))  # type: ignore
 
     async def record_migration(
         self, from_revision: Optional[str], to_revision: Optional[str]
     ) -> None:
-        await self.connection.execute(RECORD_REVISION, from_revision, to_revision)  # type: ignore
+        await self.connection.execute(RECORD_REVISION.format(schema=self.schema), from_revision, to_revision)  # type: ignore
 
     async def execute_operation(self, operation: Operation[asyncpg.Connection]) -> None:
         await operation(self.connection)
 
 
 class AsyncpgBackend:
-    def __init__(self, connection: asyncpg.Connection) -> None:
+    def __init__(self, connection: asyncpg.Connection, schema: str = "public") -> None:
         self.connection = connection
+        self.schema = schema
 
     def connect(self) -> AsyncContextManager[AsyncpgExecutor]:
         @asynccontextmanager
         async def cm() -> AsyncIterator[AsyncpgExecutor]:
             async with self.connection.transaction(isolation="serializable"):  # type: ignore
-                yield AsyncpgExecutor(self.connection)
+                yield AsyncpgExecutor(self.connection, self.schema)
 
         return cm()
 
     def prepare_operation_from_sql_file(
         self, path: pathlib.Path
     ) -> Operation[asyncpg.Connection]:
         async def operation(connection: asyncpg.Connection) -> None:
```

### Comparing `asyncpg_trek-0.3.0/pyproject.toml` & `asyncpg_trek-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpg-trek"
-version = "0.3.0"
+version = "0.3.1"
 description = "A simple migrations system for asyncpg"
 authors = ["Adrian Garcia Badaracco <adrian@adriangb.com>"]
 readme = "README.md"
 repository = "https://github.com/adriangb/asyncpg-trek"
 documentation = "https://github.com/adriangb/asyncpg-trek"
 keywords = ["asyncpg", "postgres", "postgresql", "migrations"]
 license = "MIT"
```

### Comparing `asyncpg_trek-0.3.0/PKG-INFO` & `asyncpg_trek-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpg-trek
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple migrations system for asyncpg
 Home-page: https://github.com/adriangb/asyncpg-trek
 License: MIT
 Keywords: asyncpg,postgres,postgresql,migrations
 Author: Adrian Garcia Badaracco
 Author-email: adrian@adriangb.com
 Requires-Python: >=3.7,<4
@@ -74,9 +74,9 @@
 ```
 
 You could make this an entrypoint in a docker image, an admin endpoint in your API or a helper function in your tests (or all of the above).
 How you run your migrations depends on the complexity of your system.
 For example, for simple systems it may be easy to run migrations on app startup based on a hardcoded revision.
 For more complex systems you may want to run migrations manually or via an admin API.
 
-See this release on GitHub: [v0.3.0](https://github.com/adriangb/asyncpg-trek/releases/tag/0.3.0)
+See this release on GitHub: [v0.3.1](https://github.com/adriangb/asyncpg-trek/releases/tag/0.3.1)
```

