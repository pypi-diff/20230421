# Comparing `tmp/chili-2.0.1.tar.gz` & `tmp/chili-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chili-2.0.1.tar", max compression
+gzip compressed data, was "chili-2.1.0.tar", max compression
```

## Comparing `chili-2.0.1.tar` & `chili-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1085 2023-04-19 16:12:17.796775 chili-2.0.1/LICENSE
--rw-r--r--   0        0        0    12227 2023-04-19 16:12:17.796775 chili-2.0.1/README.md
--rw-r--r--   0        0        0      614 2023-04-19 16:12:17.796775 chili-2.0.1/chili/__init__.py
--rw-r--r--   0        0        0       22 2023-04-19 16:12:17.800775 chili-2.0.1/chili/__version__.py
--rw-r--r--   0        0        0    16042 2023-04-19 16:12:17.800775 chili-2.0.1/chili/decoder.py
--rw-r--r--   0        0        0    13956 2023-04-19 16:12:17.800775 chili-2.0.1/chili/encoder.py
--rw-r--r--   0        0        0      411 2023-04-19 16:12:17.800775 chili-2.0.1/chili/error.py
--rw-r--r--   0        0        0     5741 2023-04-19 16:12:17.800775 chili-2.0.1/chili/iso_datetime.py
--rw-r--r--   0        0        0     1093 2023-04-19 16:12:17.800775 chili-2.0.1/chili/json_support.py
--rw-r--r--   0        0        0     3155 2023-04-19 16:12:17.800775 chili-2.0.1/chili/mapper.py
--rw-r--r--   0        0        0        0 2023-04-19 16:12:17.800775 chili-2.0.1/chili/py.typed
--rw-r--r--   0        0        0     1513 2023-04-19 16:12:17.800775 chili-2.0.1/chili/serializer.py
--rw-r--r--   0        0        0      260 2023-04-19 16:12:17.800775 chili-2.0.1/chili/state.py
--rw-r--r--   0        0        0     6361 2023-04-19 16:12:17.800775 chili-2.0.1/chili/typing.py
--rw-r--r--   0        0        0     1228 2023-04-19 16:12:17.800775 chili-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    13622 1970-01-01 00:00:00.000000 chili-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-21 19:55:34.660329 chili-2.1.0/LICENSE
+-rw-r--r--   0        0        0    18489 2023-04-21 19:55:34.660329 chili-2.1.0/README.md
+-rw-r--r--   0        0        0      639 2023-04-21 19:55:34.664330 chili-2.1.0/chili/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-21 19:55:34.664330 chili-2.1.0/chili/__version__.py
+-rw-r--r--   0        0        0    16863 2023-04-21 19:55:34.664330 chili-2.1.0/chili/decoder.py
+-rw-r--r--   0        0        0    14914 2023-04-21 19:55:34.664330 chili-2.1.0/chili/encoder.py
+-rw-r--r--   0        0        0      411 2023-04-21 19:55:34.664330 chili-2.1.0/chili/error.py
+-rw-r--r--   0        0        0     5741 2023-04-21 19:55:34.664330 chili-2.1.0/chili/iso_datetime.py
+-rw-r--r--   0        0        0     1093 2023-04-21 19:55:34.664330 chili-2.1.0/chili/json_support.py
+-rw-r--r--   0        0        0     3202 2023-04-21 19:55:34.664330 chili-2.1.0/chili/mapper.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:55:34.664330 chili-2.1.0/chili/py.typed
+-rw-r--r--   0        0        0     1542 2023-04-21 19:55:34.664330 chili-2.1.0/chili/serializer.py
+-rw-r--r--   0        0        0      260 2023-04-21 19:55:34.664330 chili-2.1.0/chili/state.py
+-rw-r--r--   0        0        0     6603 2023-04-21 19:55:34.664330 chili-2.1.0/chili/typing.py
+-rw-r--r--   0        0        0     1228 2023-04-21 19:55:34.664330 chili-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    19884 1970-01-01 00:00:00.000000 chili-2.1.0/PKG-INFO
```

### Comparing `chili-2.0.1/LICENSE` & `chili-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chili-2.0.1/chili/__init__.py` & `chili-2.1.0/chili/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from .decoder import Decoder, decodable, TypeDecoder, decode
 from .encoder import Encoder, encodable, TypeEncoder, encode
-from .json_support import json_encode, json_decode, JsonDecoder, JsonEncoder, JsonSerializer
+from .json_support import (
+    json_encode,
+    json_decode,
+    JsonDecoder,
+    JsonEncoder,
+    JsonSerializer,
+)
 from .serializer import serializable, Serializer
 from .mapper import Mapper, KeyScheme
 
 __all__ = [
     "Encoder",
     "JsonEncoder",
     "TypeEncoder",
```

### Comparing `chili-2.0.1/chili/decoder.py` & `chili-2.1.0/chili/decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,23 @@
     map_generic_type,
     is_optional,
     get_type_args,
     unpack_optional,
     is_decodable,
     UNDEFINED,
     is_class,
+    is_newtype,
+)
+from .error import DecoderError
+from .iso_datetime import (
+    parse_iso_datetime,
+    parse_iso_duration,
+    parse_iso_date,
+    parse_iso_time,
 )
-from .error import EncoderError, DecoderError
-from .iso_datetime import parse_iso_datetime, parse_iso_duration, parse_iso_date, parse_iso_time
 from .state import StateObject
 
 C = TypeVar("C")
 U = TypeVar("U")
 T = TypeVar("T")
 E = TypeVar("E", bound=Enum)
 
@@ -247,17 +253,18 @@
         raise DecoderError.invalid_input(value)
 
 
 class ClassDecoder(TypeDecoder):
     _fields: Dict[str, TypeDecoder]
     _schema: TypeSchema
 
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_decoders: TypeDecoders = None):
         self.class_name = class_name
         self._schema = create_schema(class_name)
+        self._extra_decoders = extra_decoders
 
     def decode(self, value: StateObject) -> Any:
         if not isinstance(value, dict):
             raise DecoderError.invalid_input
 
         if not hasattr(self, "_fields"):
             self._fields = self._build()
@@ -276,43 +283,47 @@
 
         return instance
 
     def _build(self) -> Dict[str, TypeDecoder]:
         return {name: self._build_type_decoder(field.type) for name, field in self._schema.items()}
 
     def _build_type_decoder(self, a_type: Type) -> TypeDecoder:
-        return build_type_decoder(a_type, module=self.class_name.__module__)  # type: ignore
+        return build_type_decoder(a_type, self._extra_decoders, self.class_name.__module__)  # type: ignore
 
 
 class GenericClassDecoder(ClassDecoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_decoders: TypeDecoders = None):
         self._generic_type = class_name
         self._generic_parameters = get_parameters_map(class_name)
+        self._extra_decoders = extra_decoders
         type_: Type = get_origin_type(class_name)  # type: ignore
         super().__init__(type_)
 
     def _build_type_decoder(self, a_type: Type) -> TypeDecoder:
         return build_type_decoder(
-            map_generic_type(a_type, self._generic_parameters), module=self._generic_type.__module__
+            map_generic_type(a_type, self._generic_parameters),
+            self._extra_decoders,
+            self._generic_type.__module__,
         )
 
 
 class EnumDecoder(TypeDecoder, Generic[E]):
     def __init__(self, class_name: Type):
         self.class_name = class_name
 
     def decode(self, value: Any) -> E:
         return self.class_name(value)
 
 
 class NamedTupleDecoder(TypeDecoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_decoders: TypeDecoders = None):
         self.class_name = class_name
         self._is_typed = hasattr(class_name, "__annotations__")
         self._arg_decoders: List[TypeDecoder] = []
+        self._extra_decoders = extra_decoders
         if self._is_typed:
             self._build()
 
     def decode(self, value: list) -> tuple:
         if not self._is_typed:
             return tuple(value)
 
@@ -325,23 +336,24 @@
             decoded_values.append(item)
 
         return tuple(decoded_values)
 
     def _build(self) -> None:
         field_types = self.class_name.__annotations__
         for item_type in field_types.values():
-            self._arg_decoders.append(build_type_decoder(item_type, module=self.class_name.__module__))
+            self._arg_decoders.append(build_type_decoder(item_type, self._extra_decoders, self.class_name.__module__))
 
 
 class TypedDictDecoder(TypeDecoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_decoders: TypeDecoders = None):
         self.class_name = class_name
         self._key_decoders = {}
+        self._extra_decoders = extra_decoders
         for key_name, key_type in class_name.__annotations__.items():
-            self._key_decoders[key_name] = build_type_decoder(key_type, module=class_name.__module__)
+            self._key_decoders[key_name] = build_type_decoder(key_type, self._extra_decoders, class_name.__module__)
 
     def decode(self, value: dict) -> dict:
         return {key: self._key_decoders[key].decode(item) for key, item in value.items()}
 
 
 class OptionalTypeDecoder(TypeDecoder):
     def __init__(self, type_decoder: TypeDecoder):
@@ -374,59 +386,66 @@
         return _builtin_type_decoders[a_type]
 
     origin_type = get_origin_type(a_type)
 
     if origin_type is None and is_dataclass(a_type):
         if issubclass(a_type, Generic):  # type: ignore
             raise DecoderError.invalid_type
-        return ClassDecoder(a_type)
+        return ClassDecoder(a_type, extra_decoders)
 
     if origin_type and is_dataclass(origin_type):
         if issubclass(origin_type, Generic):  # type: ignore
             return GenericClassDecoder(a_type)
-        return ClassDecoder(a_type)
+        return ClassDecoder(a_type, extra_decoders)
 
     if origin_type is None:
         origin_type = a_type
 
     if is_class(origin_type) and is_enum_type(origin_type):
         return EnumDecoder(origin_type)
 
     if is_class(origin_type) and is_named_tuple(origin_type):
-        return NamedTupleDecoder(origin_type)
+        return NamedTupleDecoder(origin_type, extra_decoders)
 
     if is_class(origin_type) and is_typed_dict(origin_type):
-        return TypedDictDecoder(origin_type)
+        return TypedDictDecoder(origin_type, extra_decoders)
 
     if origin_type is Union:
         type_args = get_type_args(a_type)
         if len(type_args) == 2 and type_args[-1] is type(None):
             return OptionalTypeDecoder(build_type_decoder(type_args[0]))  # type: ignore
         return UnionDecoder(type_args)
 
     if isinstance(a_type, typing.ForwardRef) and module is not None:
         resolved_reference = resolve_forward_reference(module, a_type)
         if resolved_reference is not None:
             return Decoder[resolved_reference](decoders=extra_decoders)  # type: ignore
 
+    if isinstance(a_type, TypeVar):
+        if a_type.__bound__ is None:
+            raise DecoderError.invalid_type(a_type)
+        return build_type_decoder(a_type.__bound__, extra_decoders, module)
+
+    if is_newtype(a_type):
+        return build_type_decoder(a_type.__supertype__, extra_decoders, module)
+
     if get_origin(origin_type) is not None:
         raise DecoderError.invalid_type(a_type)
 
     if hasattr(origin_type, _PROPERTIES):
         return Decoder[origin_type](decoders=extra_decoders)  # type: ignore
 
     if is_optional(a_type):
         return OptionalTypeDecoder(build_type_decoder(unpack_optional(a_type)))  # type: ignore
 
     if origin_type not in _supported_generics:
         raise DecoderError.invalid_type(a_type)
 
     type_attributes: List[Union[TypeDecoder, Any]] = [
-        build_type_decoder(subtype, module=module)  # type: ignore
-        if subtype is not ... else ...
+        build_type_decoder(subtype, module=module) if subtype is not ... else ...  # type: ignore
         for subtype in get_type_args(a_type)
     ]
     if len(type_attributes) == 1:
         return _supported_generics[origin_type](type_attributes[0])  # type: ignore
 
     return _supported_generics[origin_type](type_attributes)  # type: ignore
 
@@ -467,15 +486,15 @@
             prop.name: build_type_decoder(prop.type, extra_decoders=self.type_decoders)  # type: ignore
             for prop in schema.values()
         }
 
     @classmethod
     def __class_getitem__(cls, item: Type) -> Type[Decoder]:  # noqa: E501
         if not isclass(item):
-            raise EncoderError.invalid_generic_type
+            raise DecoderError.invalid_generic_type
 
         if is_dataclass(item):
             item = decodable(item)
 
         if not hasattr(item, _DECODABLE):
             raise DecoderError.invalid_type
 
@@ -484,15 +503,19 @@
             tuple([cls]),
             {
                 "__generic__": item,
             },
         )
 
 
-def decode(obj: StateObject, a_type: Type[T], decoders: Union[TypeDecoders, Dict[Any, TypeDecoder]] = None) -> T:
+def decode(
+    obj: StateObject,
+    a_type: Type[T],
+    decoders: Union[TypeDecoders, Dict[Any, TypeDecoder]] = None,
+) -> T:
     if decoders and not isinstance(decoders, TypeDecoders):
         decoders = TypeDecoders(decoders)
 
     decoder = build_type_decoder(a_type, extra_decoders=decoders)  # type: ignore
     if decoder is None:
         raise DecoderError.invalid_type
```

### Comparing `chili-2.0.1/chili/encoder.py` & `chili-2.1.0/chili/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,27 @@
 import decimal
 import typing
 from abc import abstractmethod
 from base64 import b64encode
 from enum import Enum
 from functools import lru_cache
 from inspect import isclass
-from typing import Generic, Type, Any, Dict, TypeVar, Protocol, List, Union, Callable, final, Tuple
+from typing import (
+    Generic,
+    Type,
+    Any,
+    Dict,
+    TypeVar,
+    Protocol,
+    List,
+    Union,
+    Callable,
+    final,
+    Tuple,
+)
 
 from chili.typing import (
     create_schema,
     _PROPERTIES,
     _ENCODABLE,
     TypeSchema,
     is_dataclass,
@@ -23,14 +35,15 @@
     is_named_tuple,
     is_typed_dict,
     get_parameters_map,
     map_generic_type,
     is_optional,
     get_type_args,
     unpack_optional,
+    is_newtype,
     UNDEFINED,
     is_class,
 )
 from .error import EncoderError
 from .iso_datetime import timedelta_to_iso_duration
 from .state import StateObject
 
@@ -169,16 +182,17 @@
         ]
 
 
 class ClassEncoder(TypeEncoder):
     _fields: Dict[str, TypeEncoder]
     _schema: TypeSchema
 
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_encoders: TypeEncoders = None):
         self.class_name = class_name
+        self._extra_encoders = extra_encoders
         self._schema = create_schema(class_name)
 
     def encode(self, value: Any) -> StateObject:
         if not isinstance(value, self.class_name):
             raise EncoderError.invalid_input
 
         if not hasattr(self, "_fields"):
@@ -192,27 +206,30 @@
 
         return result
 
     def _build(self) -> Dict[str, TypeEncoder]:
         return {name: self._build_type_encoder(field.type) for name, field in self._schema.items()}
 
     def _build_type_encoder(self, a_type: Type) -> TypeEncoder:
-        return build_type_encoder(a_type, module=self.class_name.__module__)  # type: ignore
+        return build_type_encoder(a_type, self._extra_encoders, self.class_name.__module__)  # type: ignore
 
 
 class GenericClassEncoder(ClassEncoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_encoders: TypeEncoders = None):
         self._generic_type = class_name
+        self._extra_encoders = extra_encoders
         self._generic_parameters = get_parameters_map(class_name)
         type_: Type = get_origin_type(class_name)  # type: ignore
         super().__init__(type_)
 
     def _build_type_encoder(self, a_type: Type) -> TypeEncoder:
         return build_type_encoder(
-            map_generic_type(a_type, self._generic_parameters), module=self._generic_type.__module__
+            map_generic_type(a_type, self._generic_parameters),
+            self._extra_encoders,
+            self._generic_type.__module__,
         )
 
 
 class EnumEncoder(TypeEncoder, Generic[E]):
     def __init__(self, enum_type: Type):
         self.enum_type = enum_type
 
@@ -220,18 +237,19 @@
         if not isinstance(value, self.enum_type):
             raise EncoderError.invalid_input
 
         return value.value
 
 
 class NamedTupleEncoder(TypeEncoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_encoders: TypeEncoders = None):
         self.type = class_name
         self._is_typed = hasattr(class_name, "__annotations__")
         self._arg_encoders: List[TypeEncoder] = []
+        self._extra_encoders = extra_encoders
         if self._is_typed:
             self._build()
 
     def encode(self, value: tuple) -> list:
         if not self._is_typed:
             return list(value)
 
@@ -239,23 +257,23 @@
             self._arg_encoders[index].encode(item) if index < len(self._arg_encoders) else item
             for index, item in enumerate(value)
         ]
 
     def _build(self) -> None:
         field_types = self.type.__annotations__
         for item_type in field_types.values():
-            self._arg_encoders.append(build_type_encoder(item_type, module=self.type.__module__))
+            self._arg_encoders.append(build_type_encoder(item_type, self._extra_encoders, self.type.__module__))
 
 
 class TypedDictEncoder(TypeEncoder):
-    def __init__(self, class_name: Type):
+    def __init__(self, class_name: Type, extra_encoders: TypeEncoders = None):
         self.type = class_name
         self._key_encoders = {}
         for key_name, key_type in class_name.__annotations__.items():
-            self._key_encoders[key_name] = build_type_encoder(key_type, module=class_name.__module__)
+            self._key_encoders[key_name] = build_type_encoder(key_type, extra_encoders, class_name.__module__)
 
     def encode(self, value: dict) -> dict:
         return {key: self._key_encoders[key].encode(item) for key, item in value.items()}
 
 
 class OptionalTypeEncoder(TypeEncoder):
     def __init__(self, type_encoder: TypeEncoder):
@@ -265,23 +283,24 @@
         if value is None:
             return None
 
         return self._encoder.encode(value)
 
 
 class UnionEncoder(TypeEncoder):
-    def __init__(self, supported_types: List[Type]):
+    def __init__(self, supported_types: List[Type], extra_encoders: TypeEncoders = None):
         self.supported_types = supported_types
+        self._extra_encoders = extra_encoders
 
     def encode(self, value: Any) -> Any:
         value_type = type(value)
         if value_type not in self.supported_types:
             raise EncoderError.invalid_input
 
-        return build_type_encoder(value_type).encode(value)  # type: ignore
+        return build_type_encoder(value_type, self._extra_encoders).encode(value)  # type: ignore
 
 
 _supported_generics = {
     list: ListEncoder,
     tuple: TupleEncoder,
     dict: DictEncoder,
     set: ListEncoder,
@@ -300,38 +319,38 @@
         return _builtin_type_encoders[a_type]
 
     origin_type = get_origin_type(a_type)
 
     if origin_type is None and is_dataclass(a_type):
         if issubclass(a_type, Generic):  # type: ignore
             raise EncoderError.invalid_type
-        return ClassEncoder(a_type)
+        return ClassEncoder(a_type, extra_encoders)
 
     if origin_type and is_dataclass(origin_type):
         if issubclass(origin_type, Generic):  # type: ignore
             return GenericClassEncoder(a_type)
-        return ClassEncoder(a_type)
+        return ClassEncoder(a_type, extra_encoders)
 
     if origin_type is None:
         origin_type = a_type
 
     if is_class(origin_type) and is_enum_type(origin_type):
         return EnumEncoder(origin_type)
 
     if is_class(origin_type) and is_named_tuple(origin_type):
-        return NamedTupleEncoder(origin_type)
+        return NamedTupleEncoder(origin_type, extra_encoders)
 
     if is_class(origin_type) and is_typed_dict(origin_type):
-        return TypedDictEncoder(origin_type)
+        return TypedDictEncoder(origin_type, extra_encoders)
 
     if origin_type is Union:
         type_args = get_type_args(a_type)
         if len(type_args) == 2 and type_args[-1] is type(None):
-            return OptionalTypeEncoder(build_type_encoder(type_args[0]))  # type: ignore
-        return UnionEncoder(type_args)
+            return OptionalTypeEncoder(build_type_encoder(type_args[0], extra_encoders))  # type: ignore
+        return UnionEncoder(type_args, extra_encoders)
 
     if isinstance(a_type, typing.ForwardRef) and module is not None:
         resolved_reference = resolve_forward_reference(module, a_type)
         if resolved_reference is not None:
             return Encoder[resolved_reference](encoders=extra_encoders)  # type: ignore[valid-type]
 
     if typing.get_origin(origin_type) is not None:
@@ -339,22 +358,29 @@
 
     if hasattr(origin_type, _PROPERTIES):
         if origin_type != a_type:
             return GenericClassEncoder(a_type)
         return Encoder[origin_type](encoders=extra_encoders)  # type: ignore[valid-type]
 
     if is_optional(a_type):
-        return OptionalTypeEncoder(build_type_encoder(unpack_optional(a_type)))  # type: ignore
+        return OptionalTypeEncoder(build_type_encoder(unpack_optional(a_type), extra_encoders))  # type: ignore
+
+    if isinstance(a_type, TypeVar):
+        if a_type.__bound__ is None:
+            raise EncoderError.invalid_type(a_type)
+        return build_type_encoder(a_type.__bound__, extra_encoders, module)
+
+    if is_newtype(a_type):
+        return build_type_encoder(a_type.__supertype__, extra_encoders, module)
 
     if origin_type not in _supported_generics:
         raise EncoderError.invalid_type(a_type)
 
     type_attributes: List[TypeEncoder] = [
-        build_type_encoder(subtype, module=module)  # type: ignore
-        if subtype is not ... else ...
+        build_type_encoder(subtype, module=module) if subtype is not ... else ...  # type: ignore
         for subtype in get_type_args(a_type)
     ]
 
     if len(type_attributes) == 1:
         return _supported_generics[origin_type](type_attributes[0])  # type: ignore
 
     return _supported_generics[origin_type](type_attributes)  # type: ignore
@@ -412,15 +438,17 @@
             {
                 "__generic__": item,
             },
         )
 
 
 def encode(
-    obj: Any, type_hint: Type = None, encoders: Union[TypeEncoders, Dict[Any, TypeEncoder]] = None
+    obj: Any,
+    type_hint: Type = None,
+    encoders: Union[TypeEncoders, Dict[Any, TypeEncoder]] = None,
 ) -> StateObject:
     if encoders and not isinstance(encoders, TypeEncoders):
         encoders = TypeEncoders(encoders)
 
     if type_hint is not None:
         encoder = build_type_encoder(type_hint, extra_encoders=encoders)  # type: ignore
     else:
```

### Comparing `chili-2.0.1/chili/iso_datetime.py` & `chili-2.1.0/chili/iso_datetime.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.1/chili/json_support.py` & `chili-2.1.0/chili/json_support.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.1/chili/mapper.py` & `chili-2.1.0/chili/mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 class Mapper:
     def __init__(self, scheme: Union[MappingScheme]):
         self.scheme = scheme
 
     def map(self, data: Dict[str, Any], skip_keys: bool = False, default_value: Any = None) -> Dict[str, Any]:
         return self._map(data, self.scheme, skip_keys, default_value)
 
-    def _map(self, data: Dict, scheme: MappingScheme, skip_keys: bool, default_value: Any = None) -> Any:
+    def _map(
+        self,
+        data: Dict,
+        scheme: MappingScheme,
+        skip_keys: bool,
+        default_value: Any = None,
+    ) -> Any:
         result = {}
         evaluated_keys = set()
         for new_key, old_key in scheme.items():
             k_type = type(old_key)
 
             if new_key is Ellipsis:
                 map_key = callable(old_key)
```

### Comparing `chili-2.0.1/chili/serializer.py` & `chili-2.1.0/chili/serializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from __future__ import annotations
 
 from typing import Type, Any, TypeVar, Generic
 
-from chili.typing import _DECODABLE, _ENCODABLE, _PROPERTIES, create_schema, is_class, is_dataclass
+from chili.typing import (
+    _DECODABLE,
+    _ENCODABLE,
+    _PROPERTIES,
+    create_schema,
+    is_class,
+    is_dataclass,
+)
 from chili.decoder import Decoder
 from chili.encoder import Encoder
 from chili.error import SerialisationError
 
 C = TypeVar("C")
 T = TypeVar("T")
```

### Comparing `chili-2.0.1/chili/typing.py` & `chili-2.1.0/chili/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,23 @@
     return (
         get_origin_type(type_name) is Union
         and bool(get_type_args(type_name))
         and get_type_args(type_name)[-1] is type(None)  # noqa
     )
 
 
+def is_newtype(type_name: Type) -> bool:
+    if not hasattr(type_name, "__qualname__"):
+        return False
+    if type_name.__qualname__ != "NewType.<locals>.new_type":
+        return False
+
+    return True
+
+
 def get_type_parameters(type_name: Type) -> List[Type]:
     return getattr(get_origin_type(type_name), "__parameters__", [])
 
 
 def get_parameters_map(type_name: Type) -> Dict[Type, Type]:
     args = get_type_args(type_name)
     parameters = get_type_parameters(type_name)
@@ -126,24 +135,26 @@
         name = ref
     if name in sys.modules[module].__dict__:
         return sys.modules[module].__dict__[name]
 
     if name in sys.modules["builtins"].__dict__:
         return sys.modules["builtins"].__dict__[name]
 
-
-
     return None
 
 
 class Property:
     __slots__ = ("name", "type", "_default_value", "_default_factory")
 
     def __init__(
-        self, name: str, property_type: Type, default_value: Any = UNDEFINED, default_factory: Callable = None
+        self,
+        name: str,
+        property_type: Type,
+        default_value: Any = UNDEFINED,
+        default_factory: Callable = None,
     ):
         self.name = name
         self.type = property_type
         self._default_value = default_value if default_value is not MISSING else UNDEFINED
         self._default_factory = default_factory
 
     @property
```

### Comparing `chili-2.0.1/pyproject.toml` & `chili-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://github.com/kodemore/chili"
 homepage = "https://github.com/kodemore/chili"
 keywords = ["serialise", "deserialise", "encode", "decode", "object", "class"]
 license = "MIT"
 name = "chili"
 readme = "README.md"
 repository = "https://github.com/kodemore/chili"
-version = "2.0.1"
+version = "2.1.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-extensions = "^4.2"
 gaffe = "0.2.0"
 
 [tool.poetry.dev-dependencies]
```

