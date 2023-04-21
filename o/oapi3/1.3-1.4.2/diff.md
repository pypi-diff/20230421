# Comparing `tmp/oapi3-1.3.tar.gz` & `tmp/oapi3-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oapi3-1.3.tar", last modified: Mon Jan 23 09:33:17 2023, max compression
+gzip compressed data, was "oapi3-1.4.2.tar", last modified: Fri Apr 21 10:01:00 2023, max compression
```

## Comparing `oapi3-1.3.tar` & `oapi3-1.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-01-23 09:33:17.682237 oapi3-1.3/
--rw-r--r--   0 motor      (501) staff       (20)     1071 2022-09-06 13:51:56.000000 oapi3-1.3/LICENSE
--rw-r--r--   0 motor      (501) staff       (20)      468 2023-01-23 09:33:17.682107 oapi3-1.3/PKG-INFO
--rw-r--r--   0 motor      (501) staff       (20)       53 2022-09-06 13:51:56.000000 oapi3-1.3/README.md
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-01-23 09:33:17.678553 oapi3-1.3/oapi3/
--rw-r--r--   0 motor      (501) staff       (20)      617 2023-01-19 13:11:11.000000 oapi3-1.3/oapi3/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)     4957 2022-09-06 13:51:56.000000 oapi3-1.3/oapi3/client.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-01-23 09:33:17.680543 oapi3-1.3/oapi3/entities/
--rw-r--r--   0 motor      (501) staff       (20)      946 2023-01-23 09:13:39.000000 oapi3-1.3/oapi3/entities/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)      192 2023-01-17 11:57:21.000000 oapi3-1.3/oapi3/entities/base.py
--rw-r--r--   0 motor      (501) staff       (20)     2715 2023-01-23 09:15:03.000000 oapi3-1.3/oapi3/entities/media_types.py
--rw-r--r--   0 motor      (501) staff       (20)     3701 2023-01-20 11:08:24.000000 oapi3-1.3/oapi3/entities/operations.py
--rw-r--r--   0 motor      (501) staff       (20)     9752 2023-01-23 09:09:51.000000 oapi3-1.3/oapi3/entities/parameters.py
--rw-r--r--   0 motor      (501) staff       (20)     2626 2023-01-19 14:12:56.000000 oapi3-1.3/oapi3/entities/paths.py
--rw-r--r--   0 motor      (501) staff       (20)      729 2023-01-17 14:18:00.000000 oapi3-1.3/oapi3/entities/schema.py
--rw-r--r--   0 motor      (501) staff       (20)     3654 2023-01-20 11:24:48.000000 oapi3-1.3/oapi3/exceptions.py
--rw-r--r--   0 motor      (501) staff       (20)     5860 2023-01-23 09:31:05.000000 oapi3-1.3/oapi3/iktomi.py
--rw-r--r--   0 motor      (501) staff       (20)     2758 2023-01-19 13:39:26.000000 oapi3-1.3/oapi3/jsonschema_validator.py
--rw-r--r--   0 motor      (501) staff       (20)     4349 2023-01-19 13:12:42.000000 oapi3-1.3/oapi3/resolve.py
--rw-r--r--   0 motor      (501) staff       (20)     3616 2023-01-23 08:58:01.000000 oapi3-1.3/oapi3/schema.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-01-23 09:33:17.679205 oapi3-1.3/oapi3.egg-info/
--rw-r--r--   0 motor      (501) staff       (20)      468 2023-01-23 09:33:17.000000 oapi3-1.3/oapi3.egg-info/PKG-INFO
--rw-r--r--   0 motor      (501) staff       (20)      614 2023-01-23 09:33:17.000000 oapi3-1.3/oapi3.egg-info/SOURCES.txt
--rw-r--r--   0 motor      (501) staff       (20)        1 2023-01-23 09:33:17.000000 oapi3-1.3/oapi3.egg-info/dependency_links.txt
--rw-r--r--   0 motor      (501) staff       (20)       41 2023-01-23 09:33:17.000000 oapi3-1.3/oapi3.egg-info/requires.txt
--rw-r--r--   0 motor      (501) staff       (20)       12 2023-01-23 09:33:17.000000 oapi3-1.3/oapi3.egg-info/top_level.txt
--rw-r--r--   0 motor      (501) staff       (20)       38 2023-01-23 09:33:17.682276 oapi3-1.3/setup.cfg
--rw-r--r--   0 motor      (501) staff       (20)      836 2023-01-23 09:32:23.000000 oapi3-1.3/setup.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-01-23 09:33:17.681843 oapi3-1.3/tests/
--rw-r--r--   0 motor      (501) staff       (20)        0 2023-01-19 13:39:59.000000 oapi3-1.3/tests/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)      123 2023-01-20 10:29:56.000000 oapi3-1.3/tests/conftest.py
--rw-r--r--   0 motor      (501) staff       (20)       35 2023-01-23 08:01:55.000000 oapi3-1.3/tests/test_iktomi.py
--rw-r--r--   0 motor      (501) staff       (20)     7727 2023-01-23 09:01:06.000000 oapi3-1.3/tests/test_request_validation.py
--rw-r--r--   0 motor      (501) staff       (20)     2688 2023-01-20 11:22:10.000000 oapi3-1.3/tests/test_response_validation.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.704018 oapi3-1.4.2/
+-rw-r--r--   0 motor      (501) staff       (20)     1071 2022-09-06 13:51:56.000000 oapi3-1.4.2/LICENSE
+-rw-r--r--   0 motor      (501) staff       (20)      507 2023-04-21 10:01:00.703901 oapi3-1.4.2/PKG-INFO
+-rw-r--r--   0 motor      (501) staff       (20)       53 2022-09-06 13:51:56.000000 oapi3-1.4.2/README.md
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.702008 oapi3-1.4.2/oapi3/
+-rw-r--r--   0 motor      (501) staff       (20)      617 2023-01-19 13:11:11.000000 oapi3-1.4.2/oapi3/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)     4957 2022-09-06 13:51:56.000000 oapi3-1.4.2/oapi3/client.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.703240 oapi3-1.4.2/oapi3/entities/
+-rw-r--r--   0 motor      (501) staff       (20)      946 2023-01-23 09:13:39.000000 oapi3-1.4.2/oapi3/entities/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)      192 2023-01-17 11:57:21.000000 oapi3-1.4.2/oapi3/entities/base.py
+-rw-r--r--   0 motor      (501) staff       (20)     2679 2023-01-31 12:08:56.000000 oapi3-1.4.2/oapi3/entities/media_types.py
+-rw-r--r--   0 motor      (501) staff       (20)     3701 2023-01-20 11:08:24.000000 oapi3-1.4.2/oapi3/entities/operations.py
+-rw-r--r--   0 motor      (501) staff       (20)    10088 2023-04-20 13:14:43.000000 oapi3-1.4.2/oapi3/entities/parameters.py
+-rw-r--r--   0 motor      (501) staff       (20)     2626 2023-01-19 14:12:56.000000 oapi3-1.4.2/oapi3/entities/paths.py
+-rw-r--r--   0 motor      (501) staff       (20)      729 2023-01-17 14:18:00.000000 oapi3-1.4.2/oapi3/entities/schema.py
+-rw-r--r--   0 motor      (501) staff       (20)     3654 2023-01-20 11:24:48.000000 oapi3-1.4.2/oapi3/exceptions.py
+-rw-r--r--   0 motor      (501) staff       (20)     5860 2023-01-23 09:31:05.000000 oapi3-1.4.2/oapi3/iktomi.py
+-rw-r--r--   0 motor      (501) staff       (20)     2758 2023-01-19 13:39:26.000000 oapi3-1.4.2/oapi3/jsonschema_validator.py
+-rw-r--r--   0 motor      (501) staff       (20)     4349 2023-01-19 13:12:42.000000 oapi3-1.4.2/oapi3/resolve.py
+-rw-r--r--   0 motor      (501) staff       (20)     3616 2023-04-20 11:57:16.000000 oapi3-1.4.2/oapi3/schema.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.702515 oapi3-1.4.2/oapi3.egg-info/
+-rw-r--r--   0 motor      (501) staff       (20)      507 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/PKG-INFO
+-rw-r--r--   0 motor      (501) staff       (20)      614 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 motor      (501) staff       (20)        1 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 motor      (501) staff       (20)       41 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/requires.txt
+-rw-r--r--   0 motor      (501) staff       (20)       12 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/top_level.txt
+-rw-r--r--   0 motor      (501) staff       (20)       38 2023-04-21 10:01:00.704058 oapi3-1.4.2/setup.cfg
+-rw-r--r--   0 motor      (501) staff       (20)      838 2023-04-21 09:59:48.000000 oapi3-1.4.2/setup.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.703753 oapi3-1.4.2/tests/
+-rw-r--r--   0 motor      (501) staff       (20)        0 2023-01-19 13:39:59.000000 oapi3-1.4.2/tests/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)      123 2023-01-20 10:29:56.000000 oapi3-1.4.2/tests/conftest.py
+-rw-r--r--   0 motor      (501) staff       (20)       35 2023-01-23 08:01:55.000000 oapi3-1.4.2/tests/test_iktomi.py
+-rw-r--r--   0 motor      (501) staff       (20)     8490 2023-01-30 16:58:08.000000 oapi3-1.4.2/tests/test_request_validation.py
+-rw-r--r--   0 motor      (501) staff       (20)     2688 2023-01-20 11:22:10.000000 oapi3-1.4.2/tests/test_response_validation.py
```

### Comparing `oapi3-1.3/LICENSE` & `oapi3-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/__init__.py` & `oapi3-1.4.2/oapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/client.py` & `oapi3-1.4.2/oapi3/client.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/entities/__init__.py` & `oapi3-1.4.2/oapi3/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/entities/media_types.py` & `oapi3-1.4.2/oapi3/entities/media_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
             for k in sorted(media_type_objs, reverse=True)
         }
 
     def match_media_type(self, media_type: str) -> MediaTypeEntity:
         ''' Match request media type '''
         media_type_parts = media_type.split('/')
         if len(media_type_parts) == 2:
-            print(media_type_parts)
             for k, v in self.media_types.items():
                 if k[0] != '*' and media_type_parts[0] != k[0]:
                     continue
                 if k[1] != '*' and media_type_parts[1] != k[1]:
                     continue
                 return v 
         raise exceptions.MediaTypeNotAllowed(
```

### Comparing `oapi3-1.3/oapi3/entities/operations.py` & `oapi3-1.4.2/oapi3/entities/operations.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/entities/parameters.py` & `oapi3-1.4.2/oapi3/entities/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,26 @@
         try:
             return int(value)
         except ValueError:
             # Not raise exception. It will be raised in schema validation.
             return value
 
 
+class BooleanParameterEntity(PrimitiveParameterEntity):
+    ''' Parameter entity for simple boolean parameters '''
+
+    def serialize(self, value: Any) -> str:
+        if value:
+            return '1'
+        return ''
+
+    def deserialize(self, value: str) -> Any:
+        return bool(value)
+
+
 class ArrayParameterEntity(PrimitiveParameterEntity):
     ''' Base parameter entity class for array parameters '''
 
     __slots__ = [
         'inner_schema',
     ]
     inner_schema: dict
@@ -157,14 +169,15 @@
 
 PRIMITIVE_SCHEMAS = {
     None: PrimitiveParameterEntity,
     'string': StringParameterEntity,
     'integer': IntegerParameterEntity,
     'long': IntegerParameterEntity,
     'double': IntegerParameterEntity,
+    'boolean': BooleanParameterEntity,
 }
 
 ARRAY_SCHEMAS = {
     ('form', False): FormNEArrayParameterEntity,
     ('pipedelimited', False): PipedelimitedNEArrayParameterEntity,
     ('spacedelimited', False): SpacedelimitedNEArrayParameterEntity,
 }
@@ -276,15 +289,15 @@
 
     def serialize(self, in_: str, values: Dict[str, Any]) -> Dict[str, str]:
         ''' Serialize parameters '''
         if in_ not in IMPLIMENTED_IN_VALUES:
             raise NotImplementedError(in_)
         return dict(
             values,
-            {
+            **{
                 k: self.parameters[in_][k].serialize(v)
                 for k, v in values.items()
                 if k in self.parameters[in_]
             }
         )
 
     def validate(self, in_: str, values: Dict[str, Any]):
```

### Comparing `oapi3-1.3/oapi3/entities/paths.py` & `oapi3-1.4.2/oapi3/entities/paths.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/entities/schema.py` & `oapi3-1.4.2/oapi3/entities/schema.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/exceptions.py` & `oapi3-1.4.2/oapi3/exceptions.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/iktomi.py` & `oapi3-1.4.2/oapi3/iktomi.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/jsonschema_validator.py` & `oapi3-1.4.2/oapi3/jsonschema_validator.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/resolve.py` & `oapi3-1.4.2/oapi3/resolve.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3/schema.py` & `oapi3-1.4.2/oapi3/schema.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/oapi3.egg-info/SOURCES.txt` & `oapi3-1.4.2/oapi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oapi3-1.3/setup.py` & `oapi3-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PY3 = sys.version_info >= (3, 0)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='oapi3',
-    version='1.3',
+    version='1.4.2',
     author="Mayorov Evgeny",
     author_email="motormen@gmail.com",
     description="Validator of openapi3 requests and responses",
     packages=find_packages(),
     package_dir={'oapi3': 'oapi3'},
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `oapi3-1.3/tests/test_request_validation.py` & `oapi3-1.4.2/tests/test_request_validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,14 +127,37 @@
             '/test_request_query_params',
             'get',
             {'param': 'xxx', 'param_required': 'yyy', 'param_int': 'ddd'},
             'application/json',
             None,
         )
 
+    # Test boolean query params
+    result = schema.validate_request(
+        '/test_request_query_params',
+        'get',
+        {'param_bool': 'xx', 'param_required': 'yyy'},
+        'application/json',
+        None,
+    )
+    assert set(result['query']) == {'param_bool', 'param_required'}
+    assert result['query']['param_bool'] is True
+    assert result['query']['param_required'] == 'yyy'
+
+    result = schema.validate_request(
+        '/test_request_query_params',
+        'get',
+        {'param_bool': '', 'param_required': 'yyy'},
+        'application/json',
+        None,
+    )
+    assert set(result['query']) == {'param_bool', 'param_required'}
+    assert result['query']['param_bool'] is False
+    assert result['query']['param_required'] == 'yyy'
+
 
 def test_request_json_query_params(schema):
     result = schema.validate_request(
         '/test_request_json_query_params',
         'get',
         {'param_json': json.dumps({'test': 4})},
         'application/json',
```

### Comparing `oapi3-1.3/tests/test_response_validation.py` & `oapi3-1.4.2/tests/test_response_validation.py`

 * *Files identical despite different names*

