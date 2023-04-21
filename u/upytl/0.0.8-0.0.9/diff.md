# Comparing `tmp/upytl-0.0.8.tar.gz` & `tmp/upytl-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\_MyPy\py4web\py4web_ombott\upytl\dist\.tmp-873098c5\upytl-0.0.8.tar", last modified: Sun Apr  2 21:01:17 2023, max compression
+gzip compressed data, was "D:\_MyPy\py4web\py4web_ombott\upytl\dist\.tmp-owobgjx7\upytl-0.0.9.tar", last modified: Fri Apr 21 07:08:40 2023, max compression
```

## Comparing `upytl-0.0.8.tar` & `upytl-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 21:01:17.466517 upytl-0.0.8/
--rw-rw-rw-   0        0        0     1114 2022-06-29 20:55:15.000000 upytl-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1006 2023-04-02 21:01:17.466517 upytl-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2022-07-04 07:12:06.000000 upytl-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-02 21:01:17.466517 upytl-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1438 2022-09-04 11:44:49.000000 upytl-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:01:17.450984 upytl-0.0.8/upytl/
--rw-rw-rw-   0        0        0      384 2023-04-02 20:59:45.000000 upytl-0.0.8/upytl/__init__.py
--rw-rw-rw-   0        0        0    28518 2023-04-01 23:52:09.000000 upytl-0.0.8/upytl/core.py
--rw-rw-rw-   0        0        0     1682 2023-03-30 20:25:39.000000 upytl-0.0.8/upytl/html.py
-drwxrwxrwx   0        0        0        0 2023-04-02 21:01:17.466517 upytl-0.0.8/upytl.egg-info/
--rw-rw-rw-   0        0        0     1006 2023-04-02 21:01:17.000000 upytl-0.0.8/upytl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-04-02 21:01:17.000000 upytl-0.0.8/upytl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 21:01:17.000000 upytl-0.0.8/upytl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-02 21:01:17.000000 upytl-0.0.8/upytl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 07:08:40.540953 upytl-0.0.9/
+-rw-rw-rw-   0        0        0     1114 2022-06-29 20:55:15.000000 upytl-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2339 2023-04-21 07:08:40.540953 upytl-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    25284 2023-04-21 06:02:34.000000 upytl-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1374 2023-04-21 06:55:12.000000 upytl-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:08:40.540953 upytl-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 07:08:40.525297 upytl-0.0.9/tests/
+-rw-rw-rw-   0        0        0      380 2023-04-21 06:20:23.000000 upytl-0.0.9/tests/test_install.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:08:40.525297 upytl-0.0.9/upytl/
+-rw-rw-rw-   0        0        0      468 2023-04-21 07:06:54.000000 upytl-0.0.9/upytl/__init__.py
+-rw-rw-rw-   0        0        0     9526 2023-04-07 21:19:06.000000 upytl-0.0.9/upytl/bulma.py
+-rw-rw-rw-   0        0        0    27635 2023-04-21 06:04:47.000000 upytl-0.0.9/upytl/core.py
+-rw-rw-rw-   0        0        0     6114 2023-04-06 11:55:19.000000 upytl-0.0.9/upytl/helpers.py
+-rw-rw-rw-   0        0        0     1682 2023-04-07 13:57:34.000000 upytl-0.0.9/upytl/html.py
+-rw-rw-rw-   0        0        0      852 2023-04-08 22:37:15.000000 upytl-0.0.9/upytl/xtemplate.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:08:40.540953 upytl-0.0.9/upytl.egg-info/
+-rw-rw-rw-   0        0        0     2339 2023-04-21 07:08:40.000000 upytl-0.0.9/upytl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-04-21 07:08:40.000000 upytl-0.0.9/upytl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:08:40.000000 upytl-0.0.9/upytl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 07:08:40.000000 upytl-0.0.9/upytl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-21 07:08:40.000000 upytl-0.0.9/upytl.egg-info/top_level.txt
```

### Comparing `upytl-0.0.8/LICENSE` & `upytl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `upytl-0.0.8/setup.py` & `upytl-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-import re
-from setuptools import setup
+[project]
+name = "upytl"
+description = "UPYTL - Ultra Pythonic Template Language"
+requires-python = ">=3.7"
+license = {file = "LICENSE"}
+keywords = ["python", "webapplication", "html", "template"]
+authors = [
+  { name="Valery Kucherov", email="valq7711@gmail.com" },
+]
+
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Text Processing :: Markup :: HTML",
+]
+
+dynamic = ["version"]
+
+[project.urls]
+homepage = "https://github.com/valq7711/upytl"
+repository = "https://github.com/valq7711/upytl"
+
+[build-system]
+requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+zip-safe = false
+include-package-data = false
+
+[tool.setuptools.packages.find]
+include= ["upytl", "upytl.*"]
+namespaces = false
 
-
-def get_module_var(varname):
-    src = 'upytl'
-    regex = re.compile(fr"^{varname}\s*\=\s*['\"](.+?)['\"]", re.M)
-    mobj = next(regex.finditer(open(f"{src}/__init__.py").read()))
-    return mobj.groups()[0]
-
-
-__author__ = get_module_var('__author__')
-__license__ = get_module_var('__license__')
-__version__ = get_module_var('__version__')
-
-
-setup(
-    name="upytl",
-    version=__version__,
-    url="https://github.com/valq7711/upytl",
-    license=__license__,
-    author=__author__,
-    author_email="valq7711@gmail.com",
-    maintainer=__author__,
-    maintainer_email="valq7711@gmail.com",
-    description="UPYTL - Ultra Pythonic Template Language",
-    platforms="any",
-    keywords='python webapplication html',
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Environment :: Web Environment",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Text Processing :: Markup :: HTML",
-    ],
-    python_requires='>=3.7',
-    packages=['upytl'],
-)
+[tool.setuptools.dynamic]
+version = {attr = "upytl.__version__"}
```

### Comparing `upytl-0.0.8/upytl/core.py` & `upytl-0.0.9/upytl/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import io
 import re
 import functools
 from enum import Enum
 from types import SimpleNamespace, CodeType
 import inspect
+import threading
 
-from typing import Union, Callable, Tuple, List, Iterable, overload, Type, Dict, Any, TypeVar, Optional
+from typing import Union, Callable, Tuple, List, Iterable, overload, Type, Dict, TypeVar, Optional
+
+from upytl.helpers import AttrsDict, ValueGetter, ValueGettersDict
 
 
 AUTO_TAG_NAME = object()
 
 
 class RenderError(Exception):
     def __init__(self, component: 'Tag', orig_exc):
@@ -47,18 +50,19 @@
             raise RenderError(self, exc) from exc
     return inner
 
 
 class RenderedTag(SimpleNamespace):
     tag_class: Type['Tag']
     attrs: dict
+    tag: Union[str, None]
 
     @property
     def tag_name(self) -> str:
-        name = self.tag_class.tag_name
+        name = self.tag
         if name and isinstance(name, str):
             return name
 
         class_name = self.tag_class.__name__
         if name is AUTO_TAG_NAME:
             class_name = class_name.lower()
         return class_name
@@ -68,83 +72,14 @@
         return self.tag_class.is_body_allowed
 
     @property
     def is_meta_tag(self) -> bool:
         return self.tag_class.is_meta_tag
 
 
-class ValueGetter:
-    is_static = True
-
-    def __init__(self, value, *, force_compile=False, is_static=False):
-        if is_static:
-            self._value_gtter = value
-            assert not callable(value)
-        else:
-            self._value_gtter = self._make_value_getter(value, force_compile)
-
-        if callable(self._value_gtter):
-            self.get = self._value_gtter
-            self.is_static = False
-        else:
-            self.get = self._get_static_value_method
-
-    def get(self, ctx):
-        '''See `__init__`'''
-        pass
-
-    def _get_static_value_method(self, ctx: dict):
-        return self._value_gtter
-
-    @staticmethod
-    def _make_value_getter(v, force_compile) -> Union[str, Callable[[dict], Any]]:
-        if force_compile:
-            if isinstance(v, str):
-                code_obj = compile(v, '<string>', 'eval')
-
-                def render(ctx: dict):
-                    return eval(code_obj, None, ctx)
-                return render
-            return v
-
-        render = v
-        if isinstance(v, bytes):
-            render = v.decode()
-
-        elif isinstance(v, str):
-            try:
-                v.format_map({})
-                # if we're here it is just string
-                # do nothing
-            except KeyError:
-                render = v.format_map
-
-        elif isinstance(v, set):
-            assert len(v) == 1
-            v = [*v][0]
-            code_obj = compile(v, '<string>', 'eval')
-
-            def render(ctx: dict):
-                return eval(code_obj, None, ctx)
-
-        return render
-
-
-class ValueGettersDict(dict):
-
-    def render(self: Dict[str, ValueGetter], ctx: dict):
-        return {
-            k: v.get(ctx) if isinstance(v, ValueGetter) else v
-            for k, v in self.items()
-        }
-
-    def copy(self):
-        return ValueGettersDict(super().copy())
-
-
 def set_info(init):
 
     @functools.wraps(init)
     def inner(self: 'Tag', *args, **kw):
         if self._info is None:
             frm = inspect.currentframe().f_back
             self._info = {'created_at': f'{frm.f_code.co_filename}:{frm.f_lineno}'}
@@ -156,39 +91,48 @@
 
 class Tag:
 
     tag_name: Union[str, object] = AUTO_TAG_NAME
 
     is_body_allowed = True  # no body - no closing tag
     is_meta_tag = False  # if True expose only body, e.g. Text, Template, MyComponent, Slot
+    ident_class = None  # identity non-overridable class
 
     # instance attributes
-    attrs: Dict[str, Union[ValueGetter, Dict[str, ValueGetter]]]
+    attrs: Dict[str, Union[ValueGetter, Dict[str, ValueGetter]]] = None
     for_loop: tuple  # (var_names, iterable_factory)
     if_cond: Tuple[str, ValueGetter]   # (kword:['If' | 'Elif' | 'Else'] , value:[callable | castable to bool])
     assign_attrs: ValueGetter
     _info: Optional[dict] = None
 
     @overload
     def __init__(
-        self, *,
+        self, _: dict = None, *,
         For=None, If=None, Elif=None, Else=None,
         Class=None, xClass=None,
         Style=None, xStyle=None,
         Data=None, xData=None,
         Attrs=None,
+        Tag=None,
         **attrs
     ):
         ...
 
     @set_info
-    def __init__(self, **attrs):
+    def __init__(self, _: dict = None, **attrs):
         """
         xClass, xStyle, xData mean eXtend Class or Style or Data
         """
+        if _ is not None:
+            _.update(attrs)
+            attrs = _
+
+        if self.attrs is not None:
+            attrs = dict(self.attrs, **attrs)
+
         self.attrs, self.for_loop, self.if_cond = self._process_attrs(attrs)
         self.assign_attrs = self.attrs.pop('Attrs', ValueGetter({}))
 
     @staticmethod
     def _compile_for(s: str) -> Tuple[str, CodeType]:
         """s = 'a, b in some'"""
         # get vars-in part
@@ -205,16 +149,30 @@
     def _process_attrs(self, attrs: dict):
         attrs, for_loop, if_cond = self._parse_attrs(attrs)
         self._wrap_in_getters(attrs)
         return attrs, for_loop, if_cond
 
     def _wrap_in_getters(self, attrs: dict):
         for k, v in attrs.items():
+            if isinstance(v, (list, tuple)):
+                # [b'button', 'is_large', ('is-{size}', 'size')] =>
+                #       {'button': True, 'is-large': 'is_large', 'is-{size}': 'size'}
+                v = dict([
+                    it if isinstance(it, tuple)
+                    else
+                        (it.decode(), True) if isinstance(it, bytes)
+                    else
+                        (str(it).replace('_', '-'), it)
+                    for it in v
+                ])
+
             if isinstance(v, dict):
-                attrs[k] = ValueGettersDict([(dk, ValueGetter(dv)) for dk, dv in v.items()])
+                attrs[k] = ValueGettersDict([
+                    (dk, ValueGetter(dv, force_compile=(k in ['Class', 'xClass']))) for dk, dv in v.items()]
+                )
             else:
                 attrs[k] = ValueGetter(v, force_compile=(k == 'Attrs'))
 
     def _parse_attrs(self, attrs: dict):
         for_loop = attrs.pop('For', None)
         if for_loop is not None:
             for_loop = self._compile_for(for_loop)
@@ -233,175 +191,123 @@
         assign_attrs = attrs.get('Attrs', None)
         if isinstance(assign_attrs, dict):
             attrs.update(assign_attrs)
             attrs.pop('Attrs')
 
         return attrs, for_loop, if_cond
 
-    @classmethod
-    def _class_render(cls, dct: dict):
-        """Render html class of a tag."""
-        return [klass for klass, enabled in dct.items() if enabled]
-
-    @classmethod
-    def _style_render(cls, dct: dict):
-        """Render html style of a tag."""
-        return [f'{prop}:{value}' for prop, value in dct.items() if value]
-
-    @classmethod
-    def _render_attrs(
-            cls, attrs: Dict[str, Union[ValueGetter, dict]], ctx: dict,
-            *, skip: dict = None, render_nested=False
-    ) -> Dict[str, Any]:
-        if skip is None:
-            skip = {}
-        ret = {}
-        for a, v in attrs.items():
-            if a in skip:
-                continue
-            if isinstance(v, ValueGetter):
-                v = v.get(ctx)
-            elif render_nested and isinstance(v, ValueGettersDict):
-                v = v.render(ctx)
-            ret[a] = v
-        return ret
-
-    @classmethod
-    def _render_attrs_postproc(cls, attrs: dict, ctx: dict):
-        args = [
-            ('Class', 'xClass', ' ', cls._class_render),
-            ('Style', 'xStyle', ';', cls._style_render)
-        ]
-        for a, exa, sep, dict_mapper in args:
-            merged = cls._render_merge_special_attrs(attrs, a, exa, sep=sep, dict_mapper=dict_mapper, ctx=ctx)
-            attrs.pop(a, None)
-            attrs.pop(exa, None)
-            if merged:
-                attrs[a.lower()] = merged
-        cls._render_data_attrs(attrs, ctx)
-
-    @classmethod
-    def _render_data_attrs(cls, attrs: dict, ctx: dict):
-        name, extra_name = 'Data', 'xData'
-        data: Dict[str, ValueGetter]
-        data, xdata = cls._resolve_extendable_attrs(attrs, name, extra_name, ctx)
-        attrs.pop(name, None)
-        attrs.pop(extra_name, None)
-        if data is None:
-            return
-        for a, v in data.items():
-            attrs[f'data-{a}'] = v
-
-    @classmethod
-    def _resolve_extendable_attrs(cls, attrs: Dict[str, Union[Any, dict]], name, extra_name, ctx: dict):
-        attr = attrs.get(name)
-        extra = attrs.get(extra_name, None)
-        if extra is not None and attr is None:
-            attr = extra
-            extra = None
-
-        if isinstance(extra, ValueGettersDict):
-            extra = extra.render(ctx)
-
-        if isinstance(attr, dict):
-            if isinstance(extra, dict):
-                attr = attr.copy()
-                attr.update(extra)
-                extra = None
-            if isinstance(attr, ValueGettersDict):
-                attr = attr.render(ctx)
-
-        return attr, extra
-
-    @classmethod
-    def _render_merge_special_attrs(
-            cls, attrs: dict, attr_name, extra_name,
-            *, sep: str, ctx: dict, dict_mapper
-    ):
-        attr, extra = cls._resolve_extendable_attrs(attrs, attr_name, extra_name, ctx)
-        if attr is None:
-            return
-
-        if isinstance(attr, dict):
-            attr = sep.join(dict_mapper(attr))
-
-        if isinstance(extra, dict):
-            extra = sep.join(dict_mapper(extra))
-
-        if extra:
-            attr = f'{attr}{sep}{extra}'
-        return attr
-
     def resolve_cond(self, ctx):
         if self.if_cond is None:
             return
         kword, v = self.if_cond
         return (kword, v.get(ctx))
 
     @classmethod
-    def _make_self_rendered(cls, attrs):
+    def _render_attrs(cls, ctx: dict, attrs: AttrsDict):
+        attrs.render(ctx)
+        return attrs
+
+    @classmethod
+    def _make_self_rendered(cls, ctx: dict, attrs: AttrsDict):
+        attrs = cls._render_attrs(ctx, attrs)
+        ident_class = cls.ident_class
+        if ident_class is not None:
+            klass = attrs.get('class')
+            klass = f'{ident_class} {klass}' if klass else ident_class
+            attrs['class'] = klass
+
+        tag_name = attrs.pop('Tag', cls.tag_name)
+
         ret = RenderedTag(
             tag_class=cls,
             attrs=attrs,
+            tag=tag_name
         )
         return ret
 
-    def render_self(self, ctx, passed_attrs: Dict[str, Union[ValueGetter, dict]] = None):
-        attrs = self.attrs.copy()
+    def _merge_attrs(self, ctx: dict, passed_attrs: AttrsDict = None, passed_defaults: AttrsDict = None):
+        if passed_defaults is not None:
+            attrs = passed_defaults.copy()
+            attrs.extend(self.attrs)
+        else:
+            attrs = AttrsDict(self.attrs)
+
         attrs.update(self.assign_attrs.get(ctx))
         if passed_attrs is not None:
-            attrs.update(passed_attrs)
+            attrs.extend(passed_attrs)
+        return attrs
 
-        rendered_attrs = self._render_attrs(attrs, ctx)
-        self._render_attrs_postproc(rendered_attrs, ctx)
-        return self._make_self_rendered(rendered_attrs)
+    def _render_text_body(self, u: 'UPYTL', body: str, ctx: dict):
+        code = u.compile_template(body)
+        if code is not None:
+            body = eval(code, None, ctx)
+        return self.format_text_body(body)
+
+    def _render_dict_body(self, u: 'UPYTL', body: dict, self_ctx: dict, ctx: dict, self_rendered: RenderedTag):
+        yield u.START_BODY
+        for ch, ch_body, loop_vars in u.iter_body(body, self_ctx):
+            ch_ctx = ctx if loop_vars is None else dict(ctx, **loop_vars)
+            yield from ch.render(u, ch_ctx, ch_body)
+        yield u.END_BODY
 
     @catch_errors
-    def render(self, u: 'UPYTL', ctx: dict, body: Union[dict, str, None], passed_attrs: dict = None):
-        self_ctx = {**u.global_ctx, **ctx}
-        self_rendered = self.render_self(self_ctx, passed_attrs)
+    def render(
+            self, u: 'UPYTL', ctx: dict, body: Union[dict, str, None], passed_attrs: dict = None,
+            passed_defaults: dict = None
+    ):
+        self_ctx = dict(u.global_ctx, **ctx)
+
+        attrs = self._merge_attrs(self_ctx, passed_attrs, passed_defaults)
+        self_rendered = self._make_self_rendered(self_ctx, attrs)
+
         yield self_rendered
         if not body:
             return
         if isinstance(body, str):
-            code = u.compile_template(body)
-            if code is not None:
-                body = eval(code, None, self_ctx)
-            yield self.format_text_body(body)
+            yield self._render_text_body(u, body, self_ctx)
             return
-
-        yield u.START_BODY
-        for ch, ch_body, loop_vars in u.iter_body(body, self_ctx):
-            ch_ctx = ctx if loop_vars is None else {**ctx, **loop_vars}
-            yield from ch.render(u, ch_ctx, ch_body)
-        yield u.END_BODY
+        yield from self._render_dict_body(u, body, self_ctx, ctx, self_rendered)
 
     def format_text_body(self, body: str):
         """Return formatted/escaped body.
 
         NOTE: This hook is only invoked if the body is a `string` (i.e. text node).
         """
         return body
 
     def __repr__(self):
-        nm = self.tag_name or self.__class__.__name__
+        nm = self.tag_name if isinstance(self.tag_name, str) else self.__class__.__name__
         return f'<{nm}({str(self.attrs)})> {self._info}'
 
 
 class VoidTag(Tag):
     is_body_allowed = False
 
 
 class MetaTag(Tag):
     tag_name = None
     is_meta_tag = True
 
 
 class Template(MetaTag):
-    pass
+
+    @classmethod
+    def _render_attrs(cls, ctx: dict, attrs: AttrsDict):
+        attrs.render_values(ctx, render_complex_extendables=True)
+        return attrs
+
+    def _render_dict_body(self, u: 'UPYTL', body: dict, self_ctx: dict, ctx: dict, self_rendered: RenderedTag):
+        rendered_attrs = self_rendered.attrs
+        if 'Is' in rendered_attrs:
+            body = body[rendered_attrs.pop('Is')]
+        yield u.START_BODY
+        for ch, ch_body, loop_vars in u.iter_body(body, self_ctx):
+            ch_ctx = ctx if loop_vars is None else dict(ctx, **loop_vars)
+            yield from ch.render(u, ch_ctx, ch_body, passed_defaults=rendered_attrs)
+        yield u.END_BODY
 
 
 class Slot(MetaTag):
 
     @overload
     def __init__(
         self, *,
@@ -416,29 +322,30 @@
         super().__init__(**attrs)
 
     @property
     def SlotName(self):
         return self.attrs['SlotName']
 
     def render(self, u: 'UPYTL', ctx: dict, body: Union[dict, str, None]):
-        self_ctx = {**u.global_ctx, **ctx}
+        self_ctx = dict(u.global_ctx, **ctx)
         slots_content_map: dict
         slots_content_map = u.pop_scope()
         slot_name = self.SlotName.get(self_ctx)
         to_slot: Tuple[dict, Tag, dict]
         to_slot = slots_content_map.get(slot_name)
         if to_slot is None:
             # render as regular tag (slot default content)
             yield from super().render(u, ctx, body)
             u.push_scope(slots_content_map)
             return
 
         del body
         stempl_ctx, stempl, stempl_body = to_slot
-        self_rendered = self.render_self(self_ctx)
+        attrs = AttrsDict(self.attrs)
+        self_rendered = self._make_self_rendered(self_ctx, attrs)
         yield self_rendered
 
         # inject slot props
         stempl: SlotTemplate
         sprops_name = stempl.render_special('SlotProps', u, ctx)
         if sprops_name:
             stempl_ctx = {**stempl_ctx, **{sprops_name: self_rendered.attrs}}
@@ -449,39 +356,48 @@
         u.push_scope(slots_content_map)
 
 
 class SlotTemplate(MetaTag):
 
     Slot: ValueGetter
     SlotProps: Union[ValueGetter, None]
-    special_attrs = {'Slot', 'SlotProps'}
+    special_attrs = ('Slot', 'SlotProps')
 
     def _process_attrs(self, attrs: dict):
         tmp = super()._process_attrs(attrs)
         attrs, extra = tmp[0], tmp[1:]
         self.Slot = attrs.pop('Slot', ValueGetter('default'))
         self.SlotProps = attrs.pop('SlotProps', None)
         return [attrs, *extra]
 
     def render_special(self, spec_attr: str, u: 'UPYTL', ctx: dict):
         assert spec_attr in self.special_attrs
         v: Union[None, ValueGetter] = getattr(self, spec_attr)
         if v is not None:
-            ctx = None if v.is_static else {**u.global_ctx, **ctx}
+            ctx = None if v.is_static else dict(u.global_ctx, **ctx)
             return v.get(ctx)
 
 
 T = TypeVar('T', bound='Component')
 
 
 class ComponentMeta(type):
     def __init__(cls: Type[T], name, bases, dct):
         super().__init__(name, bases, dct)
         if name == 'Component':
             return
+
+        # parse props
+        if 'props' not in dct and '__init__' in dct:
+            props = {}
+            for i, p in enumerate(inspect.signature(dct['__init__']).parameters.values()):
+                if i and p.kind is p.POSITIONAL_OR_KEYWORD:
+                    props[p.name] = p.default if p.default is not p.empty else ''
+            cls.props = props
+
         template_processed = cls.__dict__.get('_template_processed', False)
         if not template_processed:
             cls._template_processed = True
             if cls.template is None:
                 cls.template = cls.template_factory(cls)
 
 
@@ -492,26 +408,30 @@
     _template_processed = False
 
     # instance attrs
     props: Union[list, Dict[str, ValueGetter]]
 
     @overload
     def __init__(
-        self, *,
+        self, _: dict = None, *,
         For=None, If=None, Elif=None, Else=None,
         Class=None, xClass=None,
         Style=None, xStyle=None,
         Data=None, xData=None,
         Attrs=None,
         **attrs
     ):
         ...
 
     @set_info
-    def __init__(self, **attrs):
+    def __init__(self, _: dict = None, **attrs):
+        if _ is not None:
+            _.update(attrs)
+            attrs = _
+        self.props_set = set()
         super().__init__(**attrs)
         self.slots = set()
 
     def _parse_attrs(self, attrs: dict):
         attrs, for_loop, if_cond = super()._parse_attrs(attrs)
 
         if isinstance(self.props, list):
@@ -521,45 +441,33 @@
 
         for k, v in props.items():
             props[k] = ValueGetter(v)
 
         for k in [*attrs]:
             if k in self.props:
                 props[k] = ValueGetter(attrs.pop(k))
+                self.props_set.add(k)
         self.props = props
         return attrs, for_loop, if_cond
 
-    def _merge_attrs(self, trg: dict, src: dict):
-        trg = trg.copy()
-        extendable_attrs = ['xClass', 'xStyle', 'xData']
-        extendables = {k: trg.pop(k, None) for k in extendable_attrs}
-        trg.update(src)
-        for k, v in extendables.items():
-            if v is None:
-                continue
-            trg_v = trg.get(k)
-            if trg_v is None:
-                trg[k] = v
-                continue
-            if isinstance(trg_v, dict) and isinstance(v, dict):
-                v = v.copy()
-                v.update(trg_v)
-                trg[k] = v
-        return trg
+    @classmethod
+    def _render_attrs(cls, ctx: dict, attrs: AttrsDict):
+        return attrs
 
     @catch_errors
     def render(
             self, u: 'UPYTL', ctx: dict, body: Union[dict, str, None],
-            passed_attrs: Dict[str, Union[Any, dict]] = None
+            passed_attrs: AttrsDict = None, passed_defaults: AttrsDict = None
     ):
-        self_ctx = {**u.global_ctx, **ctx}
-        if passed_attrs is None:
-            passed_attrs = {}
-        else:
-            passed_attrs = passed_attrs.copy()
+        self_ctx = u.global_ctx.copy()
+        self_ctx.update(ctx)
+
+        passed_attrs, passed_defaults = [
+            dct.copy() if dct is not None else AttrsDict() for dct in (passed_attrs, passed_defaults)
+        ]
 
         assign_attrs: dict = self.assign_attrs.get(self_ctx)
         assign_attrs = assign_attrs.copy()
 
         if isinstance(body, str) or isinstance(body, dict) and not isinstance(next(iter(body), None), SlotTemplate):
             body = {SlotTemplate(): body}
         slots_content: Dict[SlotTemplate, Union[str, dict]] = body
@@ -569,28 +477,38 @@
         props_rendered = {}
         # maybe props passed in Attrs or in passed_attrs
         for k, v in self.props.items():
             if k in assign_attrs:
                 props_rendered[k] = assign_attrs.pop(k)
             elif k in passed_attrs:
                 props_rendered[k] = passed_attrs.pop(k)
+            elif k in passed_defaults and k not in self.props_set:
+                props_rendered[k] = passed_defaults.pop(k)
             else:
-                props_rendered[k] = v.get(self_ctx)
+                if k in self.props_set:
+                    v = v.get(self_ctx)
+                    passed_defaults.pop(k, None)
+                elif k in passed_defaults:
+                    v = passed_defaults.pop(k)
+                else:
+                    v = v.get(self_ctx)
+                props_rendered[k] = v
         self_ctx.update(props_rendered)
-        rendered_attrs = self._render_attrs(
-            self.attrs, self_ctx, skip=assign_attrs, render_nested=True
-        )
+
+        rendered_attrs = passed_defaults
+        rendered_attrs.extend(self.attrs)
+        rendered_attrs.render_values(self_ctx, skip=assign_attrs, render_complex_extendables=True)
         rendered_attrs.update(assign_attrs)
-        passed_attrs = self._merge_attrs(rendered_attrs, passed_attrs)
 
         # yeild tag/attrs
-        self_rendered = self._make_self_rendered(rendered_attrs)
-
+        self_rendered = self._make_self_rendered(self_ctx, rendered_attrs)
         yield self_rendered
+
         yield u.START_BODY
+        passed_attrs = rendered_attrs.copy().extend(passed_attrs)
         # resolve for-loop/if-else
         slots_content_map = {}
         if slots_content:
             for st, st_body, loop_vars in u.iter_body(slots_content, {**u.global_ctx, **out_ctx}):
                 st: SlotTemplate
                 st_ctx = out_ctx if loop_vars is None else {**out_ctx, **loop_vars}
                 slots_content_map[st.render_special('Slot', u, st_ctx)] = (st_ctx, st, st_body)
@@ -613,14 +531,43 @@
 
         This method can be overloaded in a derived class
         to extend the context of own template.
         """
         return props_rendered
 
 
+class _GenTag:
+    def __getattr__(self, name: str) -> Type[Tag]:
+        cls = type(name, (Tag,), {'tag_name': name.replace('_', '-')})
+        return cls
+
+
+gtag = _GenTag()
+
+
+class SlotTemplateFactory:
+    def __init__(self, slot: str):
+        self.slot = slot
+
+    def __call__(self, **kw) -> SlotTemplate:
+        kw['Slot'] = self.slot
+        return SlotTemplate(**kw)
+
+
+class SlotsEnum(Enum):
+    def __init__(self):
+        self._value_ = SlotTemplateFactory(self.name)
+
+    def slot(self, **kw) -> Slot:
+        return Slot(SlotName=self.value.slot, **kw)
+
+    def __call__(self, **kw):
+        return self.value(**kw)
+
+
 class GenericComponent(Tag):
 
     component_factory: ValueGetter
 
     def _process_attrs(self, attrs: dict):
         # attrs, *extra = super()._process_attrs(attrs)
         tmp = super()._process_attrs(attrs)
@@ -648,19 +595,27 @@
     END_BODY = Punc.END
 
     compiled_templates_cache = {}
 
     registered_components: Dict[str, Tag]
 
     def __init__(self, *, global_ctx: dict = None, default_ctx: dict = None):
+        self._local = threading.local()
         self.global_ctx = global_ctx or {}
         self.default_ctx = default_ctx or {}
-        self.scope = None
         self.registered_components = {}
 
+    @property
+    def scope(self) -> list:
+        return self._local.scope
+
+    @scope.setter
+    def scope(self, scope: list):
+        self._local.scope = scope
+
     def get_component_factory(self, name: str) -> Type[Tag]:
         return self.registered_components[name]
 
     @classmethod
     def compile_template(cls, body: str, delimiters: List[str] = None):
         if delimiters is None:
             delimiters = ['[[', ']]']
@@ -755,15 +710,18 @@
             self._render(template, ctx, out)
             return out.buf.getvalue()
         except RenderError as exc:
             exc.set_html_dump(out.buf.getvalue())
             raise
 
     def _render(self, template: Dict[Tag, dict], ctx: dict, out: 'HTMLPrinter'):
-        ctx = {**self.default_ctx, **ctx}
+        if self.default_ctx:
+            dctx = self.default_ctx.copy()
+            dctx.update(ctx)
+            ctx = dctx
         self.scope = []
         # wrap in Template to ensure foo-loop/if-else will be processed properly
         template = {Template(): template}
         for k, v in template.items():
             for it in k.render(self, ctx, v):
                 if it is self.START_BODY:
                     out.start_body()
```

### Comparing `upytl-0.0.8/upytl/html.py` & `upytl-0.0.9/upytl/html.py`

 * *Files identical despite different names*

