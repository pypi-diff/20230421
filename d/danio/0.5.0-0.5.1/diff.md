# Comparing `tmp/danio-0.5.0.tar.gz` & `tmp/danio-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danio-0.5.0.tar", max compression
+gzip compressed data, was "danio-0.5.1.tar", max compression
```

## Comparing `danio-0.5.0.tar` & `danio-0.5.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1520 2022-01-31 15:49:34.471987 danio-0.5.0/LICENSE
--rw-r--r--   0        0        0      804 2022-12-12 13:15:30.319797 danio-0.5.0/danio/__init__.py
--rw-r--r--   0        0        0     1087 2022-03-22 10:12:20.218642 danio-0.5.0/danio/aiopg.py
--rw-r--r--   0        0        0     1202 2022-03-22 10:12:20.218642 danio-0.5.0/danio/asyncpg.py
--rw-r--r--   0        0        0      840 2022-04-08 08:00:49.924962 danio-0.5.0/danio/database.py
--rw-r--r--   0        0        0      182 2022-03-18 10:19:16.165730 danio-0.5.0/danio/exception.py
--rw-r--r--   0        0        0     1668 2022-12-10 13:26:22.577218 danio-0.5.0/danio/manage.py
--rw-r--r--   0        0        0    60792 2022-12-12 13:15:30.319797 danio-0.5.0/danio/model.py
--rw-r--r--   0        0        0      925 2022-06-18 06:15:32.690275 danio-0.5.0/danio/mysql.py
--rw-r--r--   0        0        0      873 2022-03-22 10:12:20.222642 danio-0.5.0/danio/sqlite.py
--rw-r--r--   0        0        0     1651 2021-12-16 08:58:59.799999 danio-0.5.0/danio/utils.py
--rw-r--r--   0        0        0     3749 2022-03-22 10:12:20.222642 danio-0.5.0/docs/index.md
--rw-r--r--   0        0        0     1201 2022-12-12 13:15:55.331214 danio-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4524 2022-12-12 13:16:24.519317 danio-0.5.0/setup.py
--rw-r--r--   0        0        0     4612 2022-12-12 13:16:24.519613 danio-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-01-31 15:49:34.471987 danio-0.5.1/LICENSE
+-rw-r--r--   0        0        0      828 2023-04-21 05:58:13.584383 danio-0.5.1/danio/__init__.py
+-rw-r--r--   0        0        0     1087 2022-03-22 10:12:20.218642 danio-0.5.1/danio/aiopg.py
+-rw-r--r--   0        0        0     1202 2022-03-22 10:12:20.218642 danio-0.5.1/danio/asyncpg.py
+-rw-r--r--   0        0        0      851 2023-04-21 05:58:13.584383 danio-0.5.1/danio/database.py
+-rw-r--r--   0        0        0      182 2022-03-18 10:19:16.165730 danio-0.5.1/danio/exception.py
+-rw-r--r--   0        0        0     3902 2023-04-21 05:58:13.584383 danio-0.5.1/danio/manage.py
+-rw-r--r--   0        0        0    21160 2023-04-21 05:58:13.584383 danio-0.5.1/danio/model.py
+-rw-r--r--   0        0        0      925 2022-06-18 06:15:32.690275 danio-0.5.1/danio/mysql.py
+-rw-r--r--   0        0        0    41031 2023-04-21 05:58:13.584383 danio-0.5.1/danio/schema.py
+-rw-r--r--   0        0        0      873 2022-03-22 10:12:20.222642 danio-0.5.1/danio/sqlite.py
+-rw-r--r--   0        0        0     1651 2021-12-16 08:58:59.799999 danio-0.5.1/danio/utils.py
+-rw-r--r--   0        0        0     4727 2023-04-21 05:58:13.584383 danio-0.5.1/docs/index.md
+-rw-r--r--   0        0        0     1201 2023-04-21 05:58:26.072080 danio-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5523 1970-01-01 00:00:00.000000 danio-0.5.1/setup.py
+-rw-r--r--   0        0        0     5792 1970-01-01 00:00:00.000000 danio-0.5.1/PKG-INFO
```

### Comparing `danio-0.5.0/LICENSE` & `danio-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/danio/__init__.py` & `danio-0.5.1/danio/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from . import manage
 from .database import Database
 from .exception import SchemaException, ValidateException
 from .model import (
+    Model,
+)
+from .schema import (
     Operation,
     CharField,
     DateField,
     DateTimeField,
     Field,
     FloatField,
     DecimalField,
     IntField,
     TinyIntField,
     SmallIntField,
     BigIntField,
     BoolField,
     JsonField,
-    Model,
     Schema,
     TextField,
     TimeField,
     field,
 )
 
 __all__ = (
```

### Comparing `danio-0.5.0/danio/aiopg.py` & `danio-0.5.1/danio/aiopg.py`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/danio/asyncpg.py` & `danio-0.5.1/danio/asyncpg.py`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/danio/database.py` & `danio-0.5.1/danio/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 class Database(_Database):
     class Type(enum.Enum):
         MYSQL = "mysql"
         POSTGRES = "postgres"
         SQLITE = "sqlite"
 
-        @property
-        def quote(self) -> str:
+        def quote(self, content: str) -> str:
+            qt = "`"
             if self == self.POSTGRES:
-                return '"'
-            else:
-                return "`"
+                qt = '"'
+
+            return f"{qt}{content}{qt}"
 
     SUPPORTED_BACKENDS = {
         "mysql": "danio.mysql:MySQLBackend",
         "sqlite": "danio.sqlite:SQLiteBackend",
         "postgres": "danio.asyncpg:PostgresBackend",
         "aiopg": "danio.aiopg:PostgresBackend",
     }
```

### Comparing `danio-0.5.0/danio/model.py` & `danio-0.5.1/danio/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-"""
-Base ORM model with CRUD
-"""
 from __future__ import annotations
 
 import copy
 import dataclasses
 import decimal
 import enum
 import itertools
 import json
 import random
 import re
 import typing
-import warnings
 from collections import defaultdict
-from contextvars import ContextVar
 from datetime import datetime, timedelta
 from functools import reduce
 
 import cached_property
 import sqlalchemy
 
 from . import exception
 from .database import Database
-from .utils import class_property
 
-MODEL_TV = typing.TypeVar("MODEL_TV", bound="Model")
+if typing.TYPE_CHECKING:
+    from .model import MODEL_TV
+else:
+    MODEL_TV = typing.TypeVar("MODEL_TV")
+
 SCHEMA_TV = typing.TypeVar("SCHEMA_TV", bound="Schema")
 MIGRATION_TV = typing.TypeVar("MIGRATION_TV", bound="Migration")
-CRUD_TV = typing.TypeVar("CRUD_TV", bound="Crud")
 MARKER_TV = typing.TypeVar("MARKER_TV", bound="SQLMarker")
+CRUD_TV = typing.TypeVar("CRUD_TV", bound="Crud")
 CASE_TV = typing.TypeVar("CASE_TV", bound="SQLCase")
 
 
+def join(*contents, delimiter=" ") -> str:
+    return delimiter.join(tuple(filter(lambda c: c, contents)))
+
+
 @dataclasses.dataclass
 class Field:
     class FieldDefault:
         pass
 
     class NoDefault:
         pass
@@ -103,34 +105,36 @@
 
     def contains(self, values: typing.Sequence) -> SQLExpression:
         if not values:
             raise ValueError("Empty values")
 
         return SQLExpression(field=self, values=[(SQLExpression.Operator.IN, values)])
 
+    def like(self, value: typing.Any) -> SQLExpression:
+        return SQLExpression(field=self, values=[(SQLExpression.Operator.LK, value)])
+
     def case(
         self,
         expression: SQLExpression,
         value: typing.Any,
         default: typing.Any = None,
     ) -> SQLCase:
         return SQLCase(
             field=self, default=default or self.default, cast_type=self.type
         ).case(expression, value)
 
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
-        qt = type.quote
-        not_null = " NOT NULL " if self.not_null else " "
+        not_null = "NOT NULL" if self.not_null else ""
         if type == type.MYSQL:
-            return f"{qt}{self.name}{qt} {self.type}{not_null}{'AUTO_INCREMENT ' if self.auto_increment else ' '}COMMENT '{self.comment}'"
+            return f"{type.quote(self.name)} {self.type} {not_null} {'AUTO_INCREMENT' if self.auto_increment else ''} COMMENT '{self.comment}'"
         elif type == type.POSTGRES:
             # only support "serail" type for auto increment field
-            return f"{qt}{self.name}{qt} {self.type}  {'PRIMARY KEY ' if self.primary else ' '}{not_null}"
+            return f"{type.quote(self.name)} {self.type} {'PRIMARY KEY' if self.primary else ''} {not_null}"
         else:
-            return f"{qt}{self.name}{qt} {self.type} {'PRIMARY KEY ' if self.primary else ' '}{'AUTOINCREMENT ' if self.auto_increment else ' '}{not_null if not self.primary else ''}"
+            return f"{type.quote(self.name)} {self.type} {'PRIMARY KEY' if self.primary else ''} {'AUTOINCREMENT' if self.auto_increment else ''} {not_null if not self.primary else ''}"
 
     def to_python(self, value: typing.Any) -> typing.Any:
         """From databases raw to python"""
         if self.enum:
             return self.enum(value)
         return value
 
@@ -196,17 +200,14 @@
 
 @dataclasses.dataclass(eq=False)
 class CharField(Field):
     TYPE: typing.ClassVar[str] = "varchar(255)"
 
     default: str = ""
 
-    def like(self, value: typing.Any) -> SQLExpression:
-        return SQLExpression(field=self, values=[(SQLExpression.Operator.LK, value)])
-
 
 @dataclasses.dataclass(eq=False)
 class TextField(CharField):
     TYPE: typing.ClassVar[str] = "text"
 
     default: str = ""
 
@@ -281,32 +282,31 @@
     name: str = ""
 
     def __post_init__(self):
         if not self.name:
             self.name = f"{'_'.join(f.name for f in self.fields)[:15]}_{random.randint(1, 10000)}{'_uiq' if self.unique else '_idx'}"
 
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
-        qt = type.quote
         if type == type.MYSQL:
-            return (
-                f"{'UNIQUE ' if self.unique else ''}KEY "
-                f"{qt}{self.name}{qt} "
-                f"({', '.join(f'{qt}{f.name}{qt}' for f in self.fields)})"
+            return join(
+                "UNIQUE " if self.unique else "",
+                "KEY",
+                type.quote(self.name),
+                f"({', '.join(type.quote(f.name) for f in self.fields)})",
             )
         else:
             return ""
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(eq=False)
 class Schema:
     name: str
     indexes: typing.List[Index] = dataclasses.field(default_factory=list)
     fields: typing.List[Field] = dataclasses.field(default_factory=list)
     abstracted: bool = False
-    model: typing.Optional[typing.Type[Model]] = None
 
     @cached_property.cached_property
     def primary_field(self) -> Field:
         for f in self.fields:
             if f.primary:
                 return f
         raise exception.SchemaException("Primary field not found!")
@@ -354,60 +354,74 @@
                 other_indexes[k] for k in (other_indexes.keys()) - (self_indexes.keys())
             ],
             add_fields=[f for f in self.fields if f.name not in other_fields],
             drop_fields=[f for f in other.fields if f.name not in self_fields],
             change_type_fields=change_type_fields,
         )
 
+    def __eq__(self, other: object) -> bool:
+        assert isinstance(other, Schema)
+        return not bool((self - other).to_sql())
+
+    def sync_index_name(self: SCHEMA_TV, other: SCHEMA_TV) -> SCHEMA_TV:
+        if self != other:
+            raise ValueError("Not migrated!")
+        serialize = (
+            lambda idx: f"{idx.unique}_{'_'.join(sorted(f.name for f in idx.fields))}"
+        )
+        indexes = {serialize(idx): idx for idx in other.indexes}
+        for idx in self.indexes:
+            idx.name = indexes[serialize(idx)].name
+        return self
+
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
         assert self.primary_field
-        qt = type.quote
 
         if type == type.MYSQL:
-            keys = [f"PRIMARY KEY ({qt}{self.primary_field.name}{qt})"]
+            keys = [f"PRIMARY KEY ({type.quote(self.primary_field.name)})"]
             postfix = (
                 " ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;"
             )
         elif type == type.POSTGRES:
             keys = []
             postfix = ";"
         else:
             keys = []
             postfix = ";"
 
         if type == type.MYSQL:
             keys.extend([index.to_sql(type=type) for index in self.indexes])
 
         sql = (
-            f"CREATE TABLE {qt}{self.name}{qt} (\n"
+            f"CREATE TABLE {type.quote(self.name)} (\n"
             + ",\n".join(
                 itertools.chain((v.to_sql(type=type) for v in self.fields), keys)
             )
             + f"\n){postfix}"
         )
         if type != Database.Type.MYSQL:
             _sqls = []
             for index in self.indexes:
                 _sqls.append(
-                    f"CREATE {'UNIQUE ' if index.unique else ' '}INDEX {qt}{index.name}{qt} on {qt}{self.name}{qt} ({', '.join(f'{qt}{f.name}{qt}' for f in index.fields)});"
+                    f"CREATE {'UNIQUE ' if index.unique else ' '}INDEX {type.quote(index.name)} on {type.quote(self.name)} ({', '.join(f'{type.quote(f.name)}' for f in index.fields)});"
                 )
             sql += "\n".join(_sqls)
         if type == type.POSTGRES:
             _sqls = []
             for f in self.fields:
                 if f.comment:
                     _sqls.append(
                         f'COMMENT ON COLUMN "{self.name}"."{f.name}" is \'{f.comment}\';'
                     )
             sql += "\n".join(_sqls)
         return sql
 
     @classmethod
-    def from_model(cls: typing.Type[SCHEMA_TV], m: typing.Type[Model]) -> SCHEMA_TV:
-        schema = cls(name=m.table_name, model=m)
+    def from_model(cls: typing.Type[SCHEMA_TV], m: typing.Type[MODEL_TV]) -> SCHEMA_TV:
+        schema = cls(name=m.table_name)
         schema.abstracted = m.table_abstracted
         # fields
         for f in dataclasses.fields(m):
             if isinstance(f.default, Field):  # from dataclass default
                 f.default.model_name = f.name
                 if not f.default.name:
                     f.default.name = f.name
@@ -423,14 +437,15 @@
                         meta.model_name = f.name
                         if not meta.name:
                             meta.name = f.name
                             meta.__post_init__()
                         meta.default = f.default
                         schema.fields.append(meta)
                         setattr(m, f.name, meta)
+                        setattr(m, f.name.upper(), meta)
         fields = {f.model_name: f for f in schema.fields}
         # index
         for i, index_keys in enumerate((m.table_index_keys, m.table_unique_keys)):
             for keys in index_keys:
                 if keys:
                     _fields = []
                     for key in keys:
@@ -443,17 +458,17 @@
                                 f"Index: {keys} not supported"
                             )
                     schema.indexes.append(Index(fields=_fields, unique=i == 1))
         return schema
 
     @classmethod
     async def from_db(
-        cls: typing.Type[SCHEMA_TV], database: Database, m: typing.Type[Model]
+        cls: typing.Type[SCHEMA_TV], database: Database, m: typing.Type[MODEL_TV]
     ) -> typing.Optional[SCHEMA_TV]:
-        schema = cls(name=m.table_name, model=m)
+        schema = cls(name=m.table_name)
         model_names = {f.name: f.model_name for f in m.schema.fields}
         if database.type == database.type.MYSQL:
             field_name_pattern = re.compile(r"`([^ ,]*)`")
             try:
                 for line in (
                     await database.fetch_all(f"SHOW CREATE TABLE {m.table_name}")
                 )[0][1].split("\n")[1:-1]:
@@ -599,68 +614,66 @@
             drop_fields=self.add_fields,
             change_type_fields=change_type_fields,
             add_indexes=self.drop_indexes,
             drop_indexes=self.add_indexes,
         )
 
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
-        qt = type.quote
-
         sqls = []
         if self.schema and not self.old_schema:
             return self.schema.to_sql(type=type)
         elif self.old_schema and not self.schema:
-            sqls.append(f"DROP TABLE {qt}{self.old_schema.name}{qt}")
+            sqls.append(f"DROP TABLE {type.quote(self.old_schema.name)}")
         elif self.schema and self.old_schema:
             if self.old_schema.name != self.schema.name:
                 sqls.append(
-                    f"ALTER TABLE {qt}{self.old_schema.name}{qt} RENAME {qt}{self.schema.name}{qt}"
+                    f"ALTER TABLE {type.quote(self.old_schema.name)} RENAME {type.quote(self.schema.name)}"
                 )
             for i in self.drop_indexes:
                 if type == type.MYSQL:
                     if not set(f.name for f in i.fields) & set(
                         f.name for f in self.drop_fields
                     ):
                         sqls.append(
-                            f"ALTER TABLE {qt}{self.schema.name}{qt} DROP INDEX {qt}{i.name}{qt}"
+                            f"ALTER TABLE {type.quote(self.schema.name)} DROP INDEX {type.quote(i.name)}"
                         )
                 else:
-                    sqls.append(f"DROP INDEX {qt}{i.name}{qt}")
+                    sqls.append(f"DROP INDEX {type.quote(i.name)}")
             for f in self.add_fields:
                 sqls.append(
-                    f"ALTER TABLE {qt}{self.schema.name}{qt} ADD COLUMN {f.to_sql(type=type)}"
+                    f"ALTER TABLE {type.quote(self.schema.name)} ADD COLUMN {f.to_sql(type=type)}"
                 )
                 if not isinstance(f.default_value, f.NoDefault):
                     sqls[
                         -1
                     ] += f" DEFAULT {sqlalchemy.text(':df').bindparams(df=f.to_database(f.default_value)).compile(compile_kwargs={'literal_binds': True})}"
                     if type != Database.Type.SQLITE:
                         sqls.append(
-                            f"ALTER TABLE {qt}{self.schema.name}{qt} ALTER COLUMN {qt}{f.name}{qt} DROP DEFAULT"
+                            f"ALTER TABLE {type.quote(self.schema.name)} ALTER COLUMN {type.quote(f.name)} DROP DEFAULT"
                         )
             for f in self.drop_fields:
                 sqls.append(
-                    f"ALTER TABLE {qt}{self.schema.name}{qt} DROP COLUMN {qt}{f.name}{qt}"
+                    f"ALTER TABLE {type.quote(self.schema.name)} DROP COLUMN {type.quote(f.name)}"
                 )
             for f in self.change_type_fields:
                 if type == type.SQLITE:
                     raise exception.OperationException(
                         "Type changing not allowed in SQLite"
                     )
                 elif type == type.MYSQL:
                     sqls.append(
-                        f"ALTER TABLE {qt}{self.schema.name}{qt} MODIFY {qt}{f.name}{qt} {f.type}"
+                        f"ALTER TABLE {type.quote(self.schema.name)} MODIFY {type.quote(f.name)} {f.type}"
                     )
                 else:
                     sqls.append(
-                        f"ALTER TABLE {qt}{self.schema.name}{qt} ALTER COLUMN {qt}{f.name}{qt} TYPE {f.type}"
+                        f"ALTER TABLE {type.quote(self.schema.name)} ALTER COLUMN {type.quote(f.name)} TYPE {f.type}"
                     )
             for i in self.add_indexes:
                 sqls.append(
-                    f"CREATE {'UNIQUE ' if i.unique else ''}INDEX {qt}{i.name}{qt} on {qt}{self.schema.name}{qt} ({','.join(qt + f.name + qt for f in i.fields)})"
+                    f"CREATE {'UNIQUE ' if i.unique else ''}INDEX {type.quote(i.name)} on {type.quote(self.schema.name)} ({','.join(type.quote(f.name) for f in i.fields)})"
                 )
         if sqls:
             sqls[-1] += ";"
 
         return ";\n".join(sqls)
 
 
@@ -668,511 +681,14 @@
 class Operation(enum.IntEnum):
     CREATE = 1
     READ = 2
     UPDATE = 3
     DELETE = 4
 
 
-@dataclasses.dataclass
-class Model:
-    DATABASE: typing.ClassVar[ContextVar[typing.Optional[Database]]] = ContextVar(
-        "database"
-    )
-
-    id: typing.Annotated[int, IntField(primary=True, auto_increment=True)] = 0
-    # for table schema
-    _table_prefix: typing.ClassVar[str] = ""
-    _table_name_prefix: typing.ClassVar[str] = ""
-    _table_name_snake_case: typing.ClassVar[bool] = False
-    _table_index_keys: typing.ClassVar[
-        typing.Tuple[typing.Tuple[typing.Any, ...], ...]
-    ] = tuple()
-    _table_unique_keys: typing.ClassVar[
-        typing.Tuple[typing.Tuple[typing.Any, ...], ...]
-    ] = tuple()
-    _table_abstracted: typing.ClassVar[
-        bool
-    ] = True  # do not impact subclass, default false for every child class except defined as true
-    _schema: typing.ClassVar[typing.Optional[Schema]] = None
-
-    @class_property
-    @classmethod
-    def table_name(cls) -> str:
-        return cls.get_table_name()
-
-    @class_property
-    @classmethod
-    def table_index_keys(cls) -> typing.Tuple[typing.Tuple[typing.Any, ...], ...]:
-        return cls.get_table_index_keys()
-
-    @class_property
-    @classmethod
-    def table_unique_keys(cls) -> typing.Tuple[typing.Tuple[typing.Any, ...], ...]:
-        return cls.get_table_unique_keys()
-
-    @class_property
-    @classmethod
-    def table_abstracted(cls) -> bool:
-        return cls.__dict__.get("_table_abstracted", False)
-
-    @class_property
-    @classmethod
-    def schema(cls) -> Schema:
-        if not cls._schema or not cls._schema.model or cls._schema.model is not cls:
-            cls._schema = Schema.from_model(cls)
-        return cls._schema
-
-    @property
-    def primary(self) -> int:
-        assert self.schema.primary_field
-        return getattr(self, self.schema.primary_field.model_name)
-
-    def __post_init__(self):
-        self.after_init()
-
-    def after_init(self):
-        for f in self.schema.fields:
-            value = getattr(self, f.model_name)
-            if isinstance(value, Field):
-                setattr(self, f.model_name, f.default_value)
-
-    async def after_read(self):
-        pass
-
-    async def before_create(self, validate: bool = True):
-        if validate:
-            await self.validate()
-
-    async def after_create(self):
-        pass
-
-    async def before_update(self, validate: bool = True):
-        if validate:
-            await self.validate()
-
-    async def after_update(self):
-        pass
-
-    async def before_save(self):
-        pass
-
-    async def after_save(self):
-        pass
-
-    async def before_delete(self):
-        pass
-
-    async def after_delete(self):
-        pass
-
-    async def validate(self):
-        for f in self.schema.fields:
-            value = getattr(self, f.model_name)
-            # choices
-            if f.enum:
-                if isinstance(value, enum.Enum):
-                    value = value.value
-                if value not in set((c.value for c in f.enum)):
-                    raise exception.ValidateException(
-                        f"{self.__class__.__name__}.{f.model_name} value: {value} not in choices: {f.enum}"
-                    )
-            # no default
-            if isinstance(value, f.NoDefault):
-                raise exception.ValidateException(
-                    f"{self.table_name}.{f.model_name} required!"
-                )
-
-    def dump(
-        self,
-        fields: typing.Sequence[Field] = (),
-        ignore_fields: typing.Sequence[Field] = (),
-    ) -> typing.Dict[str, typing.Any]:
-        """Dump model to dict with only database fields"""
-        data = {}
-        _ignore_fields = {f.name for f in ignore_fields}
-        for f in fields or self.schema.fields:
-            if f.name in _ignore_fields:
-                continue
-            data[f.name] = getattr(self, f.model_name)
-
-        return data
-
-    async def create(
-        self: MODEL_TV,
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = (),
-        ignore_fields: typing.Sequence[Field] = (),
-        validate: bool = True,
-    ):
-        data = self.dump(fields=fields, ignore_fields=ignore_fields)
-        if (
-            self.schema.primary_field.name in data
-            and not data[self.schema.primary_field.name]
-        ):
-            data.pop(self.schema.primary_field.name)
-        await self.before_create(validate=validate)
-        setattr(
-            self,
-            self.schema.primary_field.model_name,
-            (
-                await Insert(
-                    model=self.__class__, database=database, insert_data=[data]
-                ).exec()
-            )[0],
-        )
-        await self.after_create()
-        return self
-
-    async def update(
-        self: MODEL_TV,
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = (),
-        ignore_fields: typing.Sequence[Field] = (),
-        validate: bool = True,
-    ) -> bool:
-        """
-        For PostgreSQL/SQLite, always return True
-        """
-        assert self.primary
-        await self.before_update(validate=validate)
-        data = self.dump(fields=fields, ignore_fields=ignore_fields)
-        rowcount = await self.__class__.where(
-            self.schema.primary_field == self.primary,
-            database=database,
-        ).update(**data)
-        await self.after_update()
-        return rowcount > 0
-
-    async def save(
-        self: MODEL_TV,
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = (),
-        ignore_fields: typing.Sequence[Field] = (),
-        force_insert=False,
-        validate: bool = True,
-    ) -> MODEL_TV:
-        await self.before_save()
-        if self.primary and not force_insert:
-            await self.update(
-                database=database,
-                fields=fields,
-                ignore_fields=ignore_fields,
-                validate=validate,
-            )
-        else:
-            await self.create(
-                database=database,
-                fields=fields,
-                ignore_fields=ignore_fields,
-                validate=validate,
-            )
-        await self.after_save()
-        return self
-
-    async def delete(
-        self,
-        database: typing.Optional[Database] = None,
-    ) -> bool:
-        await self.before_delete()
-        row_count = await self.__class__.where(
-            self.schema.primary_field == self.primary, database=database
-        ).delete()
-        await self.after_delete()
-        return row_count > 0
-
-    async def refetch(
-        self: MODEL_TV,
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = tuple(),
-    ) -> MODEL_TV:
-        new = await self.__class__.where(
-            self.schema.primary_field == self.primary, database=database
-        ).fetch_one(fields=fields)
-        db_fields = {f.model_name for f in fields} or {
-            f.model_name for f in self.schema.fields
-        }
-        for f in dataclasses.fields(self):
-            if f.name in db_fields:
-                setattr(self, f.name, getattr(new, f.name))
-        return self
-
-    async def get_or_create(
-        self: MODEL_TV,
-        key_fields: typing.Sequence[Field],
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = (),
-        validate: bool = True,
-        for_update: bool = False,
-    ) -> typing.Tuple[MODEL_TV, bool]:
-        if not database:
-            # using write db by default
-            database = self.__class__.get_database(Operation.CREATE, self.table_name)
-        conditions = []
-        created = False
-        for f in key_fields:
-            conditions.append(f == getattr(self, f.model_name))
-        where = self.__class__.where(*conditions, database=database)
-        if for_update:
-            where = where.for_update()
-        ins = await where.fetch_one(fields=fields)
-        if not ins:
-            try:
-                ins = await self.create(
-                    database=database, fields=fields, validate=validate
-                )
-                created = True
-            except exception.IntegrityError as e:
-                where = self.__class__.where(*conditions, database=database)
-                if for_update:
-                    where = where.for_update()
-                ins = await where.fetch_one(fields=fields)
-                if not ins:
-                    raise e
-        assert ins
-        return ins, created
-
-    async def create_or_update(
-        self: MODEL_TV,
-        key_fields: typing.Sequence[Field],
-        database: typing.Optional[Database] = None,
-        fields: typing.Sequence[Field] = (),
-        update_fields: typing.Sequence[Field] = (),
-        for_update: bool = True,
-        validate: bool = True,
-    ) -> typing.Tuple[MODEL_TV, bool, bool]:
-        """Try get_or_create then update.
-
-        For SQLite, updated will always be True.
-        """
-        if not database:
-            database = self.__class__.get_database(Operation.CREATE, self.table_name)
-        if fields and self.schema.primary_field.name not in (f.name for f in fields):
-            fields = list(fields)
-            fields.append(self.schema.primary_field)
-
-        created = False
-        updated = False
-        async with database.transaction():
-            ins, created = await self.get_or_create(
-                key_fields,
-                database=database,
-                fields=fields,
-                validate=validate,
-                for_update=for_update,
-            )
-            if not created:
-                setattr(self, self.schema.primary_field.model_name, ins.primary)
-                updated = await self.update(validate=validate, fields=update_fields)
-                ins = self
-        return ins, created, updated
-
-    @classmethod
-    def get_table_name(cls) -> str:
-        prefix = cls._table_name_prefix or cls._table_prefix
-        if cls._table_name_snake_case:
-            return prefix + re.sub(r"(?P<n>[A-Z])", r"_\g<n>", cls.__name__).lower()[1:]
-        else:
-            return prefix + cls.__name__.lower()
-
-    @classmethod
-    def get_table_index_keys(cls) -> typing.Tuple[typing.Tuple[typing.Any, ...], ...]:
-        return cls._table_index_keys
-
-    @classmethod
-    def get_table_unique_keys(cls) -> typing.Tuple[typing.Tuple[typing.Any, ...], ...]:
-        return cls._table_unique_keys
-
-    @classmethod
-    def get_database(
-        cls, operation: Operation, table: str, *args, **kwargs
-    ) -> Database:
-        """Get database instance, route database by operation"""
-        db = cls.DATABASE.get()
-        if not db:
-            raise RuntimeError("No database provide")
-        return db
-
-    @classmethod
-    def load(
-        cls: typing.Type[MODEL_TV], rows: typing.List[typing.Mapping]
-    ) -> typing.List[MODEL_TV]:
-        """Load DB data to model"""
-        instances = []
-        for row in rows:
-            data = {}
-            for f in cls.schema.fields:
-                if f.name in row:
-                    data[f.model_name] = f.to_python(row[f.name])
-            instances.append(cls(**data))
-        return instances
-
-    @classmethod
-    def where(
-        cls: typing.Type[MODEL_TV],
-        *conditions: SQLExpression,
-        database: typing.Optional[Database] = None,
-        raw="",
-        is_and=True,
-    ) -> Crud[MODEL_TV]:
-        cls.schema
-        return Crud(model=cls, database=database).where(
-            *conditions, is_and=is_and, raw=raw
-        )
-
-    @classmethod
-    async def upsert(
-        cls,
-        insert_data: typing.List[typing.Dict[str, typing.Any]],
-        database: typing.Optional[Database] = None,
-        update_fields: typing.Sequence[str] = (),
-        conflict_targets: typing.Sequence[str] = (),
-    ) -> typing.Tuple[bool, bool]:
-        """
-        Using insert on duplicate:
-          https://dev.mysql.com/doc/refman/5.6/en/insert-on-duplicate.html
-          https://www.sqlite.org/lang_upsert.html
-          https://www.postgresql.org/docs/9.4/plpgsql-control-structures.html#PLPGSQL-ERROR-TRAPPING
-
-        For MySQL, rowcount=2 means the table has been updated
-        For SQLITE, rowcount!=0 will always be true
-        For PostgreSQL, last_id != 0 and rowcount != 0 always be true
-        """
-        insert = Insert(
-            model=cls,
-            database=database,
-            insert_data=insert_data,
-            update_fields=update_fields,
-            conflict_targets=conflict_targets,
-        )
-        last_id, rowcount = await insert.exec()
-        if insert.get_database().type == Database.Type.MYSQL:
-            return rowcount == 1, rowcount == 2
-        else:
-            return last_id != 0, rowcount != 0
-
-    @classmethod
-    async def bulk_create(
-        cls: typing.Type[MODEL_TV],
-        instances: typing.Sequence[MODEL_TV],
-        fields: typing.Sequence[Field] = (),
-        database: typing.Optional[Database] = None,
-        validate: bool = True,
-    ) -> typing.Sequence[MODEL_TV]:
-        assert cls.schema.primary_field
-        if not database:
-            database = cls.get_database(Operation.CREATE, cls.table_name)
-        if (
-            database.type != database.type.POSTGRES
-            and not cls.schema.primary_field.auto_increment
-        ):
-            raise exception.OperationException(
-                f"{cls}'s primary_field must be auto incremented!"
-            )
-        if (
-            database.type == database.type.POSTGRES
-            and "serial" not in cls.schema.primary_field.type
-        ):
-            raise exception.OperationException(
-                f"{cls}'s primary_field must be auto incremented!"
-            )
-
-        for ins in instances:
-            await ins.before_create(validate=validate)
-        data = [ins.dump(fields=fields) for ins in instances]
-        if database.type != Database.Type.MYSQL:
-            for d in data:
-                if (
-                    cls.schema.primary_field.name in d
-                    and not d[cls.schema.primary_field.name]
-                ):
-                    d.pop(cls.schema.primary_field.name)
-            if len({len(d) for d in data}) != 1:
-                raise exception.OperationException(
-                    "For SQLite or PostgreSQL, all instances either have primary key value or none"
-                )
-
-        next_ins_id = (
-            await Insert(model=cls, database=database, insert_data=data).exec()
-        )[0]
-        if database.type == database.type.MYSQL:
-            for ins in instances:
-                if not ins.primary:
-                    setattr(ins, cls.schema.primary_field.model_name, next_ins_id)
-                next_ins_id = ins.primary + 1
-        else:
-            for ins in reversed(instances):
-                if not ins.primary:
-                    setattr(ins, cls.schema.primary_field.model_name, next_ins_id)
-                next_ins_id = ins.primary - 1
-
-        for ins in instances:
-            await ins.after_create()
-        return instances
-
-    @classmethod
-    async def bulk_update(
-        cls: typing.Type[MODEL_TV],
-        instances: typing.Sequence[MODEL_TV],
-        fields: typing.Sequence[Field] = (),
-        database: typing.Optional[Database] = None,
-        validate: bool = True,
-    ) -> typing.Sequence[MODEL_TV]:
-        assert cls.schema.primary_field
-        for ins in instances:
-            await ins.before_update(validate=validate)
-
-        data = []
-        for ins in instances:
-            assert ins.primary, "Need primary"
-            data.append(ins.dump(fields=fields))
-            data[-1][cls.schema.primary_field.name] = ins.primary
-
-        await CaseUpdate(
-            model=cls,
-            database=database,
-            data=data,
-        ).exec()
-
-        for ins in instances:
-            await ins.after_update()
-        return instances
-
-    @classmethod
-    async def bulk_delete(
-        cls,
-        instances: typing.Sequence[MODEL_TV],
-        database: typing.Optional[Database] = None,
-    ) -> int:
-        for ins in instances:
-            await ins.before_delete()
-        row_count = await cls.where(
-            cls.schema.primary_field.contains(tuple(ins.primary for ins in instances)),
-            database=database,
-        ).delete()
-        for ins in instances:
-            await ins.after_delete()
-        return row_count
-
-    # deprecation
-    @classmethod
-    async def count(cls, *args, **kwargs):
-        warnings.warn("Will discard", DeprecationWarning)
-        return await cls.where(*args, **kwargs).fetch_count()
-
-    @classmethod
-    async def select(cls, *args, **kwargs):
-        warnings.warn("Will discard", DeprecationWarning)
-        return await cls.where(*args, **kwargs).fetch_all()
-
-    @classmethod
-    async def get(cls, *args, **kwargs):
-        warnings.warn("Will discard", DeprecationWarning)
-        return await cls.where(*args, **kwargs).fetch_one()
-
-
 # query builder
 @dataclasses.dataclass
 class SQLMarker:
     class ID:
         def __init__(self, value: int = 0) -> None:
             self.value: int = value
 
@@ -1195,15 +711,15 @@
         self._var_index = other._var_index
         return self
 
     def _parse(
         self, value: typing.Any, type: Database.Type = Database.Type.MYSQL
     ) -> str:
         if isinstance(value, Field):
-            return f"{type.quote}{value.name}{type.quote}"
+            return type.quote(value.name)
         elif isinstance(value, SQLMarker):
             return value.sync(self).to_sql(type=type)
         elif self.field:
             return f":{self.mark(self.field.to_database(value))}"
         else:
             return f":{self.mark(value)}"
 
@@ -1280,17 +796,16 @@
 
     def __or__(self, other: object) -> SQLExpression:
         self.values.append((self.Operator.OR, other))
         return self
 
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
         assert self.field
-        qt = type.quote
 
-        sql = f"{qt}{self.field.name}{qt}"
+        sql = f"{type.quote(self.field.name)}"
         for op, value in self.values:
             if op == self.Operator.IN:
                 sql += f" {op.value} ({', '.join(self._parse(v, type=type) for v in value)})"
             elif op == self.Operator.LK:
                 sql += f" {op.value} :{self.mark(value)}"
             elif isinstance(value, SQLExpression):
                 sql = f"({sql}) {op.value} ({self._parse(value, type=type)})"
@@ -1324,35 +839,20 @@
         sql += f" ELSE {self._parse(self.default, type=type)}{cast_type} END"
 
         return sql
 
 
 @dataclasses.dataclass
 class BaseSQLBuilder(SQLMarker):
-    OPERATION: typing.ClassVar[Operation] = Operation.READ
-
-    model: typing.Optional[typing.Type[Model]] = None
-    database: typing.Optional[Database] = None
-
-    def get_database(self, operation: typing.Optional[Operation] = None):
-        assert self.model
-        if not self.database:
-            return self.model.get_database(
-                operation or self.OPERATION, self.model.table_name
-            )
-        else:
-            return self.database
+    pass
 
 
 @dataclasses.dataclass
-class Crud(BaseSQLBuilder, typing.Generic[MODEL_TV]):
-    OPERATION: typing.ClassVar[Operation] = Operation.READ
-
-    model: typing.Optional[typing.Type[MODEL_TV]] = None
-    database: typing.Optional[Database] = None
+class Crud(BaseSQLBuilder):
+    schema: typing.Optional[Schema] = None
     _where: typing.Optional[SQLExpression] = None
     _raw_where: str = ""
     _limit: int = 0
     _offset: int = 0
     _order_by: typing.List[typing.Union[Field, SQLExpression]] = dataclasses.field(
         default_factory=list
     )
@@ -1365,92 +865,14 @@
     _ignore_indexes: typing.List[
         typing.Tuple[typing.Sequence[str], str]
     ] = dataclasses.field(default_factory=list)
     _force_indexes: typing.List[
         typing.Tuple[typing.Sequence[str], str]
     ] = dataclasses.field(default_factory=list)
 
-    async def fetch_all(
-        self,
-        fields: typing.Sequence[Field] = tuple(),
-        ignore_fields: typing.Sequence[Field] = tuple(),
-    ) -> typing.List[MODEL_TV]:
-        assert self.model
-        database = self.get_database(Operation.READ)
-        instances = self.model.load(
-            [
-                dict(r)
-                for r in await database.fetch_all(
-                    self.to_select_sql(
-                        type=database.type, fields=fields, ignore_fields=ignore_fields
-                    ),
-                    self._vars,
-                )
-            ]
-        )
-        for ins in instances:
-            await ins.after_read()
-
-        return instances
-
-    async def fetch_one(
-        self,
-        fields: typing.Sequence[Field] = tuple(),
-        ignore_fields: typing.Sequence[Field] = tuple(),
-    ) -> typing.Optional[MODEL_TV]:
-        assert self.model
-        database = self.get_database(Operation.READ)
-        data = await database.fetch_one(
-            self.to_select_sql(
-                type=database.type, fields=fields, ignore_fields=ignore_fields
-            ),
-            self._vars,
-        )
-        if data:
-            ins = self.model.load([dict(data)])[0]
-            await ins.after_read()
-            return ins
-        else:
-            return None
-
-    async def fetch_row(
-        self,
-        fields: typing.Sequence[Field] = tuple(),
-        ignore_fields: typing.Sequence[Field] = tuple(),
-    ) -> typing.List[typing.Mapping]:
-        database = self.get_database(Operation.READ)
-        return await database.fetch_all(
-            self.to_select_sql(
-                type=database.type, fields=fields, ignore_fields=ignore_fields
-            ),
-            self._vars,
-        )
-
-    async def fetch_count(self) -> int:
-        database = self.get_database(Operation.READ)
-        data = await database.fetch_one(
-            self.to_select_sql(count=True, type=database.type), self._vars
-        )
-        assert data
-        return data[0]
-
-    async def delete(self) -> int:
-        database = self.get_database(Operation.DELETE)
-        return (
-            await database.execute(self.to_delete_sql(type=database.type), self._vars)
-        )[1]
-
-    async def update(self, **data) -> int:
-        database = self.get_database(Operation.UPDATE)
-        return (
-            await database.execute(
-                self.to_update_sql(data, type=database.type), self._vars
-            )
-        )[1]
-
     def where(
         self: CRUD_TV,
         *conditions: SQLExpression,
         raw="",
         is_and=True,
     ) -> CRUD_TV:
         if conditions:
@@ -1508,33 +930,32 @@
     def to_select_sql(
         self,
         count=False,
         type: Database.Type = Database.Type.MYSQL,
         fields: typing.Sequence[Field] = tuple(),
         ignore_fields: typing.Sequence[Field] = tuple(),
     ) -> str:
-        assert self.model
-        qt = type.quote
+        assert self.schema
 
         if not count:
             _ignore_fields = {f.name for f in ignore_fields}
-            sql = f"SELECT {', '.join(f'{qt}{f.name}{qt}' for f in fields or self.model.schema.fields if f.name not in _ignore_fields)} FROM {qt}{self.model.table_name}{qt}"
+            sql = f"SELECT {', '.join(f'{type.quote(f.name)}' for f in fields or self.schema.fields if f.name not in _ignore_fields)} FROM {type.quote(self.schema.name)}"
         else:
-            sql = f"SELECT COUNT(*) FROM {qt}{self.model.table_name}{qt}"
+            sql = f"SELECT COUNT(*) FROM {type.quote(self.schema.name)}"
         if type == type.MYSQL:
             for indexes in self._use_indexes:
-                sql += f" USE INDEX {indexes[1] if indexes[1] else ''} ({','.join(indexes[0])}) "
+                sql += f" USE INDEX {type.quote(indexes[1]) if indexes[1] else ''} ({','.join(type.quote(s) for s in indexes[0])}) "
             for indexes in self._ignore_indexes:
-                sql += f" IGNORE INDEX {indexes[1] if indexes[1] else ''} ({','.join(indexes[0])}) "
+                sql += f" IGNORE INDEX {type.quote(indexes[1]) if indexes[1] else ''} ({','.join(type.quote(s) for s in indexes[0])}) "
             for indexes in self._force_indexes:
-                sql += f" FORCE INDEX {indexes[1] if indexes[1] else ''} ({','.join(indexes[0])}) "
+                sql += f" FORCE INDEX {indexes[1] if indexes[1] else ''} ({','.join(type.quote(s) for s in indexes[0])}) "
         elif type == type.SQLITE:
             _use_indexes = self._use_indexes or self._force_indexes
             if _use_indexes:
-                sql += f" INDEXED BY {_use_indexes[0][0][0]} "
+                sql += f" INDEXED BY {type.quote(_use_indexes[0][0][0])} "
             if self._ignore_indexes:
                 sql += " NOT INDEXED "
         else:
             if self._use_indexes or self._force_indexes or self._ignore_indexes:
                 raise exception.OperationException(
                     "For PostgreSQL - index hints not supported"
                 )
@@ -1542,15 +963,15 @@
             sql += f" WHERE {self._where.sync(self).to_sql(type=type)}"
         elif self._raw_where:
             sql += f" WHERE {self._raw_where}"
         if not count:
             if self._order_by:
                 _order_by_sql = ", ".join(
                     [
-                        f"{qt + od.name + qt if isinstance(od, Field) else od.sync(self).to_sql(type=type)} {'ASC' if self._order_by_asc[i] else 'DESC'}"
+                        f"{type.quote(od.name) if isinstance(od, Field) else od.sync(self).to_sql(type=type)} {'ASC' if self._order_by_asc[i] else 'DESC'}"
                         for i, od in enumerate(self._order_by)
                     ]
                 )
 
                 sql += f" ORDER BY {_order_by_sql}"
             if self._limit:
                 sql += f" LIMIT :{self.mark(self._limit)}"
@@ -1573,73 +994,66 @@
                     sql += " LOCK IN SHARE MODE"
                 else:
                     sql += " FOR SHARE"
 
         return sql + ";"
 
     def to_delete_sql(self, type: Database.Type = Database.Type.MYSQL):
-        assert self.model
-        qt = type.quote
+        assert self.schema
 
-        sql = f"DELETE from {qt}{self.model.table_name}{qt}"
+        sql = f"DELETE from {type.quote(self.schema.name)}"
         if self._where:
             sql += f" WHERE {self._where.sync(self).to_sql(type=type)}"
         return sql + ";"
 
     def to_update_sql(
         self,
         data: typing.Dict[str, typing.Any],
         type: Database.Type = Database.Type.MYSQL,
     ):
-        assert self.model
-        qt = type.quote
+        assert self.schema
 
-        fields = {f.model_name: f for f in self.model.schema.fields}
+        fields = {f.model_name: f for f in self.schema.fields}
         _sqls = []
         for k, v in data.items():
             if isinstance(v, SQLMarker):
-                _sqls.append(f"{qt}{k}{qt} = {v.sync(self).to_sql(type=type)}")
+                _sqls.append(f"{type.quote(k)} = {v.sync(self).to_sql(type=type)}")
             else:
-                _sqls.append(f"{qt}{k}{qt} = :{self.mark(fields[k].to_database(v))}")
-        sql = f"UPDATE {qt}{self.model.table_name}{qt} SET {', '.join(_sqls)}"
+                _sqls.append(
+                    f"{type.quote(k)} = :{self.mark(fields[k].to_database(v))}"
+                )
+        sql = f"UPDATE {type.quote(self.schema.name)} SET {', '.join(_sqls)}"
         if self._where:
             sql += f" WHERE {self._where.sync(self).to_sql(type=type)}"
         return sql + ";"
 
 
 @dataclasses.dataclass
 class Insert(BaseSQLBuilder):
-    OPERATION: typing.ClassVar[Operation] = Operation.CREATE
+    schema: typing.Optional[Schema] = None
     insert_data: typing.Sequence[typing.Dict[str, str]] = dataclasses.field(
         default_factory=list
     )
     update_fields: typing.Sequence[str] = dataclasses.field(default_factory=list)
     conflict_targets: typing.Sequence[str] = dataclasses.field(default_factory=list)
 
-    async def exec(self) -> typing.Tuple[int, int]:
-        """
-        return last_id, row_count
-        """
-        database = self.get_database()
-        return await database.execute(self.to_sql(type=database.type), self._vars)
-
     def to_sql(self, type: Database.Type = Database.Type.MYSQL) -> str:
         assert self.insert_data
-        assert self.model
-        qt = type.quote
-        fields = {f.name: f for f in self.model.schema.fields}
+        assert self.schema
+
+        fields = {f.name: f for f in self.schema.fields}
 
         keys = list(self.insert_data[0].keys())
         vars = []
         for d in self.insert_data:
             _vars = []
             for k in keys:
                 _vars.append(self.mark(fields[k].to_database(d[k])))
             vars.append(_vars)
-        sql = f"INSERT INTO {qt}{self.model.table_name}{qt} ({', '.join(map(lambda x: f'{qt}{x}{qt}', keys))}) VALUES"
+        sql = f"INSERT INTO {type.quote(self.schema.name)} ({', '.join(map(lambda x: f'{type.quote(x)}', keys))}) VALUES"
         insert_value_sql = []
         for vs in vars:
             insert_value_sql.append(f"({', '.join(':' + v for v in vs)})")
         sql = sql + ", ".join(insert_value_sql)
         # upsert
         if self.update_fields:
             update_value_sql = []
@@ -1669,50 +1083,46 @@
                 _sql = (
                     f" ON CONFLICT ({','.join(self.conflict_targets)}) DO UPDATE SET "
                 )
                 for k in self.update_fields:
                     update_value_sql.append(f"{k} = EXCLUDED.{k}")
             sql += _sql + ", ".join(update_value_sql)
         if type == type.POSTGRES:
-            sql += f" RETURNING {self.model.schema.primary_field.name}"
+            sql += f" RETURNING {self.schema.primary_field.name}"
         return sql + ";"
 
 
 @dataclasses.dataclass
 class CaseUpdate(BaseSQLBuilder):
+    schema: typing.Optional[Schema] = None
     OPERATION: typing.ClassVar[Operation] = Operation.UPDATE
     data: typing.List[typing.Dict[str, str]] = dataclasses.field(default_factory=list)
 
-    async def exec(self) -> int:
-        database = self.get_database()
-        await database.execute(self.to_sql(type=database.type), self._vars)
-        return 1
-
     def to_sql(self, type: Database.Type = Database.Type.MYSQL):
         assert self.data
-        assert self.model
-        qt = type.quote
-        fields = {f.name: f for f in self.model.schema.fields}
+        assert self.schema
+
+        fields = {f.name: f for f in self.schema.fields}
 
         parse_data: typing.DefaultDict[str, typing.Dict[str, typing.Any]] = defaultdict(
             dict
         )
         primary_values = []
         for d in self.data:
             for k, v in d.items():
-                if k == self.model.schema.primary_field.name:
+                if k == self.schema.primary_field.name:
                     primary_values.append(v)
                 else:
-                    parse_data[k][d[self.model.schema.primary_field.name]] = fields[
+                    parse_data[k][d[self.schema.primary_field.name]] = fields[
                         k
                     ].to_database(v)
-        sql = f"UPDATE {qt}{self.model.table_name}{qt} SET"
+        sql = f"UPDATE {type.quote(self.schema.name)} SET"
         _sqls = []
         for k, vs in parse_data.items():
             case = SQLCase(cast_type=fields[k].type)
             for pv, v in vs.items():
-                case.case(self.model.schema.primary_field == pv, v)
-            _sqls.append(f" {qt}{k}{qt} = {case.sync(self).to_sql(type=type)}")
+                case.case(self.schema.primary_field == pv, v)
+            _sqls.append(f" {type.quote(k)} = {case.sync(self).to_sql(type=type)}")
         sql += ", ".join(_sqls)
-        sql += f" WHERE {(self.model.schema.primary_field.contains(primary_values)).sync(self).to_sql(type=type)};"
+        sql += f" WHERE {(self.schema.primary_field.contains(primary_values)).sync(self).to_sql(type=type)};"
 
         return sql
```

### Comparing `danio-0.5.0/danio/mysql.py` & `danio-0.5.1/danio/mysql.py`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/danio/sqlite.py` & `danio-0.5.1/danio/sqlite.py`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/danio/utils.py` & `danio-0.5.1/danio/utils.py`

 * *Files identical despite different names*

### Comparing `danio-0.5.0/pyproject.toml` & `danio-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "danio"
-version = "0.5.0"
+version = "0.5.1"
 description = "ORM for asyncio world by dataclass"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.8",
```

### Comparing `danio-0.5.0/setup.py` & `danio-0.5.1/docs/index.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,283 +1,296 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2764 616e 696f 275d 0a0a 7061   \.['danio']..pa
-00000050: 636b 6167 655f 6461 7461 203d 205c 0a7b  ckage_data = \.{
-00000060: 2727 3a20 5b27 2a27 5d7d 0a0a 696e 7374  '': ['*']}..inst
-00000070: 616c 6c5f 7265 7175 6972 6573 203d 205c  all_requires = \
-00000080: 0a5b 2763 6163 6865 642d 7072 6f70 6572  .['cached-proper
-00000090: 7479 3e3d 312e 352e 322c 3c32 2e30 2e30  ty>=1.5.2,<2.0.0
-000000a0: 272c 2027 6461 7461 6261 7365 733e 3d30  ', 'databases>=0
-000000b0: 2e36 2e30 2c3c 302e 372e 3027 5d0a 0a73  .6.0,<0.7.0']..s
-000000c0: 6574 7570 5f6b 7761 7267 7320 3d20 7b0a  etup_kwargs = {.
-000000d0: 2020 2020 276e 616d 6527 3a20 2764 616e      'name': 'dan
-000000e0: 696f 272c 0a20 2020 2027 7665 7273 696f  io',.    'versio
-000000f0: 6e27 3a20 2730 2e35 2e30 272c 0a20 2020  n': '0.5.0',.   
-00000100: 2027 6465 7363 7269 7074 696f 6e27 3a20   'description': 
-00000110: 274f 524d 2066 6f72 2061 7379 6e63 696f  'ORM for asyncio
-00000120: 2077 6f72 6c64 2062 7920 6461 7461 636c   world by datacl
-00000130: 6173 7327 2c0a 2020 2020 276c 6f6e 675f  ass',.    'long_
-00000140: 6465 7363 7269 7074 696f 6e27 3a20 2723  description': '#
-00000150: 2044 616e 696f 5c6e 5c6e 3c70 3e5c 6e3c   Danio\n\n<p>\n<
-00000160: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000170: 6769 7468 7562 2e63 6f6d 2f73 7472 6f6e  github.com/stron
-00000180: 6762 7567 6d61 6e2f 6461 6e69 6f2f 6163  gbugman/danio/ac
-00000190: 7469 6f6e 7322 3e5c 6e20 2020 203c 696d  tions">\n    <im
-000001a0: 6720 7372 633d 2268 7474 7073 3a2f 2f67  g src="https://g
-000001b0: 6974 6875 622e 636f 6d2f 7374 726f 6e67  ithub.com/strong
-000001c0: 6275 676d 616e 2f64 616e 696f 2f77 6f72  bugman/danio/wor
-000001d0: 6b66 6c6f 7773 2f55 6e69 7454 6573 742f  kflows/UnitTest/
-000001e0: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
-000001f0: 556e 6974 5465 7374 223e 5c6e 3c2f 613e  UnitTest">\n</a>
-00000200: 5c6e 3c61 2068 7265 663d 2268 7474 7073  \n<a href="https
-00000210: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000220: 6563 742f 6461 6e69 6f2f 223e 5c6e 2020  ect/danio/">\n  
-00000230: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000240: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
-00000250: 6f2f 7079 2f64 616e 696f 2e73 7667 2220  o/py/danio.svg" 
-00000260: 616c 743d 2250 6163 6b61 6765 2076 6572  alt="Package ver
-00000270: 7369 6f6e 223e 5c6e 3c2f 613e 5c6e 3c61  sion">\n</a>\n<a
-00000280: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
-00000290: 6f64 6563 6f76 2e69 6f2f 6768 2f73 7472  odecov.io/gh/str
-000002a0: 6f6e 6762 7567 6d61 6e2f 6461 6e69 6f22  ongbugman/danio"
-000002b0: 3e5c 6e20 2020 203c 696d 6720 7372 633d  >\n    <img src=
-000002c0: 2268 7474 7073 3a2f 2f63 6f64 6563 6f76  "https://codecov
-000002d0: 2e69 6f2f 6768 2f73 7472 6f6e 6762 7567  .io/gh/strongbug
-000002e0: 6d61 6e2f 6461 6e69 6f2f 6272 616e 6368  man/danio/branch
-000002f0: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-00000300: 652e 7376 6722 2061 6c74 3d22 436f 6465  e.svg" alt="Code
-00000310: 2063 6f76 6572 6167 6522 3e5c 6e3c 2f61   coverage">\n</a
-00000320: 3e5c 6e3c 2f70 3e5c 6e5c 6e5c 6e44 616e  >\n</p>\n\n\nDan
-00000330: 696f 2069 7320 6120 4f52 4d20 666f 7220  io is a ORM for 
-00000340: 7079 7468 6f6e 2061 7379 6e63 696f 2077  python asyncio w
-00000350: 6f72 6c64 2e49 7420 6973 2064 6573 6967  orld.It is desig
-00000360: 6e65 6420 746f 206d 616b 6520 6765 7474  ned to make gett
-00000370: 696e 6720 6561 7379 2061 6e64 2063 6c65  ing easy and cle
-00000380: 6172 6c79 2e49 7420 6275 696c 6473 206f  arly.It builds o
-00000390: 6e20 7079 7468 6f6e 5c27 7320 6461 7461  n python\'s data
-000003a0: 636c 6173 7320 616e 6420 656e 636f 6465  class and encode
-000003b0: 5c27 7320 5b64 6174 6162 6173 6573 5d28  \'s [databases](
-000003c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003d0: 6f6d 2f65 6e63 6f64 652f 6461 7461 6261  om/encode/databa
-000003e0: 7365 7329 5c6e 5c6e 2323 2046 6561 7475  ses)\n\n## Featu
-000003f0: 7265 735c 6e5c 6e2a 206b 6565 7020 4f4f  res\n\n* keep OO
-00000400: 4d20 696e 206d 696e 642c 2063 7573 746f  M in mind, custo
-00000410: 6d20 796f 7572 2046 6965 6c64 2061 6e64  m your Field and
-00000420: 204d 6f64 656c 2062 6568 6176 696f 7220   Model behavior 
-00000430: 6561 7369 6c79 5c6e 2a20 7479 7065 2068  easily\n* type h
-00000440: 696e 7473 2061 6e79 2077 6865 7265 2c20  ints any where, 
-00000450: 6e6f 206d 6f72 6520 6e65 6564 2074 6f20  no more need to 
-00000460: 6d65 6d6f 7269 7a65 2077 6f72 6473 2079  memorize words y
-00000470: 6f75 7220 6669 656c 6420 6e61 6d65 7320  our field names 
-00000480: 616e 7920 6d6f 7265 5c6e 2a20 6261 7365  any more\n* base
-00000490: 2043 5255 4420 6f70 6572 6174 696f 6e2c   CRUD operation,
-000004a0: 2074 7261 6e73 6163 7469 6f6e 732c 206c   transactions, l
-000004b0: 6f63 6b20 616e 6420 736f 206f 6e5c 6e2a  ock and so on\n*
-000004c0: 2073 6967 6e61 6c73 206c 696b 6520 6265   signals like be
-000004d0: 666f 7265 2073 6176 652c 2061 6674 6572  fore save, after
-000004e0: 2073 6176 6520 616e 6420 736f 206f 6e5c   save and so on\
-000004f0: 6e2a 2063 6f6d 706c 6578 206f 7065 7261  n* complex opera
-00000500: 7469 6f6e 206c 696b 6520 6275 6c6b 2063  tion like bulk c
-00000510: 7265 6174 652c 2075 7073 6572 742c 2063  reate, upsert, c
-00000520: 7265 6174 6520 6f72 2075 7064 6174 6520  reate or update 
-00000530: 616e 6420 736f 206f 6e5c 6e2a 2061 7373  and so on\n* ass
-00000540: 6973 7420 6d6f 6465 6c20 7363 6865 6d61  ist model schema
-00000550: 206d 6967 7261 7469 6f6e 5c6e 2a20 7375   migration\n* su
-00000560: 7070 6f72 7420 4d79 5351 4c2f 506f 7374  pport MySQL/Post
-00000570: 6772 6553 514c 2f53 514c 6974 655c 6e5c  greSQL/SQLite\n\
-00000580: 6e23 2320 696e 7374 616c 6c5c 6e5c 6e60  n## install\n\n`
-00000590: 7069 7020 696e 7374 616c 6c20 6461 6e69  pip install dani
-000005a0: 6f60 5c6e 5c6e 2323 2044 6f63 756d 656e  o`\n\n## Documen
-000005b0: 7473 5c6e 5c6e 5b44 616e 696f 2044 6f63  ts\n\n[Danio Doc
-000005c0: 756d 656e 745d 2868 7474 7073 3a2f 2f73  ument](https://s
-000005d0: 7472 6f6e 6762 7567 6d61 6e2e 6769 7468  trongbugman.gith
-000005e0: 7562 2e69 6f2f 6461 6e69 6f2f 295c 6e5c  ub.io/danio/)\n\
-000005f0: 6e23 2320 476c 616e 6365 5c6e 5c6e 6060  n## Glance\n\n``
-00000600: 6070 7974 686f 6e5c 6e64 6220 3d20 6461  `python\ndb = da
-00000610: 6e69 6f2e 4461 7461 6261 7365 285c 6e20  nio.Database(\n 
-00000620: 2020 2022 6d79 7371 6c3a 2f2f 726f 6f74     "mysql://root
-00000630: 3a6c 6574 6d65 696e 4073 6572 7665 723a  :letmein@server:
-00000640: 3333 3036 2f74 6573 7422 2c5c 6e20 2020  3306/test",\n   
-00000650: 206d 6178 7369 7a65 3d33 2c5c 6e20 2020   maxsize=3,\n   
-00000660: 2063 6861 7273 6574 3d22 7574 6638 6d62   charset="utf8mb
-00000670: 3422 2c5c 6e20 2020 2075 7365 5f75 6e69  4",\n    use_uni
-00000680: 636f 6465 3d54 7275 652c 5c6e 2020 2020  code=True,\n    
-00000690: 636f 6e6e 6563 745f 7469 6d65 6f75 743d  connect_timeout=
-000006a0: 3630 2c5c 6e29 5c6e 5c6e 4064 6174 6163  60,\n)\n\n@datac
-000006b0: 6c61 7373 6573 2e64 6174 6163 6c61 7373  lasses.dataclass
-000006c0: 5c6e 636c 6173 7320 5573 6572 2864 616e  \nclass User(dan
-000006d0: 696f 2e4d 6f64 656c 293a 5c6e 2020 2020  io.Model):\n    
-000006e0: 636c 6173 7320 4765 6e64 6572 2865 6e75  class Gender(enu
-000006f0: 6d2e 456e 756d 293a 5c6e 2020 2020 2020  m.Enum):\n      
-00000700: 2020 4d41 4c45 203d 2030 5c6e 2020 2020    MALE = 0\n    
-00000710: 2020 2020 4645 4d41 4c45 203d 2031 5c6e      FEMALE = 1\n
-00000720: 2020 2020 2020 2020 4f54 4845 5220 3d20          OTHER = 
-00000730: 325c 6e5c 6e20 2020 206e 616d 653a 2073  2\n\n    name: s
-00000740: 7472 203d 2064 616e 696f 2e66 6965 6c64  tr = danio.field
-00000750: 285c 6e20 2020 2020 2020 2064 616e 696f  (\n        danio
-00000760: 2e43 6861 7246 6965 6c64 2c5c 6e20 2020  .CharField,\n   
-00000770: 2020 2020 2063 6f6d 6d65 6e74 3d22 5573       comment="Us
-00000780: 6572 206e 616d 6522 2c5c 6e20 2020 2020  er name",\n     
-00000790: 2020 2064 6566 6175 6c74 3d64 616e 696f     default=danio
-000007a0: 2e43 6861 7246 6965 6c64 2e4e 6f44 6566  .CharField.NoDef
-000007b0: 6175 6c74 2c5c 6e20 2020 2029 5c6e 2020  ault,\n    )\n  
-000007c0: 2020 6167 653a 2069 6e74 203d 2064 616e    age: int = dan
-000007d0: 696f 2e66 6965 6c64 2864 616e 696f 2e49  io.field(danio.I
-000007e0: 6e74 4669 656c 6429 5c6e 2020 2020 6372  ntField)\n    cr
-000007f0: 6561 7465 645f 6174 3a20 6461 7465 7469  eated_at: dateti
-00000800: 6d65 2e64 6174 6574 696d 6520 3d20 6461  me.datetime = da
-00000810: 6e69 6f2e 6669 656c 6428 5c6e 2020 2020  nio.field(\n    
-00000820: 2020 2020 6461 6e69 6f2e 4461 7465 5469      danio.DateTi
-00000830: 6d65 4669 656c 642c 5c6e 2020 2020 2020  meField,\n      
-00000840: 2020 636f 6d6d 656e 743d 2277 6865 6e20    comment="when 
-00000850: 6372 6561 7465 6422 2c5c 6e20 2020 2029  created",\n    )
-00000860: 5c6e 2020 2020 7570 6461 7465 645f 6174  \n    updated_at
-00000870: 3a20 6461 7465 7469 6d65 2e64 6174 6574  : datetime.datet
-00000880: 696d 6520 3d20 6461 6e69 6f2e 6669 656c  ime = danio.fiel
-00000890: 6428 5c6e 2020 2020 2020 2020 6461 6e69  d(\n        dani
-000008a0: 6f2e 4461 7465 5469 6d65 4669 656c 642c  o.DateTimeField,
-000008b0: 5c6e 2020 2020 2020 2020 636f 6d6d 656e  \n        commen
-000008c0: 743d 2277 6865 6e20 6372 6561 7465 6422  t="when created"
-000008d0: 2c5c 6e20 2020 2029 5c6e 2020 2020 6765  ,\n    )\n    ge
-000008e0: 6e64 6572 3a20 4765 6e64 6572 203d 2064  nder: Gender = d
-000008f0: 616e 696f 2e66 6965 6c64 2864 616e 696f  anio.field(danio
-00000900: 2e49 6e74 4669 656c 642c 2065 6e75 6d3d  .IntField, enum=
-00000910: 4765 6e64 6572 2c20 6465 6661 756c 743d  Gender, default=
-00000920: 4765 6e64 6572 2e46 454d 414c 4529 5c6e  Gender.FEMALE)\n
-00000930: 5c6e 2020 2020 6173 796e 6320 6465 6620  \n    async def 
-00000940: 6265 666f 7265 5f63 7265 6174 6528 7365  before_create(se
-00000950: 6c66 2c20 2a2a 6b77 6172 6773 293a 5c6e  lf, **kwargs):\n
-00000960: 2020 2020 2020 2020 2320 7573 6572 5f63          # user_c
-00000970: 6f75 6e74 202b 3d20 315c 6e20 2020 2020  ount += 1\n     
-00000980: 2020 2061 7761 6974 2073 7570 6572 2829     await super()
-00000990: 2e62 6566 6f72 655f 6372 6561 7465 282a  .before_create(*
-000009a0: 2a6b 7761 7267 7329 5c6e 5c6e 2020 2020  *kwargs)\n\n    
-000009b0: 6173 796e 6320 6465 6620 6265 666f 7265  async def before
-000009c0: 5f75 7064 6174 6528 7365 6c66 2c20 2a2a  _update(self, **
-000009d0: 6b77 6172 6773 293a 5c6e 2020 2020 2020  kwargs):\n      
-000009e0: 2020 7365 6c66 2e75 7064 6174 6564 5f61    self.updated_a
-000009f0: 7420 3d20 6461 7465 7469 6d65 2e64 6174  t = datetime.dat
-00000a00: 6574 696d 652e 6e6f 7728 295c 6e5c 6e20  etime.now()\n\n 
-00000a10: 2020 2061 7379 6e63 2064 6566 2076 616c     async def val
-00000a20: 6964 6174 6528 7365 6c66 293a 5c6e 2020  idate(self):\n  
-00000a30: 2020 2020 2020 6177 6169 7420 7375 7065        await supe
-00000a40: 7228 292e 7661 6c69 6461 7465 2829 5c6e  r().validate()\n
-00000a50: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00000a60: 656c 662e 6e61 6d65 3a5c 6e20 2020 2020  elf.name:\n     
-00000a70: 2020 2020 2020 2072 6169 7365 2064 616e         raise dan
-00000a80: 696f 2e56 616c 6964 6174 6545 7863 6570  io.ValidateExcep
-00000a90: 7469 6f6e 2822 456d 7074 7920 6e61 6d65  tion("Empty name
-00000aa0: 2122 295c 6e5c 6e20 2020 2040 636c 6173  !")\n\n    @clas
-00000ab0: 736d 6574 686f 645c 6e20 2020 2064 6566  smethod\n    def
-00000ac0: 2067 6574 5f64 6174 6162 6173 6528 5c6e   get_database(\n
-00000ad0: 2020 2020 2020 2020 636c 732c 206f 7065          cls, ope
-00000ae0: 7261 7469 6f6e 3a20 6461 6e69 6f2e 4f70  ration: danio.Op
-00000af0: 6572 6174 696f 6e2c 2074 6162 6c65 3a20  eration, table: 
-00000b00: 7374 722c 202a 6172 6773 2c20 2a2a 6b77  str, *args, **kw
-00000b10: 6172 6773 5c6e 2020 2020 2920 2d3e 2064  args\n    ) -> d
-00000b20: 616e 696f 2e44 6174 6162 6173 653a 5c6e  anio.Database:\n
-00000b30: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00000b40: 625c 6e5c 6e23 2062 6173 6520 4352 5544  b\n\n# base CRUD
-00000b50: 5c6e 7573 6572 203d 2061 7761 6974 2055  \nuser = await U
-00000b60: 7365 7228 6e61 6d65 3d22 6261 746d 616e  ser(name="batman
-00000b70: 2229 2e73 6176 6528 295c 6e75 7365 7220  ").save()\nuser 
-00000b80: 3d20 6177 6169 7420 5573 6572 2e77 6865  = await User.whe
-00000b90: 7265 2855 7365 722e 6e61 6d65 203d 3d20  re(User.name == 
-00000ba0: 2262 6174 6d61 6e22 292e 6665 7463 685f  "batman").fetch_
-00000bb0: 6f6e 6528 295c 6e75 7365 722e 6765 6e64  one()\nuser.gend
-00000bc0: 6572 203d 2055 7365 722e 4765 6e64 6572  er = User.Gender
-00000bd0: 2e4d 414c 455c 6e61 7761 6974 2075 7365  .MALE\nawait use
-00000be0: 722e 7361 7665 2829 5c6e 6177 6169 7420  r.save()\nawait 
-00000bf0: 7573 6572 2e64 656c 6574 6528 295c 6e23  user.delete()\n#
-00000c00: 2073 716c 2063 6861 696e 5c6e 6177 6169   sql chain\nawai
-00000c10: 7420 5573 6572 2e77 6865 7265 2855 7365  t User.where(Use
-00000c20: 722e 6e61 6d65 2021 3d20 2222 292e 6c69  r.name != "").li
-00000c30: 6d69 7428 3130 292e 6665 7463 685f 616c  mit(10).fetch_al
-00000c40: 6c28 295c 6e23 206d 756c 7469 2077 6865  l()\n# multi whe
-00000c50: 7265 2063 6f6e 6469 7469 6f6e 5c6e 6177  re condition\naw
-00000c60: 6169 7420 5573 6572 2e77 6865 7265 2855  ait User.where(U
-00000c70: 7365 722e 6964 2021 3d20 312c 2055 7365  ser.id != 1, Use
-00000c80: 722e 6e61 6d65 2021 3d20 2222 292e 6665  r.name != "").fe
-00000c90: 7463 685f 616c 6c28 295c 6e61 7761 6974  tch_all()\nawait
-00000ca0: 2055 7365 722e 7768 6572 6528 5573 6572   User.where(User
-00000cb0: 2e69 6420 213d 2031 292e 7768 6572 6528  .id != 1).where(
-00000cc0: 5573 6572 2e6e 616d 6520 213d 2022 2229  User.name != "")
-00000cd0: 2e66 6574 6368 5f61 6c6c 2829 5c6e 6177  .fetch_all()\naw
-00000ce0: 6169 7420 5573 6572 2e77 6865 7265 2855  ait User.where(U
-00000cf0: 7365 722e 6964 203c 3d20 3130 2c20 5573  ser.id <= 10, Us
-00000d00: 6572 2e69 6420 3e3d 2032 302c 2069 735f  er.id >= 20, is_
-00000d10: 616e 643d 4661 6c73 6529 2e66 6574 6368  and=False).fetch
-00000d20: 5f61 6c6c 2829 5c6e 2320 636f 6d70 6c69  _all()\n# compli
-00000d30: 6361 7465 6420 6578 7072 6573 7369 6f6e  cated expression
-00000d40: 5c6e 6177 6169 7420 5573 6572 2e77 6865  \nawait User.whe
-00000d50: 7265 2855 7365 722e 6964 203d 3d20 3129  re(User.id == 1)
-00000d60: 2e75 7064 6174 6528 6167 653d 2855 7365  .update(age=(Use
-00000d70: 722e 6167 6520 2b20 3129 202f 2028 5573  r.age + 1) / (Us
-00000d80: 6572 2e61 6765 202f 2031 3229 202d 2032  er.age / 12) - 2
-00000d90: 295c 6e61 7761 6974 2055 7365 722e 7768  )\nawait User.wh
-00000da0: 6572 6528 2855 7365 722e 6167 6520 2b20  ere((User.age + 
-00000db0: 3129 203d 3d20 3329 2e66 6574 6368 5f61  1) == 3).fetch_a
-00000dc0: 6c6c 2829 5c6e 2320 636f 6d70 6c69 6361  ll()\n# complica
-00000dd0: 7465 6420 7371 6c20 6f70 6572 6174 696f  ted sql operatio
-00000de0: 6e5c 6e61 7761 6974 2055 7365 722e 7768  n\nawait User.wh
-00000df0: 6572 6528 5573 6572 2e69 6420 3d3d 2075  ere(User.id == u
-00000e00: 2e69 6429 2e75 7064 6174 6528 5c6e 2020  .id).update(\n  
-00000e10: 2020 6167 653d 5573 6572 2e61 6765 2e63    age=User.age.c
-00000e20: 6173 6528 5573 6572 2e61 6765 203e 2031  ase(User.age > 1
-00000e30: 302c 2031 2c20 6465 6661 756c 743d 3138  0, 1, default=18
-00000e40: 292e 6361 7365 2855 7365 722e 6167 6520  ).case(User.age 
-00000e50: 3c3d 2030 2c20 3130 295c 6e29 5c6e 6372  <= 0, 10)\n)\ncr
-00000e60: 6561 7465 642c 2075 7064 6174 6564 203d  eated, updated =
-00000e70: 2061 7761 6974 2055 7365 7250 726f 6669   await UserProfi
-00000e80: 6c65 2e75 7073 6572 7428 5c6e 2020 2020  le.upsert(\n    
-00000e90: 5b5c 6e20 2020 2020 2020 2064 6963 7428  [\n        dict(
-00000ea0: 6964 3d31 2c20 6e61 6d65 3d22 7570 7365  id=1, name="upse
-00000eb0: 7274 2229 2c5c 6e20 2020 205d 2c5c 6e20  rt"),\n    ],\n 
-00000ec0: 2020 2075 7064 6174 655f 6669 656c 6473     update_fields
-00000ed0: 3d5b 226e 616d 6522 5d2c 5c6e 295c 6e23  =["name"],\n)\n#
-00000ee0: 2062 756c 6b20 6f70 6572 6174 696f 6e5c   bulk operation\
-00000ef0: 6e61 7761 6974 2055 7365 722e 6275 6c6b  nawait User.bulk
-00000f00: 5f63 7265 6174 6528 5b55 7365 7228 6e61  _create([User(na
-00000f10: 6d65 3d66 2275 7365 725f 7b69 7d22 2920  me=f"user_{i}") 
-00000f20: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
-00000f30: 3029 5d29 5c6e 6177 6169 7420 5573 6572  0)])\nawait User
-00000f40: 2e62 756c 6b5f 7570 6461 7465 2861 7761  .bulk_update(awa
-00000f50: 6974 2055 7365 722e 6665 7463 685f 616c  it User.fetch_al
-00000f60: 6c28 2929 5c6e 6177 6169 7420 5573 6572  l())\nawait User
-00000f70: 2e62 756c 6b5f 6465 6c65 7465 2861 7761  .bulk_delete(awa
-00000f80: 6974 2055 7365 722e 6665 7463 685f 616c  it User.fetch_al
-00000f90: 6c28 2929 5c6e 2320 7368 6f72 7463 7574  l())\n# shortcut
-00000fa0: 5c6e 7573 6572 2c20 6372 6561 7465 6420  \nuser, created 
-00000fb0: 3d20 6177 6169 7420 5573 6572 2869 643d  = await User(id=
-00000fc0: 312c 206e 616d 653d 2263 7265 6174 6564  1, name="created
-00000fd0: 3f22 292e 6765 745f 6f72 5f63 7265 6174  ?").get_or_creat
-00000fe0: 6528 5c6e 2020 2020 6b65 795f 6669 656c  e(\n    key_fiel
-00000ff0: 6473 3d28 5573 6572 2e69 642c 295c 6e29  ds=(User.id,)\n)
-00001000: 5c6e 7573 6572 2c20 6372 6561 7465 642c  \nuser, created,
-00001010: 2075 7064 6174 6564 203d 2061 7761 6974   updated = await
-00001020: 2055 7365 7228 6964 3d32 2c20 6e61 6d65   User(id=2, name
-00001030: 3d22 7570 6461 7465 643f 2229 2e63 7265  ="updated?").cre
-00001040: 6174 655f 6f72 5f75 7064 6174 6528 5c6e  ate_or_update(\n
-00001050: 2020 2020 6b65 795f 6669 656c 6473 3d28      key_fields=(
-00001060: 5573 6572 2e69 642c 295c 6e29 5c6e 6060  User.id,)\n)\n``
-00001070: 6027 2c0a 2020 2020 2761 7574 686f 7227  `',.    'author'
-00001080: 3a20 2773 7472 6f6e 6762 7567 6d61 6e27  : 'strongbugman'
-00001090: 2c0a 2020 2020 2761 7574 686f 725f 656d  ,.    'author_em
-000010a0: 6169 6c27 3a20 2773 7472 6f6e 6762 7567  ail': 'strongbug
-000010b0: 6d61 6e40 676d 6169 6c2e 636f 6d27 2c0a  man@gmail.com',.
-000010c0: 2020 2020 276d 6169 6e74 6169 6e65 7227      'maintainer'
-000010d0: 3a20 4e6f 6e65 2c0a 2020 2020 276d 6169  : None,.    'mai
-000010e0: 6e74 6169 6e65 725f 656d 6169 6c27 3a20  ntainer_email': 
-000010f0: 4e6f 6e65 2c0a 2020 2020 2775 726c 273a  None,.    'url':
-00001100: 204e 6f6e 652c 0a20 2020 2027 7061 636b   None,.    'pack
-00001110: 6167 6573 273a 2070 6163 6b61 6765 732c  ages': packages,
-00001120: 0a20 2020 2027 7061 636b 6167 655f 6461  .    'package_da
-00001130: 7461 273a 2070 6163 6b61 6765 5f64 6174  ta': package_dat
-00001140: 612c 0a20 2020 2027 696e 7374 616c 6c5f  a,.    'install_
-00001150: 7265 7175 6972 6573 273a 2069 6e73 7461  requires': insta
-00001160: 6c6c 5f72 6571 7569 7265 732c 0a20 2020  ll_requires,.   
-00001170: 2027 7079 7468 6f6e 5f72 6571 7569 7265   'python_require
-00001180: 7327 3a20 273e 3d33 2e38 2c3c 342e 3027  s': '>=3.8,<4.0'
-00001190: 2c0a 7d0a 0a0a 7365 7475 7028 2a2a 7365  ,.}...setup(**se
-000011a0: 7475 705f 6b77 6172 6773 290a            tup_kwargs).
+00000000: 2320 4461 6e69 6f0a 0a3c 703e 0a3c 6120  # Danio..<p>.<a 
+00000010: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00000020: 7468 7562 2e63 6f6d 2f73 7472 6f6e 6762  thub.com/strongb
+00000030: 7567 6d61 6e2f 6461 6e69 6f2f 6163 7469  ugman/danio/acti
+00000040: 6f6e 7322 3e0a 2020 2020 3c69 6d67 2073  ons">.    <img s
+00000050: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000060: 7562 2e63 6f6d 2f73 7472 6f6e 6762 7567  ub.com/strongbug
+00000070: 6d61 6e2f 6461 6e69 6f2f 776f 726b 666c  man/danio/workfl
+00000080: 6f77 732f 556e 6974 5465 7374 2f62 6164  ows/UnitTest/bad
+00000090: 6765 2e73 7667 2220 616c 743d 2255 6e69  ge.svg" alt="Uni
+000000a0: 7454 6573 7422 3e0a 3c2f 613e 0a3c 6120  tTest">.</a>.<a 
+000000b0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+000000c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f64  pi.org/project/d
+000000d0: 616e 696f 2f22 3e0a 2020 2020 3c69 6d67  anio/">.    <img
+000000e0: 2073 7263 3d22 6874 7470 733a 2f2f 6261   src="https://ba
+000000f0: 6467 652e 6675 7279 2e69 6f2f 7079 2f64  dge.fury.io/py/d
+00000100: 616e 696f 2e73 7667 2220 616c 743d 2250  anio.svg" alt="P
+00000110: 6163 6b61 6765 2076 6572 7369 6f6e 223e  ackage version">
+00000120: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+00000130: 7474 7073 3a2f 2f63 6f64 6563 6f76 2e69  ttps://codecov.i
+00000140: 6f2f 6768 2f73 7472 6f6e 6762 7567 6d61  o/gh/strongbugma
+00000150: 6e2f 6461 6e69 6f22 3e0a 2020 2020 3c69  n/danio">.    <i
+00000160: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000170: 636f 6465 636f 762e 696f 2f67 682f 7374  codecov.io/gh/st
+00000180: 726f 6e67 6275 676d 616e 2f64 616e 696f  rongbugman/danio
+00000190: 2f62 7261 6e63 682f 6d61 696e 2f67 7261  /branch/main/gra
+000001a0: 7068 2f62 6164 6765 2e73 7667 2220 616c  ph/badge.svg" al
+000001b0: 743d 2243 6f64 6520 636f 7665 7261 6765  t="Code coverage
+000001c0: 223e 0a3c 2f61 3e0a 3c2f 703e 0a0a 0a44  ">.</a>.</p>...D
+000001d0: 616e 696f 2069 7320 6120 4f52 4d20 666f  anio is a ORM fo
+000001e0: 7220 7079 7468 6f6e 2061 7379 6e63 696f  r python asyncio
+000001f0: 2077 6f72 6c64 2e49 7420 6973 2064 6573   world.It is des
+00000200: 6967 6e65 6420 746f 206d 616b 6520 6765  igned to make ge
+00000210: 7474 696e 6720 6561 7379 2061 6e64 2063  tting easy and c
+00000220: 6c65 6172 6c79 2e49 7420 6275 696c 6473  learly.It builds
+00000230: 206f 6e20 7079 7468 6f6e 2773 2064 6174   on python's dat
+00000240: 6163 6c61 7373 2061 6e64 2065 6e63 6f64  aclass and encod
+00000250: 6527 7320 5b64 6174 6162 6173 6573 5d28  e's [databases](
+00000260: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000270: 6f6d 2f65 6e63 6f64 652f 6461 7461 6261  om/encode/databa
+00000280: 7365 7329 0a0a 2323 2046 6561 7475 7265  ses)..## Feature
+00000290: 730a 0a2a 206b 6565 7020 4f4f 4d20 696e  s..* keep OOM in
+000002a0: 206d 696e 642c 2063 7573 746f 6d20 796f   mind, custom yo
+000002b0: 7572 2046 6965 6c64 2061 6e64 204d 6f64  ur Field and Mod
+000002c0: 656c 2062 6568 6176 696f 7220 6561 7369  el behavior easi
+000002d0: 6c79 0a2a 2074 7970 6520 6869 6e74 7320  ly.* type hints 
+000002e0: 616e 7920 7768 6572 652c 206e 6f20 6d6f  any where, no mo
+000002f0: 7265 206e 6565 6420 746f 206d 656d 6f72  re need to memor
+00000300: 697a 6520 776f 7264 7320 796f 7572 2066  ize words your f
+00000310: 6965 6c64 206e 616d 6573 2061 6e79 206d  ield names any m
+00000320: 6f72 650a 2a20 6261 7365 2043 5255 4420  ore.* base CRUD 
+00000330: 6f70 6572 6174 696f 6e2c 2074 7261 6e73  operation, trans
+00000340: 6163 7469 6f6e 732c 206c 6f63 6b20 616e  actions, lock an
+00000350: 6420 736f 206f 6e0a 2a20 7369 676e 616c  d so on.* signal
+00000360: 7320 6c69 6b65 2062 6566 6f72 6520 7361  s like before sa
+00000370: 7665 2c20 6166 7465 7220 7361 7665 2061  ve, after save a
+00000380: 6e64 2073 6f20 6f6e 0a2a 2063 6f6d 706c  nd so on.* compl
+00000390: 6578 206f 7065 7261 7469 6f6e 206c 696b  ex operation lik
+000003a0: 6520 6275 6c6b 2063 7265 6174 652c 2075  e bulk create, u
+000003b0: 7073 6572 742c 2063 7265 6174 6520 6f72  psert, create or
+000003c0: 2075 7064 6174 6520 616e 6420 736f 206f   update and so o
+000003d0: 6e0a 2a20 6173 7369 7374 206d 6f64 656c  n.* assist model
+000003e0: 2073 6368 656d 6120 6d69 6772 6174 696f   schema migratio
+000003f0: 6e0a 2a20 7375 7070 6f72 7420 4d79 5351  n.* support MySQ
+00000400: 4c2f 506f 7374 6772 6553 514c 2f53 514c  L/PostgreSQL/SQL
+00000410: 6974 650a 2a20 6869 6e74 7320 6765 6e65  ite.* hints gene
+00000420: 7261 7469 6f6e 0a0a 2323 2069 6e73 7461  ration..## insta
+00000430: 6c6c 0a0a 6070 6970 2069 6e73 7461 6c6c  ll..`pip install
+00000440: 2064 616e 696f 600a 0a23 2320 446f 6375   danio`..## Docu
+00000450: 6d65 6e74 730a 0a5b 4461 6e69 6f20 446f  ments..[Danio Do
+00000460: 6375 6d65 6e74 5d28 6874 7470 733a 2f2f  cument](https://
+00000470: 7374 726f 6e67 6275 676d 616e 2e67 6974  strongbugman.git
+00000480: 6875 622e 696f 2f64 616e 696f 2f29 0a0a  hub.io/danio/)..
+00000490: 2323 2047 6c61 6e63 650a 0a60 6060 7079  ## Glance..```py
+000004a0: 7468 6f6e 0a64 6220 3d20 6461 6e69 6f2e  thon.db = danio.
+000004b0: 4461 7461 6261 7365 280a 2020 2020 226d  Database(.    "m
+000004c0: 7973 716c 3a2f 2f72 6f6f 743a 6c65 746d  ysql://root:letm
+000004d0: 6569 6e40 7365 7276 6572 3a33 3330 362f  ein@server:3306/
+000004e0: 7465 7374 222c 0a20 2020 206d 6178 7369  test",.    maxsi
+000004f0: 7a65 3d33 2c0a 2020 2020 6368 6172 7365  ze=3,.    charse
+00000500: 743d 2275 7466 386d 6234 222c 0a20 2020  t="utf8mb4",.   
+00000510: 2075 7365 5f75 6e69 636f 6465 3d54 7275   use_unicode=Tru
+00000520: 652c 0a20 2020 2063 6f6e 6e65 6374 5f74  e,.    connect_t
+00000530: 696d 656f 7574 3d36 302c 0a29 0a0a 4064  imeout=60,.)..@d
+00000540: 6174 6163 6c61 7373 6573 2e64 6174 6163  ataclasses.datac
+00000550: 6c61 7373 0a63 6c61 7373 2055 7365 7228  lass.class User(
+00000560: 6461 6e69 6f2e 4d6f 6465 6c29 3a0a 2020  danio.Model):.  
+00000570: 2020 2320 6175 746f 2067 656e 6572 6174    # auto generat
+00000580: 6564 2062 7920 6461 6e69 6f3a 0a20 2020  ed by danio:.   
+00000590: 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   # -------------
+000005a0: 2d2d 2d2d 2d2d 2d44 616e 696f 2048 696e  -------Danio Hin
+000005b0: 7473 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ts--------------
+000005c0: 2d2d 2d2d 2d2d 0a20 2020 2023 2054 4142  ------.    # TAB
+000005d0: 4c45 204e 414d 453a 2075 7365 720a 2020  LE NAME: user.  
+000005e0: 2020 2320 5441 424c 4520 4953 204d 4947    # TABLE IS MIG
+000005f0: 5241 5445 4421 0a20 2020 2049 443a 2074  RATED!.    ID: t
+00000600: 7970 696e 672e 436c 6173 7356 6172 5b64  yping.ClassVar[d
+00000610: 616e 696f 2e46 6965 6c64 5d20 2023 2022  anio.Field]  # "
+00000620: 6964 2220 7365 7269 616c 2050 5249 4d41  id" serial PRIMA
+00000630: 5259 204b 4559 204e 4f54 204e 554c 4c0a  RY KEY NOT NULL.
+00000640: 2020 2020 4e41 4d45 3a20 7479 7069 6e67      NAME: typing
+00000650: 2e43 6c61 7373 5661 725b 6461 6e69 6f2e  .ClassVar[danio.
+00000660: 4669 656c 645d 2020 2320 226e 616d 6522  Field]  # "name"
+00000670: 2076 6172 6368 6172 2832 3535 2920 204e   varchar(255)  N
+00000680: 4f54 204e 554c 4c0a 2020 2020 4147 453a  OT NULL.    AGE:
+00000690: 2074 7970 696e 672e 436c 6173 7356 6172   typing.ClassVar
+000006a0: 5b64 616e 696f 2e46 6965 6c64 5d20 2023  [danio.Field]  #
+000006b0: 2022 6167 6522 2069 6e74 2020 4e4f 5420   "age" int  NOT 
+000006c0: 4e55 4c4c 0a20 2020 2043 5245 4154 4544  NULL.    CREATED
+000006d0: 5f41 543a 2074 7970 696e 672e 436c 6173  _AT: typing.Clas
+000006e0: 7356 6172 5b0a 2020 2020 2020 2020 6461  sVar[.        da
+000006f0: 6e69 6f2e 4669 656c 640a 2020 2020 5d20  nio.Field.    ] 
+00000700: 2023 2022 6372 6561 7465 645f 6174 2220   # "created_at" 
+00000710: 7469 6d65 7374 616d 7020 7769 7468 6f75  timestamp withou
+00000720: 7420 7469 6d65 207a 6f6e 6520 204e 4f54  t time zone  NOT
+00000730: 204e 554c 4c0a 2020 2020 5550 4441 5445   NULL.    UPDATE
+00000740: 445f 4154 3a20 7479 7069 6e67 2e43 6c61  D_AT: typing.Cla
+00000750: 7373 5661 725b 0a20 2020 2020 2020 2064  ssVar[.        d
+00000760: 616e 696f 2e46 6965 6c64 0a20 2020 205d  anio.Field.    ]
+00000770: 2020 2320 2275 7064 6174 6564 5f61 7422    # "updated_at"
+00000780: 2074 696d 6573 7461 6d70 2077 6974 686f   timestamp witho
+00000790: 7574 2074 696d 6520 7a6f 6e65 2020 4e4f  ut time zone  NO
+000007a0: 5420 4e55 4c4c 0a20 2020 2047 454e 4445  T NULL.    GENDE
+000007b0: 523a 2074 7970 696e 672e 436c 6173 7356  R: typing.ClassV
+000007c0: 6172 5b64 616e 696f 2e46 6965 6c64 5d20  ar[danio.Field] 
+000007d0: 2023 2022 6765 6e64 6572 2220 696e 7420   # "gender" int 
+000007e0: 204e 4f54 204e 554c 4c0a 2020 2020 2320   NOT NULL.    # 
+000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000800: 2d2d 2d2d 4461 6e69 6f20 4869 6e74 732d  ----Danio Hints-
+00000810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000820: 2d2d 2d0a 0a20 2020 2063 6c61 7373 2047  ---..    class G
+00000830: 656e 6465 7228 656e 756d 2e45 6e75 6d29  ender(enum.Enum)
+00000840: 3a0a 2020 2020 2020 2020 4d41 4c45 203d  :.        MALE =
+00000850: 2030 0a20 2020 2020 2020 2046 454d 414c   0.        FEMAL
+00000860: 4520 3d20 310a 2020 2020 2020 2020 4f54  E = 1.        OT
+00000870: 4845 5220 3d20 320a 0a20 2020 2069 643a  HER = 2..    id:
+00000880: 2074 7970 696e 672e 416e 6e6f 7461 7465   typing.Annotate
+00000890: 645b 696e 742c 2064 616e 696f 2e49 6e74  d[int, danio.Int
+000008a0: 4669 656c 6428 7072 696d 6172 793d 5472  Field(primary=Tr
+000008b0: 7565 2c20 7479 7065 3d22 7365 7269 616c  ue, type="serial
+000008c0: 2229 5d20 3d20 300a 2020 2020 6e61 6d65  ")] = 0.    name
+000008d0: 3a20 7479 7069 6e67 2e41 6e6e 6f74 6174  : typing.Annotat
+000008e0: 6564 5b73 7472 2c20 6461 6e69 6f2e 4368  ed[str, danio.Ch
+000008f0: 6172 4669 656c 6428 636f 6d6d 656e 743d  arField(comment=
+00000900: 2255 7365 7220 6e61 6d65 2229 5d20 3d20  "User name")] = 
+00000910: 2222 0a20 2020 2061 6765 3a20 7479 7069  "".    age: typi
+00000920: 6e67 2e41 6e6e 6f74 6174 6564 5b69 6e74  ng.Annotated[int
+00000930: 2c20 6461 6e69 6f2e 496e 7446 6965 6c64  , danio.IntField
+00000940: 5d20 3d20 300a 2020 2020 6372 6561 7465  ] = 0.    create
+00000950: 645f 6174 3a20 7479 7069 6e67 2e41 6e6e  d_at: typing.Ann
+00000960: 6f74 6174 6564 5b0a 2020 2020 2020 2020  otated[.        
+00000970: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
+00000980: 652c 0a20 2020 2020 2020 2064 616e 696f  e,.        danio
+00000990: 2e44 6174 6554 696d 6546 6965 6c64 2874  .DateTimeField(t
+000009a0: 7970 653d 2274 696d 6573 7461 6d70 2077  ype="timestamp w
+000009b0: 6974 686f 7574 2074 696d 6520 7a6f 6e65  ithout time zone
+000009c0: 222c 2063 6f6d 6d65 6e74 3d22 7768 656e  ", comment="when
+000009d0: 2063 7265 6174 6564 2229 2c0a 2020 2020   created"),.    
+000009e0: 5d20 3d20 6461 7461 636c 6173 7365 732e  ] = dataclasses.
+000009f0: 6669 656c 6428 6465 6661 756c 745f 6661  field(default_fa
+00000a00: 6374 6f72 793d 6461 7465 7469 6d65 2e64  ctory=datetime.d
+00000a10: 6174 6574 696d 652e 6e6f 7729 0a20 2020  atetime.now).   
+00000a20: 2075 7064 6174 6564 5f61 743a 2074 7970   updated_at: typ
+00000a30: 696e 672e 416e 6e6f 7461 7465 645b 0a20  ing.Annotated[. 
+00000a40: 2020 2020 2020 2064 6174 6574 696d 652e         datetime.
+00000a50: 6461 7465 7469 6d65 2c0a 2020 2020 2020  datetime,.      
+00000a60: 2020 6461 6e69 6f2e 4461 7465 5469 6d65    danio.DateTime
+00000a70: 4669 656c 6428 7479 7065 3d22 7469 6d65  Field(type="time
+00000a80: 7374 616d 7020 7769 7468 6f75 7420 7469  stamp without ti
+00000a90: 6d65 207a 6f6e 6522 2c20 636f 6d6d 656e  me zone", commen
+00000aa0: 743d 2277 6865 6e20 7570 6461 7465 6422  t="when updated"
+00000ab0: 292c 0a20 2020 205d 203d 2064 6174 6163  ),.    ] = datac
+00000ac0: 6c61 7373 6573 2e66 6965 6c64 2864 6566  lasses.field(def
+00000ad0: 6175 6c74 5f66 6163 746f 7279 3d64 6174  ault_factory=dat
+00000ae0: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
+00000af0: 6f77 290a 2020 2020 6765 6e64 6572 3a20  ow).    gender: 
+00000b00: 7479 7069 6e67 2e41 6e6e 6f74 6174 6564  typing.Annotated
+00000b10: 5b47 656e 6465 722c 2064 616e 696f 2e49  [Gender, danio.I
+00000b20: 6e74 4669 656c 6428 656e 756d 3d47 656e  ntField(enum=Gen
+00000b30: 6465 7229 5d20 3d20 4765 6e64 6572 2e4d  der)] = Gender.M
+00000b40: 414c 450a 0a0a 2020 2020 6173 796e 6320  ALE...    async 
+00000b50: 6465 6620 6265 666f 7265 5f63 7265 6174  def before_creat
+00000b60: 6528 7365 6c66 2c20 7661 6c69 6461 7465  e(self, validate
+00000b70: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+00000b80: 6177 6169 7420 7375 7065 7228 292e 6265  await super().be
+00000b90: 666f 7265 5f63 7265 6174 6528 7661 6c69  fore_create(vali
+00000ba0: 6461 7465 3d54 7275 6529 0a0a 2020 2020  date=True)..    
+00000bb0: 6173 796e 6320 6465 6620 6265 666f 7265  async def before
+00000bc0: 5f75 7064 6174 6528 7365 6c66 2c20 7661  _update(self, va
+00000bd0: 6c69 6461 7465 3d54 7275 6529 3a0a 2020  lidate=True):.  
+00000be0: 2020 2020 2020 7365 6c66 2e75 7064 6174        self.updat
+00000bf0: 6564 5f61 7420 3d20 6461 7465 7469 6d65  ed_at = datetime
+00000c00: 2e64 6174 6574 696d 652e 6e6f 7728 290a  .datetime.now().
+00000c10: 2020 2020 2020 2020 6177 6169 7420 7375          await su
+00000c20: 7065 7228 292e 6265 666f 7265 5f75 7064  per().before_upd
+00000c30: 6174 6528 7661 6c69 6461 7465 3d54 7275  ate(validate=Tru
+00000c40: 6529 0a0a 2020 2020 6173 796e 6320 6465  e)..    async de
+00000c50: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00000c60: 3a0a 2020 2020 2020 2020 6177 6169 7420  :.        await 
+00000c70: 7375 7065 7228 292e 7661 6c69 6461 7465  super().validate
+00000c80: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
+00000c90: 7420 7365 6c66 2e6e 616d 653a 0a20 2020  t self.name:.   
+00000ca0: 2020 2020 2020 2020 2072 6169 7365 2064           raise d
+00000cb0: 616e 696f 2e56 616c 6964 6174 6545 7863  anio.ValidateExc
+00000cc0: 6570 7469 6f6e 2822 456d 7074 7920 6e61  eption("Empty na
+00000cd0: 6d65 2122 290a 0a20 2020 2040 636c 6173  me!")..    @clas
+00000ce0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00000cf0: 6765 745f 6461 7461 6261 7365 280a 2020  get_database(.  
+00000d00: 2020 2020 2020 636c 732c 206f 7065 7261        cls, opera
+00000d10: 7469 6f6e 3a20 6461 6e69 6f2e 4f70 6572  tion: danio.Oper
+00000d20: 6174 696f 6e2c 2074 6162 6c65 3a20 7374  ation, table: st
+00000d30: 722c 202a 6172 6773 2c20 2a2a 6b77 6172  r, *args, **kwar
+00000d40: 6773 0a20 2020 2029 202d 3e20 6461 6e69  gs.    ) -> dani
+00000d50: 6f2e 4461 7461 6261 7365 3a0a 2020 2020  o.Database:.    
+00000d60: 2020 2020 7265 7475 726e 2064 620a 0a23      return db..#
+00000d70: 2062 6173 6520 4352 5544 0a75 7365 7220   base CRUD.user 
+00000d80: 3d20 6177 6169 7420 5573 6572 286e 616d  = await User(nam
+00000d90: 653d 2262 6174 6d61 6e22 292e 7361 7665  e="batman").save
+00000da0: 2829 0a75 7365 7220 3d20 6177 6169 7420  ().user = await 
+00000db0: 5573 6572 2e77 6865 7265 2855 7365 722e  User.where(User.
+00000dc0: 4e41 4d45 203d 3d20 2262 6174 6d61 6e22  NAME == "batman"
+00000dd0: 292e 6665 7463 685f 6f6e 6528 290a 7573  ).fetch_one().us
+00000de0: 6572 2e67 656e 6465 7220 3d20 5573 6572  er.gender = User
+00000df0: 2e47 656e 6465 722e 4d41 4c45 0a61 7761  .Gender.MALE.awa
+00000e00: 6974 2075 7365 722e 7361 7665 2829 0a61  it user.save().a
+00000e10: 7761 6974 2075 7365 722e 6465 6c65 7465  wait user.delete
+00000e20: 2829 0a23 2073 716c 2063 6861 696e 0a61  ().# sql chain.a
+00000e30: 7761 6974 2055 7365 722e 7768 6572 6528  wait User.where(
+00000e40: 5573 6572 2e4e 414d 4520 213d 2022 2229  User.NAME != "")
+00000e50: 2e6c 696d 6974 2831 3029 2e66 6574 6368  .limit(10).fetch
+00000e60: 5f61 6c6c 2829 0a23 206d 756c 7469 2077  _all().# multi w
+00000e70: 6865 7265 2063 6f6e 6469 7469 6f6e 0a61  here condition.a
+00000e80: 7761 6974 2055 7365 722e 7768 6572 6528  wait User.where(
+00000e90: 5573 6572 2e49 4420 213d 2031 2c20 5573  User.ID != 1, Us
+00000ea0: 6572 2e4e 414d 4520 213d 2022 2229 2e66  er.NAME != "").f
+00000eb0: 6574 6368 5f61 6c6c 2829 0a61 7761 6974  etch_all().await
+00000ec0: 2055 7365 722e 7768 6572 6528 5573 6572   User.where(User
+00000ed0: 2e49 4420 213d 2031 292e 7768 6572 6528  .ID != 1).where(
+00000ee0: 5573 6572 2e4e 414d 4520 213d 2022 2229  User.NAME != "")
+00000ef0: 2e66 6574 6368 5f61 6c6c 2829 0a61 7761  .fetch_all().awa
+00000f00: 6974 2055 7365 722e 7768 6572 6528 5573  it User.where(Us
+00000f10: 6572 2e49 4420 3c3d 2031 302c 2055 7365  er.ID <= 10, Use
+00000f20: 722e 4944 203e 3d20 3230 2c20 6973 5f61  r.ID >= 20, is_a
+00000f30: 6e64 3d46 616c 7365 292e 6665 7463 685f  nd=False).fetch_
+00000f40: 616c 6c28 290a 2320 636f 6d70 6c69 6361  all().# complica
+00000f50: 7465 6420 6578 7072 6573 7369 6f6e 0a61  ted expression.a
+00000f60: 7761 6974 2055 7365 722e 7768 6572 6528  wait User.where(
+00000f70: 5573 6572 2e49 4420 3d3d 2031 292e 7570  User.ID == 1).up
+00000f80: 6461 7465 2861 6765 3d28 5573 6572 2e41  date(age=(User.A
+00000f90: 4745 202b 2031 2920 2f20 2855 7365 722e  GE + 1) / (User.
+00000fa0: 4147 4520 2f20 3132 2920 2d20 3229 0a61  AGE / 12) - 2).a
+00000fb0: 7761 6974 2055 7365 722e 7768 6572 6528  wait User.where(
+00000fc0: 2855 7365 722e 4147 4520 2b20 3129 203d  (User.AGE + 1) =
+00000fd0: 3d20 3329 2e66 6574 6368 5f61 6c6c 2829  = 3).fetch_all()
+00000fe0: 0a23 2063 6f6d 706c 6963 6174 6564 2073  .# complicated s
+00000ff0: 716c 206f 7065 7261 7469 6f6e 0a61 7761  ql operation.awa
+00001000: 6974 2055 7365 722e 7768 6572 6528 5573  it User.where(Us
+00001010: 6572 2e49 4420 3d3d 2075 2e69 6429 2e75  er.ID == u.id).u
+00001020: 7064 6174 6528 0a20 2020 2061 6765 3d55  pdate(.    age=U
+00001030: 7365 722e 4147 452e 6361 7365 2855 7365  ser.AGE.case(Use
+00001040: 722e 4147 4520 3e20 3130 2c20 312c 2064  r.AGE > 10, 1, d
+00001050: 6566 6175 6c74 3d31 3829 2e63 6173 6528  efault=18).case(
+00001060: 5573 6572 2e41 4745 203c 3d20 302c 2031  User.AGE <= 0, 1
+00001070: 3029 0a29 0a63 7265 6174 6564 2c20 7570  0).).created, up
+00001080: 6461 7465 6420 3d20 6177 6169 7420 5573  dated = await Us
+00001090: 6572 5072 6f66 696c 652e 7570 7365 7274  erProfile.upsert
+000010a0: 280a 2020 2020 5b0a 2020 2020 2020 2020  (.    [.        
+000010b0: 6469 6374 2869 643d 312c 206e 616d 653d  dict(id=1, name=
+000010c0: 2275 7073 6572 7422 292c 0a20 2020 205d  "upsert"),.    ]
+000010d0: 2c0a 2020 2020 7570 6461 7465 5f66 6965  ,.    update_fie
+000010e0: 6c64 733d 5b22 6e61 6d65 225d 2c0a 290a  lds=["name"],.).
+000010f0: 2320 6275 6c6b 206f 7065 7261 7469 6f6e  # bulk operation
+00001100: 0a61 7761 6974 2055 7365 722e 6275 6c6b  .await User.bulk
+00001110: 5f63 7265 6174 6528 5b55 7365 7228 6e61  _create([User(na
+00001120: 6d65 3d66 2275 7365 725f 7b69 7d22 2920  me=f"user_{i}") 
+00001130: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
+00001140: 3029 5d29 0a61 7761 6974 2055 7365 722e  0)]).await User.
+00001150: 6275 6c6b 5f75 7064 6174 6528 6177 6169  bulk_update(awai
+00001160: 7420 5573 6572 2e66 6574 6368 5f61 6c6c  t User.fetch_all
+00001170: 2829 290a 6177 6169 7420 5573 6572 2e62  ()).await User.b
+00001180: 756c 6b5f 6465 6c65 7465 2861 7761 6974  ulk_delete(await
+00001190: 2055 7365 722e 6665 7463 685f 616c 6c28   User.fetch_all(
+000011a0: 2929 0a23 2073 686f 7274 6375 740a 7573  )).# shortcut.us
+000011b0: 6572 2c20 6372 6561 7465 6420 3d20 6177  er, created = aw
+000011c0: 6169 7420 5573 6572 2869 643d 312c 206e  ait User(id=1, n
+000011d0: 616d 653d 2263 7265 6174 6564 3f22 292e  ame="created?").
+000011e0: 6765 745f 6f72 5f63 7265 6174 6528 0a20  get_or_create(. 
+000011f0: 2020 206b 6579 5f66 6965 6c64 733d 2855     key_fields=(U
+00001200: 7365 722e 4944 2c29 0a29 0a75 7365 722c  ser.ID,).).user,
+00001210: 2063 7265 6174 6564 2c20 7570 6461 7465   created, update
+00001220: 6420 3d20 6177 6169 7420 5573 6572 2869  d = await User(i
+00001230: 643d 322c 206e 616d 653d 2275 7064 6174  d=2, name="updat
+00001240: 6564 3f22 292e 6372 6561 7465 5f6f 725f  ed?").create_or_
+00001250: 7570 6461 7465 280a 2020 2020 6b65 795f  update(.    key_
+00001260: 6669 656c 6473 3d28 5573 6572 2e49 442c  fields=(User.ID,
+00001270: 290a 290a 6060 60                        ).).```
```

### Comparing `danio-0.5.0/PKG-INFO` & `danio-0.5.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: danio
-Version: 0.5.0
+Version: 0.5.1
 Summary: ORM for asyncio world by dataclass
 License: BSD 3-Clause
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -42,14 +46,15 @@
 * keep OOM in mind, custom your Field and Model behavior easily
 * type hints any where, no more need to memorize words your field names any more
 * base CRUD operation, transactions, lock and so on
 * signals like before save, after save and so on
 * complex operation like bulk create, upsert, create or update and so on
 * assist model schema migration
 * support MySQL/PostgreSQL/SQLite
+* hints generation
 
 ## install
 
 `pip install danio`
 
 ## Documents
 
@@ -64,83 +69,97 @@
     charset="utf8mb4",
     use_unicode=True,
     connect_timeout=60,
 )
 
 @dataclasses.dataclass
 class User(danio.Model):
+    # auto generated by danio:
+    # --------------------Danio Hints--------------------
+    # TABLE NAME: user
+    # TABLE IS MIGRATED!
+    ID: typing.ClassVar[danio.Field]  # "id" serial PRIMARY KEY NOT NULL
+    NAME: typing.ClassVar[danio.Field]  # "name" varchar(255)  NOT NULL
+    AGE: typing.ClassVar[danio.Field]  # "age" int  NOT NULL
+    CREATED_AT: typing.ClassVar[
+        danio.Field
+    ]  # "created_at" timestamp without time zone  NOT NULL
+    UPDATED_AT: typing.ClassVar[
+        danio.Field
+    ]  # "updated_at" timestamp without time zone  NOT NULL
+    GENDER: typing.ClassVar[danio.Field]  # "gender" int  NOT NULL
+    # --------------------Danio Hints--------------------
+
     class Gender(enum.Enum):
         MALE = 0
         FEMALE = 1
         OTHER = 2
 
-    name: str = danio.field(
-        danio.CharField,
-        comment="User name",
-        default=danio.CharField.NoDefault,
-    )
-    age: int = danio.field(danio.IntField)
-    created_at: datetime.datetime = danio.field(
-        danio.DateTimeField,
-        comment="when created",
-    )
-    updated_at: datetime.datetime = danio.field(
-        danio.DateTimeField,
-        comment="when created",
-    )
-    gender: Gender = danio.field(danio.IntField, enum=Gender, default=Gender.FEMALE)
-
-    async def before_create(self, **kwargs):
-        # user_count += 1
-        await super().before_create(**kwargs)
+    id: typing.Annotated[int, danio.IntField(primary=True, type="serial")] = 0
+    name: typing.Annotated[str, danio.CharField(comment="User name")] = ""
+    age: typing.Annotated[int, danio.IntField] = 0
+    created_at: typing.Annotated[
+        datetime.datetime,
+        danio.DateTimeField(type="timestamp without time zone", comment="when created"),
+    ] = dataclasses.field(default_factory=datetime.datetime.now)
+    updated_at: typing.Annotated[
+        datetime.datetime,
+        danio.DateTimeField(type="timestamp without time zone", comment="when updated"),
+    ] = dataclasses.field(default_factory=datetime.datetime.now)
+    gender: typing.Annotated[Gender, danio.IntField(enum=Gender)] = Gender.MALE
+
+
+    async def before_create(self, validate=True):
+        await super().before_create(validate=True)
 
-    async def before_update(self, **kwargs):
+    async def before_update(self, validate=True):
         self.updated_at = datetime.datetime.now()
+        await super().before_update(validate=True)
 
     async def validate(self):
         await super().validate()
         if not self.name:
             raise danio.ValidateException("Empty name!")
 
     @classmethod
     def get_database(
         cls, operation: danio.Operation, table: str, *args, **kwargs
     ) -> danio.Database:
         return db
 
 # base CRUD
 user = await User(name="batman").save()
-user = await User.where(User.name == "batman").fetch_one()
+user = await User.where(User.NAME == "batman").fetch_one()
 user.gender = User.Gender.MALE
 await user.save()
 await user.delete()
 # sql chain
-await User.where(User.name != "").limit(10).fetch_all()
+await User.where(User.NAME != "").limit(10).fetch_all()
 # multi where condition
-await User.where(User.id != 1, User.name != "").fetch_all()
-await User.where(User.id != 1).where(User.name != "").fetch_all()
-await User.where(User.id <= 10, User.id >= 20, is_and=False).fetch_all()
+await User.where(User.ID != 1, User.NAME != "").fetch_all()
+await User.where(User.ID != 1).where(User.NAME != "").fetch_all()
+await User.where(User.ID <= 10, User.ID >= 20, is_and=False).fetch_all()
 # complicated expression
-await User.where(User.id == 1).update(age=(User.age + 1) / (User.age / 12) - 2)
-await User.where((User.age + 1) == 3).fetch_all()
+await User.where(User.ID == 1).update(age=(User.AGE + 1) / (User.AGE / 12) - 2)
+await User.where((User.AGE + 1) == 3).fetch_all()
 # complicated sql operation
-await User.where(User.id == u.id).update(
-    age=User.age.case(User.age > 10, 1, default=18).case(User.age <= 0, 10)
+await User.where(User.ID == u.id).update(
+    age=User.AGE.case(User.AGE > 10, 1, default=18).case(User.AGE <= 0, 10)
 )
 created, updated = await UserProfile.upsert(
     [
         dict(id=1, name="upsert"),
     ],
     update_fields=["name"],
 )
 # bulk operation
 await User.bulk_create([User(name=f"user_{i}") for i in range(10)])
 await User.bulk_update(await User.fetch_all())
 await User.bulk_delete(await User.fetch_all())
 # shortcut
 user, created = await User(id=1, name="created?").get_or_create(
-    key_fields=(User.id,)
+    key_fields=(User.ID,)
 )
 user, created, updated = await User(id=2, name="updated?").create_or_update(
-    key_fields=(User.id,)
+    key_fields=(User.ID,)
 )
 ```
```

