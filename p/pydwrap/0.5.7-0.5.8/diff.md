# Comparing `tmp/pydwrap-0.5.7.tar.gz` & `tmp/pydwrap-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydwrap-0.5.7.tar", max compression
+gzip compressed data, was "pydwrap-0.5.8.tar", max compression
```

## Comparing `pydwrap-0.5.7.tar` & `pydwrap-0.5.8.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-03-24 13:21:49.321460 pydwrap-0.5.7/LICENSE
--rw-r--r--   0        0        0     1205 2023-03-24 13:53:27.176284 pydwrap-0.5.7/README.md
--rw-r--r--   0        0        0       69 2023-03-30 16:20:21.356084 pydwrap-0.5.7/pydwrap/__init__.py
--rw-r--r--   0        0        0     4168 2023-04-13 21:03:38.694510 pydwrap-0.5.7/pydwrap/main.py
--rw-r--r--   0        0        0     1203 2023-04-13 21:05:56.281711 pydwrap-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 pydwrap-0.5.7/setup.py
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pydwrap-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-13 21:37:36.137941 pydwrap-0.5.8/LICENSE
+-rw-r--r--   0        0        0     1205 2023-04-13 21:37:36.137941 pydwrap-0.5.8/README.md
+-rw-r--r--   0        0        0       69 2023-04-13 21:37:36.137941 pydwrap-0.5.8/pydwrap/__init__.py
+-rw-r--r--   0        0        0     4390 2023-04-21 20:43:09.749102 pydwrap-0.5.8/pydwrap/main.py
+-rw-r--r--   0        0        0     1203 2023-04-21 20:43:49.656625 pydwrap-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 pydwrap-0.5.8/PKG-INFO
```

### Comparing `pydwrap-0.5.7/LICENSE` & `pydwrap-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwrap-0.5.7/README.md` & `pydwrap-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pydwrap-0.5.7/pydwrap/main.py` & `pydwrap-0.5.8/pydwrap/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Generic, Type, TypeVar, cast, get_origin
 
 from pydantic import BaseModel as OriginalBaseModel
 from pydantic import create_model, root_validator
 from pydantic.fields import ModelField
+from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.typing import is_none_type
 
 _T = TypeVar("_T")
 _V = TypeVar("_V")
 ValidatorOptionValue = TypeVar("ValidatorOptionValue", bound="BaseModel")
 
 
@@ -33,15 +34,17 @@
     def __get_validators__(cls):
         yield cls.option_validator
 
     @classmethod
     def option_validator(cls, v: Any, field: ModelField) -> Option[_T]:
         field_name: str = field.name.removeprefix("_").removesuffix("_")
         if field.outer_type_ is Option:
-            raise TypeError("To type an Option, it is necessary to specify a parameter in its generic.")
+            raise TypeError(
+                "To type an Option, it is necessary to specify a parameter in its generic."
+            )
         if v is None:
             return cls(v)
         if isinstance(v, cls) and v.is_none:
             return v
         validator = _create_validator_option_value(
             field_name,
             v.unwrap() if isinstance(v, cls) else v,
@@ -68,24 +71,27 @@
         """
         if variant is None:
             raise TypeError("Variant should not be type NoneType.")
         return self.__value if self.__value is not None else variant
 
 
 class BaseModel(OriginalBaseModel):
-    @root_validator(pre=True)  # NOTE: Pycharm doesn't understand that @root_validator returns a classmethod.
+    @root_validator(
+        pre=True
+    )  # NOTE: Pycharm doesn't understand that @root_validator returns a classmethod.
     @classmethod
     def _pre_root_validator(cls, values: dict[str, Any]) -> dict[str, Any]:
         model_schema = cls.schema()
         fields = _get_default_fields(model_schema)
         fields.update(_get_required_option_fields(cls.__annotations__, model_schema))
         fields.update(values)
         return {
             field: Option(value)
-            if _is_option_type(cls.__annotations__.get(field, None)) and not isinstance(value, Option)
+            if _is_option_type(cls.__annotations__.get(field, None))
+            and not isinstance(value, Option)
             else value
             for field, value in fields.items()
         }
 
 
 def _is_option_type(type_: Type[Any]) -> bool:
     if is_none_type(type_):
@@ -94,30 +100,41 @@
     if is_none_type(origin):
         return False
     return origin is Option
 
 
 def _get_default_fields(schema: dict[str, Any]) -> dict[str, Any]:
     properties = cast(dict[str, Any], schema.get("properties", {}))
-    return {k: properties[k]["default"] for k in properties if "default" in properties[k]}
+    return {
+        k: properties[k]["default"] for k in properties if "default" in properties[k]
+    }
 
 
-def _get_required_option_fields(model_annotations: dict[str, Any], schema: dict[str, Any]) -> dict[str, Option]:
+def _get_required_option_fields(
+    model_annotations: dict[str, Any], schema: dict[str, Any]
+) -> dict[str, Option]:
     properties = cast(dict[str, Any], schema.get("properties", {}))
     return {
         k: Option()
         for k in properties
-        if k in schema.get("required", []) or "default" not in properties[k] and _is_option_type(model_annotations[k])
+        if k in schema.get("required", [])
+        or "default" not in properties[k]
+        and _is_option_type(model_annotations[k])
     }
 
 
-def _create_validator_option_value(field_name: str, field_value: Any, field_type: Type[Any]) -> ValidatorOptionValue:
+def _create_validator_option_value(
+    field_name: str, field_value: Any, field_type: Type[Any]
+) -> ValidatorOptionValue:
     return create_model(
         "ValidatorOptionValue",
         __base__=BaseModel,
         **{
             field_name: (
                 field_type,
                 field_value,
             )
         },
     )()
+
+
+ENCODERS_BY_TYPE.update({Option: lambda o: None if o.is_none else o.unwrap()})
```

### Comparing `pydwrap-0.5.7/pyproject.toml` & `pydwrap-0.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydwrap"
-version = "0.5.7"
+version = "0.5.8"
 description = "pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object."
 authors = ["Georgy howl <howluwqz1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydwrap"}]
 homepage = "https://github.com/luwqz1/pydwrap"
 repository = "https://github.com/luwqz1/pydwrap"
```

### Comparing `pydwrap-0.5.7/PKG-INFO` & `pydwrap-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydwrap
-Version: 0.5.7
+Version: 0.5.8
 Summary: pydwrap stores a Option object to implement unpacking of values if they are not None. The BaseModel object is also a little extended to work with the Option object.
 Home-page: https://github.com/luwqz1/pydwrap
 License: MIT
 Keywords: python,wrapping,optional handle,basemodel fields,option,pydwrap
 Author: Georgy howl
 Author-email: howluwqz1@gmail.com
 Requires-Python: >=3.9,<4.0
```

