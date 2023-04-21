# Comparing `tmp/scrape_schema-0.0.1.tar.gz` & `tmp/scrape_schema-0.0.2.tar.gz`

## Comparing `scrape_schema-0.0.1.tar` & `scrape_schema-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/__init__.py
--rw-r--r--   0        0        0    16388 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 scrape_schema-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    17589 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/README.md
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.2/PKG-INFO
```

### Comparing `scrape_schema-0.0.1/scrape_schema/base.py` & `scrape_schema-0.0.2/scrape_schema/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,17 @@
     def _is_iterable_and_not_string_type(value_type: Type) -> bool:
         return issubclass(value_type, Iterable) and not issubclass(
             value_type, (ByteString, str)
         )
 
     @staticmethod
     def _is_iterable_and_not_string_value(value: T) -> bool:
-        return isinstance(value, Iterable) and not (isinstance(value, (ByteString, str)))
+        return isinstance(value, Iterable) and not (
+            isinstance(value, (ByteString, str))
+        )
 
     def _cast_type(self, type_annotation: Type, value: Any) -> Any:
         value_type = type(value)
         type_origin = get_origin(type_annotation)
         type_args = get_args(type_annotation)
 
         # skip if value type is annotated correct or is missing
@@ -224,28 +226,36 @@
                 "`%s.%s` value not found, set default `%s` value",
                 instance.__class__.__name__,
                 name,
                 self.default,
             )
             value = self.default
         else:
-            logger.debug("`%s.%s = %s` raw value(s)", instance.__class__.__name__, name, value)
+            logger.debug(
+                "`%s.%s = %s` raw value(s)", instance.__class__.__name__, name, value
+            )
 
         if self._is_iterable_and_not_string_value(value):
             value = self._filter(value)
             if self.filter_:
-                logger.debug("filter_ `%s.%s = %s`", instance.__class__.__name__, name, value)
+                logger.debug(
+                    "filter_ `%s.%s = %s`", instance.__class__.__name__, name, value
+                )
 
         value = self._callback(value)
         if self.callback:
-            logger.debug("callback `%s.%s = %s`", instance.__class__.__name__, name, value)
+            logger.debug(
+                "callback `%s.%s = %s`", instance.__class__.__name__, name, value
+            )
 
         if self.factory:
             value = self._factory(value)
-            logger.debug("factory `%s.%s = %s`", instance.__class__.__name__, name, value)
+            logger.debug(
+                "factory `%s.%s = %s`", instance.__class__.__name__, name, value
+            )
         else:
             value = self._typing(instance, name, value)
         return value
 
     def _filter(self, value: T) -> Any:
         """filter parsed value by filter_ function, if it passed
 
@@ -321,15 +331,17 @@
 
 class BaseSchema:
     class Config(BaseSchemaConfig):
         pass
 
     @staticmethod
     def _is_annotated_field(attr: Type):
-        return get_origin(attr) is Annotated and isinstance(get_args(attr)[-1], BaseField)
+        return get_origin(attr) is Annotated and isinstance(
+            get_args(attr)[-1], BaseField
+        )
 
     @staticmethod
     def _is_annotated_tuple_fields(attr: Type):
         return (
             get_origin(attr) is Annotated
             and isinstance(get_args(attr)[-1], tuple)
             and all(isinstance(fld, BaseField) for fld in get_args(attr)[-1])
@@ -443,30 +455,65 @@
                     name,
                     field.__class__.__name__,
                     value,
                 )
 
                 if _fails_counter > self.Config.fails_attempt:
                     raise ParseFailAttemptsError(
-                        f"{_fails_counter} of {len(_fields.keys())} " "fields failed parse."
+                        f"{_fails_counter} of {len(_fields.keys())} "
+                        "fields failed parse."
                     )
             logger.debug(
                 "`%s.%s[%s] = %s`",
                 self.__class__.__name__,
                 name,
                 field.__class__.__name__,
                 value,
             )
             setattr(self, name, value)
-        logger.debug("%s done! Fields fails: %i", self.__class__.__name__, _fails_counter)
+        logger.debug(
+            "%s done! Fields fails: %i", self.__class__.__name__, _fails_counter
+        )
 
     @classmethod
-    def init_list(cls, markups: list[str]) -> list[Self]:
+    def init_list(cls, markups: Iterable[str]) -> list[Self]:
+        """Init list of schemas by markups sequence
+
+        :param markups: - iterable markups sequence
+        """
         return [cls(markup) for markup in markups]
 
+    @classmethod
+    def from_list(cls, markups: Iterable[str]) -> list[Self]:
+        """Init list of schemas by markups sequence
+
+        :param markups: iterable markups sequence
+        """
+        return cls.init_list(markups)
+
+    @classmethod
+    def from_crop_rule_list(
+        cls, markup: str, *, crop_rule: Callable[[str], Iterable[str]]
+    ) -> list[Self]:
+        """Init list of schemas by crop_rule
+
+        :param markup: markup string
+        :param crop_rule: crop rule function to *parts*
+        """
+        return cls.init_list(crop_rule(markup))
+
+    @classmethod
+    def from_crop_rule(cls, markup: str, *, crop_rule: Callable[[str], str]) -> Self:
+        """Init single schema by crop_rule
+
+        :param markup: markup string
+        :param crop_rule: crop rule function to *part*.
+        """
+        return cls(crop_rule(markup))
+
     @staticmethod
     def _to_dict(value: BaseSchema | list | dict):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
             if all(isinstance(val, BaseSchema) for val in value):
```

### Comparing `scrape_schema-0.0.1/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.2/scrape_schema/callbacks/slax.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     def wrapper(markup: str) -> list[str]:
         parser = HTMLParser(markup, **slax_config)
         return [m.html for m in parser.css(query)]
 
     return wrapper
 
 
-def get_attr(name: str, default: Optional[Any] = None) -> Callable[[Node | Any], str | Any]:
+def get_attr(
+    name: str, default: Optional[Any] = None
+) -> Callable[[Node | Any], str | Any]:
     """get attribute from Node object
 
     :param name: tag name
     :param default: default value, if tag is not founded. default None
     """
 
     def wrapper(node: Node | Any) -> str:
```

### Comparing `scrape_schema-0.0.1/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.2/scrape_schema/callbacks/soup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 
 def replace_text(
     old: str, new: str, count: int = -1, *, separator: str = "", strip: bool = False
 ) -> Callable[[Tag | Any], str | Any]:
     def wrapper(tag: Tag | Any) -> str | Any:
         if isinstance(tag, Tag):
-            return tag.get_text(separator=separator, strip=strip).replace(old, new, count)
+            return tag.get_text(separator=separator, strip=strip).replace(
+                old, new, count
+            )
         return tag
 
     return wrapper
 
 
 def element_to_dict(element: str) -> dict[str, str | dict]:
     """Convert string element to dict
@@ -40,15 +42,17 @@
     if not (match := RE_TAG_NAME.search(element)):
         raise TypeError(f"Element `{element}` is not HTML tag")
     tag_name = match.group(1)
     attrs = dict(RE_TAG_ATTRS.findall(element))
     return {"name": tag_name, "attrs": attrs}
 
 
-def get_text(separator: str = "", strip: bool = False) -> Callable[[Tag | Any], str | Any]:
+def get_text(
+    separator: str = "", strip: bool = False
+) -> Callable[[Tag | Any], str | Any]:
     """get text from bs4.Tag
 
     :param separator: separator. default ""
     :param strip: strip flag. default False
     :return:
     """
```

### Comparing `scrape_schema-0.0.1/scrape_schema/fields/nested.py` & `scrape_schema-0.0.2/scrape_schema/fields/nested.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,17 @@
         :param crop_rule: function for crop markdown to part
         :param factory: function for convert to another type. Default convert to `schema`
         """
         super().__init__(factory=factory)
         self._schema = schema
         self.crop_rule = crop_rule
 
-    def __call__(self, instance: BaseSchema, name: str, markup: str) -> BaseSchema | Any:
+    def __call__(
+        self, instance: BaseSchema, name: str, markup: str
+    ) -> BaseSchema | Any:
         markup = self._parse(markup)
         new_markup = self.crop_rule(markup)
         value = self._schema(new_markup)
         return self._factory(value)
 
 
 class NestedList(BaseNested):
@@ -52,12 +54,14 @@
         :param factory: function for convert to another type. Default convert to `schema`
         """
         super().__init__(factory=factory)
         self.crop_rule = crop_rule
         self._schema = schema
         self.crop_rule = crop_rule
 
-    def __call__(self, instance: BaseSchema, name: str, markup: str) -> list[BaseSchema] | Any:
+    def __call__(
+        self, instance: BaseSchema, name: str, markup: str
+    ) -> list[BaseSchema] | Any:
         markup = self._parse(markup)
         new_markups = self.crop_rule(markup)
         value = self._schema.init_list(new_markups)
         return self._factory(value)
```

### Comparing `scrape_schema-0.0.1/scrape_schema/fields/regex.py` & `scrape_schema-0.0.2/scrape_schema/fields/regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
         :param group: match group. default 1
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param callback: function eval result. default None
         :param factory: function cast final result. If passed - ignore type-casting. Default None
         """
         super().__init__(default=default, callback=callback, factory=factory)
-        self.pattern = re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        self.pattern = (
+            re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        )
         self.group = group
 
     def _parse(self, markup: str) -> Optional[str]:
         if result := self.pattern.search(markup):
             return result.group(self.group)
         return None
 
@@ -83,16 +85,20 @@
         :param group: match group. default 1
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default None
         :param factory: function cast final result. If passed - ignore type-casting. Default None
         """
-        super().__init__(default=default, filter_=filter_, callback=callback, factory=factory)
-        self.pattern = re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        super().__init__(
+            default=default, filter_=filter_, callback=callback, factory=factory
+        )
+        self.pattern = (
+            re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        )
         self.group = group
 
     def _parse(self, markup: str) -> list[str]:
         if matches := self.pattern.finditer(markup):
             return [m.group(self.group) for m in matches]
         return []
 
@@ -112,15 +118,17 @@
         :param pattern: re.compile pattern or string. Pattern required named groups
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param callback: function eval result. default None
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
         super().__init__(default=default, callback=callback, factory=factory)
-        self.pattern = re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        self.pattern = (
+            re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        )
         if not self.pattern.groupindex:
             raise AttributeError(f"{pattern.pattern} required named groups")  # type: ignore
 
     def _parse(self, markup: str) -> dict[str, str]:
         return result.groupdict() if (result := self.pattern.search(markup)) else {}
 
 
@@ -140,16 +148,20 @@
         :param pattern: re.compile pattern or string. Pattern required named groups
         :param flags: regex compile flags. default 0
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default None
         :param factory: function cast final result. If passed - ignore type-casting. Default None
         """
-        super().__init__(default=default, callback=callback, filter_=filter_, factory=factory)
-        self.pattern = re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        super().__init__(
+            default=default, callback=callback, filter_=filter_, factory=factory
+        )
+        self.pattern = (
+            re.compile(pattern, flags) if isinstance(pattern, str) else pattern
+        )
         if not self.pattern.groupindex:
             raise AttributeError(f"{pattern.pattern} required named groups")  # type: ignore
 
     def _parse(self, markup: str) -> list[dict[str, str]]:
         if results := self.pattern.finditer(markup):
             return [result.groupdict() for result in results]
         return []
```

### Comparing `scrape_schema-0.0.1/scrape_schema/fields/slax.py` & `scrape_schema-0.0.2/scrape_schema/fields/slax.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,12 +69,14 @@
 
         :param selector: css selector
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
-        super().__init__(default=default, callback=callback, factory=factory, filter_=filter_)
+        super().__init__(
+            default=default, callback=callback, factory=factory, filter_=filter_
+        )
         self.selector = selector
 
     def _parse(self, markup: HTMLParser) -> list[Node]:
         return markup.css(self.selector)
```

### Comparing `scrape_schema-0.0.1/scrape_schema/fields/soup.py` & `scrape_schema-0.0.2/scrape_schema/fields/soup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,17 @@
 
         :param element: html tag or dict of keyword args for BeautifulSoup(...).find_all method
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
-        super().__init__(default=default, callback=callback, factory=factory, filter_=filter_)
+        super().__init__(
+            default=default, callback=callback, factory=factory, filter_=filter_
+        )
         self.element = element_to_dict(element) if isinstance(element, str) else element
 
     def _parse(self, markup: BeautifulSoup | Tag) -> ResultSet:
         return markup.find_all(**self.element)
 
 
 class SoupSelect(BaseSoup):
@@ -126,12 +128,14 @@
 
         :param selector: css selector
         :param default: default value if match not founded. default None
         :param filter_: function for filter result list. default None
         :param callback: function eval result. default get text from element
         :param factory: function final cast result. If passed - ignore type-casting. Default None
         """
-        super().__init__(default=default, callback=callback, factory=factory, filter_=filter_)
+        super().__init__(
+            default=default, callback=callback, factory=factory, filter_=filter_
+        )
         self.selector = selector
 
     def _parse(self, markup: BeautifulSoup | Tag) -> ResultSet:
         return markup.select(self.selector)
```

### Comparing `scrape_schema-0.0.1/.gitignore` & `scrape_schema-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.1/LICENSE` & `scrape_schema-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.1/README.md` & `scrape_schema-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.1/pyproject.toml` & `scrape_schema-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 Examples = "https://github.com/vypivshiy/scrape-schema/examples"
 
 
 [project.optional-dependencies]
 selectolax = ["selectolax"]
 bs4 = ["bs4"]
 all = ["selectolax", "bs4"]
+dev = ["bs4", "selectolax", "flake8", "black", "isort", "pytest", "mypy"]
+docs = ["mkdocs-material"]
 
 [tool.hatch.version]
 path = "scrape_schema/__init__.py"
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs-material"
@@ -87,13 +89,13 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.mypy]
 pretty = true
 ignore_missing_imports = true
-exclude = ["env", ".env", "venv", "tests/*", "__pycache__"]
+exclude = ["env", ".env", "venv", "tests/*", "__pycache__", "examples"]
 files = "scrape_schema/*.py,scrape_schema/fields/*.py,scrape_schema/callbacks/*.py"
 
 [tool.black]
```

### Comparing `scrape_schema-0.0.1/PKG-INFO` & `scrape_schema-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -23,14 +23,24 @@
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions; python_version < '3.11'
 Provides-Extra: all
 Requires-Dist: bs4; extra == 'all'
 Requires-Dist: selectolax; extra == 'all'
 Provides-Extra: bs4
 Requires-Dist: bs4; extra == 'bs4'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: bs4; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: selectolax; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == 'docs'
 Provides-Extra: selectolax
 Requires-Dist: selectolax; extra == 'selectolax'
 Description-Content-Type: text/markdown
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Documentation Status](https://readthedocs.org/projects/scrape-schema/badge/?version=latest)](https://scrape-schema.readthedocs.io/en/latest/?badge=latest)
 # Scrape-schema
```

