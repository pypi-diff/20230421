# Comparing `tmp/stlog-0.0.7.tar.gz` & `tmp/stlog-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlog-0.0.7.tar", max compression
+gzip compressed data, was "stlog-0.0.8.tar", max compression
```

## Comparing `stlog-0.0.7.tar` & `stlog-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-04-10 12:45:31.855016 stlog-0.0.7/LICENSE
--rw-r--r--   0        0        0     8010 2023-04-10 12:45:31.855016 stlog-0.0.7/README.md
--rw-r--r--   0        0        0     1240 2023-04-10 12:45:54.319048 stlog-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-10 12:45:53.971048 stlog-0.0.7/stlog/__init__.py
--rw-r--r--   0        0        0      301 2023-04-10 12:45:53.971048 stlog-0.0.7/stlog/__init__.py.restore_version
--rw-r--r--   0        0        0     2641 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/adapter.py
--rw-r--r--   0        0        0     7277 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/base.py
--rw-r--r--   0        0        0     2638 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/context.py
--rw-r--r--   0        0        0    12794 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/formatter.py
--rw-r--r--   0        0        0     2499 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/handler.py
--rw-r--r--   0        0        0     4920 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/output.py
--rw-r--r--   0        0        0     4793 2023-04-10 12:45:31.859016 stlog-0.0.7/stlog/setup.py
--rw-r--r--   0        0        0     8562 1970-01-01 00:00:00.000000 stlog-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 15:06:41.936559 stlog-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8365 2023-04-21 15:06:41.936559 stlog-0.0.8/README.md
+-rw-r--r--   0        0        0     1089 2023-04-21 15:07:02.157027 stlog-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      593 2023-04-21 15:07:01.813020 stlog-0.0.8/stlog/__init__.py
+-rw-r--r--   0        0        0     2658 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/adapter.py
+-rw-r--r--   0        0        0     7632 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/base.py
+-rw-r--r--   0        0        0     2638 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/context.py
+-rw-r--r--   0        0        0    12850 2023-04-21 15:06:41.940559 stlog-0.0.8/stlog/formatter.py
+-rw-r--r--   0        0        0     2499 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/handler.py
+-rw-r--r--   0        0        0     3284 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/kvformatter.py
+-rw-r--r--   0        0        0     5109 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/output.py
+-rw-r--r--   0        0        0     7070 2023-04-21 15:06:41.944559 stlog-0.0.8/stlog/setup.py
+-rw-r--r--   0        0        0     8917 1970-01-01 00:00:00.000000 stlog-0.0.8/PKG-INFO
```

### Comparing `stlog-0.0.7/LICENSE` & `stlog-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stlog-0.0.7/README.md` & `stlog-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-<!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
-     and execute 'poetry run poe readme' to regenerate this README.md file -->
+ <!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
+      and execute 'poetry run invoke readme' to regenerate this README.md file -->
 
-# stlog
+ # stlog
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fabien-marty/stlog/lint.yaml)](https://github.com/fabien-marty/stlog/actions/workflows/lint.yaml)
 [![Codecov](https://img.shields.io/codecov/c/github/fabien-marty/stlog)](https://app.codecov.io/github/fabien-marty/stlog)
 [![pypi badge](https://img.shields.io/pypi/v/stlog?color=brightgreen)](https://pypi.org/project/stlog/)
 
 [Full documentation](https://fabien-marty.github.io/stlog/)
 
@@ -67,14 +67,38 @@
 
 ### Installation
 
 ```
 pip install stlog
 ```
 
+### Very minimal usage
+
+```python
+import stlog
+
+stlog.info("It works", foo="bar", x=123)
+stlog.critical("Houston, we have a problem!")
+ 
+```
+
+Output (without `rich` library installed):
+
+```
+2023-03-29T14:48:37Z root [   INFO   ] It works {foo=bar x=123}
+2023-03-29T14:48:37Z root [ CRITICAL ] Houston, we have a problem!
+ 
+```
+
+Output (with `rich` library installed):
+
+![rich output](docs/python/qs0.svg)
+ 
+
+
 ### Basic usage
 
 ```python
 from stlog import getLogger, setup
 
 # Set the logging default configuration (human output on stderr)
 setup()
@@ -178,53 +202,49 @@
 JSON ouput (on `stdout`) for machines:
 
 ```json
 {
     "client_id": 456,
     "foo": "bar",
     "http_method": "GET",
-    "logger": {
-        "name": "__main__"
-    },
+    "level": "INFO",
+    "logger": "__main__",
     "message": "It works",
     "request_id": "4c2383f5",
     "source": {
         "funcName": "<module>",
         "lineno": 21,
         "module": "qs3",
         "path": "/path/filename.py",
         "process": 6789,
         "processName": "MainProcess",
         "thread": 12345,
         "threadName": "MainThread"
     },
-    "status": "info",
-    "timestamp": "2023-03-29T14:48:37Z",
+    "time": "2023-03-29T14:48:37Z",
     "x": 123
 }
 {
     "client_id": 456,
     "http_method": "GET",
-    "logger": {
-        "name": "__main__"
-    },
+    "level": "CRITICAL",
+    "logger": "__main__",
     "message": "Houston, we have a problem!",
     "request_id": "4c2383f5",
     "source": {
         "funcName": "<module>",
         "lineno": 22,
         "module": "qs3",
         "path": "/path/filename.py",
         "process": 6789,
         "processName": "MainProcess",
         "thread": 12345,
         "threadName": "MainThread"
     },
-    "status": "critical",
-    "timestamp": "2023-03-29T14:48:37Z"
+    "time": "2023-03-29T14:48:37Z"
 }
  
 ```
 
 <!--quickstart-end-->
 
 ## Roadmap
```

### Comparing `stlog-0.0.7/pyproject.toml` & `stlog-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 [tool.poetry]
 name = "stlog"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Fabien MARTY <fabien.marty@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "stlog"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.247"
 mypy = "^1.0.1"
 black = "^23.1.0"
-poethepoet = "^0.18.1"
 pdoc3 = "^0.10.0"
 mkdocs-material = "^9.0.13"
 rich = "^13.3.2"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 mkdocs-macros-plugin = "^0.7.0"
 mkdocs-include-markdown-plugin = "^4.0.4"
 types-pyyaml = "^6.0.12.8"
 jinja2-shell-extension = "^2.0.0"
 termtosvg = "^1.1.0"
-import-linter = "^1.8.0"
 dunamai = "^1.16.0"
+invoke = "^2.0.0"
+types-invoke = "^2.0.0.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.importlinter]
-root_package = "stlog"
-include_external_packages = true
-
 [tool.ruff]
 # Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F", "W", "N", "UP", "B", "I", "PL", "RUF"]
 ignore = [
     "E501",
     "PLR2004"
 ]
 line-length = 88
 target-version = "py37"
 extend-exclude = ["docs/python", "html"]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
 
-[tool.poe]
-include = "tasks.toml"
-
-[tool.poe.env]
-PACKAGE = "stlog"
-
-
 [tool.mypy]
 exclude = ['^html/.*']
```

### Comparing `stlog-0.0.7/stlog/adapter.py` & `stlog-0.0.8/stlog/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 import collections
 import logging
 import typing
 
-from stlog.base import RESERVED_ATTRS, STLOG_EXTRA_KEY, check_json_types_or_raise
+from stlog.base import (
+    RESERVED_ATTRS,
+    STLOG_EXTRA_KEY,
+    check_json_types_or_raise,
+)
 from stlog.context import LogContext
 
 
 # ligthly adapted from https://github.com/Mergifyio/daiquiri/blob/main/daiquiri/__init__.py
 class _KeywordArgumentAdapter(logging.LoggerAdapter):
     """Logger adapter to add keyword arguments to log record's extra data.
```

### Comparing `stlog-0.0.7/stlog/base.py` & `stlog-0.0.8/stlog/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 import json
 import numbers
 import os
 import re
 import types
 from dataclasses import dataclass, field
+from string import Template
 from typing import Any, Callable, Match
 
 STLOG_EXTRA_KEY = "_stlog_extra"
 RICH_AVAILABLE = False
 try:
     from rich.traceback import Traceback
 
@@ -19,20 +20,21 @@
     pass
 
 
 TRUE_VALUES = ("1", "true", "yes")
 FALSE_VALUES = ("0", "false", "no")
 
 
-class StLogError(Exception):
+class StlogError(Exception):
     pass
 
 
 @dataclass
 class GlobalLoggingConfig:
+    setup: bool = False
     program_name: str = field(
         default_factory=lambda: os.path.basename(inspect.stack()[-1][1])
     )
     _unit_tests_mode: bool = (
         os.environ.get("STLOG_UNIT_TESTS_MODE", "0").lower() in TRUE_VALUES
     )
 
@@ -62,35 +64,37 @@
     "process",
     "processName",
     "relativeCreated",
     "stack_info",
     "thread",
     "threadName",
     "extra",  # specific to stlog
+    "extras",  # specific to stlog
+    STLOG_EXTRA_KEY,  # specific to stlog
     "rich_escaped_message",  # specific to stlog
     "rich_escaped_extras",  # specific to stlog
     "rich_level_style",  # specific to stlog
 )
 
 
 def check_json_types_or_raise(to_check: Any) -> None:
     if to_check is None:
         return
     if not isinstance(to_check, (dict, list, bool, str, int, float, bool)):
-        raise StLogError(
+        raise StlogError(
             "to_check should be a dict/list/bool/str/int/float/bool/None, found %s"
             % type(to_check)
         )
     if isinstance(to_check, list):
         for item in to_check:
             check_json_types_or_raise(item)
     elif isinstance(to_check, dict):
         for key, value in to_check.items():
             if not isinstance(key, str):
-                raise StLogError("dict keys should be str, found %s" % type(key))
+                raise StlogError("dict keys should be str, found %s" % type(key))
             check_json_types_or_raise(value)
 
 
 # Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
 def logfmt_format_string(value: str) -> str:
     needs_dquote_escaping = '"' in value
     needs_newline_escaping = "\n" in value
@@ -111,36 +115,14 @@
     elif isinstance(value, bool):
         return "true" if value else "false"
     elif isinstance(value, numbers.Number):
         return str(value)
     return logfmt_format_string(str(value))
 
 
-# Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
-def logfmt_format(kvs: dict[str, Any], ignore_compound_types: bool = True) -> str:
-    return " ".join(
-        [
-            f"{key}={logfmt_format_value(value)}"
-            for key, value in kvs.items()
-            if not ignore_compound_types or (not isinstance(value, (dict, list, set)))
-        ]
-    )
-
-
-# Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
-def rich_logfmt_format(kvs: dict[str, Any], ignore_compound_types: bool = True) -> str:
-    return " ".join(
-        [
-            f"[repr.attrib_name]{key}[/repr.attrib_name][repr.attrib_equal]=[/repr.attrib_equal][repr.attrib_value]{logfmt_format_value(value)}[/repr.attrib_value]"
-            for key, value in kvs.items()
-            if not ignore_compound_types or (not isinstance(value, (dict, list, set)))
-        ]
-    )
-
-
 def _get_env_json_context() -> dict[str, Any]:
     env_key = "STLOG_ENV_JSON_CONTEXT"
     env_context = os.environ.get(env_key, None)
     if env_context is not None:
         try:
             return json.loads(env_context)
         except Exception:
@@ -165,19 +147,19 @@
 
 def get_env_context() -> dict[str, Any]:
     if check_env_true("STLOG_IGNORE_ENV_CONTEXT", False):
         return {}
     env_context = {**_get_env_context(), **_get_env_json_context()}
     for key in env_context.keys():
         if key in RESERVED_ATTRS:
-            raise StLogError("key: %s is not allowed (reserved key)", key)
+            raise StlogError("key: %s is not allowed (reserved key)", key)
         if not isinstance(key, str):
-            raise StLogError("key: %s must be str", key)
+            raise StlogError("key: %s must be str", key)
         if not key.isidentifier():
-            raise StLogError(
+            raise StlogError(
                 "key: %s not allowed (must be a valid python identifier)", key
             )
     return env_context
 
 
 def check_true(value: str | None, default: bool = False) -> bool:
     if value is None:
@@ -239,7 +221,40 @@
     def escape_backslashes(match: Match[str]) -> str:
         """Called by re.sub replace matches."""
         backslashes, text = match.groups()
         return f"{backslashes}{backslashes}\\{text}"
 
     markup = _escape(escape_backslashes, markup)
     return markup
+
+
+# Adapted from https://github.com/madzak/python-json-logger/blob/master/src/pythonjsonlogger/jsonlogger.py
+def parse_format(fmt: str | None, style: str) -> list[str]:
+    """
+    Parses format string looking for substitutions
+
+    This method is responsible for returning a list of fields (as strings)
+    to include in all log messages.
+    """
+    if not fmt:
+        return []
+    if style == "$":
+        formatter_style_pattern = re.compile(r"\$\{(.+?)\}", re.IGNORECASE)
+    elif style == "{":
+        formatter_style_pattern = re.compile(r"\{(.+?)\}", re.IGNORECASE)
+    elif style == "%":
+        formatter_style_pattern = re.compile(r"%\((.+?)\)", re.IGNORECASE)
+    else:
+        raise ValueError("Unsupported style: %s" % style)
+    return formatter_style_pattern.findall(fmt)
+
+
+def format_string(fmt: str | None, style: str, record_dict: dict[str, Any]) -> str:
+    if not fmt:
+        return ""
+    if style == "$":
+        return Template(fmt).substitute(**record_dict)
+    elif style == "{":
+        return fmt.format(**record_dict)
+    elif style == "%":
+        return fmt % record_dict
+    raise StlogError("Invalid style: %s" % style)
```

### Comparing `stlog-0.0.7/stlog/context.py` & `stlog-0.0.8/stlog/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 from contextlib import contextmanager
 from contextvars import ContextVar, Token
 from typing import Any, Mapping
 
 from stlog.base import (
     RESERVED_ATTRS,
-    StLogError,
+    StlogError,
     check_json_types_or_raise,
     get_env_context,
 )
 
 ENV_CONTEXT = get_env_context()
 _LOGGING_CONTEXT_VAR: ContextVar = ContextVar(
     "stlog_logging_context", default=ENV_CONTEXT
@@ -33,15 +33,15 @@
         """Reset the execution log context."""
         _LOGGING_CONTEXT_VAR.set(ENV_CONTEXT)
 
     @classmethod
     def _add(cls, **kwargs: Any) -> Token:
         for key in kwargs.keys():
             if key in RESERVED_ATTRS:
-                raise StLogError("key: %s is not allowed (reserved key)" % key)
+                raise StlogError("key: %s is not allowed (reserved key)" % key)
         for val in kwargs.values():
             check_json_types_or_raise(val)
         new_context = _LOGGING_CONTEXT_VAR.get()
         # we create a new dict here as set() does a shallow copy
         return _LOGGING_CONTEXT_VAR.set(copy.deepcopy({**new_context, **kwargs}))
 
     @classmethod
```

### Comparing `stlog-0.0.7/stlog/formatter.py` & `stlog-0.0.8/stlog/formatter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,143 @@
 from __future__ import annotations
 
 import fnmatch
 import json
 import logging
 import re
 import time
-from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Callable, Sequence
 
 from stlog.base import (
     GLOBAL_LOGGING_CONFIG,
     STLOG_EXTRA_KEY,
-    check_env_true,
-    logfmt_format,
-    rich_logfmt_format,
+    format_string,
+    logfmt_format_value,
+    parse_format,
     rich_markup_escape,
 )
+from stlog.kvformatter import (
+    JsonKVFormatter,
+    KVFormatter,
+    LogFmtKVFormatter,
+    _truncate_serialize,
+    _truncate_str,
+)
 
 DEFAULT_STLOG_HUMAN_FORMAT = "{asctime} {name} [{levelname:^10s}] {message}{extras}"
 DEFAULT_STLOG_RICH_HUMAN_FORMAT = ":arrow_forward: [log.time]{asctime}[/log.time] {name} [{rich_level_style}]{levelname:^8s}[/{rich_level_style}] [bold]{rich_escaped_message}[/bold]{extras}"
-DEFAULT_STLOG_DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
-STLOG_DEFAULT_LOGFMT_IGNORE_COMPOUND_TYPES = check_env_true(
-    "STLOG_LOGFMT_IGNORE_COMPOUND_TYPES", True
+DEFAULT_STLOG_LOGFMT_FORMAT = (
+    "time={asctime} logger={name} level={levelname} message={message}{extras}"
 )
-
-
-def _truncate_str(str_value: str, limit: int = 0) -> str:
-    if limit <= 0:
-        return str_value
-    if len(str_value) > limit:
-        return str_value[0 : (limit - 3)] + "..."
-    return str_value
-
-
-def _truncate_serialize(value: Any, limit: int = 0) -> str:
-    try:
-        serialized = str(value)
-    except Exception:
-        serialized = "[can't serialize]"
-    return _truncate_str(serialized, limit)
+DEFAULT_STLOG_JSON_FORMAT = """
+{{
+    "time": {asctime},
+    "logger": {name},
+    "level": {levelname},
+    "message": {message},
+    "source": {{
+        "path": {pathname},
+        "lineno": {lineno},
+        "module": {module},
+        "funcName": {funcName},
+        "process": {process},
+        "processName": {processName},
+        "thread": {thread},
+        "threadName": {threadName}
+    }}
+}}
+"""
+DEFAULT_STLOG_DATE_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 
 def _unit_tests_converter(val: float | None) -> time.struct_time:
     # always the same value
     return time.gmtime(1680101317)
 
 
 @dataclass
 class Formatter(logging.Formatter):
     """Abstract base class for `stlog` formatters.
 
     Attributes:
         fmt: the default format for the formatter.
         datefmt: the format to use for `{asctime}` placeholder.
-        style: FIXME
+        style: can be '%', '{' or '$' to select how the format string will be merged with its data
+            (see https://docs.python.org/3/library/logging.html#logging.Formatter for details)
         include_extras_keys_fnmatchs: fnmatch patterns list for including keys in `{extra}` placeholder.
         exclude_extras_keys_fnmatchs: fnmatch patterns list for excluding keys in `{extra}` placeholder.
         extra_key_rename_fn: callable which takes a key name and return a renamed key to use
             (or None to ignore the key/value).
         extra_key_max_length: maximum size of extra keys to be included in `{extra}` placeholder
             (after this limit, the value will be truncated and ... will be added at the end, 0 means "no limit").
         converter: time converter function (use `time.gmtime` (default) for UTC date/times, use `time.time`
             for local date/times), if you change the default, please change also `datefmt` keyword.
+        kv_formatter: key values special formatter for formatting `{extras}`
+            placeholder.
+        include_reserved_attrs_in_extras: automatical include some reserved
+            logrecord attributes in "extras" (example: `["process", "thread"]`).
 
     """
 
-    fmt: str | None = DEFAULT_STLOG_HUMAN_FORMAT
+    fmt: str | None = None
     datefmt: str | None = DEFAULT_STLOG_DATE_FORMAT
     style: str = "{"
-    include_extras_keys_fnmatchs: Sequence[str] = ("*",)
-    exclude_extras_keys_fnmatchs: Sequence[str] = ("_*",)
+    include_extras_keys_fnmatchs: Sequence[str] | None = None
+    exclude_extras_keys_fnmatchs: Sequence[str] | None = None
     extra_key_rename_fn: Callable[[str], str | None] | None = None
     extra_key_max_length: int = 32
     converter: Callable[[float | None], time.struct_time] = time.gmtime
+    kv_formatter: KVFormatter | None = None
+    include_reserved_attrs_in_extras: Sequence[str] = field(default_factory=list)
+    _placeholders_in_fmt: list[str] | None = field(
+        init=False, default=None, repr=False, compare=False
+    )
+
+    @property
+    def placeholders_in_fmt(self) -> list[str]:
+        if self._placeholders_in_fmt is None:
+            self._placeholders_in_fmt = parse_format(self.fmt, self.style)
+        return self._placeholders_in_fmt
+
+    def _make_extras_string(
+        self,
+        record: logging.LogRecord,
+    ) -> str:
+        if self.kv_formatter is None:
+            return ""
+        if not hasattr(record, STLOG_EXTRA_KEY):
+            return ""
+        kvs: dict[str, Any] = {}
+        for k in list(getattr(record, STLOG_EXTRA_KEY)) + list(
+            self.include_reserved_attrs_in_extras
+        ):
+            key = self._make_extra_key_name(k)
+            if key:
+                kvs[key] = getattr(record, k)
+        return self.kv_formatter.format(kvs)
 
     def __post_init__(self):
         super().__init__(  # explicit call because logging.Formatter is not a dataclass
             fmt=self.fmt, datefmt=self.datefmt, style=self.style  # type: ignore
         )
         self.include_extra_keys_patterns: list[re.Pattern] = [
-            re.compile(fnmatch.translate(x)) for x in self.include_extras_keys_fnmatchs
-        ]
-        self.exclude_extra_keys_patterns: list[re.Pattern] = [
-            re.compile(fnmatch.translate(x)) for x in self.exclude_extras_keys_fnmatchs
-        ]
+            re.compile(fnmatch.translate("*"))
+        ]  # all by default
+        self.exclude_extra_keys_patterns: list[re.Pattern] = []  # empty by default
+        if self.include_extras_keys_fnmatchs is not None:
+            self.include_extra_keys_patterns = [
+                re.compile(fnmatch.translate(x))
+                for x in self.include_extras_keys_fnmatchs
+            ]
+        if self.exclude_extras_keys_fnmatchs is not None:
+            self.exclude_extra_keys_patterns = [
+                re.compile(fnmatch.translate(x))
+                for x in self.exclude_extras_keys_fnmatchs
+            ]
         if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
             self.converter = _unit_tests_converter
 
     def _make_extra_key_name(self, extra_key: str) -> str | None:
         new_extra_key: str | None = extra_key
         if self.extra_key_rename_fn is not None:
             new_extra_key = (self.extra_key_rename_fn)(extra_key)
@@ -103,115 +152,31 @@
         for pattern in self.exclude_extra_keys_patterns:
             if re.match(pattern, new_extra_key):
                 return None
         return _truncate_str(new_extra_key, self.extra_key_max_length)
 
     def format(self, record: logging.LogRecord) -> str:
         if GLOBAL_LOGGING_CONFIG._unit_tests_mode:
+            # FIXME: it would be better as a Filter, wouldn't be?
             # fix some fields in record to get always the same values
             record.filename = "filename.py"
             record.pathname = "/path/filename.py"
             record.thread = 12345
             record.process = 6789
             record.processName = "MainProcess"
             record.threadName = "MainThread"
         return super().format(record)
 
 
-@dataclass
-class KVFormatter(ABC):
-    """Abstract base class to format extras key-values."""
-
-    @abstractmethod
-    def format(self, kvs: dict[str, Any]) -> str:
-        pass
-
-
-# Adapted from https://github.com/Mergifyio/daiquiri/blob/main/daiquiri/formatter.py
-@dataclass
-class TemplateKVFormatter(KVFormatter):
-    """Class to format extra key-values as a string with templates.
-
-    Extra keywords are merged into a `{extra}` placeholder.
-
-    Example::
-
-        {foo="bar", foo2=123}
-
-    will be formatted as:
-
-        [foo: bar] [foo2: 123]
-
-    Attributes:
-        extras_template: the template to format a key/value:
-            `{0}` placeholder is the key, `{1}` is the value.
-        extras_separator: the separator between multiple key/values.
-        extras_prefix: the prefix before key/value parts.
-        extras_suffix: the suffix after key/values parts.
-        extra_value_max_serialized_length: maximum size of extra values to be included in `{extra}` placeholder
-            (after this limit, the value will be truncated and ... will be added at the end, 0 means "no limit").
-
-    """
-
-    extras_template: str = "[{0}: {1}]"
-    extras_separator: str = " "
-    extras_prefix: str = " "
-    extras_suffix: str = ""
-    extra_value_max_serialized_length: int = 40
-
-    def format(self, kvs: dict[str, Any]) -> str:
-        res: str = ""
-        tmp: list[str] = []
-        for k, v in sorted(kvs.items(), key=lambda x: x[0]):
-            serialized = _truncate_serialize(v, self.extra_value_max_serialized_length)
-            if serialized is None:
-                continue
-            tmp.append(self.extras_template.format(k, serialized))
-        res = self.extras_separator.join(tmp)
-        if res != "":
-            res = self.extras_prefix + res + self.extras_suffix
-        return res
-
-
-# Adapted from https://github.com/jteppinette/python-logfmter/blob/main/logfmter/formatter.py
-@dataclass
-class LogFmtKVFormatter(KVFormatter):
-    ignore_compound_types: bool = STLOG_DEFAULT_LOGFMT_IGNORE_COMPOUND_TYPES
-    extras_prefix: str = " {"
-    extras_suffix: str = "}"
-
-    def _format(self, kvs: dict[str, Any]) -> str:
-        return logfmt_format(
-            dict(sorted(kvs.items())), ignore_compound_types=self.ignore_compound_types
-        )
-
-    def format(self, kvs: dict[str, Any]) -> str:
-        tmp = self._format(kvs)
-        if not tmp:
-            return ""
-        return self.extras_prefix + tmp + self.extras_suffix
-
-
-@dataclass
-class RichLogFmtKVFormatter(LogFmtKVFormatter):
-    extras_prefix: str = "\n    :arrow_right_hook: "
-    extras_suffix: str = ""
-
-    def _format(self, kvs: dict[str, Any]) -> str:
-        return rich_logfmt_format(
-            dict(sorted(kvs.items())), ignore_compound_types=self.ignore_compound_types
-        )
-
-
 # Adapted from https://github.com/Mergifyio/daiquiri/blob/main/daiquiri/formatter.py
 @dataclass
 class HumanFormatter(Formatter):
     """Formatter for a "human" output.
 
-    Extra keywords are merged into a `{extra}` placeholder by a `stlog.formatter.KVFormatter`.
+    Extra keywords are merged into a `{extra}` placeholder by a `stlog.kvformatter.KVFormatter`.
 
     If you use this placeholder on your `fmt`, any keywords
     passed to a logging call will be formatted into a "extras" string and
     included in a logging message.
 
     Example::
 
@@ -220,54 +185,52 @@
     will cause an "extras" string of::
 
         {foo=bar foo2=123}
 
     You can change the way the `{extra}` placeholder is formatted
     by providing a KVFormatter object.
 
-    Attributes:
-        include_reserved_attrs_in_extras: automatical include some reserved
-            logrecord attributes in "extras" (example: `["process", "thread"]`).
-        kvs_formatter: key values special formatter for formatting `{extra}`
-            placeholder.
-
     """
 
-    include_reserved_attrs_in_extras: Sequence[str] = field(default_factory=list)
-    kvs_formatter: KVFormatter = field(default_factory=LogFmtKVFormatter)
-
-    def _make_extras_string(self, record: logging.LogRecord) -> str:
-        if not hasattr(record, STLOG_EXTRA_KEY):
-            return ""
-        kvs: dict[str, Any] = {}
-        for k in list(getattr(record, STLOG_EXTRA_KEY)) + list(
-            self.include_reserved_attrs_in_extras
-        ):
-            key = self._make_extra_key_name(k)
-            if key:
-                kvs[key] = getattr(record, k)
-        return self.kvs_formatter.format(kvs)
+    def __post_init__(self):
+        if self.fmt is None:
+            self.fmt = DEFAULT_STLOG_HUMAN_FORMAT
+        if self.kv_formatter is None:
+            self.kv_formatter = LogFmtKVFormatter()
+        if self.exclude_extras_keys_fnmatchs is None:
+            self.exclude_extras_keys_fnmatchs = ("_*",)
+        super().__post_init__()
 
     def _add_extras(self, record: logging.LogRecord) -> None:
         record.extras = self._make_extras_string(record)
 
     def _remove_extras(self, record: logging.LogRecord) -> None:
         delattr(record, "extras")
 
     def format(self, record: logging.LogRecord) -> str:
-        self._add_extras(record)
+        if "extras" in self.placeholders_in_fmt:
+            self._add_extras(record)
         s = super().format(record)
-        self._remove_extras(record)
+        if "extras" in self.placeholders_in_fmt:
+            self._remove_extras(record)
         return s
 
 
 @dataclass
 class RichHumanFormatter(HumanFormatter):
-    fmt: str | None = DEFAULT_STLOG_RICH_HUMAN_FORMAT
-    kvs_formatter: KVFormatter = field(default_factory=RichLogFmtKVFormatter)
+    def __post_init__(self):
+        if self.kv_formatter is None:
+            self.kv_formatter = LogFmtKVFormatter(
+                prefix="\n    :arrow_right_hook: ",
+                suffix="",
+                template="[repr.attrib_name]{key}[/repr.attrib_name][repr.attrib_equal]=[/repr.attrib_equal][repr.attrib_value]{value}[/repr.attrib_value]",
+            )
+        if self.fmt is None:
+            self.fmt = DEFAULT_STLOG_RICH_HUMAN_FORMAT
+        super().__post_init__()
 
     def _add_extras(self, record: logging.LogRecord) -> None:
         super()._add_extras(record)
         record.rich_escaped_message = rich_markup_escape(record.getMessage())
         record.rich_escaped_extras = rich_markup_escape(record.extras)  # type: ignore
         level = record.levelname.lower()
         if level in ["notset", "debug", "info", "critical"]:
@@ -296,55 +259,83 @@
     """Simple "extra_key_rename" function to remove leading underscores."""
     if key.startswith("_"):
         return key[1:]
     return key
 
 
 @dataclass
+class LogFmtFormatter(Formatter):
+    def __post_init__(self):
+        if self.kv_formatter is None:
+            self.kv_formatter = LogFmtKVFormatter(prefix=" ", suffix="")
+        if self.fmt is None:
+            self.fmt = DEFAULT_STLOG_LOGFMT_FORMAT
+        super().__post_init__()
+
+    def format(self, record: logging.LogRecord) -> str:
+        record.message = record.getMessage()
+        if self.usesTime():
+            record.asctime = self.formatTime(record, self.datefmt)
+        record_dict: dict[str, Any] = {
+            k: logfmt_format_value(getattr(record, k))
+            for k in self.placeholders_in_fmt
+            if k != "extras"
+        }
+        if "extras" in self.placeholders_in_fmt:
+            record_dict["extras"] = self._make_extras_string(record)
+        return format_string(self.fmt, self.style, record_dict)
+
+
+@dataclass
 class JsonFormatter(Formatter):
     """Formatter for a JSON / parsing friendly output."""
 
     extra_key_max_length: int = 0
-    exclude_extras_keys_fnmatchs: Sequence[str] = field(default_factory=list)
-    extra_key_rename_fn: Callable[
-        [str], str | None
-    ] | None = json_formatter_default_extra_key_rename_fn
     indent: int | None = None
     sort_keys: bool = True
+    include_extras_in_key: str | None = None
+    exc_info_key: str | None = "exc_info"
+    stack_info_key: str | None = "stack_info"
+
+    def __post_init__(self):
+        if self.kv_formatter is None:
+            self.kv_formatter = JsonKVFormatter()
+        if self.fmt is None:
+            self.fmt = DEFAULT_STLOG_JSON_FORMAT
+        if self.extra_key_rename_fn is None:
+            self.extra_key_rename_fn = json_formatter_default_extra_key_rename_fn
+        super().__post_init__()
 
     def json_serialize(self, message_dict: dict[str, Any]) -> str:
         return json.dumps(
             message_dict,
             indent=self.indent,
             sort_keys=self.sort_keys,
             default=_truncate_serialize,
         )
 
     def format(self, record: logging.LogRecord) -> str:
-        message_dict: dict[str, Any] = {
-            "status": record.levelname.lower(),
-            "logger": {"name": record.name},
-            "source": {
-                "path": record.pathname,
-                "lineno": record.lineno,
-                "module": record.module,
-                "funcName": record.funcName,
-            },
-            "message": record.getMessage(),
-            "timestamp": self.formatTime(record, self.datefmt),
+        record.message = record.getMessage()
+        if self.usesTime():
+            record.asctime = self.formatTime(record, self.datefmt)
+        record_dict: dict[str, Any] = {
+            k: json.dumps(getattr(record, k))
+            for k in self.placeholders_in_fmt
+            if k != "extras"
         }
-        for k in ("process", "processName", "thread", "threadName"):
-            if getattr(record, k, None):
-                message_dict["source"][k] = getattr(record, k)
-        for k in getattr(record, STLOG_EXTRA_KEY, set()):
-            key = self._make_extra_key_name(k)
-            if not key:
-                continue
-            message_dict[key] = getattr(record, k)
-            message_dict["timestamp"] = self.formatTime(record, self.datefmt)
-        if record.exc_info:
-            message_dict["exc_info"] = self.formatException(record.exc_info)
-        elif record.exc_text:
-            message_dict["exc_info"] = record.exc_text
-        if record.stack_info:
-            message_dict["stack_info"] = self.formatStack(record.stack_info)
-        return self.json_serialize(message_dict)
+        s = format_string(self.fmt, self.style, record_dict)
+        obj = json.loads(s)
+        extras_obj = json.loads(self._make_extras_string(record))
+        if self.include_extras_in_key:
+            obj[self.include_extras_in_key] = extras_obj
+        else:
+            for key, value in extras_obj.items():
+                if key not in obj:
+                    obj[key] = value
+        if self.exc_info_key:
+            if record.exc_info:
+                obj[self.exc_info_key] = self.formatException(record.exc_info)
+            elif record.exc_text:
+                obj[self.exc_info_key] = record.exc_text
+        if self.stack_info_key and record.stack_info:
+            obj[self.stack_info_key] = self.formatStack(record.stack_info)
+        return self.json_serialize(obj)
```

### Comparing `stlog-0.0.7/stlog/handler.py` & `stlog-0.0.8/stlog/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 
 from stlog.base import (
     RESERVED_ATTRS,
     STLOG_EXTRA_KEY,
-    StLogError,
+    StlogError,
     rich_dump_exception_on_console,
 )
 from stlog.context import LogContext
 
 
 class ContextReinjectHandlerWrapper(logging.Handler):
     """Logging Handler (built as a wrapper/adapter of another handler) to reinject `stlog.LogContext`
@@ -55,15 +55,15 @@
 class CustomRichHandler(logging.Handler):
     def __init__(self, console, level: int = logging.NOTSET, **kwargs):
         self.console = console
         super().__init__(level=level)
 
     def emit(self, record: logging.LogRecord):
         if self.formatter is None:
-            raise StLogError("no formatted set")
+            raise StlogError("no formatted set")
         self.console.print(self.formatter.format(record))
         if record.exc_info:
             exc_type, exc_value, exc_traceback = record.exc_info
             assert exc_type is not None
             assert exc_value is not None
             rich_dump_exception_on_console(
                 self.console, exc_type, exc_value, exc_traceback
```

### Comparing `stlog-0.0.7/stlog/output.py` & `stlog-0.0.8/stlog/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import logging.handlers
 import os
 import sys
 import typing
 from dataclasses import dataclass, field
 
-from stlog.base import StLogError
+from stlog.base import StlogError
 from stlog.formatter import (
     HumanFormatter,
     RichHumanFormatter,
 )
 from stlog.handler import CustomRichHandler
 
 RICH_INSTALLED: bool = False
@@ -69,15 +69,15 @@
 
     def get_handler(self) -> logging.Handler:
         """Get the configured Python logging Handler."""
         return self._handler
 
     def get_formatter_or_raise(self) -> logging.Formatter:
         if self.formatter is None:
-            raise StLogError("formatter is not set")
+            raise StlogError("formatter is not set")
         return self.formatter
 
 
 @dataclass
 class StreamOutput(Output):
     """Represent an output to a stream (stdout, stderr...).
 
@@ -99,29 +99,30 @@
 @dataclass
 class RichStreamOutput(StreamOutput):
     force_terminal: bool = True
     console: typing.Any = None
 
     def __post_init__(self):
         if not RICH_INSTALLED:
-            raise StLogError("Rich is not installed and RichStreamOutput is specified")
+            raise StlogError("Rich is not installed and RichStreamOutput is specified")
         if self.formatter is None:
             self.formatter = RichHumanFormatter()
         if self.console is None:
             self.console = Console(
                 file=self.stream,
                 force_terminal=True if self.force_terminal else None,
                 highlight=False,
             )
         self.set_handler(CustomRichHandler(console=self.console))
 
 
 def make_stream_or_rich_stream_output(
     stream: typing.TextIO = sys.stderr,
     use_rich: bool | None = DEFAULT_USE_RICH,
+    **kwargs,
 ) -> StreamOutput:
     """Create automatically a `stlog.output.RichStreamOutput` or a (classic)`stlog.output.StreamOutput`.
 
     To get a `stlog.output.RichStreamOutput`, following conditions must be true:
 
     - `rich` library must be installed and available in python path
     - `use_rich` parameter must be `True` (forced mode) or `None` (automatic mode)
@@ -136,22 +137,25 @@
 
     Attributes:
         stream: the stream to use (`typing.TextIO`), default to `sys.stderr`.
         use_rich: if None, use [rich output](https://github.com/Textualize/rich/blob/master/README.md) if possible
         (rich installed and supported tty), if True/False force the usage (or not).
 
     """
+    for key in ("formatter", "force_terminal"):
+        if key in kwargs:
+            raise StlogError(f"you can't use {key} in kwargs for this function")
     _use_rich: bool = False
     if use_rich is not None:
         # manual mode
         _use_rich = use_rich
     else:
         # automatic mode
         if RICH_INSTALLED:
             c = Console(file=stream)
             _use_rich = c.is_terminal
     if _use_rich:
         return RichStreamOutput(
-            stream=stream, force_terminal=True, formatter=RichHumanFormatter()
+            stream=stream, force_terminal=True, formatter=RichHumanFormatter(), **kwargs
         )
     else:
-        return StreamOutput(stream=stream)
+        return StreamOutput(stream=stream, **kwargs)
```

### Comparing `stlog-0.0.7/PKG-INFO` & `stlog-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlog
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 License: MIT
 Author: Fabien MARTY
 Author-email: fabien.marty@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 
-<!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
-     and execute 'poetry run poe readme' to regenerate this README.md file -->
+ <!-- WARNING: generated from README.md.j2, do not modify this file manually but modify README.md.j2 instead
+      and execute 'poetry run invoke readme' to regenerate this README.md file -->
 
-# stlog
+ # stlog
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fabien-marty/stlog/lint.yaml)](https://github.com/fabien-marty/stlog/actions/workflows/lint.yaml)
 [![Codecov](https://img.shields.io/codecov/c/github/fabien-marty/stlog)](https://app.codecov.io/github/fabien-marty/stlog)
 [![pypi badge](https://img.shields.io/pypi/v/stlog?color=brightgreen)](https://pypi.org/project/stlog/)
 
 [Full documentation](https://fabien-marty.github.io/stlog/)
 
@@ -84,14 +84,38 @@
 
 ### Installation
 
 ```
 pip install stlog
 ```
 
+### Very minimal usage
+
+```python
+import stlog
+
+stlog.info("It works", foo="bar", x=123)
+stlog.critical("Houston, we have a problem!")
+ 
+```
+
+Output (without `rich` library installed):
+
+```
+2023-03-29T14:48:37Z root [   INFO   ] It works {foo=bar x=123}
+2023-03-29T14:48:37Z root [ CRITICAL ] Houston, we have a problem!
+ 
+```
+
+Output (with `rich` library installed):
+
+![rich output](docs/python/qs0.svg)
+ 
+
+
 ### Basic usage
 
 ```python
 from stlog import getLogger, setup
 
 # Set the logging default configuration (human output on stderr)
 setup()
@@ -195,53 +219,49 @@
 JSON ouput (on `stdout`) for machines:
 
 ```json
 {
     "client_id": 456,
     "foo": "bar",
     "http_method": "GET",
-    "logger": {
-        "name": "__main__"
-    },
+    "level": "INFO",
+    "logger": "__main__",
     "message": "It works",
     "request_id": "4c2383f5",
     "source": {
         "funcName": "<module>",
         "lineno": 21,
         "module": "qs3",
         "path": "/path/filename.py",
         "process": 6789,
         "processName": "MainProcess",
         "thread": 12345,
         "threadName": "MainThread"
     },
-    "status": "info",
-    "timestamp": "2023-03-29T14:48:37Z",
+    "time": "2023-03-29T14:48:37Z",
     "x": 123
 }
 {
     "client_id": 456,
     "http_method": "GET",
-    "logger": {
-        "name": "__main__"
-    },
+    "level": "CRITICAL",
+    "logger": "__main__",
     "message": "Houston, we have a problem!",
     "request_id": "4c2383f5",
     "source": {
         "funcName": "<module>",
         "lineno": 22,
         "module": "qs3",
         "path": "/path/filename.py",
         "process": 6789,
         "processName": "MainProcess",
         "thread": 12345,
         "threadName": "MainThread"
     },
-    "status": "critical",
-    "timestamp": "2023-03-29T14:48:37Z"
+    "time": "2023-03-29T14:48:37Z"
 }
  
 ```
 
 <!--quickstart-end-->
 
 ## Roadmap
```

