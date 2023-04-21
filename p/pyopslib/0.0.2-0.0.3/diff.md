# Comparing `tmp/pyopslib-0.0.2.tar.gz` & `tmp/pyopslib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopslib-0.0.2.tar", max compression
+gzip compressed data, was "pyopslib-0.0.3.tar", max compression
```

## Comparing `pyopslib-0.0.2.tar` & `pyopslib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0       88 2023-03-21 11:56:08.639588 pyopslib-0.0.2/Readme.md
--rw-r--r--   0        0        0     4273 2023-03-22 09:53:45.629147 pyopslib-0.0.2/opslib/ansible.py
--rw-r--r--   0        0        0     2488 2023-03-22 13:04:39.870238 pyopslib-0.0.2/opslib/cli.py
--rw-r--r--   0        0        0      826 2023-03-22 07:46:12.783948 pyopslib-0.0.2/opslib/lazy.py
--rw-r--r--   0        0        0     1588 2023-03-14 14:12:04.364843 pyopslib-0.0.2/opslib/local.py
--rw-r--r--   0        0        0     4891 2023-03-22 09:52:30.379178 pyopslib-0.0.2/opslib/operations.py
--rw-r--r--   0        0        0     5954 2023-03-22 09:53:05.045481 pyopslib-0.0.2/opslib/places.py
--rw-r--r--   0        0        0     1739 2023-03-21 15:45:23.582131 pyopslib-0.0.2/opslib/props.py
--rw-r--r--   0        0        0      747 2023-03-12 19:49:46.914247 pyopslib-0.0.2/opslib/results.py
--rw-r--r--   0        0        0     2326 2023-03-22 13:04:39.871104 pyopslib-0.0.2/opslib/state.py
--rw-r--r--   0        0        0     4755 2023-03-22 10:58:56.683244 pyopslib-0.0.2/opslib/terraform.py
--rw-r--r--   0        0        0     2043 2023-03-22 13:04:39.872430 pyopslib-0.0.2/opslib/things.py
--rw-r--r--   0        0        0     1588 2023-03-16 15:30:17.600169 pyopslib-0.0.2/opslib/uptodate.py
--rw-r--r--   0        0        0     1111 2023-03-12 19:51:22.597610 pyopslib-0.0.2/opslib/utils.py
--rw-r--r--   0        0        0      749 2023-03-22 13:08:46.842842 pyopslib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 pyopslib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2853 2023-03-24 12:40:51.434593 pyopslib-0.0.3/Readme.md
+-rw-r--r--   0        0        0     6888 2023-03-31 11:24:46.441580 pyopslib-0.0.3/opslib/ansible.py
+-rw-r--r--   0        0        0      648 2023-03-25 14:45:14.773127 pyopslib-0.0.3/opslib/callbacks.py
+-rw-r--r--   0        0        0     4258 2023-04-10 17:49:10.777498 pyopslib-0.0.3/opslib/cli.py
+-rw-r--r--   0        0        0     3568 2023-04-06 17:36:30.708665 pyopslib-0.0.3/opslib/components.py
+-rw-r--r--   0        0        0     1940 2023-04-21 12:01:21.910079 pyopslib-0.0.3/opslib/extras/http.py
+-rw-r--r--   0        0        0     3285 2023-04-12 19:01:51.934605 pyopslib-0.0.3/opslib/extras/restic.py
+-rw-r--r--   0        0        0     3464 2023-03-26 14:10:06.150347 pyopslib-0.0.3/opslib/extras/systemd.py
+-rw-r--r--   0        0        0     3511 2023-04-02 17:35:28.524145 pyopslib-0.0.3/opslib/extras/tailscale.py
+-rw-r--r--   0        0        0     1733 2023-04-09 18:41:39.319970 pyopslib-0.0.3/opslib/lazy.py
+-rw-r--r--   0        0        0     3279 2023-03-31 11:24:46.442621 pyopslib-0.0.3/opslib/local.py
+-rw-r--r--   0        0        0     6123 2023-03-31 11:24:46.442798 pyopslib-0.0.3/opslib/operations.py
+-rw-r--r--   0        0        0    11578 2023-03-31 11:24:46.443089 pyopslib-0.0.3/opslib/places.py
+-rw-r--r--   0        0        0     2567 2023-04-05 17:25:24.501390 pyopslib-0.0.3/opslib/props.py
+-rw-r--r--   0        0        0     1350 2023-03-31 11:24:46.443434 pyopslib-0.0.3/opslib/results.py
+-rw-r--r--   0        0        0     2477 2023-03-29 19:10:27.025773 pyopslib-0.0.3/opslib/state.py
+-rw-r--r--   0        0        0     9133 2023-04-21 12:15:18.028724 pyopslib-0.0.3/opslib/terraform.py
+-rw-r--r--   0        0        0     1612 2023-04-20 18:49:48.015650 pyopslib-0.0.3/opslib/uptodate.py
+-rw-r--r--   0        0        0     1111 2023-03-12 19:51:22.597610 pyopslib-0.0.3/opslib/utils.py
+-rw-r--r--   0        0        0      770 2023-04-21 12:21:21.316646 pyopslib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 pyopslib-0.0.3/PKG-INFO
```

### Comparing `pyopslib-0.0.2/opslib/state.py` & `pyopslib-0.0.3/opslib/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,60 +3,66 @@
 import sys
 from functools import cached_property
 from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
 
-class ThingStateDirectory:
+class ComponentStateDirectory:
     def __init__(self, meta):
         self.meta = meta
 
         if meta.parent is None:
-            self._prefix = meta.thing.get_state_directory()
+            self._prefix = meta.component.get_state_directory()
 
         else:
             self._prefix = meta.parent._meta.statedir._prefix / meta.name
 
         self._path = self._prefix / "_statedir"
 
     def init(self):
+        changed = False
+
         if not self._prefix.exists():
-            logger.debug("ThingState init %s", self._prefix)
+            logger.debug("ComponentState init %s", self._prefix)
             self._prefix.mkdir(mode=0o700)
+            changed = True
 
         if not self._path.exists():
-            logger.debug("ThingState init %s", self._path)
+            logger.debug("ComponentState init %s", self._path)
             self._path.mkdir(mode=0o700)
+            changed = True
+
+        return changed
 
     @cached_property
     def path(self):
         assert (
             self._path.is_dir()
-        ), f"State directory for {self.meta.thing!r} missing, please run `init`."
+        ), f"State directory for {self.meta.component!r} missing, please run `init`."
         return self._path
 
 
 class StateDirectory:
     def __get__(self, obj, objtype=None):
-        return ThingStateDirectory(obj)
+        return ComponentStateDirectory(obj)
 
 
 def default_state_directory(stack):
     module = sys.modules[stack.__module__]
     return Path(module.__file__).parent / ".opslib"
 
 
-class ThingJsonState:
-    def __init__(self, thing):
-        self.thing = thing
+class ComponentJsonState:
+    def __init__(self, component):
+        self.component = component
 
     @cached_property
     def _path(self):
-        return self.thing._meta.statedir.path / "state.json"
+        return self.component._meta.statedir.path / "state.json"
 
     @cached_property
     def _data(self):
         try:
             with self._path.open() as f:
                 return json.load(f)
 
@@ -88,8 +94,8 @@
 
     def __iter__(self):
         return iter(self._data.items())
 
 
 class JsonState:
     def __get__(self, obj, objtype=None):
-        return ThingJsonState(obj)
+        return ComponentJsonState(obj)
```

### Comparing `pyopslib-0.0.2/opslib/uptodate.py` & `pyopslib-0.0.3/opslib/uptodate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import hashlib
 import json
 from functools import partial, wraps
 
 from .results import Result
 
 
-class ThingUpToDate:
-    def __init__(self, thing, get_snapshot):
-        self.thing = thing
+class ComponentUpToDate:
+    def __init__(self, component, get_snapshot):
+        self.component = component
         self.get_snapshot = get_snapshot
 
     @property
     def _path(self):
-        return self.thing._meta.statedir.path / "uptodate.json"
+        return self.component._meta.statedir.path / "uptodate.json"
 
     def _get_hash(self):
         snapshot = self.get_snapshot()
         buffer = json.dumps(snapshot, sort_keys=True).encode("utf8")
         return hashlib.sha256(buffer).hexdigest()
 
     def set(self, uptodate):
@@ -30,15 +30,15 @@
             hash = None
 
         return hash == self._get_hash() if hash else False
 
 
 class UpToDate:
     def __get__(self, obj, objtype=None):
-        return ThingUpToDate(obj, partial(self.snapshot_func, obj))
+        return ComponentUpToDate(obj, partial(self.snapshot_func, obj))
 
     def snapshot(self, func):
         self.snapshot_func = func
         return func
 
     def refresh(self, func):
         @wraps(func)
```

### Comparing `pyopslib-0.0.2/opslib/utils.py` & `pyopslib-0.0.3/opslib/utils.py`

 * *Files identical despite different names*

### Comparing `pyopslib-0.0.2/pyproject.toml` & `pyopslib-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "pyopslib"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Pythonic toolkit to manage infrastructure."
 authors = ["Alex Morega <alex@grep.ro>"]
 license = "MIT"
 readme = "Readme.md"
 packages = [
   { include = "opslib" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beartype = "^0.12.0"
 click = "^8.1.3"
 ansible-core = "^2.14.3"
+requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-black-ng = "^0.4.1"
 pytest-isort = "^3.1.0"
 sphinx = "^6.1.3"
 sphinx-autobuild = "^2021.3.14"
```

