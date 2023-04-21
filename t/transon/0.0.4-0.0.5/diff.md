# Comparing `tmp/transon-0.0.4.tar.gz` & `tmp/transon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transon-0.0.4.tar", max compression
+gzip compressed data, was "transon-0.0.5.tar", max compression
```

## Comparing `transon-0.0.4.tar` & `transon-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      298 2023-04-02 18:25:35.966125 transon-0.0.4/README.md
--rw-r--r--   0        0        0      453 2023-04-02 18:25:35.966125 transon-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-02 18:25:35.966125 transon-0.0.4/transon/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-02 18:25:35.970125 transon-0.0.4/transon/docs.py
--rw-r--r--   0        0        0      173 2023-04-02 18:25:35.970125 transon-0.0.4/transon/functions.py
--rw-r--r--   0        0        0     1455 2023-04-02 18:25:35.970125 transon-0.0.4/transon/operators.py
--rw-r--r--   0        0        0    14914 2023-04-02 18:25:35.970125 transon-0.0.4/transon/rules.py
--rw-r--r--   0        0        0        0 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/__init__.py
--rw-r--r--   0        0        0     1102 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/base.py
--rw-r--r--   0        0        0      347 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/base_attr.py
--rw-r--r--   0        0        0      763 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/base_join.py
--rw-r--r--   0        0        0       68 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/conftest.py
--rw-r--r--   0        0        0     3036 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_attr.py
--rw-r--r--   0        0        0     1080 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_chain.py
--rw-r--r--   0        0        0      984 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_convert.py
--rw-r--r--   0        0        0     4225 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_expr.py
--rw-r--r--   0        0        0     1981 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_file.py
--rw-r--r--   0        0        0     2102 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_format.py
--rw-r--r--   0        0        0     2890 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_join.py
--rw-r--r--   0        0        0     3565 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_map.py
--rw-r--r--   0        0        0     2952 2023-04-02 18:25:35.970125 transon-0.0.4/transon/tests/test_no_content.py
--rw-r--r--   0        0        0     7802 2023-04-02 18:25:35.970125 transon-0.0.4/transon/transformers.py
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 transon-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3276 2023-04-20 21:25:21.823450 transon-0.0.5/README.md
+-rw-r--r--   0        0        0      735 2023-04-20 21:25:21.827450 transon-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-20 21:25:21.827450 transon-0.0.5/transon/__init__.py
+-rw-r--r--   0        0        0     2831 2023-04-20 21:25:21.827450 transon-0.0.5/transon/docs.py
+-rw-r--r--   0        0        0      173 2023-04-20 21:25:21.827450 transon-0.0.5/transon/functions.py
+-rw-r--r--   0        0        0     1455 2023-04-20 21:25:21.827450 transon-0.0.5/transon/operators.py
+-rw-r--r--   0        0        0    16737 2023-04-20 21:25:21.827450 transon-0.0.5/transon/rules.py
+-rw-r--r--   0        0        0        0 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/__init__.py
+-rw-r--r--   0        0        0     1576 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/base.py
+-rw-r--r--   0        0        0      347 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/base_attr.py
+-rw-r--r--   0        0        0      763 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/base_join.py
+-rw-r--r--   0        0        0       68 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/conftest.py
+-rw-r--r--   0        0        0     4339 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_attr.py
+-rw-r--r--   0        0        0     1080 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_chain.py
+-rw-r--r--   0        0        0      984 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_convert.py
+-rw-r--r--   0        0        0     4225 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_expr.py
+-rw-r--r--   0        0        0     1981 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_file.py
+-rw-r--r--   0        0        0     2248 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_filter.py
+-rw-r--r--   0        0        0     2102 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_format.py
+-rw-r--r--   0        0        0      604 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_include.py
+-rw-r--r--   0        0        0     2890 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_join.py
+-rw-r--r--   0        0        0     3866 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_map.py
+-rw-r--r--   0        0        0     2952 2023-04-20 21:25:21.827450 transon-0.0.5/transon/tests/test_no_content.py
+-rw-r--r--   0        0        0     8130 2023-04-20 21:25:21.827450 transon-0.0.5/transon/transformers.py
+-rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 transon-0.0.5/PKG-INFO
```

### Comparing `transon-0.0.4/transon/docs.py` & `transon-0.0.5/transon/docs.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,34 @@
 
 import transon
 from transon.tests.base import TableDataBaseCase
 from transon.transformers import Transformer
 
 
 @lru_cache(maxsize=None)
-def get_test_cases_by_tags():
+def get_test_cases():
     project_root = os.path.dirname(os.path.dirname(transon.__file__))
     unittest.defaultTestLoader.discover(project_root)
+    return list(TableDataBaseCase.iterate_valid_cases())
 
-    tests_by_tag = defaultdict(list)
-    for case in TableDataBaseCase.iterate_valid_cases():
-        for tag in case.tags:
-            tests_by_tag[tag].append(case)
-    return tests_by_tag
+
+@lru_cache(maxsize=None)
+def get_test_cases_by_tag(tag: str):
+    return [
+        case
+        for case in get_test_cases()
+        if tag in case.tags
+    ]
+
+
+@lru_cache(maxsize=None)
+def get_test_case_by_name(name: str):
+    for case in get_test_cases():
+        if case.__name__ == name:
+            return case
 
 
 def get_rules_docs(cls=Transformer):
     return [
         {
             'name': rule.__rule_name__,
             'doc': inspect.getdoc(rule),
@@ -40,39 +51,37 @@
             'doc': inspect.cleandoc(param_docs),
         }
         for param_name, param_docs in rule.__rule_params__.items()
     ]
 
 
 def get_test_cases_for_rule(rule_name):
-    tests_by_tag = get_test_cases_by_tags()
     return [
         {
             'name': case.__name__,
             'doc': inspect.getdoc(case),
             'template': case.template,
             'data': case.data,
             'result': case.result,
         }
-        for case in tests_by_tag[rule_name]
+        for case in get_test_cases_by_tag(rule_name)
     ]
 
 
 def get_test_cases_for_rule_param(rule_name, param_name):
-    tests_by_tag = get_test_cases_by_tags()
     tag = f'{rule_name}:{param_name}'
     return [
         {
             'name': case.__name__,
             'doc': inspect.getdoc(case),
             'template': case.template,
             'data': case.data,
             'result': case.result,
         }
-        for case in tests_by_tag[tag]
+        for case in get_test_cases_by_tag(tag)
     ]
 
 
 def get_all_docs(cls=Transformer):
     return {
         'doc': inspect.getdoc(cls),
         'rules': [
```

### Comparing `transon-0.0.4/transon/operators.py` & `transon-0.0.5/transon/operators.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/rules.py` & `transon-0.0.5/transon/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,26 +107,36 @@
 Can be dynamic.
 """,
 )
 def rule_attr(t: Transformer, template, context: Context):
     """
     Returns values of attribute or item from current value in context.
     Can search in deeply nested structures with path.
-    If attribute is not present an exception will be thrown.
+    If attribute is not present returns no value.
 
     Parameters are mutually exclusive.
     """
     if 'name' in template:
         t_name = template['name']
         name = t.walk(t_name, context)
-        return context.this[name]
+        try:
+            return context.this[name]
+        except KeyError:
+            return t.NO_CONTENT
+        except IndexError:
+            return t.NO_CONTENT
     elif 'names' in template:
         t_names = template['names']
         names = t.walk(t_names, context)
-        return reduce(operator.getitem, names, context.this)
+        try:
+            return reduce(operator.getitem, names, context.this)
+        except KeyError:
+            return t.NO_CONTENT
+        except IndexError:
+            return t.NO_CONTENT
     else:
         raise DefinitionError('either `name` of `names` attribute is required for `attr` rule')
 
 
 @Transformer.register_rule(
     'object',
     key="Defines template for name of attribute.",
@@ -146,56 +156,60 @@
     if key is t.NO_CONTENT:
         return {}
     if value is t.NO_CONTENT:
         return {}
     return {key: value}
 
 
+def _iter_contexts(context: Context):
+    data = context.this
+    if isinstance(data, list):
+        for index, _item in enumerate(data):
+            yield context.derive(this=_item, index=index, item=_item)
+    elif isinstance(data, dict):
+        for index, (_key, _value) in enumerate(data.items()):
+            yield context.derive(this=_value, index=index, key=_key, value=_value)
+    else:
+        raise TransformationError(f"value is not iterable: {data!r}")
+
+
 @Transformer.register_rule(
     'map',
     item="Defines template for items when producing the `list`",
     items="Defines templates for series of items when producing the `list`",
     key="Defines template for key when producing the `dict`",
     value="Defines template for value when producing the `dict`",
 )
 def rule_map(t: Transformer, template, context: Context):
     """
     Iterates over `list` or `dict` and produces new `dict` or `list` with items based on template.
     """
-    def iter_contexts(data):
-        if isinstance(data, list):
-            for index, _item in enumerate(data):
-                yield context.derive(this=_item, index=index, item=_item)
-        elif isinstance(data, dict):
-            for index, (_key, _value) in enumerate(data.items()):
-                yield context.derive(this=_value, index=index, key=_key, value=_value)
-
     if 'item' in template:
         t_item = template['item']
         result = []
-        for sub_context in iter_contexts(context.this):
+        for sub_context in _iter_contexts(context):
             item = t.walk(t_item, sub_context)
             if item is t.NO_CONTENT:
                 continue
             result.append(item)
         return result
     elif 'items' in template:
         t_items = template['items']
         result = []
-        for sub_context in iter_contexts(context.this):
+        for sub_context in _iter_contexts(context):
             for item in t.walk(t_items, sub_context):
                 if item is t.NO_CONTENT:
                     continue
                 result.append(item)
         return result
     elif 'key' in template and 'value' in template:
         t_key = template['key']
         t_value = template['value']
         result = {}
-        for sub_context in iter_contexts(context.this):
+        for sub_context in _iter_contexts(context):
             key = t.walk(t_key, sub_context)
             value = t.walk(t_value, sub_context)
             if key is t.NO_CONTENT:
                 continue
             if value is t.NO_CONTENT:
                 continue
             result[key] = value
@@ -204,14 +218,49 @@
     raise DefinitionError(
         'either `item` or `items` or `key/value` properties '
         'are required for `map` rule'
     )
 
 
 @Transformer.register_rule(
+    'filter',
+    cond="Defines template for condition",
+)
+def rule_filter(t: Transformer, template, context: Context):
+    """
+    Iterates over `list` or `dict` and filters out items regarding condition calculation.
+    """
+
+    t_cond = t.require(template, 'cond')
+
+    def _iterate_with_condition(_context: Context):
+        for _sub_context in _iter_contexts(_context):
+            cond = t.walk(t_cond, _sub_context)
+            if cond is t.NO_CONTENT:
+                continue
+            if not cond:
+                continue
+            yield _sub_context
+
+    data = context.this
+    if isinstance(data, list):
+        return [
+            sub_context.item
+            for sub_context in _iterate_with_condition(context)
+        ]
+    elif isinstance(data, dict):
+        return {
+            sub_context.key: sub_context.value
+            for sub_context in _iterate_with_condition(context)
+        }
+    else:
+        raise TransformationError(f"value is not iterable: {data!r}")
+
+
+@Transformer.register_rule(
     'zip',
     items="Defines the list of lists",
 )
 def rule_zip(t: Transformer, template, context: Context):
     """
     Works exactly like `zip` function in python.
     Converts collection of lists into list of items.
@@ -455,7 +504,19 @@
         value = t.walk(t_value, context)
     if isinstance(value, list):
         return pattern.format(*value)
     elif isinstance(value, dict):
         return pattern.format(**value)
     else:
         return pattern.format(value)
+
+
+@Transformer.register_rule(
+    'include',
+    name="Name or path to template. Can be dynamic. Meaning of this depends of provided template loader.",
+)
+def rule_include(t: Transformer, template, context: Context):
+    t_name = t.require(template, 'name')
+    name = t.walk(t_name, context)
+    sub_transformer = t.template_loader(name)
+    result = sub_transformer.transform(context.this)
+    return t.NO_CONTENT if result is sub_transformer.NO_CONTENT else result
```

### Comparing `transon-0.0.4/transon/tests/base_join.py` & `transon-0.0.5/transon/tests/base_join.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_chain.py` & `transon-0.0.5/transon/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_convert.py` & `transon-0.0.5/transon/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_expr.py` & `transon-0.0.5/transon/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_file.py` & `transon-0.0.5/transon/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_format.py` & `transon-0.0.5/transon/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_join.py` & `transon-0.0.5/transon/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/tests/test_map.py` & `transon-0.0.5/transon/tests/test_map.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+import pytest
+
 from . import base
+from transon import (
+    Transformer,
+    TransformationError,
+)
 
 
 class MapListToList(base.TableDataBaseCase):
     """
     Maps two lists obtained from different attributes of input.
     Then joins two obtained lists into single resulting list.
     """
@@ -116,14 +122,24 @@
     result = [
         'a', 1,
         'b', 2,
         'c', 3,
     ]
 
 
+def test_invalid_value():
+    template = {
+        '$': 'map',
+        'item': {'$': 'item'},
+    }
+    transformer = Transformer(template)
+    with pytest.raises(TransformationError):
+        transformer.transform(1)
+
+
 class MapListsToDict(base.TableDataBaseCase):
     """
     Zips two lists containing keys and values together into pairs.
     Then iterates over list of pairs and produces resulting dict.
     """
     tags = ['chain', 'zip', 'map:key', 'map:value', 'attr:name']
     template = {
```

### Comparing `transon-0.0.4/transon/tests/test_no_content.py` & `transon-0.0.5/transon/tests/test_no_content.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.4/transon/transformers.py` & `transon-0.0.5/transon/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,21 +63,27 @@
 
 class NoContent:
     def __getitem__(self, _):
         return self
 
 
 FileWriterType = Callable[[str, any], NoReturn]
+TemplateLoaderType = Callable[[str], 'Transformer']
 
 
 # noinspection PyUnusedLocal
-def no_file_writer(name, data):  # pragma: no cover
+def no_file_writer(name: str, data):  # pragma: no cover
     return
 
 
+# noinspection PyUnusedLocal
+def no_template_loader(name: str) -> 'Transformer':   # pragma: no cover
+    raise RuntimeError(f'template with name `{name}` was not found')
+
+
 class Transformer:
     """
     `Transformer` class interpolates template with input data.
     Format of output is defined by template.
     Input is used to fill values into template placeholders.
 
     ```python
@@ -222,17 +228,25 @@
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls._operators = {}
         cls._rules = {}
         cls._functions = {}
 
-    def __init__(self, template, *, file_writer: FileWriterType = no_file_writer, marker: str = DEFAULT_MARKER):
+    def __init__(
+            self,
+            template,
+            *,
+            file_writer: FileWriterType = no_file_writer,
+            template_loader: TemplateLoaderType = no_template_loader,
+            marker: str = DEFAULT_MARKER,
+    ):
         self.template = template
         self.file_writer = file_writer
+        self.template_loader = template_loader
         self.marker = marker
 
     def walk_list(self, template, context):
         return [
             self.walk(item, context)
             for item in template
         ]
@@ -270,11 +284,8 @@
         if name not in template:
             rule = template[self.marker]
             raise DefinitionError(f'`{name}` property is required for `{rule}` rule')
         return template[name]
 
     def transform(self, data):
         context = Context(this=data)
-        result = self.walk(self.template, context)
-        if result is self.NO_CONTENT:
-            return None
-        return result
+        return self.walk(self.template, context)
```

