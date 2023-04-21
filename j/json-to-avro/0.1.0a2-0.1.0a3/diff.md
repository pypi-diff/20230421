# Comparing `tmp/json_to_avro-0.1.0a2.tar.gz` & `tmp/json_to_avro-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_to_avro-0.1.0a2.tar", max compression
+gzip compressed data, was "json_to_avro-0.1.0a3.tar", max compression
```

## Comparing `json_to_avro-0.1.0a2.tar` & `json_to_avro-0.1.0a3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-04-04 02:26:42.522535 json_to_avro-0.1.0a2/LICENSE
--rw-r--r--   0        0        0      164 2023-04-04 02:26:42.522747 json_to_avro-0.1.0a2/README.md
--rw-r--r--   0        0        0      118 2023-04-04 03:08:07.257369 json_to_avro-0.1.0a2/json_to_avro/__init__.py
--rw-r--r--   0        0        0      137 2023-04-02 12:57:49.274953 json_to_avro-0.1.0a2/json_to_avro/avro_schema/__init__.py
--rw-r--r--   0        0        0      382 2023-04-03 00:51:50.805483 json_to_avro-0.1.0a2/json_to_avro/avro_schema/avro_schema_candidate.py
--rw-r--r--   0        0        0    22789 2023-04-03 00:51:32.672085 json_to_avro-0.1.0a2/json_to_avro/avro_schema/mergeable_avro_schema.py
--rw-r--r--   0        0        0      627 2023-04-02 12:47:35.245199 json_to_avro-0.1.0a2/json_to_avro/avro_schema/registered_avro_schema.py
--rw-r--r--   0        0        0      236 2023-04-04 03:06:12.999164 json_to_avro-0.1.0a2/json_to_avro/avroable_data.py
--rw-r--r--   0        0        0     2385 2023-04-04 03:06:13.003710 json_to_avro-0.1.0a2/json_to_avro/json_to_avro.py
--rw-r--r--   0        0        0     2248 2023-04-04 03:06:12.994200 json_to_avro-0.1.0a2/json_to_avro/schema_provider.py
--rw-r--r--   0        0        0      733 2023-04-04 03:09:26.636942 json_to_avro-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 json_to_avro-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-04 02:26:42.522535 json_to_avro-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0      164 2023-04-04 02:26:42.522747 json_to_avro-0.1.0a3/README.md
+-rw-r--r--   0        0        0      194 2023-04-13 03:08:27.218434 json_to_avro-0.1.0a3/json_to_avro/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-21 00:04:25.942111 json_to_avro-0.1.0a3/json_to_avro/avro_schema/__init__.py
+-rw-r--r--   0        0        0      369 2023-04-13 10:47:53.464735 json_to_avro-0.1.0a3/json_to_avro/avro_schema/avro_schema_candidate.py
+-rw-r--r--   0        0        0    21973 2023-04-16 04:07:57.682016 json_to_avro-0.1.0a3/json_to_avro/avro_schema/mergeable_avro_schema.py
+-rw-r--r--   0        0        0      627 2023-04-13 03:07:50.323202 json_to_avro-0.1.0a3/json_to_avro/avro_schema/registered_avro_schema.py
+-rw-r--r--   0        0        0      236 2023-04-13 03:07:50.323401 json_to_avro-0.1.0a3/json_to_avro/avroable_data.py
+-rw-r--r--   0        0        0     2385 2023-04-13 03:07:50.323603 json_to_avro-0.1.0a3/json_to_avro/json_to_avro.py
+-rw-r--r--   0        0        0     2816 2023-04-21 00:30:05.218588 json_to_avro-0.1.0a3/json_to_avro/schema_provider.py
+-rw-r--r--   0        0        0      733 2023-04-21 00:31:11.857365 json_to_avro-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 json_to_avro-0.1.0a3/PKG-INFO
```

### Comparing `json_to_avro-0.1.0a2/LICENSE` & `json_to_avro-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_avro-0.1.0a2/json_to_avro/avro_schema/mergeable_avro_schema.py` & `json_to_avro-0.1.0a3/json_to_avro/avro_schema/mergeable_avro_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,86 +1,54 @@
 import dataclasses
 import json
 from typing import (
-    List,
-    TypedDict,
     Any,
-    Optional,
-    Literal,
 )
-from json_to_avro.json_to_avro.avroable_data import AvroableData, Json
-
-NullAvroType = Literal["null"]
-PrimitiveAvroType = Literal["string", "long", "double", "boolean"]
-
-
-class ArrayAvroType(TypedDict, total=False):
-    type: Literal["array"]
-    items: "AvroType"
-    default: Optional[Any]
-
-
-class AvroField(TypedDict, total=False):
-    name: str
-    type: "AvroType"
-    default: Optional[Any]
-
-
-class RecordAvroType(TypedDict, total=False):
-    type: Literal["record"]
-    name: str
-    fields: List[AvroField]
-    default: Optional[Any]
-
-
-class NullableAvroType(TypedDict, total=False):
-    type: list[Literal["null"] | "AvroType"]
-
-
-AvroType = NullAvroType | PrimitiveAvroType | ArrayAvroType | RecordAvroType
 
+from json_to_avro.avroable_data import AvroableData
 
 PYTHON_TO_AVRO_TYPES = {
     str: "string",
     int: "long",
     float: "double",
     bool: "boolean",
     list: "array",
     dict: "record",
 }
+
 @dataclasses.dataclass
 class MergeableAvroSchema:
-    schema_dict: RecordAvroType
+    schema_dict: dict
 
     def __add__(self, other: "MergeableAvroSchema") -> "MergeableAvroSchema":
         return self.merge_schemas(self.schema_dict, other.schema_dict)
 
     @classmethod
     def merge_schemas(
-        cls, self_data: RecordAvroType, other_data: RecordAvroType
+        cls, self_data: dict, other_data: dict
     ) -> "MergeableAvroSchema":
         return cls(cls._merge_schemas(self_data, other_data))
 
     @classmethod
     def _merge_schemas(
         cls,
-        self_data: RecordAvroType,
-        other_data: RecordAvroType,
-    ) -> RecordAvroType:
-        combined_fields = []
+        self_data: Any,
+        other_data: Any,
+    ) -> Any:
+        combined_fields: list[Any] = []
         for fst, snd in list(
             zip(
                 sorted(self_data["fields"], key=lambda r: r["name"]),
                 sorted(other_data["fields"], key=lambda r: r["name"]),
             )
         ):
             combined_fields = [*combined_fields, fst, snd]
 
         existing_schema_fields = set(field["name"] for field in self_data["fields"])
-        updated_fields: dict[str, AvroField] = {}
+        updated_fields: dict[Any, Any] = {}
 
         for field in combined_fields:
             match updated_fields.get(field["name"]), field:
                 # if updated field and the new are the same, overwrite
                 case (existing, new) if existing == new:
                     updated_fields[field["name"]] = field
                 # if the field already exists in the schema, add it to the update set
@@ -484,15 +452,15 @@
                 case _:
                     print(type(field["type"]))
                     print(type(updated_fields[field["name"]]["type"]))
                     raise NotImplementedError(
                         f"Can't merge {field} with {updated_fields[field['name']]}"
                     )
 
-        return RecordAvroType(
+        return dict(
             name=self_data["name"],
             type="record",
             fields=sorted(list(updated_fields.values()), key=lambda f: f["name"]),
         )
 
     @property
     def schema_str(self) -> str:
@@ -504,17 +472,17 @@
             schema_dict=cls.convert_json_to_avro_schema(
                 msg.data, msg.record_name
             ),
         )
 
     @staticmethod
     def convert_json_to_avro_schema(
-        json_data: dict[str, Json], name: str
-    ) -> RecordAvroType:
-        avro_schema: RecordAvroType = {"type": "record", "name": name, "fields": []}
+        json_data: Any, name: str
+    ) -> dict:
+        avro_schema: dict = {"type": "record", "name": name, "fields": []}
 
         for key, value in json_data.items():
             match value:
                 case dict(_):
                     avro_schema["fields"].append(
                         {
                             "name": key,
```

### Comparing `json_to_avro-0.1.0a2/json_to_avro/avro_schema/registered_avro_schema.py` & `json_to_avro-0.1.0a3/json_to_avro/avro_schema/registered_avro_schema.py`

 * *Files identical despite different names*

### Comparing `json_to_avro-0.1.0a2/json_to_avro/json_to_avro.py` & `json_to_avro-0.1.0a3/json_to_avro/json_to_avro.py`

 * *Files identical despite different names*

### Comparing `json_to_avro-0.1.0a2/json_to_avro/schema_provider.py` & `json_to_avro-0.1.0a3/json_to_avro/schema_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+import functools
+from typing import Callable, Optional
+
 from schema_registry.client import AsyncSchemaRegistryClient, SchemaRegistryClient
 from schema_registry.client.utils import SchemaVersion
 
 from json_to_avro.avro_schema.avro_schema_candidate import AvroSchemaCandidate
 from json_to_avro.avro_schema.registered_avro_schema import RegisteredAvroSchema, RegisteredAvroSchemaId
+from loguru import logger
+
+
+def ensure_backwards_transitive_compatibility(func: Callable) -> Callable:
+    @functools.wraps(func)
+    def wraps(*args):
+        self, subject, *_ = args
+        if subject not in self.current_schema_table:
+            logger.debug("Setting compatibility to BACKWARD_TRANSITIVE for %s" % subject)
+            self.schema_registry_client.update_compatibility("BACKWARD_TRANSITIVE", subject)
+        return func(*args)
+    return wraps
 
 
 class SchemaProvider:
     def __init__(
         self,
         current_schema_table: dict[str, RegisteredAvroSchema],
         schema_registry_client: SchemaRegistryClient,
@@ -21,14 +36,15 @@
 
     def __getitem__(self, subject: str) -> RegisteredAvroSchema:
         """Unsafe version of `get`
         :raises KeyError
         """
         return self.current_schema_table[subject]
 
+    @ensure_backwards_transitive_compatibility
     def get(self, subject_name: str) -> RegisteredAvroSchema | None:
         if subject_name in self.current_schema_table:
             return self.current_schema_table[subject_name]
 
         schema_version: SchemaVersion | None = self.schema_registry_client.get_schema(
             subject_name, version="latest"
         )
```

### Comparing `json_to_avro-0.1.0a2/pyproject.toml` & `json_to_avro-0.1.0a3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "json-to-avro"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = "Convert arbitrary JSON data to avro serialized data, registering transitively backwards compatible schemas with Kafka Schema Registry along the way."
 authors = ["Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "json_to_avro"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-schema-registry-client = {extras = ["avro"], version = "^2.4.1"}
-loguru = "^0.6.0"
+python-schema-registry-client = {extras = ["avro"], version = "^2.4.3"}
+loguru = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.0.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.3"
 black = "^23.1.0"
```

### Comparing `json_to_avro-0.1.0a2/PKG-INFO` & `json_to_avro-0.1.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: json-to-avro
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: Convert arbitrary JSON data to avro serialized data, registering transitively backwards compatible schemas with Kafka Schema Registry along the way.
 License: MIT
 Author: Brad Boggs
 Author-email: bboggs@streambit.software
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: python-schema-registry-client[avro] (>=2.4.1,<3.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: python-schema-registry-client[avro] (>=2.4.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # json-to-avro
 Convert arbitrary JSON data to avro serialized data, registering transitively backwards compatible schemas with Kafka Schema Registry along the way.
```

