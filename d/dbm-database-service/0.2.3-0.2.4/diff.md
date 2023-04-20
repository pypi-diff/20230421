# Comparing `tmp/dbm_database_service-0.2.3.tar.gz` & `tmp/dbm_database_service-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm_database_service-0.2.3.tar", max compression
+gzip compressed data, was "dbm_database_service-0.2.4.tar", max compression
```

## Comparing `dbm_database_service-0.2.3.tar` & `dbm_database_service-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.3/dbm_database_service/__init__.py
--rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.3/dbm_database_service/connectors.py
--rw-r--r--   0        0        0     3208 2023-04-20 19:41:30.227951 dbm_database_service-0.2.3/dbm_database_service/managers.py
--rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.3/dbm_database_service/models/__init__.py
--rw-r--r--   0        0        0     1612 2023-04-17 21:13:25.033005 dbm_database_service-0.2.3/dbm_database_service/models/column.py
--rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.3/dbm_database_service/models/config.py
--rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.3/dbm_database_service/models/datatype.py
--rw-r--r--   0        0        0      930 2023-04-20 19:41:30.108418 dbm_database_service-0.2.3/dbm_database_service/models/table.py
--rw-r--r--   0        0        0      655 2023-04-20 19:41:30.217534 dbm_database_service-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.3/README.md
--rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-12 14:45:46.980021 dbm_database_service-0.2.4/dbm_database_service/__init__.py
+-rw-r--r--   0        0        0     6676 2023-04-17 21:03:44.747568 dbm_database_service-0.2.4/dbm_database_service/connectors.py
+-rw-r--r--   0        0        0     3208 2023-04-20 19:41:30.227951 dbm_database_service-0.2.4/dbm_database_service/managers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:01:03.393096 dbm_database_service-0.2.4/dbm_database_service/models/__init__.py
+-rw-r--r--   0        0        0     1616 2023-04-20 19:48:51.057728 dbm_database_service-0.2.4/dbm_database_service/models/column.py
+-rw-r--r--   0        0        0      849 2023-04-17 21:13:25.022589 dbm_database_service-0.2.4/dbm_database_service/models/config.py
+-rw-r--r--   0        0        0     1232 2023-04-17 21:13:25.043780 dbm_database_service-0.2.4/dbm_database_service/models/datatype.py
+-rw-r--r--   0        0        0      930 2023-04-20 19:41:30.108418 dbm_database_service-0.2.4/dbm_database_service/models/table.py
+-rw-r--r--   0        0        0      655 2023-04-20 22:18:11.978518 dbm_database_service-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    13467 2023-04-18 09:36:53.242538 dbm_database_service-0.2.4/README.md
+-rw-r--r--   0        0        0    13586 1970-01-01 00:00:00.000000 dbm_database_service-0.2.4/PKG-INFO
```

### Comparing `dbm_database_service-0.2.3/dbm_database_service/connectors.py` & `dbm_database_service-0.2.4/dbm_database_service/connectors.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/dbm_database_service/managers.py` & `dbm_database_service-0.2.4/dbm_database_service/managers.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/dbm_database_service/models/column.py` & `dbm_database_service-0.2.4/dbm_database_service/models/column.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 @dataclass
 class Column:
     """ Needs minimum of name and datatype to parse and can be extended by primary key, autoincrement, unique, default, not_null"""
     name: str
     datatype: DataType
     primary_key: bool = False
-    autoincrement: bool = False
+    auto_increment: bool = False
     unique: bool = False
     default: Any = None
     not_null: bool = False
 
     def __post_init__(self) -> None:
         """ Validates if provided arguments are valid """
         namespaces = self.__dict__
         constraints = {
             "name": {Constraint.STRING_REGEX: r'^[a-zA-Z_][a-zA-Z0-9_]{1,64}$'},
             "primary_key": {Constraint.IS_TYPE: bool},
-            "autoincrement": {Constraint.IS_TYPE: bool},
+            "auto_increment": {Constraint.IS_TYPE: bool},
             "unique": {Constraint.IS_TYPE: bool},
             "not_null": {Constraint.IS_TYPE: bool}
         }
         validate_json_data(namespaces, constraints)
 
     def __str__(self):
         """ Will be parsed in other objects. Outcome is valid sql string describing column """
         return f"{self.name} {self.datatype}" \
                f"{' primary key' if self.primary_key else ''}" \
-               f"{' autoincrement' if self.autoincrement else ''}" \
+               f"{' auto_increment' if self.auto_increment else ''}" \
                f"{' unique' if self.unique else ''}" \
                f"{' not null' if self.not_null else ''}" \
                f"{f' default {self.default}' if self.default else ''}"
```

### Comparing `dbm_database_service-0.2.3/dbm_database_service/models/config.py` & `dbm_database_service-0.2.4/dbm_database_service/models/config.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/dbm_database_service/models/datatype.py` & `dbm_database_service-0.2.4/dbm_database_service/models/datatype.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/dbm_database_service/models/table.py` & `dbm_database_service-0.2.4/dbm_database_service/models/table.py`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/pyproject.toml` & `dbm_database_service-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbm-database-service"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Smolke <d.smolczynski1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dbm_database_service"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dbm_database_service-0.2.3/README.md` & `dbm_database_service-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dbm_database_service-0.2.3/PKG-INFO` & `dbm_database_service-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbm-database-service
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: easyvalid-data-validator (>=0.1.1,<0.2.0)
```

