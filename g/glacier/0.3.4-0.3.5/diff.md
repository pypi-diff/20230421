# Comparing `tmp/glacier-0.3.4.tar.gz` & `tmp/glacier-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier-0.3.4.tar", last modified: Tue Mar 22 09:24:58 2022, max compression
+gzip compressed data, was "glacier-0.3.5.tar", max compression
```

## Comparing `glacier-0.3.4.tar` & `glacier-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1071 2022-03-22 09:19:38.979008 glacier-0.3.4/LICENSE
--rw-r--r--   0        0        0       34 2022-03-22 09:19:38.983008 glacier-0.3.4/glacier/__init__.py
--rw-r--r--   0        0        0     8325 2022-03-22 09:19:38.983008 glacier-0.3.4/glacier/core.py
--rw-r--r--   0        0        0     7855 2022-03-22 09:19:38.983008 glacier-0.3.4/glacier/docstring.py
--rw-r--r--   0        0        0      493 2022-03-22 09:19:38.983008 glacier-0.3.4/glacier/misc.py
--rw-r--r--   0        0        0        0 2022-03-22 09:19:38.983008 glacier-0.3.4/glacier/py.typed
--rw-r--r--   0        0        0      986 2022-03-22 09:19:38.983008 glacier-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      729 2022-03-22 09:24:58.542699 glacier-0.3.4/setup.py
--rw-r--r--   0        0        0      597 2022-03-22 09:24:58.543051 glacier-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 04:27:15.100552 glacier-0.3.5/LICENSE
+-rw-r--r--   0        0        0       34 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/__init__.py
+-rw-r--r--   0        0        0     8558 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/core.py
+-rw-r--r--   0        0        0     7855 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/docstring.py
+-rw-r--r--   0        0        0      493 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/misc.py
+-rw-r--r--   0        0        0        0 2023-04-21 04:27:15.100552 glacier-0.3.5/glacier/py.typed
+-rw-r--r--   0        0        0      934 2023-04-21 04:27:15.104552 glacier-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 glacier-0.3.5/PKG-INFO
```

### Comparing `glacier-0.3.4/LICENSE` & `glacier-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier-0.3.4/glacier/core.py` & `glacier-0.3.5/glacier/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import functools
 from enum import Enum
 from inspect import Parameter, signature
 from typing import (Any, Callable, Coroutine, Dict, List, Optional, Type,
                     TypeVar, Union)
 
 import click
-import click_completion
+try:
+    import click_completion
+    loads_completion = True
+except Exception:
+    loads_completion = False
+    ...
 from click_help_colors import HelpColorsCommand, HelpColorsGroup
 
 from glacier.docstring import (Doc, GoogleParser, NumpyParser, Parser,
                                RestructuredTextParser)
 from glacier.misc import coro
 
 """
@@ -165,15 +170,15 @@
                     '--' + param.name.replace('_', '-'),
                     type=param.annotation,
                     **common_kwargs,
                 )(click_f)
             elif issubclass(param.annotation, Enum):
                 click_f = click.option(  # type: ignore
                     '--' + param.name.replace('_', '-'),
-                    type=click.Choice(enum_map[param.name].keys()),
+                    type=click.Choice(list(enum_map[param.name].keys())),
                     **common_kwargs,
                 )(click_f)
 
     if click_group:
         return click_group.command(  # type: ignore
             cls=HelpColorsCommand,
             context_settings=CONTEXT_SETTINGS,
@@ -194,30 +199,31 @@
     @functools.wraps(f)
     def wrapped(*args: Any, **kwargs: Any) -> T:
         return f(*args, **kwargs)
     wrapped.__name__ = name
     return wrapped
 
 
-@click.option(
-    '-i',
-    '--case-insensitive/--no-case-insensitive',
-    help="Case insensitive completion",
-)
-@click.argument(
-    'shell',
-    required=False,
-    type=click_completion.DocumentedChoice(click_completion.core.shells),
-)
-def show_completion(shell: str, case_insensitive: bool) -> None:
-    """Show the click-completion-command completion code"""
-    extra_env = {
-        '_CLICK_COMPLETION_COMMAND_CASE_INSENSITIVE_COMPLETE': 'ON'
-    } if case_insensitive else {}
-    click.echo(click_completion.core.get_code(shell, extra_env=extra_env))
+if loads_completion:
+    @click.option(
+        '-i',
+        '--case-insensitive/--no-case-insensitive',
+        help="Case insensitive completion",
+    )
+    @click.argument(
+        'shell',
+        required=False,
+        type=click_completion.DocumentedChoice(click_completion.core.shells),
+    )
+    def show_completion(shell: str, case_insensitive: bool) -> None:
+        """Show the click-completion-command completion code"""
+        extra_env = {
+            '_CLICK_COMPLETION_COMMAND_CASE_INSENSITIVE_COMPLETE': 'ON'
+        } if case_insensitive else {}
+        click.echo(click_completion.core.get_code(shell, extra_env=extra_env))
 
 
 def glacier_group(
     f: Union[
         List[GlacierFunction],
         Dict[str, Union[GlacierFunction, GlacierUnit]],
     ],
@@ -261,15 +267,15 @@
                     _f,  # type: ignore
                     group,
                     name,
                 )
     else:
         raise Exception("The arguments of glacier is wrong.")
 
-    if parent_group is None:
+    if parent_group is None and loads_completion:
         group.command(  # type: ignore
             cls=HelpColorsCommand,
             context_settings=CONTEXT_SETTINGS,
             **DEFAULT_COLOR_OPTIONS,  # type: ignore
         )(show_completion)
 
     return group  # type: ignore
@@ -285,9 +291,10 @@
     """
 
     if callable(f):
         # Only one function is passed.
         entry_point_f = _get_click_command(f)
     else:
         entry_point_f = glacier_group(f)  # type: ignore
-    click_completion.init()
+    if loads_completion:
+        click_completion.init()
     entry_point_f()
```

### Comparing `glacier-0.3.4/glacier/docstring.py` & `glacier-0.3.5/glacier/docstring.py`

 * *Files identical despite different names*

### Comparing `glacier-0.3.4/pyproject.toml` & `glacier-0.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "glacier"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Hiroki Konishi <relastle@gmail.com>"]
 license = "MIT"
 packages = [
   {include = "glacier"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-click-completion = "^0.5.2"
 typing-extensions = "^4.1.1"
 click = "^8.0.4"
 click-help-colors = "^0.9.1"
 importlib-metadata = "^4.11.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "==6.0.1"
@@ -39,9 +38,8 @@
 strict_optional = true
 no_implicit_optional = true
 show_error_context = true
 show_column_numbers = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 warn_return_any = true
-show_none_errors = true
 warn_unused_ignores = false
```

### Comparing `glacier-0.3.4/PKG-INFO` & `glacier-0.3.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: glacier
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 License: MIT
 Author: Hiroki Konishi
 Author-email: relastle@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: click-completion (>=0.5.2,<0.6.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
```

