# Comparing `tmp/scrape_schema-0.0.2.tar.gz` & `tmp/scrape_schema-0.0.3.tar.gz`

## Comparing `scrape_schema-0.0.2.tar` & `scrape_schema-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/__init__.py
--rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/README.md
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    18312 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/README.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/PKG-INFO
```

### Comparing `scrape_schema-0.0.2/scrape_schema/base.py` & `scrape_schema-0.0.3/scrape_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -410,15 +410,15 @@
                 or not value
             ):
                 continue
             else:
                 return value
         return value
 
-    def __init__(self, markup: str):
+    def _parse_markup_to_fields(self, markup: str) -> None:
         """
         :param str markup: text target
         """
         self.__fields_annotations__: dict[str, Type] = {}
 
         _fields = self._get_fields()
         _parsers: dict[Type[Any], Any] = {}
@@ -470,50 +470,72 @@
                 value,
             )
             setattr(self, name, value)
         logger.debug(
             "%s done! Fields fails: %i", self.__class__.__name__, _fails_counter
         )
 
+    def __init__(self, markup: str, *, parse_markup: bool = True, **kwargs):
+        """
+        :param markup: markup string target
+        :param parse_markup: parse field markups. Default True
+        :param kwargs: any kwargs attrs
+        """
+        # TODO rewrite init constructor
+        if parse_markup:
+            self._parse_markup_to_fields(markup)
+
+        for k, v in kwargs.items():
+            setattr(self, k, v)
+
     @classmethod
     def init_list(cls, markups: Iterable[str]) -> list[Self]:
         """Init list of schemas by markups sequence
 
         :param markups: - iterable markups sequence
         """
-        return [cls(markup) for markup in markups]
+        warnings.warn(
+            "This method deprecated, usage `from_list`",
+            category=DeprecationWarning,
+            stacklevel=2,
+        )
+        return cls.from_list(markups)
 
     @classmethod
     def from_list(cls, markups: Iterable[str]) -> list[Self]:
         """Init list of schemas by markups sequence
 
         :param markups: iterable markups sequence
         """
-        return cls.init_list(markups)
+        return [cls(markup) for markup in markups]
 
     @classmethod
     def from_crop_rule_list(
         cls, markup: str, *, crop_rule: Callable[[str], Iterable[str]]
     ) -> list[Self]:
         """Init list of schemas by crop_rule
 
         :param markup: markup string
         :param crop_rule: crop rule function to *parts*
         """
-        return cls.init_list(crop_rule(markup))
+        return cls.from_list(crop_rule(markup))
 
     @classmethod
     def from_crop_rule(cls, markup: str, *, crop_rule: Callable[[str], str]) -> Self:
         """Init single schema by crop_rule
 
         :param markup: markup string
         :param crop_rule: crop rule function to *part*.
         """
         return cls(crop_rule(markup))
 
+    @classmethod
+    def from_markup(cls, markup: str) -> Self:
+        return cls(markup, parse_markup=True)
+
     @staticmethod
     def _to_dict(value: BaseSchema | list | dict):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
```

### Comparing `scrape_schema-0.0.2/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.3/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.3/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/scrape_schema/fields/nested.py` & `scrape_schema-0.0.3/scrape_schema/fields/nested.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from ..base import BaseField, BaseSchema
 
 __all__ = ["BaseNested", "Nested", "NestedList"]
 
 
 class BaseNested(BaseField):
-    def _parse(self, markup: str) -> str:
-        return markup
+    def _parse(self, _: str) -> str:
+        return _
 
 
 class Nested(BaseNested):
     def __init__(
         self,
         schema: Type[BaseSchema],
         *,
@@ -30,16 +30,15 @@
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
     ) -> BaseSchema | Any:
         markup = self._parse(markup)
-        new_markup = self.crop_rule(markup)
-        value = self._schema(new_markup)
+        value = self._schema.from_crop_rule(markup, crop_rule=self.crop_rule)
         return self._factory(value)
 
 
 class NestedList(BaseNested):
     def __init__(
         self,
         schema: Type[BaseSchema],
@@ -58,10 +57,9 @@
         self._schema = schema
         self.crop_rule = crop_rule
 
     def __call__(
         self, instance: BaseSchema, name: str, markup: str
     ) -> list[BaseSchema] | Any:
         markup = self._parse(markup)
-        new_markups = self.crop_rule(markup)
-        value = self._schema.init_list(new_markups)
+        value = self._schema.from_crop_rule_list(markup, crop_rule=self.crop_rule)
         return self._factory(value)
```

### Comparing `scrape_schema-0.0.2/scrape_schema/fields/regex.py` & `scrape_schema-0.0.3/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/scrape_schema/fields/slax.py` & `scrape_schema-0.0.3/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/scrape_schema/fields/soup.py` & `scrape_schema-0.0.3/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/.gitignore` & `scrape_schema-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/LICENSE` & `scrape_schema-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/README.md` & `scrape_schema-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.2/pyproject.toml` & `scrape_schema-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -92,10 +92,16 @@
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
 exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
 files = "scrape_schema/*.py,scrape_schema/fields/*.py,scrape_schema/callbacks/*.py"
 
-[tool.black]
+[tool.pytest.ini_options]
+filterwarnings = [
+    "error",
+    "ignore::RuntimeWarning",
+    # note the use of single quote below to denote "raw" strings in TOML
+    'ignore: Failed parse',
+]
```

### Comparing `scrape_schema-0.0.2/PKG-INFO` & `scrape_schema-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

