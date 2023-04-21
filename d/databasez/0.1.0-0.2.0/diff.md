# Comparing `tmp/databasez-0.1.0.tar.gz` & `tmp/databasez-0.2.0.tar.gz`

## Comparing `databasez-0.1.0.tar` & `databasez-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/__init__.py
--rw-r--r--   0        0        0    21451 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/core.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/importer.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/interfaces.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/py.typed
--rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/testclient.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/__init__.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/aiopg.py
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/asyncmy.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/mssql.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/mysql.py
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/postgres.py
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/common/__init__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/common/records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/compilers/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/compilers/psycopg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/dialects/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.1.0/databasez/backends/dialects/psycopg.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 databasez-0.1.0/README.md
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 databasez-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 databasez-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/__init__.py
+-rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/core.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/importer.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/interfaces.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/py.typed
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/testclient.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/__init__.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/aiopg.py
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/asyncmy.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/mssql.py
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/mysql.py
+-rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/postgres.py
+-rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/common/__init__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/common/records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/compilers/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/compilers/psycopg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/dialects/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.2.0/databasez/backends/dialects/psycopg.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.2.0/README.md
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 databasez-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10747 2020-02-02 00:00:00.000000 databasez-0.2.0/PKG-INFO
```

### Comparing `databasez-0.1.0/databasez/core.py` & `databasez-0.2.0/databasez/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import typing
 from contextvars import ContextVar
 from types import TracebackType
 from urllib.parse import SplitResult, parse_qsl, unquote, urlencode, urlsplit
 
 from sqlalchemy import text
 from sqlalchemy.sql import ClauseElement
+from sqlalchemy.util._concurrency_py3k import greenlet_spawn
 
 from databasez.importer import import_from_string
 from databasez.interfaces import DatabaseBackend, Record
 
 if typing.TYPE_CHECKING:
     from databasez.types import DictAny
 
@@ -393,14 +394,19 @@
 
         return Transaction(connection_callable, force_rollback, **kwargs)
 
     @property
     def raw_connection(self) -> typing.Any:
         return self._connection.raw_connection
 
+    async def run_sync(
+        self, fn: typing.Callable[..., typing.Any], *arg: typing.Any, **kw: typing.Any
+    ) -> typing.Any:
+        return await greenlet_spawn(fn, self._connection.raw_connection, *arg, **kw)
+
     @staticmethod
     def _build_query(
         query: typing.Union[ClauseElement, str], values: typing.Optional[dict] = None
     ) -> ClauseElement:
         if isinstance(query, str):
             query = text(query)
```

### Comparing `databasez-0.1.0/databasez/importer.py` & `databasez-0.2.0/databasez/importer.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/interfaces.py` & `databasez-0.2.0/databasez/interfaces.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/testclient.py` & `databasez-0.2.0/databasez/testclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import asyncio
 import os
 import typing
 from typing import Any
 
+import nest_asyncio
 import sqlalchemy as sa
 from sqlalchemy.exc import OperationalError, ProgrammingError
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy_utils.functions.database import _set_url_database, _sqlite_file_exists, make_url
 from sqlalchemy_utils.functions.orm import quote
 
 from databasez import Database, DatabaseURL
 
+nest_asyncio.apply()
+
 
 async def _get_scalar_result(engine: typing.Any, sql: typing.Any) -> Any:
     try:
         async with engine.connect() as conn:
             return await conn.scalar(sql)
     except Exception:
         return False
```

### Comparing `databasez-0.1.0/databasez/backends/aiopg.py` & `databasez-0.2.0/databasez/backends/aiopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/asyncmy.py` & `databasez-0.2.0/databasez/backends/asyncmy.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/mssql.py` & `databasez-0.2.0/databasez/backends/mssql.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/mysql.py` & `databasez-0.2.0/databasez/backends/mysql.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/postgres.py` & `databasez-0.2.0/databasez/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/sqlite.py` & `databasez-0.2.0/databasez/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/common/records.py` & `databasez-0.2.0/databasez/backends/common/records.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/databasez/backends/dialects/psycopg.py` & `databasez-0.2.0/databasez/backends/dialects/psycopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/LICENSE.md` & `databasez-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databasez-0.1.0/README.md` & `databasez-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 **Databasez**.
 
 This package is 100% backwards compatible with [Databases](https://github.com/encode/databases/)
 from Encode and will remain like this for the time being but adding extra features and regular
 updates as well as continuing to be community driven.
 
 By the time this project was created, Databases was yet to merge possible SQLAlchemy 2.0 changes
-from the author of this package and therefore, this package aims to have that done and unblock
+from the author of this package and therefore, this package aims to unblock
 a lot of the projects out there that want SQLAlchemy 2.0 with the best of databases with new features.
 
 A lot of packages depends of Databases and this was the main reason for the fork of **Databasez**.
 The need of progressing.
 
 It allows you to make queries using the powerful [SQLAlchemy Core][sqlalchemy-core]
 expression language, and provides support for PostgreSQL, MySQL, SQLite and MSSQL.
@@ -177,15 +177,15 @@
 # Run a database query.
 query = "SELECT * FROM HighScores"
 rows = await database.fetch_all(query=query)
 
 print("High Scores:", rows)
 ```
 
-Check out the documentation on [making database queries](https://www.encode.io/databases/database_queries/)
+Check out the documentation on [making database queries](https://databasez.tarsild.io/queries/)
 for examples of how to start using databases together with SQLAlchemy core expressions.
 
 
 [sqlalchemy-core]: https://docs.sqlalchemy.org/en/latest/core/
 [sqlalchemy-core-tutorial]: https://docs.sqlalchemy.org/en/latest/core/tutorial.html
 [alembic]: https://alembic.sqlalchemy.org/en/latest/
 [psycopg2]: https://www.psycopg.org/
@@ -201,8 +201,8 @@
 [esmerald]: https://github.com/dymmond/esmerald
 [starlette]: https://github.com/encode/starlette
 [sanic]: https://github.com/huge-success/sanic
 [responder]: https://github.com/kennethreitz/responder
 [quart]: https://gitlab.com/pgjones/quart
 [aiohttp]: https://github.com/aio-libs/aiohttp
 [tornado]: https://github.com/tornadoweb/tornado
-[fastapi]: https://github.com/tiangolo/fastapi
+[fastapi]: https://github.com/tiangolo/fastapi
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 and adding extra features common and useful to the many, [Databases](https://
 github.com/encode/databases/) was forked to become **Databasez**. This package
 is 100% backwards compatible with [Databases](https://github.com/encode/
 databases/) from Encode and will remain like this for the time being but adding
 extra features and regular updates as well as continuing to be community
 driven. By the time this project was created, Databases was yet to merge
 possible SQLAlchemy 2.0 changes from the author of this package and therefore,
-this package aims to have that done and unblock a lot of the projects out there
-that want SQLAlchemy 2.0 with the best of databases with new features. A lot of
-packages depends of Databases and this was the main reason for the fork of
+this package aims to unblock a lot of the projects out there that want
+SQLAlchemy 2.0 with the best of databases with new features. A lot of packages
+depends of Databases and this was the main reason for the fork of
 **Databasez**. The need of progressing. It allows you to make queries using the
 powerful [SQLAlchemy Core][sqlalchemy-core] expression language, and provides
 support for PostgreSQL, MySQL, SQLite and MSSQL. Databasez is suitable for
 integrating against any async Web framework, such as [Esmerald][esmerald],
 [Starlette][starlette], [Sanic][sanic], [Responder][responder], [Quart][quart],
 [aiohttp][aiohttp], [Tornado][tornado], or [FastAPI][fastapi]. Databasez was
 built for Python 3.8+ and on the top of the newest **SQLAlchemy 2** and gives
@@ -57,23 +57,23 @@
 (id INTEGER PRIMARY KEY, name VARCHAR(100), score INTEGER)""" await
 database.execute(query=query) # Insert some data. query = "INSERT INTO
 HighScores(name, score) VALUES (:name, :score)" values = [ {"name": "Daisy",
 "score": 92}, {"name": "Neil", "score": 87}, {"name": "Carol", "score": 43}, ]
 await database.execute_many(query=query, values=values) # Run a database query.
 query = "SELECT * FROM HighScores" rows = await database.fetch_all(query=query)
 print("High Scores:", rows) ``` Check out the documentation on [making database
-queries](https://www.encode.io/databases/database_queries/) for examples of how
-to start using databases together with SQLAlchemy core expressions.
-[sqlalchemy-core]: https://docs.sqlalchemy.org/en/latest/core/ [sqlalchemy-
-core-tutorial]: https://docs.sqlalchemy.org/en/latest/core/tutorial.html
-[alembic]: https://alembic.sqlalchemy.org/en/latest/ [psycopg2]: https://
-www.psycopg.org/ [pymysql]: https://github.com/PyMySQL/PyMySQL [pyodbc]: https:
-//github.com/mkleehammer/pyodbc [asyncpg]: https://github.com/MagicStack/
-asyncpg [aiopg]: https://github.com/aio-libs/aiopg [aiomysql]: https://
-github.com/aio-libs/aiomysql [asyncmy]: https://github.com/long2ice/asyncmy
-[aiosqlite]: https://github.com/omnilib/aiosqlite [aioodbc]: https://
-aioodbc.readthedocs.io/en/latest/ [esmerald]: https://github.com/dymmond/
-esmerald [starlette]: https://github.com/encode/starlette [sanic]: https://
-github.com/huge-success/sanic [responder]: https://github.com/kennethreitz/
-responder [quart]: https://gitlab.com/pgjones/quart [aiohttp]: https://
-github.com/aio-libs/aiohttp [tornado]: https://github.com/tornadoweb/tornado
-[fastapi]: https://github.com/tiangolo/fastapi
+queries](https://databasez.tarsild.io/queries/) for examples of how to start
+using databases together with SQLAlchemy core expressions. [sqlalchemy-core]:
+https://docs.sqlalchemy.org/en/latest/core/ [sqlalchemy-core-tutorial]: https:/
+/docs.sqlalchemy.org/en/latest/core/tutorial.html [alembic]: https://
+alembic.sqlalchemy.org/en/latest/ [psycopg2]: https://www.psycopg.org/
+[pymysql]: https://github.com/PyMySQL/PyMySQL [pyodbc]: https://github.com/
+mkleehammer/pyodbc [asyncpg]: https://github.com/MagicStack/asyncpg [aiopg]:
+https://github.com/aio-libs/aiopg [aiomysql]: https://github.com/aio-libs/
+aiomysql [asyncmy]: https://github.com/long2ice/asyncmy [aiosqlite]: https://
+github.com/omnilib/aiosqlite [aioodbc]: https://aioodbc.readthedocs.io/en/
+latest/ [esmerald]: https://github.com/dymmond/esmerald [starlette]: https://
+github.com/encode/starlette [sanic]: https://github.com/huge-success/sanic
+[responder]: https://github.com/kennethreitz/responder [quart]: https://
+gitlab.com/pgjones/quart [aiohttp]: https://github.com/aio-libs/aiohttp
+[tornado]: https://github.com/tornadoweb/tornado [fastapi]: https://github.com/
+tiangolo/fastapi
```

### Comparing `databasez-0.1.0/pyproject.toml` & `databasez-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["sqlalchemy>=2.0.8,<2.0.10"]
+dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.9,<2.1"]
 keywords = [
     "mysql",
     "postgres",
     "sqlalchemy",
     "sqlite",
     "asyncio",
     "esmerald",
@@ -53,15 +53,15 @@
 Documentation = "https://databasez.dymmond.com/"
 Changelog = "https://databasez.dymmond.com/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/dymmond/databasez"
 
 [project.optional-dependencies]
 test = [
-    "autoflake>=2.0.2,<3.0.0",
+    "autoflake>=2.1.1,<3.0.0",
     "black>=23.3.0,<24.0.0",
     "esmerald>=1.1.0",
     "isort>=5.12.0,<6.0.0",
     "mypy>=1.1.0,<2.0.0",
     "pytest>=7.2.2,<8.0.0",
     "pytest-cov>=4.0.0,<5.0.0",
     "starlette>=0.26.1",
@@ -74,14 +74,15 @@
 dev = [
     "asyncmy>=0.2.7,<0.3.0",
     "aiopg>=1.4.0,<2.0.0",
     "aiomysql>=0.1.1,<0.2.0",
     "aiosqlite>=0.18.0,<0.20.0",
     "asyncpg>=0.27.0,<0.30.0",
     "aioodbc>=0.4.0,<0.5.0",
+    "pre-commit>=2.17.0,<4.0.0",
     "psycopg2-binary>=2.9.6,<3.0.0",
     "pymysql>=1.0.3,<2.0.0",
     "pyodbc>=4.0.35,<5.0.0",
 ]
 
 doc = [
     "mkautodoc>=0.2.0,<0.3.0",
```

### Comparing `databasez-0.1.0/PKG-INFO` & `databasez-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6461 7461  : 2.1.Name: data
 00000020: 6261 7365 7a0a 5665 7273 696f 6e3a 2030  basez.Version: 0
-00000030: 2e31 2e30 0a53 756d 6d61 7279 3a20 4173  .1.0.Summary: As
+00000030: 2e32 2e30 0a53 756d 6d61 7279 3a20 4173  .2.0.Summary: As
 00000040: 796e 6320 6461 7461 6261 7365 2073 7570  ync database sup
 00000050: 706f 7274 2066 6f72 2050 7974 686f 6e2e  port for Python.
 00000060: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
 00000070: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
 00000080: 6769 7468 7562 2e63 6f6d 2f64 796d 6d6f  github.com/dymmo
 00000090: 6e64 2f64 6174 6162 6173 657a 0a50 726f  nd/databasez.Pro
 000000a0: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
@@ -104,565 +104,569 @@
 00000670: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
 00000680: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
 00000690: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
 000006a0: 6f64 756c 6573 0a43 6c61 7373 6966 6965  odules.Classifie
 000006b0: 723a 2054 7970 696e 6720 3a3a 2054 7970  r: Typing :: Typ
 000006c0: 6564 0a52 6571 7569 7265 732d 5079 7468  ed.Requires-Pyth
 000006d0: 6f6e 3a20 3e3d 332e 380a 5265 7175 6972  on: >=3.8.Requir
-000006e0: 6573 2d44 6973 743a 2073 716c 616c 6368  es-Dist: sqlalch
-000006f0: 656d 793c 322e 302e 3130 2c3e 3d32 2e30  emy<2.0.10,>=2.0
-00000700: 2e38 0a50 726f 7669 6465 732d 4578 7472  .8.Provides-Extr
-00000710: 613a 2061 696f 6d79 7371 6c0a 5265 7175  a: aiomysql.Requ
-00000720: 6972 6573 2d44 6973 743a 2061 696f 6d79  ires-Dist: aiomy
-00000730: 7371 6c3b 2065 7874 7261 203d 3d20 2761  sql; extra == 'a
-00000740: 696f 6d79 7371 6c27 0a50 726f 7669 6465  iomysql'.Provide
-00000750: 732d 4578 7472 613a 2061 696f 6f64 6263  s-Extra: aioodbc
-00000760: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000770: 6169 6f6f 6462 633b 2065 7874 7261 203d  aioodbc; extra =
-00000780: 3d20 2761 696f 6f64 6263 270a 5072 6f76  = 'aioodbc'.Prov
-00000790: 6964 6573 2d45 7874 7261 3a20 6169 6f70  ides-Extra: aiop
-000007a0: 670a 5265 7175 6972 6573 2d44 6973 743a  g.Requires-Dist:
-000007b0: 2061 696f 7067 3b20 6578 7472 6120 3d3d   aiopg; extra ==
-000007c0: 2027 6169 6f70 6727 0a50 726f 7669 6465   'aiopg'.Provide
-000007d0: 732d 4578 7472 613a 2061 696f 7371 6c69  s-Extra: aiosqli
-000007e0: 7465 0a52 6571 7569 7265 732d 4469 7374  te.Requires-Dist
-000007f0: 3a20 6169 6f73 716c 6974 653b 2065 7874  : aiosqlite; ext
-00000800: 7261 203d 3d20 2761 696f 7371 6c69 7465  ra == 'aiosqlite
-00000810: 270a 5072 6f76 6964 6573 2d45 7874 7261  '.Provides-Extra
-00000820: 3a20 6173 796e 636d 790a 5265 7175 6972  : asyncmy.Requir
-00000830: 6573 2d44 6973 743a 2061 7379 6e63 6d79  es-Dist: asyncmy
-00000840: 3b20 6578 7472 6120 3d3d 2027 6173 796e  ; extra == 'asyn
-00000850: 636d 7927 0a50 726f 7669 6465 732d 4578  cmy'.Provides-Ex
-00000860: 7472 613a 2061 7379 6e63 7067 0a52 6571  tra: asyncpg.Req
-00000870: 7569 7265 732d 4469 7374 3a20 6173 796e  uires-Dist: asyn
-00000880: 6370 673b 2065 7874 7261 203d 3d20 2761  cpg; extra == 'a
-00000890: 7379 6e63 7067 270a 5072 6f76 6964 6573  syncpg'.Provides
-000008a0: 2d45 7874 7261 3a20 6465 760a 5265 7175  -Extra: dev.Requ
-000008b0: 6972 6573 2d44 6973 743a 2061 696f 6d79  ires-Dist: aiomy
-000008c0: 7371 6c3c 302e 322e 302c 3e3d 302e 312e  sql<0.2.0,>=0.1.
-000008d0: 313b 2065 7874 7261 203d 3d20 2764 6576  1; extra == 'dev
-000008e0: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-000008f0: 2061 696f 6f64 6263 3c30 2e35 2e30 2c3e   aioodbc<0.5.0,>
-00000900: 3d30 2e34 2e30 3b20 6578 7472 6120 3d3d  =0.4.0; extra ==
-00000910: 2027 6465 7627 0a52 6571 7569 7265 732d   'dev'.Requires-
-00000920: 4469 7374 3a20 6169 6f70 673c 322e 302e  Dist: aiopg<2.0.
-00000930: 302c 3e3d 312e 342e 303b 2065 7874 7261  0,>=1.4.0; extra
-00000940: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
-00000950: 6573 2d44 6973 743a 2061 696f 7371 6c69  es-Dist: aiosqli
-00000960: 7465 3c30 2e32 302e 302c 3e3d 302e 3138  te<0.20.0,>=0.18
-00000970: 2e30 3b20 6578 7472 6120 3d3d 2027 6465  .0; extra == 'de
-00000980: 7627 0a52 6571 7569 7265 732d 4469 7374  v'.Requires-Dist
-00000990: 3a20 6173 796e 636d 793c 302e 332e 302c  : asyncmy<0.3.0,
-000009a0: 3e3d 302e 322e 373b 2065 7874 7261 203d  >=0.2.7; extra =
-000009b0: 3d20 2764 6576 270a 5265 7175 6972 6573  = 'dev'.Requires
-000009c0: 2d44 6973 743a 2061 7379 6e63 7067 3c30  -Dist: asyncpg<0
-000009d0: 2e33 302e 302c 3e3d 302e 3237 2e30 3b20  .30.0,>=0.27.0; 
-000009e0: 6578 7472 6120 3d3d 2027 6465 7627 0a52  extra == 'dev'.R
-000009f0: 6571 7569 7265 732d 4469 7374 3a20 7073  equires-Dist: ps
-00000a00: 7963 6f70 6732 2d62 696e 6172 793c 332e  ycopg2-binary<3.
-00000a10: 302e 302c 3e3d 322e 392e 363b 2065 7874  0.0,>=2.9.6; ext
-00000a20: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
-00000a30: 6972 6573 2d44 6973 743a 2070 796d 7973  ires-Dist: pymys
-00000a40: 716c 3c32 2e30 2e30 2c3e 3d31 2e30 2e33  ql<2.0.0,>=1.0.3
-00000a50: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
-00000a60: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a70: 7079 6f64 6263 3c35 2e30 2e30 2c3e 3d34  pyodbc<5.0.0,>=4
-00000a80: 2e30 2e33 353b 2065 7874 7261 203d 3d20  .0.35; extra == 
-00000a90: 2764 6576 270a 5072 6f76 6964 6573 2d45  'dev'.Provides-E
-00000aa0: 7874 7261 3a20 646f 630a 5265 7175 6972  xtra: doc.Requir
-00000ab0: 6573 2d44 6973 743a 206d 6478 2d69 6e63  es-Dist: mdx-inc
-00000ac0: 6c75 6465 3c32 2e30 2e30 2c3e 3d31 2e34  lude<2.0.0,>=1.4
-00000ad0: 2e31 3b20 6578 7472 6120 3d3d 2027 646f  .1; extra == 'do
-00000ae0: 6327 0a52 6571 7569 7265 732d 4469 7374  c'.Requires-Dist
-00000af0: 3a20 6d6b 6175 746f 646f 633c 302e 332e  : mkautodoc<0.3.
-00000b00: 302c 3e3d 302e 322e 303b 2065 7874 7261  0,>=0.2.0; extra
-00000b10: 203d 3d20 2764 6f63 270a 5265 7175 6972   == 'doc'.Requir
-00000b20: 6573 2d44 6973 743a 206d 6b64 6f63 732d  es-Dist: mkdocs-
-00000b30: 6d61 726b 646f 776e 6578 7472 6164 6174  markdownextradat
-00000b40: 612d 706c 7567 696e 3c30 2e33 2e30 2c3e  a-plugin<0.3.0,>
-00000b50: 3d30 2e31 2e37 3b20 6578 7472 6120 3d3d  =0.1.7; extra ==
-00000b60: 2027 646f 6327 0a52 6571 7569 7265 732d   'doc'.Requires-
-00000b70: 4469 7374 3a20 6d6b 646f 6373 2d6d 6174  Dist: mkdocs-mat
-00000b80: 6572 6961 6c3d 3d39 2e31 2e35 3b20 6578  erial==9.1.5; ex
-00000b90: 7472 6120 3d3d 2027 646f 6327 0a52 6571  tra == 'doc'.Req
-00000ba0: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
-00000bb0: 6373 3c32 2e30 2e30 2c3e 3d31 2e34 2e32  cs<2.0.0,>=1.4.2
-00000bc0: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
-00000bd0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000be0: 6d6b 646f 6373 7472 696e 6773 3c30 2e32  mkdocstrings<0.2
-00000bf0: 312e 302c 3e3d 302e 3139 2e30 3b20 6578  1.0,>=0.19.0; ex
-00000c00: 7472 6120 3d3d 2027 646f 6327 0a52 6571  tra == 'doc'.Req
-00000c10: 7569 7265 732d 4469 7374 3a20 7079 7961  uires-Dist: pyya
-00000c20: 6d6c 3c37 2e30 2e30 2c3e 3d35 2e33 2e31  ml<7.0.0,>=5.3.1
-00000c30: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
-00000c40: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c50: 206d 7973 716c 0a52 6571 7569 7265 732d   mysql.Requires-
-00000c60: 4469 7374 3a20 6169 6f6d 7973 716c 3b20  Dist: aiomysql; 
-00000c70: 6578 7472 6120 3d3d 2027 6d79 7371 6c27  extra == 'mysql'
-00000c80: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c90: 2070 6f73 7467 7265 7371 6c0a 5265 7175   postgresql.Requ
-00000ca0: 6972 6573 2d44 6973 743a 2061 7379 6e63  ires-Dist: async
-00000cb0: 7067 3b20 6578 7472 6120 3d3d 2027 706f  pg; extra == 'po
-00000cc0: 7374 6772 6573 716c 270a 5072 6f76 6964  stgresql'.Provid
-00000cd0: 6573 2d45 7874 7261 3a20 7371 6c69 7465  es-Extra: sqlite
-00000ce0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000cf0: 6169 6f73 716c 6974 653b 2065 7874 7261  aiosqlite; extra
-00000d00: 203d 3d20 2773 716c 6974 6527 0a50 726f   == 'sqlite'.Pro
-00000d10: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
-00000d20: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
-00000d30: 2061 7574 6f66 6c61 6b65 3c33 2e30 2e30   autoflake<3.0.0
-00000d40: 2c3e 3d32 2e30 2e32 3b20 6578 7472 6120  ,>=2.0.2; extra 
-00000d50: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
-00000d60: 6573 2d44 6973 743a 2062 6c61 636b 3c32  es-Dist: black<2
-00000d70: 342e 302e 302c 3e3d 3233 2e33 2e30 3b20  4.0.0,>=23.3.0; 
-00000d80: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
-00000d90: 5265 7175 6972 6573 2d44 6973 743a 2065  Requires-Dist: e
-00000da0: 736d 6572 616c 643e 3d31 2e31 2e30 3b20  smerald>=1.1.0; 
-00000db0: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
-00000dc0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
-00000dd0: 736f 7274 3c36 2e30 2e30 2c3e 3d35 2e31  sort<6.0.0,>=5.1
-00000de0: 322e 303b 2065 7874 7261 203d 3d20 2774  2.0; extra == 't
-00000df0: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
-00000e00: 7374 3a20 6d79 7079 3c32 2e30 2e30 2c3e  st: mypy<2.0.0,>
-00000e10: 3d31 2e31 2e30 3b20 6578 7472 6120 3d3d  =1.1.0; extra ==
-00000e20: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
-00000e30: 2d44 6973 743a 2070 7974 6573 742d 636f  -Dist: pytest-co
-00000e40: 763c 352e 302e 302c 3e3d 342e 302e 303b  v<5.0.0,>=4.0.0;
-00000e50: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
-00000e60: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000e70: 7079 7465 7374 3c38 2e30 2e30 2c3e 3d37  pytest<8.0.0,>=7
-00000e80: 2e32 2e32 3b20 6578 7472 6120 3d3d 2027  .2.2; extra == '
-00000e90: 7465 7374 270a 5265 7175 6972 6573 2d44  test'.Requires-D
-00000ea0: 6973 743a 2072 6571 7565 7374 733e 3d32  ist: requests>=2
-00000eb0: 2e32 382e 323b 2065 7874 7261 203d 3d20  .28.2; extra == 
-00000ec0: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
-00000ed0: 4469 7374 3a20 7275 6666 3c31 2e30 2e30  Dist: ruff<1.0.0
-00000ee0: 2c3e 3d30 2e30 2e32 3536 3b20 6578 7472  ,>=0.0.256; extr
-00000ef0: 6120 3d3d 2027 7465 7374 270a 5265 7175  a == 'test'.Requ
-00000f00: 6972 6573 2d44 6973 743a 2073 7461 726c  ires-Dist: starl
-00000f10: 6574 7465 3e3d 302e 3236 2e31 3b20 6578  ette>=0.26.1; ex
-00000f20: 7472 6120 3d3d 2027 7465 7374 270a 5072  tra == 'test'.Pr
-00000f30: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
-00000f40: 7374 696e 670a 5265 7175 6972 6573 2d44  sting.Requires-D
-00000f50: 6973 743a 2073 716c 616c 6368 656d 792d  ist: sqlalchemy-
-00000f60: 7574 696c 733e 3d30 2e34 302e 303b 2065  utils>=0.40.0; e
-00000f70: 7874 7261 203d 3d20 2774 6573 7469 6e67  xtra == 'testing
-00000f80: 270a 4465 7363 7269 7074 696f 6e2d 436f  '.Description-Co
-00000f90: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
-00000fa0: 2f6d 6172 6b64 6f77 6e0a 0a23 2044 6174  /markdown..# Dat
-00000fb0: 6162 6173 657a 0a0a 3c70 2061 6c69 676e  abasez..<p align
-00000fc0: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
-00000fd0: 6872 6566 3d22 6874 7470 733a 2f2f 6461  href="https://da
-00000fe0: 7461 6261 7365 7a2e 7461 7273 696c 642e  tabasez.tarsild.
-00000ff0: 696f 223e 3c69 6d67 2073 7263 3d22 6874  io"><img src="ht
-00001000: 7470 733a 2f2f 7265 732e 636c 6f75 6469  tps://res.cloudi
-00001010: 6e61 7279 2e63 6f6d 2f64 796d 6d6f 6e64  nary.com/dymmond
-00001020: 2f69 6d61 6765 2f75 706c 6f61 642f 7631  /image/upload/v1
-00001030: 3638 3036 3131 3632 362f 6461 7461 6261  680611626/databa
-00001040: 7365 7a2f 6c6f 676f 2d63 6d70 5f6c 7569  sez/logo-cmp_lui
-00001050: 7a62 302e 706e 6722 2061 6c74 3d27 6461  zb0.png" alt='da
-00001060: 7461 6261 7365 7a27 3e3c 2f61 3e0a 3c2f  tabasez'></a>.</
-00001070: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
-00001080: 6e74 6572 223e 0a20 2020 203c 656d 3ef0  nter">.    <em>.
-00001090: 9f9a 8020 4173 796e 6320 6461 7461 6261  ... Async databa
-000010a0: 7365 2073 7570 706f 7274 2066 6f72 2050  se support for P
-000010b0: 7974 686f 6e2e 20f0 9f9a 803c 2f65 6d3e  ython. ....</em>
-000010c0: 0a3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  .</p>..<p align=
-000010d0: 2263 656e 7465 7222 3e0a 3c61 2068 7265  "center">.<a hre
-000010e0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000010f0: 622e 636f 6d2f 7461 7273 696c 2f64 6174  b.com/tarsil/dat
-00001100: 6162 6173 657a 2f77 6f72 6b66 6c6f 7773  abasez/workflows
-00001110: 2f54 6573 7425 3230 5375 6974 652f 6261  /Test%20Suite/ba
-00001120: 6467 652e 7376 673f 6576 656e 743d 7075  dge.svg?event=pu
-00001130: 7368 2662 7261 6e63 683d 6d61 696e 2220  sh&branch=main" 
-00001140: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00001150: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
-00001160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001170: 6d2f 7461 7273 696c 2f64 6174 6162 6173  m/tarsil/databas
-00001180: 657a 2f77 6f72 6b66 6c6f 7773 2f54 6573  ez/workflows/Tes
-00001190: 7425 3230 5375 6974 652f 6261 6467 652e  t%20Suite/badge.
-000011a0: 7376 673f 6576 656e 743d 7075 7368 2662  svg?event=push&b
-000011b0: 7261 6e63 683d 6d61 696e 2220 616c 743d  ranch=main" alt=
-000011c0: 2254 6573 7420 5375 6974 6522 3e0a 3c2f  "Test Suite">.</
-000011d0: 613e 0a0a 3c61 2068 7265 663d 2268 7474  a>..<a href="htt
-000011e0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-000011f0: 6f6a 6563 742f 6461 7461 6261 7365 7a22  oject/databasez"
-00001200: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-00001210: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
-00001220: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00001230: 6c64 732e 696f 2f70 7970 692f 762f 6461  lds.io/pypi/v/da
-00001240: 7461 6261 7365 7a3f 636f 6c6f 723d 2532  tabasez?color=%2
-00001250: 3333 3444 3035 3826 6c61 6265 6c3d 7079  334D058&label=py
-00001260: 7069 2532 3070 6163 6b61 6765 2220 616c  pi%20package" al
-00001270: 743d 2250 6163 6b61 6765 2076 6572 7369  t="Package versi
-00001280: 6f6e 223e 0a3c 2f61 3e0a 0a3c 6120 6872  on">.</a>..<a hr
-00001290: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
-000012a0: 2e6f 7267 2f70 726f 6a65 6374 2f64 6174  .org/project/dat
-000012b0: 6162 6173 657a 2220 7461 7267 6574 3d22  abasez" target="
-000012c0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-000012d0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-000012e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000012f0: 7069 2f70 7976 6572 7369 6f6e 732f 6461  pi/pyversions/da
-00001300: 7461 6261 7365 7a2e 7376 673f 636f 6c6f  tabasez.svg?colo
-00001310: 723d 2532 3333 3444 3035 3822 2061 6c74  r=%2334D058" alt
-00001320: 3d22 5375 7070 6f72 7465 6420 5079 7468  ="Supported Pyth
-00001330: 6f6e 2076 6572 7369 6f6e 7322 3e0a 3c2f  on versions">.</
-00001340: 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a 2a2a  a>.</p>..---..**
-00001350: 446f 6375 6d65 6e74 6174 696f 6e2a 2a3a  Documentation**:
-00001360: 205b 6874 7470 733a 2f2f 6461 7461 6261   [https://databa
-00001370: 7365 7a2e 7461 7273 696c 642e 696f 5d28  sez.tarsild.io](
-00001380: 6874 7470 733a 2f2f 6461 7461 6261 7365  https://database
-00001390: 7a2e 7461 7273 696c 642e 696f 2920 f09f  z.tarsild.io) ..
-000013a0: 939a 0a0a 2a2a 536f 7572 6365 2043 6f64  ....**Source Cod
-000013b0: 652a 2a3a 205b 6874 7470 733a 2f2f 6769  e**: [https://gi
-000013c0: 7468 7562 2e63 6f6d 2f74 6172 7369 6c2f  thub.com/tarsil/
-000013d0: 6461 7461 6261 7365 7a5d 2868 7474 7073  databasez](https
-000013e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7461  ://github.com/ta
-000013f0: 7273 696c 2f64 6174 6162 6173 657a 290a  rsil/databasez).
-00001400: 0a2d 2d2d 0a0a 2323 204d 6f74 6976 6174  .---..## Motivat
-00001410: 696f 6e0a 0a54 6865 7265 2069 7320 6120  ion..There is a 
-00001420: 6772 6561 7420 7061 636b 6167 6520 6672  great package fr
-00001430: 6f6d 205b 456e 636f 6465 5d28 6874 7470  om [Encode](http
-00001440: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00001450: 6e63 6f64 652f 6461 7461 6261 7365 732f  ncode/databases/
-00001460: 2920 7468 6174 2077 6173 2064 6f69 6e67  ) that was doing
-00001470: 2077 6861 740a 7468 6973 2070 6163 6b61   what.this packa
-00001480: 6765 2077 6173 2069 6e69 7469 616c 6c79  ge was initially
-00001490: 2066 6f72 6b65 6420 746f 2064 6f20 6275   forked to do bu
-000014a0: 7420 456e 636f 6465 2069 7320 616c 736f  t Encode is also
-000014b0: 2076 6572 7920 6275 7379 2077 6974 6820   very busy with 
-000014c0: 6f74 6865 7220 7072 6f6a 6563 7473 2061  other projects a
-000014d0: 6e64 0a77 6974 686f 7574 2074 6865 2070  nd.without the p
-000014e0: 726f 7065 7220 7469 6d65 2074 6f20 6d61  roper time to ma
-000014f0: 696e 7461 696e 2074 6865 2073 6f20 6d75  intain the so mu
-00001500: 6368 2072 6571 7569 7265 6420 7061 636b  ch required pack
-00001510: 6167 652e 0a0a 4672 6f6d 2061 206e 6565  age...From a nee
-00001520: 6420 746f 2065 7874 656e 6420 746f 206e  d to extend to n
-00001530: 6577 2064 7269 7665 7273 2061 6e64 206e  ew drivers and n
-00001540: 6577 6573 7420 7465 6368 6e6f 6c6f 6769  ewest technologi
-00001550: 6573 2061 6e64 2061 6464 696e 6720 6578  es and adding ex
-00001560: 7472 6120 6665 6174 7572 6573 2063 6f6d  tra features com
-00001570: 6d6f 6e20 616e 640a 7573 6566 756c 2074  mon and.useful t
-00001580: 6f20 7468 6520 6d61 6e79 2c20 5b44 6174  o the many, [Dat
-00001590: 6162 6173 6573 5d28 6874 7470 733a 2f2f  abases](https://
-000015a0: 6769 7468 7562 2e63 6f6d 2f65 6e63 6f64  github.com/encod
-000015b0: 652f 6461 7461 6261 7365 732f 2920 7761  e/databases/) wa
-000015c0: 7320 666f 726b 6564 2074 6f20 6265 636f  s forked to beco
-000015d0: 6d65 0a2a 2a44 6174 6162 6173 657a 2a2a  me.**Databasez**
-000015e0: 2e0a 0a54 6869 7320 7061 636b 6167 6520  ...This package 
-000015f0: 6973 2031 3030 2520 6261 636b 7761 7264  is 100% backward
-00001600: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
-00001610: 6820 5b44 6174 6162 6173 6573 5d28 6874  h [Databases](ht
-00001620: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001630: 2f65 6e63 6f64 652f 6461 7461 6261 7365  /encode/database
-00001640: 732f 290a 6672 6f6d 2045 6e63 6f64 6520  s/).from Encode 
-00001650: 616e 6420 7769 6c6c 2072 656d 6169 6e20  and will remain 
-00001660: 6c69 6b65 2074 6869 7320 666f 7220 7468  like this for th
-00001670: 6520 7469 6d65 2062 6569 6e67 2062 7574  e time being but
-00001680: 2061 6464 696e 6720 6578 7472 6120 6665   adding extra fe
-00001690: 6174 7572 6573 2061 6e64 2072 6567 756c  atures and regul
-000016a0: 6172 0a75 7064 6174 6573 2061 7320 7765  ar.updates as we
-000016b0: 6c6c 2061 7320 636f 6e74 696e 7569 6e67  ll as continuing
-000016c0: 2074 6f20 6265 2063 6f6d 6d75 6e69 7479   to be community
-000016d0: 2064 7269 7665 6e2e 0a0a 4279 2074 6865   driven...By the
-000016e0: 2074 696d 6520 7468 6973 2070 726f 6a65   time this proje
-000016f0: 6374 2077 6173 2063 7265 6174 6564 2c20  ct was created, 
-00001700: 4461 7461 6261 7365 7320 7761 7320 7965  Databases was ye
-00001710: 7420 746f 206d 6572 6765 2070 6f73 7369  t to merge possi
-00001720: 626c 6520 5351 4c41 6c63 6865 6d79 2032  ble SQLAlchemy 2
-00001730: 2e30 2063 6861 6e67 6573 0a66 726f 6d20  .0 changes.from 
-00001740: 7468 6520 6175 7468 6f72 206f 6620 7468  the author of th
-00001750: 6973 2070 6163 6b61 6765 2061 6e64 2074  is package and t
-00001760: 6865 7265 666f 7265 2c20 7468 6973 2070  herefore, this p
-00001770: 6163 6b61 6765 2061 696d 7320 746f 2068  ackage aims to h
-00001780: 6176 6520 7468 6174 2064 6f6e 6520 616e  ave that done an
-00001790: 6420 756e 626c 6f63 6b0a 6120 6c6f 7420  d unblock.a lot 
-000017a0: 6f66 2074 6865 2070 726f 6a65 6374 7320  of the projects 
-000017b0: 6f75 7420 7468 6572 6520 7468 6174 2077  out there that w
-000017c0: 616e 7420 5351 4c41 6c63 6865 6d79 2032  ant SQLAlchemy 2
-000017d0: 2e30 2077 6974 6820 7468 6520 6265 7374  .0 with the best
-000017e0: 206f 6620 6461 7461 6261 7365 7320 7769   of databases wi
-000017f0: 7468 206e 6577 2066 6561 7475 7265 732e  th new features.
-00001800: 0a0a 4120 6c6f 7420 6f66 2070 6163 6b61  ..A lot of packa
-00001810: 6765 7320 6465 7065 6e64 7320 6f66 2044  ges depends of D
-00001820: 6174 6162 6173 6573 2061 6e64 2074 6869  atabases and thi
-00001830: 7320 7761 7320 7468 6520 6d61 696e 2072  s was the main r
-00001840: 6561 736f 6e20 666f 7220 7468 6520 666f  eason for the fo
-00001850: 726b 206f 6620 2a2a 4461 7461 6261 7365  rk of **Database
-00001860: 7a2a 2a2e 0a54 6865 206e 6565 6420 6f66  z**..The need of
-00001870: 2070 726f 6772 6573 7369 6e67 2e0a 0a49   progressing...I
-00001880: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
-00001890: 6d61 6b65 2071 7565 7269 6573 2075 7369  make queries usi
-000018a0: 6e67 2074 6865 2070 6f77 6572 6675 6c20  ng the powerful 
-000018b0: 5b53 514c 416c 6368 656d 7920 436f 7265  [SQLAlchemy Core
-000018c0: 5d5b 7371 6c61 6c63 6865 6d79 2d63 6f72  ][sqlalchemy-cor
-000018d0: 655d 0a65 7870 7265 7373 696f 6e20 6c61  e].expression la
-000018e0: 6e67 7561 6765 2c20 616e 6420 7072 6f76  nguage, and prov
-000018f0: 6964 6573 2073 7570 706f 7274 2066 6f72  ides support for
-00001900: 2050 6f73 7467 7265 5351 4c2c 204d 7953   PostgreSQL, MyS
-00001910: 514c 2c20 5351 4c69 7465 2061 6e64 204d  QL, SQLite and M
-00001920: 5353 514c 2e0a 0a44 6174 6162 6173 657a  SSQL...Databasez
-00001930: 2069 7320 7375 6974 6162 6c65 2066 6f72   is suitable for
-00001940: 2069 6e74 6567 7261 7469 6e67 2061 6761   integrating aga
-00001950: 696e 7374 2061 6e79 2061 7379 6e63 2057  inst any async W
-00001960: 6562 2066 7261 6d65 776f 726b 2c20 7375  eb framework, su
-00001970: 6368 2061 7320 5b45 736d 6572 616c 645d  ch as [Esmerald]
-00001980: 5b65 736d 6572 616c 645d 2c0a 5b53 7461  [esmerald],.[Sta
-00001990: 726c 6574 7465 5d5b 7374 6172 6c65 7474  rlette][starlett
-000019a0: 655d 2c20 5b53 616e 6963 5d5b 7361 6e69  e], [Sanic][sani
-000019b0: 635d 2c20 5b52 6573 706f 6e64 6572 5d5b  c], [Responder][
-000019c0: 7265 7370 6f6e 6465 725d 2c20 5b51 7561  responder], [Qua
-000019d0: 7274 5d5b 7175 6172 745d 2c20 5b61 696f  rt][quart], [aio
-000019e0: 6874 7470 5d5b 6169 6f68 7474 705d 2c0a  http][aiohttp],.
-000019f0: 5b54 6f72 6e61 646f 5d5b 746f 726e 6164  [Tornado][tornad
-00001a00: 6f5d 2c20 6f72 205b 4661 7374 4150 495d  o], or [FastAPI]
-00001a10: 5b66 6173 7461 7069 5d2e 0a0a 4461 7461  [fastapi]...Data
-00001a20: 6261 7365 7a20 7761 7320 6275 696c 7420  basez was built 
-00001a30: 666f 7220 5079 7468 6f6e 2033 2e38 2b20  for Python 3.8+ 
-00001a40: 616e 6420 6f6e 2074 6865 2074 6f70 206f  and on the top o
-00001a50: 6620 7468 6520 6e65 7765 7374 202a 2a53  f the newest **S
-00001a60: 514c 416c 6368 656d 7920 322a 2a20 616e  QLAlchemy 2** an
-00001a70: 6420 6769 7665 7320 796f 750a 7369 6d70  d gives you.simp
-00001a80: 6c65 2061 7379 6e63 696f 2073 7570 706f  le asyncio suppo
-00001a90: 7274 2066 6f72 2061 2072 616e 6765 206f  rt for a range o
-00001aa0: 6620 6461 7461 6261 7365 732e 0a0a 2323  f databases...##
-00001ab0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
-00001ac0: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
-00001ad0: 7374 616c 6c20 6461 7461 6261 7365 7a0a  stall databasez.
-00001ae0: 6060 600a 0a49 6620 796f 7520 6172 6520  ```..If you are 
-00001af0: 696e 7465 7265 7374 6564 2069 6e20 7573  interested in us
-00001b00: 696e 6720 7468 6520 5b74 6573 7420 636c  ing the [test cl
-00001b10: 6965 6e74 5d28 2e2f 7465 7374 2d63 6c69  ient](./test-cli
-00001b20: 656e 742e 6d64 292c 2079 6f75 2063 616e  ent.md), you can
-00001b30: 2061 6c73 6f20 696e 7374 616c 6c3a 0a0a   also install:..
-00001b40: 6060 6073 6865 6c6c 0a24 2070 6970 2069  ```shell.$ pip i
-00001b50: 6e73 7461 6c6c 2064 6174 6162 6173 657a  nstall databasez
-00001b60: 5b74 6573 7469 6e67 5d0a 6060 600a 0a23  [testing].```..#
-00001b70: 2320 5768 6174 2064 6f65 7320 6461 7461  # What does data
-00001b80: 6261 7365 7a20 7375 7070 6f72 7420 6174  basez support at
-00001b90: 2074 6865 206d 6f6d 656e 740a 0a44 6174   the moment..Dat
-00001ba0: 6162 6173 657a 2063 7572 7265 6e74 6c79  abasez currently
-00001bb0: 2073 7570 706f 7274 7320 6073 716c 6974   supports `sqlit
-00001bc0: 6560 2c20 6070 6f73 7467 7265 7360 2c20  e`, `postgres`, 
-00001bd0: 606d 7973 716c 6020 616e 6420 6073 716c  `mysql` and `sql
-00001be0: 2073 6572 7665 7260 2e20 4d6f 7265 2064   server`. More d
-00001bf0: 7269 7665 7273 2063 616e 2061 6e64 0a77  rivers can and.w
-00001c00: 696c 6c20 6265 2061 6464 6564 2069 6e20  ill be added in 
-00001c10: 7468 6520 6675 7475 7265 2e0a 0a44 6174  the future...Dat
-00001c20: 6162 6173 6520 6472 6976 6572 7320 7375  abase drivers su
-00001c30: 7070 6f72 7465 6420 6172 653a 0a0a 2a20  pported are:..* 
-00001c40: 5b61 7379 6e63 7067 5d5b 6173 796e 6370  [asyncpg][asyncp
-00001c50: 675d 202d 2046 6f72 2070 6f73 7467 7265  g] - For postgre
-00001c60: 732e 0a2a 205b 6169 6f70 675d 5b61 696f  s..* [aiopg][aio
-00001c70: 7067 5d20 2d20 466f 7220 706f 7374 6772  pg] - For postgr
-00001c80: 6573 2e0a 2a20 5b61 696f 6d79 7371 6c5d  es..* [aiomysql]
-00001c90: 5b61 696f 6d79 7371 6c5d 202d 2046 6f72  [aiomysql] - For
-00001ca0: 204d 7953 514c 2f4d 6172 6961 4442 2e0a   MySQL/MariaDB..
-00001cb0: 2a20 5b61 7379 6e63 6d79 5d5b 6173 796e  * [asyncmy][asyn
-00001cc0: 636d 795d 202d 2046 6f72 204d 7953 514c  cmy] - For MySQL
-00001cd0: 2f4d 6172 6961 4442 2e0a 2a20 5b61 696f  /MariaDB..* [aio
-00001ce0: 7371 6c69 7465 5d5b 6169 6f73 716c 6974  sqlite][aiosqlit
-00001cf0: 655d 202d 2046 6f72 2053 514c 6974 652e  e] - For SQLite.
-00001d00: 0a2a 205b 6169 6f6f 6462 635d 5b61 696f  .* [aioodbc][aio
-00001d10: 6f64 6263 5d20 2d20 466f 7220 4d53 5351  odbc] - For MSSQ
-00001d20: 4c20 2853 514c 2053 6572 7665 7229 2e0a  L (SQL Server)..
-00001d30: 0a23 2323 2044 7269 7665 7220 696e 7374  .### Driver inst
-00001d40: 616c 6c61 7469 6f6e 0a0a 596f 7520 6361  allation..You ca
-00001d50: 6e20 696e 7374 616c 6c20 7468 6520 7265  n install the re
-00001d60: 7175 6972 6564 2064 6174 6162 6173 6520  quired database 
-00001d70: 6472 6976 6572 7320 7769 7468 3a0a 0a23  drivers with:..#
-00001d80: 2323 2320 506f 7374 6772 6573 0a0a 6060  ### Postgres..``
-00001d90: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
-00001da0: 7461 6c6c 2064 6174 6162 6173 657a 5b61  tall databasez[a
-00001db0: 7379 6e63 7067 5d0a 6060 600a 0a6f 720a  syncpg].```..or.
-00001dc0: 0a60 6060 7368 656c 6c0a 2420 7069 7020  .```shell.$ pip 
-00001dd0: 696e 7374 616c 6c20 6461 7461 6261 7365  install database
-00001de0: 7a5b 6169 6f70 675d 0a60 6060 0a0a 2323  z[aiopg].```..##
-00001df0: 2323 204d 7953 514c 2f4d 6172 6961 4442  ## MySQL/MariaDB
-00001e00: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
-00001e10: 2069 6e73 7461 6c6c 2064 6174 6162 6173   install databas
-00001e20: 657a 5b61 696f 6d79 7371 6c5d 0a60 6060  ez[aiomysql].```
-00001e30: 0a0a 6f72 0a0a 6060 6073 6865 6c6c 0a24  ..or..```shell.$
-00001e40: 2070 6970 2069 6e73 7461 6c6c 2064 6174   pip install dat
-00001e50: 6162 6173 657a 5b61 7379 6e63 6d79 5d0a  abasez[asyncmy].
-00001e60: 6060 600a 0a23 2323 2320 5351 4c69 7465  ```..#### SQLite
-00001e70: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
-00001e80: 2069 6e73 7461 6c6c 2064 6174 6162 6173   install databas
-00001e90: 657a 5b61 696f 7371 6c69 7465 5d0a 6060  ez[aiosqlite].``
-00001ea0: 600a 0a23 2323 2320 4d53 5351 4c0a 0a60  `..#### MSSQL..`
-00001eb0: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
-00001ec0: 7374 616c 6c20 6461 7461 6261 7365 7a5b  stall databasez[
-00001ed0: 6169 6f6f 6462 635d 0a60 6060 0a0a 2121  aioodbc].```..!!
-00001ee0: 2120 4e6f 7465 0a20 2020 204e 6f74 6520  ! Note.    Note 
-00001ef0: 7468 6174 2069 6620 796f 7520 6172 6520  that if you are 
-00001f00: 7573 696e 6720 616e 7920 7379 6e63 6872  using any synchr
-00001f10: 6f6e 6f75 7320 5351 4c41 6c63 6865 6d79  onous SQLAlchemy
-00001f20: 2066 756e 6374 696f 6e73 2073 7563 6820   functions such 
-00001f30: 6173 2060 656e 6769 6e65 2e63 7265 6174  as `engine.creat
-00001f40: 655f 616c 6c28 2960 0a20 2020 206f 7220  e_all()`.    or 
-00001f50: 5b61 6c65 6d62 6963 5d5b 616c 656d 6269  [alembic][alembi
-00001f60: 635d 206d 6967 7261 7469 6f6e 7320 7468  c] migrations th
-00001f70: 656e 2079 6f75 2073 7469 6c6c 2068 6176  en you still hav
-00001f80: 6520 746f 2069 6e73 7461 6c6c 2061 2073  e to install a s
-00001f90: 796e 6368 726f 6e6f 7573 2044 4220 6472  ynchronous DB dr
-00001fa0: 6976 6572 3a0a 2020 2020 5b70 7379 636f  iver:.    [psyco
-00001fb0: 7067 325d 5b70 7379 636f 7067 325d 2066  pg2][psycopg2] f
-00001fc0: 6f72 2050 6f73 7467 7265 5351 4c2c 205b  or PostgreSQL, [
-00001fd0: 7079 6d79 7371 6c5d 5b70 796d 7973 716c  pymysql][pymysql
-00001fe0: 5d20 666f 7220 4d79 5351 4c20 616e 640a  ] for MySQL and.
-00001ff0: 2020 2020 5b70 796f 6462 635d 5b70 796f      [pyodbc][pyo
-00002000: 6462 635d 2066 6f72 2053 514c 2053 6572  dbc] for SQL Ser
-00002010: 7665 722e 0a0a 2d2d 2d0a 0a23 2320 5175  ver...---..## Qu
-00002020: 6963 6b73 7461 7274 0a0a 466f 7220 6120  ickstart..For a 
-00002030: 7369 6d70 6c65 2071 7569 636b 7374 6172  simple quickstar
-00002040: 7420 6578 616d 706c 652c 2077 6520 7769  t example, we wi
-00002050: 6c6c 2062 6520 6372 6561 7469 6e67 2061  ll be creating a
-00002060: 2073 696d 706c 6520 5351 4c69 7465 2064   simple SQLite d
-00002070: 6174 6162 6173 6520 746f 2072 756e 2073  atabase to run s
-00002080: 6f6d 6520 7175 6572 6965 730a 6167 6169  ome queries.agai
-00002090: 6e73 742e 0a0a 4669 7273 742c 2069 6e73  nst...First, ins
-000020a0: 7461 6c6c 2074 6865 2072 6571 7569 7265  tall the require
-000020b0: 6420 6472 6976 6572 7320 666f 7220 6053  d drivers for `S
-000020c0: 514c 6974 6560 2061 6e64 2060 6970 7974  QLite` and `ipyt
-000020d0: 686f 6e60 2e20 5468 6520 6069 7079 7468  hon`. The `ipyth
-000020e0: 6f6e 6020 6973 2074 6f20 6861 7665 2061  on` is to have a
-000020f0: 6e0a 696e 7465 7261 6374 6976 6520 7079  n.interactive py
-00002100: 7468 6f6e 2073 6865 6c6c 2077 6974 6820  thon shell with 
-00002110: 736f 6d65 2065 7874 7261 732e 2049 5079  some extras. IPy
-00002120: 7468 6f6e 2061 6c73 6f20 7375 7070 6f72  thon also suppor
-00002130: 7473 2060 6177 6169 7460 2c20 7768 6963  ts `await`, whic
-00002140: 6820 6973 2065 7861 6374 6c79 0a77 6861  h is exactly.wha
-00002150: 7420 7765 206e 6565 642e 205b 5365 6520  t we need. [See 
-00002160: 6d6f 7265 2064 6574 6169 6c73 5d28 6874  more details](ht
-00002170: 7470 733a 2f2f 6970 7974 686f 6e2e 6f72  tps://ipython.or
-00002180: 672f 2920 6162 6f75 7420 6974 2e0a 0a2a  g/) about it...*
-00002190: 2a49 6e73 7461 6c6c 2074 6865 2072 6571  *Install the req
-000021a0: 7569 7265 6420 6472 6976 6572 732a 2a0a  uired drivers**.
-000021b0: 0a60 6060 7368 656c 6c0a 2420 7069 7020  .```shell.$ pip 
-000021c0: 696e 7374 616c 6c20 6461 7461 6261 7365  install database
-000021d0: 735b 6169 6f73 716c 6974 655d 0a24 2070  s[aiosqlite].$ p
-000021e0: 6970 2069 6e73 7461 6c6c 2069 7079 7468  ip install ipyth
-000021f0: 6f6e 0a60 6060 0a0a 4e6f 7720 6672 6f6d  on.```..Now from
-00002200: 2074 6865 2063 6f6e 736f 6c65 2c20 7765   the console, we
-00002210: 2063 616e 2072 756e 2061 2073 696d 706c   can run a simpl
-00002220: 6520 6578 616d 706c 652e 0a0a 0a60 6060  e example....```
-00002230: 7079 7468 6f6e 0a23 2043 7265 6174 6520  python.# Create 
-00002240: 6120 6461 7461 6261 7365 2069 6e73 7461  a database insta
-00002250: 6e63 652c 2061 6e64 2063 6f6e 6e65 6374  nce, and connect
-00002260: 2074 6f20 6974 2e0a 6672 6f6d 2064 6174   to it..from dat
-00002270: 6162 6173 657a 2069 6d70 6f72 7420 4461  abasez import Da
-00002280: 7461 6261 7365 0a0a 6461 7461 6261 7365  tabase..database
-00002290: 203d 2044 6174 6162 6173 6528 2273 716c   = Database("sql
-000022a0: 6974 652b 6169 6f73 716c 6974 653a 2f2f  ite+aiosqlite://
-000022b0: 2f65 7861 6d70 6c65 2e64 6222 290a 6177  /example.db").aw
-000022c0: 6169 7420 6461 7461 6261 7365 2e63 6f6e  ait database.con
-000022d0: 6e65 6374 2829 0a0a 2320 4372 6561 7465  nect()..# Create
-000022e0: 2061 2074 6162 6c65 2e0a 7175 6572 7920   a table..query 
-000022f0: 3d20 2222 2243 5245 4154 4520 5441 424c  = """CREATE TABL
-00002300: 4520 4869 6768 5363 6f72 6573 2028 6964  E HighScores (id
-00002310: 2049 4e54 4547 4552 2050 5249 4d41 5259   INTEGER PRIMARY
-00002320: 204b 4559 2c20 6e61 6d65 2056 4152 4348   KEY, name VARCH
-00002330: 4152 2831 3030 292c 2073 636f 7265 2049  AR(100), score I
-00002340: 4e54 4547 4552 2922 2222 0a61 7761 6974  NTEGER)""".await
-00002350: 2064 6174 6162 6173 652e 6578 6563 7574   database.execut
-00002360: 6528 7175 6572 793d 7175 6572 7929 0a0a  e(query=query)..
-00002370: 2320 496e 7365 7274 2073 6f6d 6520 6461  # Insert some da
-00002380: 7461 2e0a 7175 6572 7920 3d20 2249 4e53  ta..query = "INS
-00002390: 4552 5420 494e 544f 2048 6967 6853 636f  ERT INTO HighSco
-000023a0: 7265 7328 6e61 6d65 2c20 7363 6f72 6529  res(name, score)
-000023b0: 2056 414c 5545 5320 283a 6e61 6d65 2c20   VALUES (:name, 
-000023c0: 3a73 636f 7265 2922 0a76 616c 7565 7320  :score)".values 
-000023d0: 3d20 5b0a 2020 2020 7b22 6e61 6d65 223a  = [.    {"name":
-000023e0: 2022 4461 6973 7922 2c20 2273 636f 7265   "Daisy", "score
-000023f0: 223a 2039 327d 2c0a 2020 2020 7b22 6e61  ": 92},.    {"na
-00002400: 6d65 223a 2022 4e65 696c 222c 2022 7363  me": "Neil", "sc
-00002410: 6f72 6522 3a20 3837 7d2c 0a20 2020 207b  ore": 87},.    {
-00002420: 226e 616d 6522 3a20 2243 6172 6f6c 222c  "name": "Carol",
-00002430: 2022 7363 6f72 6522 3a20 3433 7d2c 0a5d   "score": 43},.]
-00002440: 0a61 7761 6974 2064 6174 6162 6173 652e  .await database.
-00002450: 6578 6563 7574 655f 6d61 6e79 2871 7565  execute_many(que
-00002460: 7279 3d71 7565 7279 2c20 7661 6c75 6573  ry=query, values
-00002470: 3d76 616c 7565 7329 0a0a 2320 5275 6e20  =values)..# Run 
-00002480: 6120 6461 7461 6261 7365 2071 7565 7279  a database query
-00002490: 2e0a 7175 6572 7920 3d20 2253 454c 4543  ..query = "SELEC
-000024a0: 5420 2a20 4652 4f4d 2048 6967 6853 636f  T * FROM HighSco
-000024b0: 7265 7322 0a72 6f77 7320 3d20 6177 6169  res".rows = awai
-000024c0: 7420 6461 7461 6261 7365 2e66 6574 6368  t database.fetch
-000024d0: 5f61 6c6c 2871 7565 7279 3d71 7565 7279  _all(query=query
-000024e0: 290a 0a70 7269 6e74 2822 4869 6768 2053  )..print("High S
-000024f0: 636f 7265 733a 222c 2072 6f77 7329 0a60  cores:", rows).`
-00002500: 6060 0a0a 4368 6563 6b20 6f75 7420 7468  ``..Check out th
-00002510: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00002520: 6f6e 205b 6d61 6b69 6e67 2064 6174 6162  on [making datab
-00002530: 6173 6520 7175 6572 6965 735d 2868 7474  ase queries](htt
-00002540: 7073 3a2f 2f77 7777 2e65 6e63 6f64 652e  ps://www.encode.
-00002550: 696f 2f64 6174 6162 6173 6573 2f64 6174  io/databases/dat
-00002560: 6162 6173 655f 7175 6572 6965 732f 290a  abase_queries/).
-00002570: 666f 7220 6578 616d 706c 6573 206f 6620  for examples of 
-00002580: 686f 7720 746f 2073 7461 7274 2075 7369  how to start usi
-00002590: 6e67 2064 6174 6162 6173 6573 2074 6f67  ng databases tog
-000025a0: 6574 6865 7220 7769 7468 2053 514c 416c  ether with SQLAl
-000025b0: 6368 656d 7920 636f 7265 2065 7870 7265  chemy core expre
-000025c0: 7373 696f 6e73 2e0a 0a0a 5b73 716c 616c  ssions....[sqlal
-000025d0: 6368 656d 792d 636f 7265 5d3a 2068 7474  chemy-core]: htt
-000025e0: 7073 3a2f 2f64 6f63 732e 7371 6c61 6c63  ps://docs.sqlalc
-000025f0: 6865 6d79 2e6f 7267 2f65 6e2f 6c61 7465  hemy.org/en/late
-00002600: 7374 2f63 6f72 652f 0a5b 7371 6c61 6c63  st/core/.[sqlalc
-00002610: 6865 6d79 2d63 6f72 652d 7475 746f 7269  hemy-core-tutori
-00002620: 616c 5d3a 2068 7474 7073 3a2f 2f64 6f63  al]: https://doc
-00002630: 732e 7371 6c61 6c63 6865 6d79 2e6f 7267  s.sqlalchemy.org
-00002640: 2f65 6e2f 6c61 7465 7374 2f63 6f72 652f  /en/latest/core/
-00002650: 7475 746f 7269 616c 2e68 746d 6c0a 5b61  tutorial.html.[a
-00002660: 6c65 6d62 6963 5d3a 2068 7474 7073 3a2f  lembic]: https:/
-00002670: 2f61 6c65 6d62 6963 2e73 716c 616c 6368  /alembic.sqlalch
-00002680: 656d 792e 6f72 672f 656e 2f6c 6174 6573  emy.org/en/lates
-00002690: 742f 0a5b 7073 7963 6f70 6732 5d3a 2068  t/.[psycopg2]: h
-000026a0: 7474 7073 3a2f 2f77 7777 2e70 7379 636f  ttps://www.psyco
-000026b0: 7067 2e6f 7267 2f0a 5b70 796d 7973 716c  pg.org/.[pymysql
-000026c0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-000026d0: 622e 636f 6d2f 5079 4d79 5351 4c2f 5079  b.com/PyMySQL/Py
-000026e0: 4d79 5351 4c0a 5b70 796f 6462 635d 3a20  MySQL.[pyodbc]: 
-000026f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002700: 6f6d 2f6d 6b6c 6565 6861 6d6d 6572 2f70  om/mkleehammer/p
-00002710: 796f 6462 630a 5b61 7379 6e63 7067 5d3a  yodbc.[asyncpg]:
-00002720: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00002730: 636f 6d2f 4d61 6769 6353 7461 636b 2f61  com/MagicStack/a
-00002740: 7379 6e63 7067 0a5b 6169 6f70 675d 3a20  syncpg.[aiopg]: 
-00002750: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002760: 6f6d 2f61 696f 2d6c 6962 732f 6169 6f70  om/aio-libs/aiop
-00002770: 670a 5b61 696f 6d79 7371 6c5d 3a20 6874  g.[aiomysql]: ht
-00002780: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002790: 2f61 696f 2d6c 6962 732f 6169 6f6d 7973  /aio-libs/aiomys
-000027a0: 716c 0a5b 6173 796e 636d 795d 3a20 6874  ql.[asyncmy]: ht
-000027b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000027c0: 2f6c 6f6e 6732 6963 652f 6173 796e 636d  /long2ice/asyncm
-000027d0: 790a 5b61 696f 7371 6c69 7465 5d3a 2068  y.[aiosqlite]: h
-000027e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000027f0: 6d2f 6f6d 6e69 6c69 622f 6169 6f73 716c  m/omnilib/aiosql
-00002800: 6974 650a 5b61 696f 6f64 6263 5d3a 2068  ite.[aioodbc]: h
-00002810: 7474 7073 3a2f 2f61 696f 6f64 6263 2e72  ttps://aioodbc.r
-00002820: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00002830: 2f6c 6174 6573 742f 0a0a 5b65 736d 6572  /latest/..[esmer
-00002840: 616c 645d 3a20 6874 7470 733a 2f2f 6769  ald]: https://gi
-00002850: 7468 7562 2e63 6f6d 2f64 796d 6d6f 6e64  thub.com/dymmond
-00002860: 2f65 736d 6572 616c 640a 5b73 7461 726c  /esmerald.[starl
-00002870: 6574 7465 5d3a 2068 7474 7073 3a2f 2f67  ette]: https://g
-00002880: 6974 6875 622e 636f 6d2f 656e 636f 6465  ithub.com/encode
-00002890: 2f73 7461 726c 6574 7465 0a5b 7361 6e69  /starlette.[sani
-000028a0: 635d 3a20 6874 7470 733a 2f2f 6769 7468  c]: https://gith
-000028b0: 7562 2e63 6f6d 2f68 7567 652d 7375 6363  ub.com/huge-succ
-000028c0: 6573 732f 7361 6e69 630a 5b72 6573 706f  ess/sanic.[respo
-000028d0: 6e64 6572 5d3a 2068 7474 7073 3a2f 2f67  nder]: https://g
-000028e0: 6974 6875 622e 636f 6d2f 6b65 6e6e 6574  ithub.com/kennet
-000028f0: 6872 6569 747a 2f72 6573 706f 6e64 6572  hreitz/responder
-00002900: 0a5b 7175 6172 745d 3a20 6874 7470 733a  .[quart]: https:
-00002910: 2f2f 6769 746c 6162 2e63 6f6d 2f70 676a  //gitlab.com/pgj
-00002920: 6f6e 6573 2f71 7561 7274 0a5b 6169 6f68  ones/quart.[aioh
-00002930: 7474 705d 3a20 6874 7470 733a 2f2f 6769  ttp]: https://gi
-00002940: 7468 7562 2e63 6f6d 2f61 696f 2d6c 6962  thub.com/aio-lib
-00002950: 732f 6169 6f68 7474 700a 5b74 6f72 6e61  s/aiohttp.[torna
-00002960: 646f 5d3a 2068 7474 7073 3a2f 2f67 6974  do]: https://git
-00002970: 6875 622e 636f 6d2f 746f 726e 6164 6f77  hub.com/tornadow
-00002980: 6562 2f74 6f72 6e61 646f 0a5b 6661 7374  eb/tornado.[fast
-00002990: 6170 695d 3a20 6874 7470 733a 2f2f 6769  api]: https://gi
-000029a0: 7468 7562 2e63 6f6d 2f74 6961 6e67 6f6c  thub.com/tiangol
-000029b0: 6f2f 6661 7374 6170 69                   o/fastapi
+000006e0: 6573 2d44 6973 743a 206e 6573 742d 6173  es-Dist: nest-as
+000006f0: 796e 6369 6f3c 322e 302e 302c 3e3d 312e  yncio<2.0.0,>=1.
+00000700: 352e 360a 5265 7175 6972 6573 2d44 6973  5.6.Requires-Dis
+00000710: 743a 2073 716c 616c 6368 656d 793c 322e  t: sqlalchemy<2.
+00000720: 312c 3e3d 322e 302e 390a 5072 6f76 6964  1,>=2.0.9.Provid
+00000730: 6573 2d45 7874 7261 3a20 6169 6f6d 7973  es-Extra: aiomys
+00000740: 716c 0a52 6571 7569 7265 732d 4469 7374  ql.Requires-Dist
+00000750: 3a20 6169 6f6d 7973 716c 3b20 6578 7472  : aiomysql; extr
+00000760: 6120 3d3d 2027 6169 6f6d 7973 716c 270a  a == 'aiomysql'.
+00000770: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000780: 6169 6f6f 6462 630a 5265 7175 6972 6573  aioodbc.Requires
+00000790: 2d44 6973 743a 2061 696f 6f64 6263 3b20  -Dist: aioodbc; 
+000007a0: 6578 7472 6120 3d3d 2027 6169 6f6f 6462  extra == 'aioodb
+000007b0: 6327 0a50 726f 7669 6465 732d 4578 7472  c'.Provides-Extr
+000007c0: 613a 2061 696f 7067 0a52 6571 7569 7265  a: aiopg.Require
+000007d0: 732d 4469 7374 3a20 6169 6f70 673b 2065  s-Dist: aiopg; e
+000007e0: 7874 7261 203d 3d20 2761 696f 7067 270a  xtra == 'aiopg'.
+000007f0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000800: 6169 6f73 716c 6974 650a 5265 7175 6972  aiosqlite.Requir
+00000810: 6573 2d44 6973 743a 2061 696f 7371 6c69  es-Dist: aiosqli
+00000820: 7465 3b20 6578 7472 6120 3d3d 2027 6169  te; extra == 'ai
+00000830: 6f73 716c 6974 6527 0a50 726f 7669 6465  osqlite'.Provide
+00000840: 732d 4578 7472 613a 2061 7379 6e63 6d79  s-Extra: asyncmy
+00000850: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000860: 6173 796e 636d 793b 2065 7874 7261 203d  asyncmy; extra =
+00000870: 3d20 2761 7379 6e63 6d79 270a 5072 6f76  = 'asyncmy'.Prov
+00000880: 6964 6573 2d45 7874 7261 3a20 6173 796e  ides-Extra: asyn
+00000890: 6370 670a 5265 7175 6972 6573 2d44 6973  cpg.Requires-Dis
+000008a0: 743a 2061 7379 6e63 7067 3b20 6578 7472  t: asyncpg; extr
+000008b0: 6120 3d3d 2027 6173 796e 6370 6727 0a50  a == 'asyncpg'.P
+000008c0: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+000008d0: 6576 0a52 6571 7569 7265 732d 4469 7374  ev.Requires-Dist
+000008e0: 3a20 6169 6f6d 7973 716c 3c30 2e32 2e30  : aiomysql<0.2.0
+000008f0: 2c3e 3d30 2e31 2e31 3b20 6578 7472 6120  ,>=0.1.1; extra 
+00000900: 3d3d 2027 6465 7627 0a52 6571 7569 7265  == 'dev'.Require
+00000910: 732d 4469 7374 3a20 6169 6f6f 6462 633c  s-Dist: aioodbc<
+00000920: 302e 352e 302c 3e3d 302e 342e 303b 2065  0.5.0,>=0.4.0; e
+00000930: 7874 7261 203d 3d20 2764 6576 270a 5265  xtra == 'dev'.Re
+00000940: 7175 6972 6573 2d44 6973 743a 2061 696f  quires-Dist: aio
+00000950: 7067 3c32 2e30 2e30 2c3e 3d31 2e34 2e30  pg<2.0.0,>=1.4.0
+00000960: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
+00000970: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000980: 6169 6f73 716c 6974 653c 302e 3230 2e30  aiosqlite<0.20.0
+00000990: 2c3e 3d30 2e31 382e 303b 2065 7874 7261  ,>=0.18.0; extra
+000009a0: 203d 3d20 2764 6576 270a 5265 7175 6972   == 'dev'.Requir
+000009b0: 6573 2d44 6973 743a 2061 7379 6e63 6d79  es-Dist: asyncmy
+000009c0: 3c30 2e33 2e30 2c3e 3d30 2e32 2e37 3b20  <0.3.0,>=0.2.7; 
+000009d0: 6578 7472 6120 3d3d 2027 6465 7627 0a52  extra == 'dev'.R
+000009e0: 6571 7569 7265 732d 4469 7374 3a20 6173  equires-Dist: as
+000009f0: 796e 6370 673c 302e 3330 2e30 2c3e 3d30  yncpg<0.30.0,>=0
+00000a00: 2e32 372e 303b 2065 7874 7261 203d 3d20  .27.0; extra == 
+00000a10: 2764 6576 270a 5265 7175 6972 6573 2d44  'dev'.Requires-D
+00000a20: 6973 743a 2070 7265 2d63 6f6d 6d69 743c  ist: pre-commit<
+00000a30: 342e 302e 302c 3e3d 322e 3137 2e30 3b20  4.0.0,>=2.17.0; 
+00000a40: 6578 7472 6120 3d3d 2027 6465 7627 0a52  extra == 'dev'.R
+00000a50: 6571 7569 7265 732d 4469 7374 3a20 7073  equires-Dist: ps
+00000a60: 7963 6f70 6732 2d62 696e 6172 793c 332e  ycopg2-binary<3.
+00000a70: 302e 302c 3e3d 322e 392e 363b 2065 7874  0.0,>=2.9.6; ext
+00000a80: 7261 203d 3d20 2764 6576 270a 5265 7175  ra == 'dev'.Requ
+00000a90: 6972 6573 2d44 6973 743a 2070 796d 7973  ires-Dist: pymys
+00000aa0: 716c 3c32 2e30 2e30 2c3e 3d31 2e30 2e33  ql<2.0.0,>=1.0.3
+00000ab0: 3b20 6578 7472 6120 3d3d 2027 6465 7627  ; extra == 'dev'
+00000ac0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000ad0: 7079 6f64 6263 3c35 2e30 2e30 2c3e 3d34  pyodbc<5.0.0,>=4
+00000ae0: 2e30 2e33 353b 2065 7874 7261 203d 3d20  .0.35; extra == 
+00000af0: 2764 6576 270a 5072 6f76 6964 6573 2d45  'dev'.Provides-E
+00000b00: 7874 7261 3a20 646f 630a 5265 7175 6972  xtra: doc.Requir
+00000b10: 6573 2d44 6973 743a 206d 6478 2d69 6e63  es-Dist: mdx-inc
+00000b20: 6c75 6465 3c32 2e30 2e30 2c3e 3d31 2e34  lude<2.0.0,>=1.4
+00000b30: 2e31 3b20 6578 7472 6120 3d3d 2027 646f  .1; extra == 'do
+00000b40: 6327 0a52 6571 7569 7265 732d 4469 7374  c'.Requires-Dist
+00000b50: 3a20 6d6b 6175 746f 646f 633c 302e 332e  : mkautodoc<0.3.
+00000b60: 302c 3e3d 302e 322e 303b 2065 7874 7261  0,>=0.2.0; extra
+00000b70: 203d 3d20 2764 6f63 270a 5265 7175 6972   == 'doc'.Requir
+00000b80: 6573 2d44 6973 743a 206d 6b64 6f63 732d  es-Dist: mkdocs-
+00000b90: 6d61 726b 646f 776e 6578 7472 6164 6174  markdownextradat
+00000ba0: 612d 706c 7567 696e 3c30 2e33 2e30 2c3e  a-plugin<0.3.0,>
+00000bb0: 3d30 2e31 2e37 3b20 6578 7472 6120 3d3d  =0.1.7; extra ==
+00000bc0: 2027 646f 6327 0a52 6571 7569 7265 732d   'doc'.Requires-
+00000bd0: 4469 7374 3a20 6d6b 646f 6373 2d6d 6174  Dist: mkdocs-mat
+00000be0: 6572 6961 6c3d 3d39 2e31 2e35 3b20 6578  erial==9.1.5; ex
+00000bf0: 7472 6120 3d3d 2027 646f 6327 0a52 6571  tra == 'doc'.Req
+00000c00: 7569 7265 732d 4469 7374 3a20 6d6b 646f  uires-Dist: mkdo
+00000c10: 6373 3c32 2e30 2e30 2c3e 3d31 2e34 2e32  cs<2.0.0,>=1.4.2
+00000c20: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
+00000c30: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000c40: 6d6b 646f 6373 7472 696e 6773 3c30 2e32  mkdocstrings<0.2
+00000c50: 312e 302c 3e3d 302e 3139 2e30 3b20 6578  1.0,>=0.19.0; ex
+00000c60: 7472 6120 3d3d 2027 646f 6327 0a52 6571  tra == 'doc'.Req
+00000c70: 7569 7265 732d 4469 7374 3a20 7079 7961  uires-Dist: pyya
+00000c80: 6d6c 3c37 2e30 2e30 2c3e 3d35 2e33 2e31  ml<7.0.0,>=5.3.1
+00000c90: 3b20 6578 7472 6120 3d3d 2027 646f 6327  ; extra == 'doc'
+00000ca0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000cb0: 206d 7973 716c 0a52 6571 7569 7265 732d   mysql.Requires-
+00000cc0: 4469 7374 3a20 6169 6f6d 7973 716c 3b20  Dist: aiomysql; 
+00000cd0: 6578 7472 6120 3d3d 2027 6d79 7371 6c27  extra == 'mysql'
+00000ce0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000cf0: 2070 6f73 7467 7265 7371 6c0a 5265 7175   postgresql.Requ
+00000d00: 6972 6573 2d44 6973 743a 2061 7379 6e63  ires-Dist: async
+00000d10: 7067 3b20 6578 7472 6120 3d3d 2027 706f  pg; extra == 'po
+00000d20: 7374 6772 6573 716c 270a 5072 6f76 6964  stgresql'.Provid
+00000d30: 6573 2d45 7874 7261 3a20 7371 6c69 7465  es-Extra: sqlite
+00000d40: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000d50: 6169 6f73 716c 6974 653b 2065 7874 7261  aiosqlite; extra
+00000d60: 203d 3d20 2773 716c 6974 6527 0a50 726f   == 'sqlite'.Pro
+00000d70: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
+00000d80: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
+00000d90: 2061 7574 6f66 6c61 6b65 3c33 2e30 2e30   autoflake<3.0.0
+00000da0: 2c3e 3d32 2e31 2e31 3b20 6578 7472 6120  ,>=2.1.1; extra 
+00000db0: 3d3d 2027 7465 7374 270a 5265 7175 6972  == 'test'.Requir
+00000dc0: 6573 2d44 6973 743a 2062 6c61 636b 3c32  es-Dist: black<2
+00000dd0: 342e 302e 302c 3e3d 3233 2e33 2e30 3b20  4.0.0,>=23.3.0; 
+00000de0: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
+00000df0: 5265 7175 6972 6573 2d44 6973 743a 2065  Requires-Dist: e
+00000e00: 736d 6572 616c 643e 3d31 2e31 2e30 3b20  smerald>=1.1.0; 
+00000e10: 6578 7472 6120 3d3d 2027 7465 7374 270a  extra == 'test'.
+00000e20: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+00000e30: 736f 7274 3c36 2e30 2e30 2c3e 3d35 2e31  sort<6.0.0,>=5.1
+00000e40: 322e 303b 2065 7874 7261 203d 3d20 2774  2.0; extra == 't
+00000e50: 6573 7427 0a52 6571 7569 7265 732d 4469  est'.Requires-Di
+00000e60: 7374 3a20 6d79 7079 3c32 2e30 2e30 2c3e  st: mypy<2.0.0,>
+00000e70: 3d31 2e31 2e30 3b20 6578 7472 6120 3d3d  =1.1.0; extra ==
+00000e80: 2027 7465 7374 270a 5265 7175 6972 6573   'test'.Requires
+00000e90: 2d44 6973 743a 2070 7974 6573 742d 636f  -Dist: pytest-co
+00000ea0: 763c 352e 302e 302c 3e3d 342e 302e 303b  v<5.0.0,>=4.0.0;
+00000eb0: 2065 7874 7261 203d 3d20 2774 6573 7427   extra == 'test'
+00000ec0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000ed0: 7079 7465 7374 3c38 2e30 2e30 2c3e 3d37  pytest<8.0.0,>=7
+00000ee0: 2e32 2e32 3b20 6578 7472 6120 3d3d 2027  .2.2; extra == '
+00000ef0: 7465 7374 270a 5265 7175 6972 6573 2d44  test'.Requires-D
+00000f00: 6973 743a 2072 6571 7565 7374 733e 3d32  ist: requests>=2
+00000f10: 2e32 382e 323b 2065 7874 7261 203d 3d20  .28.2; extra == 
+00000f20: 2774 6573 7427 0a52 6571 7569 7265 732d  'test'.Requires-
+00000f30: 4469 7374 3a20 7275 6666 3c31 2e30 2e30  Dist: ruff<1.0.0
+00000f40: 2c3e 3d30 2e30 2e32 3536 3b20 6578 7472  ,>=0.0.256; extr
+00000f50: 6120 3d3d 2027 7465 7374 270a 5265 7175  a == 'test'.Requ
+00000f60: 6972 6573 2d44 6973 743a 2073 7461 726c  ires-Dist: starl
+00000f70: 6574 7465 3e3d 302e 3236 2e31 3b20 6578  ette>=0.26.1; ex
+00000f80: 7472 6120 3d3d 2027 7465 7374 270a 5072  tra == 'test'.Pr
+00000f90: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
+00000fa0: 7374 696e 670a 5265 7175 6972 6573 2d44  sting.Requires-D
+00000fb0: 6973 743a 2073 716c 616c 6368 656d 792d  ist: sqlalchemy-
+00000fc0: 7574 696c 733e 3d30 2e34 302e 303b 2065  utils>=0.40.0; e
+00000fd0: 7874 7261 203d 3d20 2774 6573 7469 6e67  xtra == 'testing
+00000fe0: 270a 4465 7363 7269 7074 696f 6e2d 436f  '.Description-Co
+00000ff0: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00001000: 2f6d 6172 6b64 6f77 6e0a 0a23 2044 6174  /markdown..# Dat
+00001010: 6162 6173 657a 0a0a 3c70 2061 6c69 676e  abasez..<p align
+00001020: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00001030: 6872 6566 3d22 6874 7470 733a 2f2f 6461  href="https://da
+00001040: 7461 6261 7365 7a2e 7461 7273 696c 642e  tabasez.tarsild.
+00001050: 696f 223e 3c69 6d67 2073 7263 3d22 6874  io"><img src="ht
+00001060: 7470 733a 2f2f 7265 732e 636c 6f75 6469  tps://res.cloudi
+00001070: 6e61 7279 2e63 6f6d 2f64 796d 6d6f 6e64  nary.com/dymmond
+00001080: 2f69 6d61 6765 2f75 706c 6f61 642f 7631  /image/upload/v1
+00001090: 3638 3036 3131 3632 362f 6461 7461 6261  680611626/databa
+000010a0: 7365 7a2f 6c6f 676f 2d63 6d70 5f6c 7569  sez/logo-cmp_lui
+000010b0: 7a62 302e 706e 6722 2061 6c74 3d27 6461  zb0.png" alt='da
+000010c0: 7461 6261 7365 7a27 3e3c 2f61 3e0a 3c2f  tabasez'></a>.</
+000010d0: 703e 0a0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
+000010e0: 6e74 6572 223e 0a20 2020 203c 656d 3ef0  nter">.    <em>.
+000010f0: 9f9a 8020 4173 796e 6320 6461 7461 6261  ... Async databa
+00001100: 7365 2073 7570 706f 7274 2066 6f72 2050  se support for P
+00001110: 7974 686f 6e2e 20f0 9f9a 803c 2f65 6d3e  ython. ....</em>
+00001120: 0a3c 2f70 3e0a 0a3c 7020 616c 6967 6e3d  .</p>..<p align=
+00001130: 2263 656e 7465 7222 3e0a 3c61 2068 7265  "center">.<a hre
+00001140: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001150: 622e 636f 6d2f 7461 7273 696c 2f64 6174  b.com/tarsil/dat
+00001160: 6162 6173 657a 2f77 6f72 6b66 6c6f 7773  abasez/workflows
+00001170: 2f54 6573 7425 3230 5375 6974 652f 6261  /Test%20Suite/ba
+00001180: 6467 652e 7376 673f 6576 656e 743d 7075  dge.svg?event=pu
+00001190: 7368 2662 7261 6e63 683d 6d61 696e 2220  sh&branch=main" 
+000011a0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+000011b0: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+000011c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000011d0: 6d2f 7461 7273 696c 2f64 6174 6162 6173  m/tarsil/databas
+000011e0: 657a 2f77 6f72 6b66 6c6f 7773 2f54 6573  ez/workflows/Tes
+000011f0: 7425 3230 5375 6974 652f 6261 6467 652e  t%20Suite/badge.
+00001200: 7376 673f 6576 656e 743d 7075 7368 2662  svg?event=push&b
+00001210: 7261 6e63 683d 6d61 696e 2220 616c 743d  ranch=main" alt=
+00001220: 2254 6573 7420 5375 6974 6522 3e0a 3c2f  "Test Suite">.</
+00001230: 613e 0a0a 3c61 2068 7265 663d 2268 7474  a>..<a href="htt
+00001240: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00001250: 6f6a 6563 742f 6461 7461 6261 7365 7a22  oject/databasez"
+00001260: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001270: 3e0a 2020 2020 3c69 6d67 2073 7263 3d22  >.    <img src="
+00001280: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001290: 6c64 732e 696f 2f70 7970 692f 762f 6461  lds.io/pypi/v/da
+000012a0: 7461 6261 7365 7a3f 636f 6c6f 723d 2532  tabasez?color=%2
+000012b0: 3333 3444 3035 3826 6c61 6265 6c3d 7079  334D058&label=py
+000012c0: 7069 2532 3070 6163 6b61 6765 2220 616c  pi%20package" al
+000012d0: 743d 2250 6163 6b61 6765 2076 6572 7369  t="Package versi
+000012e0: 6f6e 223e 0a3c 2f61 3e0a 0a3c 6120 6872  on">.</a>..<a hr
+000012f0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00001300: 2e6f 7267 2f70 726f 6a65 6374 2f64 6174  .org/project/dat
+00001310: 6162 6173 657a 2220 7461 7267 6574 3d22  abasez" target="
+00001320: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
+00001330: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00001340: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00001350: 7069 2f70 7976 6572 7369 6f6e 732f 6461  pi/pyversions/da
+00001360: 7461 6261 7365 7a2e 7376 673f 636f 6c6f  tabasez.svg?colo
+00001370: 723d 2532 3333 3444 3035 3822 2061 6c74  r=%2334D058" alt
+00001380: 3d22 5375 7070 6f72 7465 6420 5079 7468  ="Supported Pyth
+00001390: 6f6e 2076 6572 7369 6f6e 7322 3e0a 3c2f  on versions">.</
+000013a0: 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a 2a2a  a>.</p>..---..**
+000013b0: 446f 6375 6d65 6e74 6174 696f 6e2a 2a3a  Documentation**:
+000013c0: 205b 6874 7470 733a 2f2f 6461 7461 6261   [https://databa
+000013d0: 7365 7a2e 7461 7273 696c 642e 696f 5d28  sez.tarsild.io](
+000013e0: 6874 7470 733a 2f2f 6461 7461 6261 7365  https://database
+000013f0: 7a2e 7461 7273 696c 642e 696f 2920 f09f  z.tarsild.io) ..
+00001400: 939a 0a0a 2a2a 536f 7572 6365 2043 6f64  ....**Source Cod
+00001410: 652a 2a3a 205b 6874 7470 733a 2f2f 6769  e**: [https://gi
+00001420: 7468 7562 2e63 6f6d 2f74 6172 7369 6c2f  thub.com/tarsil/
+00001430: 6461 7461 6261 7365 7a5d 2868 7474 7073  databasez](https
+00001440: 3a2f 2f67 6974 6875 622e 636f 6d2f 7461  ://github.com/ta
+00001450: 7273 696c 2f64 6174 6162 6173 657a 290a  rsil/databasez).
+00001460: 0a2d 2d2d 0a0a 2323 204d 6f74 6976 6174  .---..## Motivat
+00001470: 696f 6e0a 0a54 6865 7265 2069 7320 6120  ion..There is a 
+00001480: 6772 6561 7420 7061 636b 6167 6520 6672  great package fr
+00001490: 6f6d 205b 456e 636f 6465 5d28 6874 7470  om [Encode](http
+000014a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+000014b0: 6e63 6f64 652f 6461 7461 6261 7365 732f  ncode/databases/
+000014c0: 2920 7468 6174 2077 6173 2064 6f69 6e67  ) that was doing
+000014d0: 2077 6861 740a 7468 6973 2070 6163 6b61   what.this packa
+000014e0: 6765 2077 6173 2069 6e69 7469 616c 6c79  ge was initially
+000014f0: 2066 6f72 6b65 6420 746f 2064 6f20 6275   forked to do bu
+00001500: 7420 456e 636f 6465 2069 7320 616c 736f  t Encode is also
+00001510: 2076 6572 7920 6275 7379 2077 6974 6820   very busy with 
+00001520: 6f74 6865 7220 7072 6f6a 6563 7473 2061  other projects a
+00001530: 6e64 0a77 6974 686f 7574 2074 6865 2070  nd.without the p
+00001540: 726f 7065 7220 7469 6d65 2074 6f20 6d61  roper time to ma
+00001550: 696e 7461 696e 2074 6865 2073 6f20 6d75  intain the so mu
+00001560: 6368 2072 6571 7569 7265 6420 7061 636b  ch required pack
+00001570: 6167 652e 0a0a 4672 6f6d 2061 206e 6565  age...From a nee
+00001580: 6420 746f 2065 7874 656e 6420 746f 206e  d to extend to n
+00001590: 6577 2064 7269 7665 7273 2061 6e64 206e  ew drivers and n
+000015a0: 6577 6573 7420 7465 6368 6e6f 6c6f 6769  ewest technologi
+000015b0: 6573 2061 6e64 2061 6464 696e 6720 6578  es and adding ex
+000015c0: 7472 6120 6665 6174 7572 6573 2063 6f6d  tra features com
+000015d0: 6d6f 6e20 616e 640a 7573 6566 756c 2074  mon and.useful t
+000015e0: 6f20 7468 6520 6d61 6e79 2c20 5b44 6174  o the many, [Dat
+000015f0: 6162 6173 6573 5d28 6874 7470 733a 2f2f  abases](https://
+00001600: 6769 7468 7562 2e63 6f6d 2f65 6e63 6f64  github.com/encod
+00001610: 652f 6461 7461 6261 7365 732f 2920 7761  e/databases/) wa
+00001620: 7320 666f 726b 6564 2074 6f20 6265 636f  s forked to beco
+00001630: 6d65 0a2a 2a44 6174 6162 6173 657a 2a2a  me.**Databasez**
+00001640: 2e0a 0a54 6869 7320 7061 636b 6167 6520  ...This package 
+00001650: 6973 2031 3030 2520 6261 636b 7761 7264  is 100% backward
+00001660: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
+00001670: 6820 5b44 6174 6162 6173 6573 5d28 6874  h [Databases](ht
+00001680: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001690: 2f65 6e63 6f64 652f 6461 7461 6261 7365  /encode/database
+000016a0: 732f 290a 6672 6f6d 2045 6e63 6f64 6520  s/).from Encode 
+000016b0: 616e 6420 7769 6c6c 2072 656d 6169 6e20  and will remain 
+000016c0: 6c69 6b65 2074 6869 7320 666f 7220 7468  like this for th
+000016d0: 6520 7469 6d65 2062 6569 6e67 2062 7574  e time being but
+000016e0: 2061 6464 696e 6720 6578 7472 6120 6665   adding extra fe
+000016f0: 6174 7572 6573 2061 6e64 2072 6567 756c  atures and regul
+00001700: 6172 0a75 7064 6174 6573 2061 7320 7765  ar.updates as we
+00001710: 6c6c 2061 7320 636f 6e74 696e 7569 6e67  ll as continuing
+00001720: 2074 6f20 6265 2063 6f6d 6d75 6e69 7479   to be community
+00001730: 2064 7269 7665 6e2e 0a0a 4279 2074 6865   driven...By the
+00001740: 2074 696d 6520 7468 6973 2070 726f 6a65   time this proje
+00001750: 6374 2077 6173 2063 7265 6174 6564 2c20  ct was created, 
+00001760: 4461 7461 6261 7365 7320 7761 7320 7965  Databases was ye
+00001770: 7420 746f 206d 6572 6765 2070 6f73 7369  t to merge possi
+00001780: 626c 6520 5351 4c41 6c63 6865 6d79 2032  ble SQLAlchemy 2
+00001790: 2e30 2063 6861 6e67 6573 0a66 726f 6d20  .0 changes.from 
+000017a0: 7468 6520 6175 7468 6f72 206f 6620 7468  the author of th
+000017b0: 6973 2070 6163 6b61 6765 2061 6e64 2074  is package and t
+000017c0: 6865 7265 666f 7265 2c20 7468 6973 2070  herefore, this p
+000017d0: 6163 6b61 6765 2061 696d 7320 746f 2075  ackage aims to u
+000017e0: 6e62 6c6f 636b 0a61 206c 6f74 206f 6620  nblock.a lot of 
+000017f0: 7468 6520 7072 6f6a 6563 7473 206f 7574  the projects out
+00001800: 2074 6865 7265 2074 6861 7420 7761 6e74   there that want
+00001810: 2053 514c 416c 6368 656d 7920 322e 3020   SQLAlchemy 2.0 
+00001820: 7769 7468 2074 6865 2062 6573 7420 6f66  with the best of
+00001830: 2064 6174 6162 6173 6573 2077 6974 6820   databases with 
+00001840: 6e65 7720 6665 6174 7572 6573 2e0a 0a41  new features...A
+00001850: 206c 6f74 206f 6620 7061 636b 6167 6573   lot of packages
+00001860: 2064 6570 656e 6473 206f 6620 4461 7461   depends of Data
+00001870: 6261 7365 7320 616e 6420 7468 6973 2077  bases and this w
+00001880: 6173 2074 6865 206d 6169 6e20 7265 6173  as the main reas
+00001890: 6f6e 2066 6f72 2074 6865 2066 6f72 6b20  on for the fork 
+000018a0: 6f66 202a 2a44 6174 6162 6173 657a 2a2a  of **Databasez**
+000018b0: 2e0a 5468 6520 6e65 6564 206f 6620 7072  ..The need of pr
+000018c0: 6f67 7265 7373 696e 672e 0a0a 4974 2061  ogressing...It a
+000018d0: 6c6c 6f77 7320 796f 7520 746f 206d 616b  llows you to mak
+000018e0: 6520 7175 6572 6965 7320 7573 696e 6720  e queries using 
+000018f0: 7468 6520 706f 7765 7266 756c 205b 5351  the powerful [SQ
+00001900: 4c41 6c63 6865 6d79 2043 6f72 655d 5b73  LAlchemy Core][s
+00001910: 716c 616c 6368 656d 792d 636f 7265 5d0a  qlalchemy-core].
+00001920: 6578 7072 6573 7369 6f6e 206c 616e 6775  expression langu
+00001930: 6167 652c 2061 6e64 2070 726f 7669 6465  age, and provide
+00001940: 7320 7375 7070 6f72 7420 666f 7220 506f  s support for Po
+00001950: 7374 6772 6553 514c 2c20 4d79 5351 4c2c  stgreSQL, MySQL,
+00001960: 2053 514c 6974 6520 616e 6420 4d53 5351   SQLite and MSSQ
+00001970: 4c2e 0a0a 4461 7461 6261 7365 7a20 6973  L...Databasez is
+00001980: 2073 7569 7461 626c 6520 666f 7220 696e   suitable for in
+00001990: 7465 6772 6174 696e 6720 6167 6169 6e73  tegrating agains
+000019a0: 7420 616e 7920 6173 796e 6320 5765 6220  t any async Web 
+000019b0: 6672 616d 6577 6f72 6b2c 2073 7563 6820  framework, such 
+000019c0: 6173 205b 4573 6d65 7261 6c64 5d5b 6573  as [Esmerald][es
+000019d0: 6d65 7261 6c64 5d2c 0a5b 5374 6172 6c65  merald],.[Starle
+000019e0: 7474 655d 5b73 7461 726c 6574 7465 5d2c  tte][starlette],
+000019f0: 205b 5361 6e69 635d 5b73 616e 6963 5d2c   [Sanic][sanic],
+00001a00: 205b 5265 7370 6f6e 6465 725d 5b72 6573   [Responder][res
+00001a10: 706f 6e64 6572 5d2c 205b 5175 6172 745d  ponder], [Quart]
+00001a20: 5b71 7561 7274 5d2c 205b 6169 6f68 7474  [quart], [aiohtt
+00001a30: 705d 5b61 696f 6874 7470 5d2c 0a5b 546f  p][aiohttp],.[To
+00001a40: 726e 6164 6f5d 5b74 6f72 6e61 646f 5d2c  rnado][tornado],
+00001a50: 206f 7220 5b46 6173 7441 5049 5d5b 6661   or [FastAPI][fa
+00001a60: 7374 6170 695d 2e0a 0a44 6174 6162 6173  stapi]...Databas
+00001a70: 657a 2077 6173 2062 7569 6c74 2066 6f72  ez was built for
+00001a80: 2050 7974 686f 6e20 332e 382b 2061 6e64   Python 3.8+ and
+00001a90: 206f 6e20 7468 6520 746f 7020 6f66 2074   on the top of t
+00001aa0: 6865 206e 6577 6573 7420 2a2a 5351 4c41  he newest **SQLA
+00001ab0: 6c63 6865 6d79 2032 2a2a 2061 6e64 2067  lchemy 2** and g
+00001ac0: 6976 6573 2079 6f75 0a73 696d 706c 6520  ives you.simple 
+00001ad0: 6173 796e 6369 6f20 7375 7070 6f72 7420  asyncio support 
+00001ae0: 666f 7220 6120 7261 6e67 6520 6f66 2064  for a range of d
+00001af0: 6174 6162 6173 6573 2e0a 0a23 2320 496e  atabases...## In
+00001b00: 7374 616c 6c61 7469 6f6e 0a0a 6060 6073  stallation..```s
+00001b10: 6865 6c6c 0a24 2070 6970 2069 6e73 7461  hell.$ pip insta
+00001b20: 6c6c 2064 6174 6162 6173 657a 0a60 6060  ll databasez.```
+00001b30: 0a0a 4966 2079 6f75 2061 7265 2069 6e74  ..If you are int
+00001b40: 6572 6573 7465 6420 696e 2075 7369 6e67  erested in using
+00001b50: 2074 6865 205b 7465 7374 2063 6c69 656e   the [test clien
+00001b60: 745d 282e 2f74 6573 742d 636c 6965 6e74  t](./test-client
+00001b70: 2e6d 6429 2c20 796f 7520 6361 6e20 616c  .md), you can al
+00001b80: 736f 2069 6e73 7461 6c6c 3a0a 0a60 6060  so install:..```
+00001b90: 7368 656c 6c0a 2420 7069 7020 696e 7374  shell.$ pip inst
+00001ba0: 616c 6c20 6461 7461 6261 7365 7a5b 7465  all databasez[te
+00001bb0: 7374 696e 675d 0a60 6060 0a0a 2323 2057  sting].```..## W
+00001bc0: 6861 7420 646f 6573 2064 6174 6162 6173  hat does databas
+00001bd0: 657a 2073 7570 706f 7274 2061 7420 7468  ez support at th
+00001be0: 6520 6d6f 6d65 6e74 0a0a 4461 7461 6261  e moment..Databa
+00001bf0: 7365 7a20 6375 7272 656e 746c 7920 7375  sez currently su
+00001c00: 7070 6f72 7473 2060 7371 6c69 7465 602c  pports `sqlite`,
+00001c10: 2060 706f 7374 6772 6573 602c 2060 6d79   `postgres`, `my
+00001c20: 7371 6c60 2061 6e64 2060 7371 6c20 7365  sql` and `sql se
+00001c30: 7276 6572 602e 204d 6f72 6520 6472 6976  rver`. More driv
+00001c40: 6572 7320 6361 6e20 616e 640a 7769 6c6c  ers can and.will
+00001c50: 2062 6520 6164 6465 6420 696e 2074 6865   be added in the
+00001c60: 2066 7574 7572 652e 0a0a 4461 7461 6261   future...Databa
+00001c70: 7365 2064 7269 7665 7273 2073 7570 706f  se drivers suppo
+00001c80: 7274 6564 2061 7265 3a0a 0a2a 205b 6173  rted are:..* [as
+00001c90: 796e 6370 675d 5b61 7379 6e63 7067 5d20  yncpg][asyncpg] 
+00001ca0: 2d20 466f 7220 706f 7374 6772 6573 2e0a  - For postgres..
+00001cb0: 2a20 5b61 696f 7067 5d5b 6169 6f70 675d  * [aiopg][aiopg]
+00001cc0: 202d 2046 6f72 2070 6f73 7467 7265 732e   - For postgres.
+00001cd0: 0a2a 205b 6169 6f6d 7973 716c 5d5b 6169  .* [aiomysql][ai
+00001ce0: 6f6d 7973 716c 5d20 2d20 466f 7220 4d79  omysql] - For My
+00001cf0: 5351 4c2f 4d61 7269 6144 422e 0a2a 205b  SQL/MariaDB..* [
+00001d00: 6173 796e 636d 795d 5b61 7379 6e63 6d79  asyncmy][asyncmy
+00001d10: 5d20 2d20 466f 7220 4d79 5351 4c2f 4d61  ] - For MySQL/Ma
+00001d20: 7269 6144 422e 0a2a 205b 6169 6f73 716c  riaDB..* [aiosql
+00001d30: 6974 655d 5b61 696f 7371 6c69 7465 5d20  ite][aiosqlite] 
+00001d40: 2d20 466f 7220 5351 4c69 7465 2e0a 2a20  - For SQLite..* 
+00001d50: 5b61 696f 6f64 6263 5d5b 6169 6f6f 6462  [aioodbc][aioodb
+00001d60: 635d 202d 2046 6f72 204d 5353 514c 2028  c] - For MSSQL (
+00001d70: 5351 4c20 5365 7276 6572 292e 0a0a 2323  SQL Server)...##
+00001d80: 2320 4472 6976 6572 2069 6e73 7461 6c6c  # Driver install
+00001d90: 6174 696f 6e0a 0a59 6f75 2063 616e 2069  ation..You can i
+00001da0: 6e73 7461 6c6c 2074 6865 2072 6571 7569  nstall the requi
+00001db0: 7265 6420 6461 7461 6261 7365 2064 7269  red database dri
+00001dc0: 7665 7273 2077 6974 683a 0a0a 2323 2323  vers with:..####
+00001dd0: 2050 6f73 7467 7265 730a 0a60 6060 7368   Postgres..```sh
+00001de0: 656c 6c0a 2420 7069 7020 696e 7374 616c  ell.$ pip instal
+00001df0: 6c20 6461 7461 6261 7365 7a5b 6173 796e  l databasez[asyn
+00001e00: 6370 675d 0a60 6060 0a0a 6f72 0a0a 6060  cpg].```..or..``
+00001e10: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
+00001e20: 7461 6c6c 2064 6174 6162 6173 657a 5b61  tall databasez[a
+00001e30: 696f 7067 5d0a 6060 600a 0a23 2323 2320  iopg].```..#### 
+00001e40: 4d79 5351 4c2f 4d61 7269 6144 420a 0a60  MySQL/MariaDB..`
+00001e50: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
+00001e60: 7374 616c 6c20 6461 7461 6261 7365 7a5b  stall databasez[
+00001e70: 6169 6f6d 7973 716c 5d0a 6060 600a 0a6f  aiomysql].```..o
+00001e80: 720a 0a60 6060 7368 656c 6c0a 2420 7069  r..```shell.$ pi
+00001e90: 7020 696e 7374 616c 6c20 6461 7461 6261  p install databa
+00001ea0: 7365 7a5b 6173 796e 636d 795d 0a60 6060  sez[asyncmy].```
+00001eb0: 0a0a 2323 2323 2053 514c 6974 650a 0a60  ..#### SQLite..`
+00001ec0: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
+00001ed0: 7374 616c 6c20 6461 7461 6261 7365 7a5b  stall databasez[
+00001ee0: 6169 6f73 716c 6974 655d 0a60 6060 0a0a  aiosqlite].```..
+00001ef0: 2323 2323 204d 5353 514c 0a0a 6060 6073  #### MSSQL..```s
+00001f00: 6865 6c6c 0a24 2070 6970 2069 6e73 7461  hell.$ pip insta
+00001f10: 6c6c 2064 6174 6162 6173 657a 5b61 696f  ll databasez[aio
+00001f20: 6f64 6263 5d0a 6060 600a 0a21 2121 204e  odbc].```..!!! N
+00001f30: 6f74 650a 2020 2020 4e6f 7465 2074 6861  ote.    Note tha
+00001f40: 7420 6966 2079 6f75 2061 7265 2075 7369  t if you are usi
+00001f50: 6e67 2061 6e79 2073 796e 6368 726f 6e6f  ng any synchrono
+00001f60: 7573 2053 514c 416c 6368 656d 7920 6675  us SQLAlchemy fu
+00001f70: 6e63 7469 6f6e 7320 7375 6368 2061 7320  nctions such as 
+00001f80: 6065 6e67 696e 652e 6372 6561 7465 5f61  `engine.create_a
+00001f90: 6c6c 2829 600a 2020 2020 6f72 205b 616c  ll()`.    or [al
+00001fa0: 656d 6269 635d 5b61 6c65 6d62 6963 5d20  embic][alembic] 
+00001fb0: 6d69 6772 6174 696f 6e73 2074 6865 6e20  migrations then 
+00001fc0: 796f 7520 7374 696c 6c20 6861 7665 2074  you still have t
+00001fd0: 6f20 696e 7374 616c 6c20 6120 7379 6e63  o install a sync
+00001fe0: 6872 6f6e 6f75 7320 4442 2064 7269 7665  hronous DB drive
+00001ff0: 723a 0a20 2020 205b 7073 7963 6f70 6732  r:.    [psycopg2
+00002000: 5d5b 7073 7963 6f70 6732 5d20 666f 7220  ][psycopg2] for 
+00002010: 506f 7374 6772 6553 514c 2c20 5b70 796d  PostgreSQL, [pym
+00002020: 7973 716c 5d5b 7079 6d79 7371 6c5d 2066  ysql][pymysql] f
+00002030: 6f72 204d 7953 514c 2061 6e64 0a20 2020  or MySQL and.   
+00002040: 205b 7079 6f64 6263 5d5b 7079 6f64 6263   [pyodbc][pyodbc
+00002050: 5d20 666f 7220 5351 4c20 5365 7276 6572  ] for SQL Server
+00002060: 2e0a 0a2d 2d2d 0a0a 2323 2051 7569 636b  ...---..## Quick
+00002070: 7374 6172 740a 0a46 6f72 2061 2073 696d  start..For a sim
+00002080: 706c 6520 7175 6963 6b73 7461 7274 2065  ple quickstart e
+00002090: 7861 6d70 6c65 2c20 7765 2077 696c 6c20  xample, we will 
+000020a0: 6265 2063 7265 6174 696e 6720 6120 7369  be creating a si
+000020b0: 6d70 6c65 2053 514c 6974 6520 6461 7461  mple SQLite data
+000020c0: 6261 7365 2074 6f20 7275 6e20 736f 6d65  base to run some
+000020d0: 2071 7565 7269 6573 0a61 6761 696e 7374   queries.against
+000020e0: 2e0a 0a46 6972 7374 2c20 696e 7374 616c  ...First, instal
+000020f0: 6c20 7468 6520 7265 7175 6972 6564 2064  l the required d
+00002100: 7269 7665 7273 2066 6f72 2060 5351 4c69  rivers for `SQLi
+00002110: 7465 6020 616e 6420 6069 7079 7468 6f6e  te` and `ipython
+00002120: 602e 2054 6865 2060 6970 7974 686f 6e60  `. The `ipython`
+00002130: 2069 7320 746f 2068 6176 6520 616e 0a69   is to have an.i
+00002140: 6e74 6572 6163 7469 7665 2070 7974 686f  nteractive pytho
+00002150: 6e20 7368 656c 6c20 7769 7468 2073 6f6d  n shell with som
+00002160: 6520 6578 7472 6173 2e20 4950 7974 686f  e extras. IPytho
+00002170: 6e20 616c 736f 2073 7570 706f 7274 7320  n also supports 
+00002180: 6061 7761 6974 602c 2077 6869 6368 2069  `await`, which i
+00002190: 7320 6578 6163 746c 790a 7768 6174 2077  s exactly.what w
+000021a0: 6520 6e65 6564 2e20 5b53 6565 206d 6f72  e need. [See mor
+000021b0: 6520 6465 7461 696c 735d 2868 7474 7073  e details](https
+000021c0: 3a2f 2f69 7079 7468 6f6e 2e6f 7267 2f29  ://ipython.org/)
+000021d0: 2061 626f 7574 2069 742e 0a0a 2a2a 496e   about it...**In
+000021e0: 7374 616c 6c20 7468 6520 7265 7175 6972  stall the requir
+000021f0: 6564 2064 7269 7665 7273 2a2a 0a0a 6060  ed drivers**..``
+00002200: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
+00002210: 7461 6c6c 2064 6174 6162 6173 6573 5b61  tall databases[a
+00002220: 696f 7371 6c69 7465 5d0a 2420 7069 7020  iosqlite].$ pip 
+00002230: 696e 7374 616c 6c20 6970 7974 686f 6e0a  install ipython.
+00002240: 6060 600a 0a4e 6f77 2066 726f 6d20 7468  ```..Now from th
+00002250: 6520 636f 6e73 6f6c 652c 2077 6520 6361  e console, we ca
+00002260: 6e20 7275 6e20 6120 7369 6d70 6c65 2065  n run a simple e
+00002270: 7861 6d70 6c65 2e0a 0a0a 6060 6070 7974  xample....```pyt
+00002280: 686f 6e0a 2320 4372 6561 7465 2061 2064  hon.# Create a d
+00002290: 6174 6162 6173 6520 696e 7374 616e 6365  atabase instance
+000022a0: 2c20 616e 6420 636f 6e6e 6563 7420 746f  , and connect to
+000022b0: 2069 742e 0a66 726f 6d20 6461 7461 6261   it..from databa
+000022c0: 7365 7a20 696d 706f 7274 2044 6174 6162  sez import Datab
+000022d0: 6173 650a 0a64 6174 6162 6173 6520 3d20  ase..database = 
+000022e0: 4461 7461 6261 7365 2822 7371 6c69 7465  Database("sqlite
+000022f0: 2b61 696f 7371 6c69 7465 3a2f 2f2f 6578  +aiosqlite:///ex
+00002300: 616d 706c 652e 6462 2229 0a61 7761 6974  ample.db").await
+00002310: 2064 6174 6162 6173 652e 636f 6e6e 6563   database.connec
+00002320: 7428 290a 0a23 2043 7265 6174 6520 6120  t()..# Create a 
+00002330: 7461 626c 652e 0a71 7565 7279 203d 2022  table..query = "
+00002340: 2222 4352 4541 5445 2054 4142 4c45 2048  ""CREATE TABLE H
+00002350: 6967 6853 636f 7265 7320 2869 6420 494e  ighScores (id IN
+00002360: 5445 4745 5220 5052 494d 4152 5920 4b45  TEGER PRIMARY KE
+00002370: 592c 206e 616d 6520 5641 5243 4841 5228  Y, name VARCHAR(
+00002380: 3130 3029 2c20 7363 6f72 6520 494e 5445  100), score INTE
+00002390: 4745 5229 2222 220a 6177 6169 7420 6461  GER)""".await da
+000023a0: 7461 6261 7365 2e65 7865 6375 7465 2871  tabase.execute(q
+000023b0: 7565 7279 3d71 7565 7279 290a 0a23 2049  uery=query)..# I
+000023c0: 6e73 6572 7420 736f 6d65 2064 6174 612e  nsert some data.
+000023d0: 0a71 7565 7279 203d 2022 494e 5345 5254  .query = "INSERT
+000023e0: 2049 4e54 4f20 4869 6768 5363 6f72 6573   INTO HighScores
+000023f0: 286e 616d 652c 2073 636f 7265 2920 5641  (name, score) VA
+00002400: 4c55 4553 2028 3a6e 616d 652c 203a 7363  LUES (:name, :sc
+00002410: 6f72 6529 220a 7661 6c75 6573 203d 205b  ore)".values = [
+00002420: 0a20 2020 207b 226e 616d 6522 3a20 2244  .    {"name": "D
+00002430: 6169 7379 222c 2022 7363 6f72 6522 3a20  aisy", "score": 
+00002440: 3932 7d2c 0a20 2020 207b 226e 616d 6522  92},.    {"name"
+00002450: 3a20 224e 6569 6c22 2c20 2273 636f 7265  : "Neil", "score
+00002460: 223a 2038 377d 2c0a 2020 2020 7b22 6e61  ": 87},.    {"na
+00002470: 6d65 223a 2022 4361 726f 6c22 2c20 2273  me": "Carol", "s
+00002480: 636f 7265 223a 2034 337d 2c0a 5d0a 6177  core": 43},.].aw
+00002490: 6169 7420 6461 7461 6261 7365 2e65 7865  ait database.exe
+000024a0: 6375 7465 5f6d 616e 7928 7175 6572 793d  cute_many(query=
+000024b0: 7175 6572 792c 2076 616c 7565 733d 7661  query, values=va
+000024c0: 6c75 6573 290a 0a23 2052 756e 2061 2064  lues)..# Run a d
+000024d0: 6174 6162 6173 6520 7175 6572 792e 0a71  atabase query..q
+000024e0: 7565 7279 203d 2022 5345 4c45 4354 202a  uery = "SELECT *
+000024f0: 2046 524f 4d20 4869 6768 5363 6f72 6573   FROM HighScores
+00002500: 220a 726f 7773 203d 2061 7761 6974 2064  ".rows = await d
+00002510: 6174 6162 6173 652e 6665 7463 685f 616c  atabase.fetch_al
+00002520: 6c28 7175 6572 793d 7175 6572 7929 0a0a  l(query=query)..
+00002530: 7072 696e 7428 2248 6967 6820 5363 6f72  print("High Scor
+00002540: 6573 3a22 2c20 726f 7773 290a 6060 600a  es:", rows).```.
+00002550: 0a43 6865 636b 206f 7574 2074 6865 2064  .Check out the d
+00002560: 6f63 756d 656e 7461 7469 6f6e 206f 6e20  ocumentation on 
+00002570: 5b6d 616b 696e 6720 6461 7461 6261 7365  [making database
+00002580: 2071 7565 7269 6573 5d28 6874 7470 733a   queries](https:
+00002590: 2f2f 6461 7461 6261 7365 7a2e 7461 7273  //databasez.tars
+000025a0: 696c 642e 696f 2f71 7565 7269 6573 2f29  ild.io/queries/)
+000025b0: 0a66 6f72 2065 7861 6d70 6c65 7320 6f66  .for examples of
+000025c0: 2068 6f77 2074 6f20 7374 6172 7420 7573   how to start us
+000025d0: 696e 6720 6461 7461 6261 7365 7320 746f  ing databases to
+000025e0: 6765 7468 6572 2077 6974 6820 5351 4c41  gether with SQLA
+000025f0: 6c63 6865 6d79 2063 6f72 6520 6578 7072  lchemy core expr
+00002600: 6573 7369 6f6e 732e 0a0a 0a5b 7371 6c61  essions....[sqla
+00002610: 6c63 6865 6d79 2d63 6f72 655d 3a20 6874  lchemy-core]: ht
+00002620: 7470 733a 2f2f 646f 6373 2e73 716c 616c  tps://docs.sqlal
+00002630: 6368 656d 792e 6f72 672f 656e 2f6c 6174  chemy.org/en/lat
+00002640: 6573 742f 636f 7265 2f0a 5b73 716c 616c  est/core/.[sqlal
+00002650: 6368 656d 792d 636f 7265 2d74 7574 6f72  chemy-core-tutor
+00002660: 6961 6c5d 3a20 6874 7470 733a 2f2f 646f  ial]: https://do
+00002670: 6373 2e73 716c 616c 6368 656d 792e 6f72  cs.sqlalchemy.or
+00002680: 672f 656e 2f6c 6174 6573 742f 636f 7265  g/en/latest/core
+00002690: 2f74 7574 6f72 6961 6c2e 6874 6d6c 0a5b  /tutorial.html.[
+000026a0: 616c 656d 6269 635d 3a20 6874 7470 733a  alembic]: https:
+000026b0: 2f2f 616c 656d 6269 632e 7371 6c61 6c63  //alembic.sqlalc
+000026c0: 6865 6d79 2e6f 7267 2f65 6e2f 6c61 7465  hemy.org/en/late
+000026d0: 7374 2f0a 5b70 7379 636f 7067 325d 3a20  st/.[psycopg2]: 
+000026e0: 6874 7470 733a 2f2f 7777 772e 7073 7963  https://www.psyc
+000026f0: 6f70 672e 6f72 672f 0a5b 7079 6d79 7371  opg.org/.[pymysq
+00002700: 6c5d 3a20 6874 7470 733a 2f2f 6769 7468  l]: https://gith
+00002710: 7562 2e63 6f6d 2f50 794d 7953 514c 2f50  ub.com/PyMySQL/P
+00002720: 794d 7953 514c 0a5b 7079 6f64 6263 5d3a  yMySQL.[pyodbc]:
+00002730: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002740: 636f 6d2f 6d6b 6c65 6568 616d 6d65 722f  com/mkleehammer/
+00002750: 7079 6f64 6263 0a5b 6173 796e 6370 675d  pyodbc.[asyncpg]
+00002760: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00002770: 2e63 6f6d 2f4d 6167 6963 5374 6163 6b2f  .com/MagicStack/
+00002780: 6173 796e 6370 670a 5b61 696f 7067 5d3a  asyncpg.[aiopg]:
+00002790: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000027a0: 636f 6d2f 6169 6f2d 6c69 6273 2f61 696f  com/aio-libs/aio
+000027b0: 7067 0a5b 6169 6f6d 7973 716c 5d3a 2068  pg.[aiomysql]: h
+000027c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000027d0: 6d2f 6169 6f2d 6c69 6273 2f61 696f 6d79  m/aio-libs/aiomy
+000027e0: 7371 6c0a 5b61 7379 6e63 6d79 5d3a 2068  sql.[asyncmy]: h
+000027f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002800: 6d2f 6c6f 6e67 3269 6365 2f61 7379 6e63  m/long2ice/async
+00002810: 6d79 0a5b 6169 6f73 716c 6974 655d 3a20  my.[aiosqlite]: 
+00002820: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002830: 6f6d 2f6f 6d6e 696c 6962 2f61 696f 7371  om/omnilib/aiosq
+00002840: 6c69 7465 0a5b 6169 6f6f 6462 635d 3a20  lite.[aioodbc]: 
+00002850: 6874 7470 733a 2f2f 6169 6f6f 6462 632e  https://aioodbc.
+00002860: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00002870: 6e2f 6c61 7465 7374 2f0a 0a5b 6573 6d65  n/latest/..[esme
+00002880: 7261 6c64 5d3a 2068 7474 7073 3a2f 2f67  rald]: https://g
+00002890: 6974 6875 622e 636f 6d2f 6479 6d6d 6f6e  ithub.com/dymmon
+000028a0: 642f 6573 6d65 7261 6c64 0a5b 7374 6172  d/esmerald.[star
+000028b0: 6c65 7474 655d 3a20 6874 7470 733a 2f2f  lette]: https://
+000028c0: 6769 7468 7562 2e63 6f6d 2f65 6e63 6f64  github.com/encod
+000028d0: 652f 7374 6172 6c65 7474 650a 5b73 616e  e/starlette.[san
+000028e0: 6963 5d3a 2068 7474 7073 3a2f 2f67 6974  ic]: https://git
+000028f0: 6875 622e 636f 6d2f 6875 6765 2d73 7563  hub.com/huge-suc
+00002900: 6365 7373 2f73 616e 6963 0a5b 7265 7370  cess/sanic.[resp
+00002910: 6f6e 6465 725d 3a20 6874 7470 733a 2f2f  onder]: https://
+00002920: 6769 7468 7562 2e63 6f6d 2f6b 656e 6e65  github.com/kenne
+00002930: 7468 7265 6974 7a2f 7265 7370 6f6e 6465  threitz/responde
+00002940: 720a 5b71 7561 7274 5d3a 2068 7474 7073  r.[quart]: https
+00002950: 3a2f 2f67 6974 6c61 622e 636f 6d2f 7067  ://gitlab.com/pg
+00002960: 6a6f 6e65 732f 7175 6172 740a 5b61 696f  jones/quart.[aio
+00002970: 6874 7470 5d3a 2068 7474 7073 3a2f 2f67  http]: https://g
+00002980: 6974 6875 622e 636f 6d2f 6169 6f2d 6c69  ithub.com/aio-li
+00002990: 6273 2f61 696f 6874 7470 0a5b 746f 726e  bs/aiohttp.[torn
+000029a0: 6164 6f5d 3a20 6874 7470 733a 2f2f 6769  ado]: https://gi
+000029b0: 7468 7562 2e63 6f6d 2f74 6f72 6e61 646f  thub.com/tornado
+000029c0: 7765 622f 746f 726e 6164 6f0a 5b66 6173  web/tornado.[fas
+000029d0: 7461 7069 5d3a 2068 7474 7073 3a2f 2f67  tapi]: https://g
+000029e0: 6974 6875 622e 636f 6d2f 7469 616e 676f  ithub.com/tiango
+000029f0: 6c6f 2f66 6173 7461 7069 0a              lo/fastapi.
```

