# Comparing `tmp/omnicloud_airport-0.0.1rc7.tar.gz` & `tmp/omnicloud_airport-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnicloud_airport-0.0.1rc7.tar", max compression
+gzip compressed data, was "omnicloud_airport-0.0.2.dev1.tar", max compression
```

## Comparing `omnicloud_airport-0.0.1rc7.tar` & `omnicloud_airport-0.0.2.dev1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-04-01 21:33:27.424779 omnicloud_airport-0.0.1rc7/LICENSE
--rw-r--r--   0        0        0     2812 2023-04-01 21:33:27.424779 omnicloud_airport-0.0.1rc7/README.md
--rw-r--r--   0        0        0      125 2023-04-01 21:33:27.424779 omnicloud_airport-0.0.1rc7/omnicloud/airport/__init__.py
--rw-r--r--   0        0        0       38 2023-04-01 21:33:27.424779 omnicloud_airport-0.0.1rc7/omnicloud/airport/abc/__init__.py
--rw-r--r--   0        0        0     4655 2023-04-01 21:33:27.424779 omnicloud_airport-0.0.1rc7/omnicloud/airport/abc/_terminal.py
--rw-r--r--   0        0        0     2220 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/__init__.py
--rw-r--r--   0        0        0      283 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/_dict/__init__.py
--rw-r--r--   0        0        0       27 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/_dict/_local/__init__.py
--rw-r--r--   0        0        0      987 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/_dict/_local/json.py
--rw-r--r--   0        0        0       76 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/__init__.py
--rw-r--r--   0        0        0     1661 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/dict.py
--rw-r--r--   0        0        0      830 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/files.py
--rw-r--r--   0        0        0      845 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/json.py
--rw-r--r--   0        0        0     2208 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/pkg.py
--rw-r--r--   0        0        0      540 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/type.py
--rw-r--r--   0        0        0     1361 2023-04-01 21:33:27.428780 omnicloud_airport-0.0.1rc7/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 omnicloud_airport-0.0.1rc7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/LICENSE
+-rw-r--r--   0        0        0     2812 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/README.md
+-rw-r--r--   0        0        0      125 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/__init__.py
+-rw-r--r--   0        0        0       38 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/abc/__init__.py
+-rw-r--r--   0        0        0     4655 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/abc/_terminal.py
+-rw-r--r--   0        0        0     2286 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/_dict/__init__.py
+-rw-r--r--   0        0        0       56 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/_dict/_local/__init__.py
+-rw-r--r--   0        0        0      987 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/_dict/_local/json.py
+-rw-r--r--   0        0        0     1244 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/_dict/_local/yaml.py
+-rw-r--r--   0        0        0       76 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/__init__.py
+-rw-r--r--   0        0        0     1661 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/dict.py
+-rw-r--r--   0        0        0      867 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/files.py
+-rw-r--r--   0        0        0      845 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/json.py
+-rw-r--r--   0        0        0     2208 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/pkg.py
+-rw-r--r--   0        0        0      540 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/type.py
+-rw-r--r--   0        0        0     1341 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/yaml.py
+-rw-r--r--   0        0        0     1378 2023-04-21 12:02:17.429016 omnicloud_airport-0.0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     3806 1970-01-01 00:00:00.000000 omnicloud_airport-0.0.2.dev1/PKG-INFO
```

### Comparing `omnicloud_airport-0.0.1rc7/LICENSE` & `omnicloud_airport-0.0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/README.md` & `omnicloud_airport-0.0.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/abc/_terminal.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/abc/_terminal.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/__init__.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path as _path
 from os import scandir as _scandir
 from sys import modules as _modules
 
 from ..abc import Building as _Building
 from ..tools.type import underscore_to_camelcase as _2camelcase
 
-infobox = {}
+infobox = {}  # It is an idea to have a global infobox (map) for all terminals
 __all__ = ['infobox']
 
 
 def _import_terminals(start_dir, package_name):
 
     with _scandir(start_dir) as entries:
         for entry in entries:
```

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/terminals/_dict/_local/json.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/terminals/_dict/_local/json.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/dict.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/dict.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/files.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from .dict import enrich as _enrich
 from .dict import item_converter as _converter
 
 __all__ = [
+    'parameters',
     'kw4open'
 ]
 
 
+parameters = {
+    'open': ['buffering', 'errors', 'newline', 'closefd', 'opener', 'encoding']
+}
+
+
 def kw4open(options: dict, mode: str, name4log: str | None = None) -> dict:
 
     if not name4log:
         name4log = kw4open.__name__
 
-    open_params = ['buffering', 'errors', 'newline', 'closefd', 'opener', 'encoding']
-
     kwargs = {}  # it is important because the open() function doesn't contains **kwargs
 
     # set default values; low priority
     kwargs = _enrich(kwargs, options, "encoding", "utf-8")
 
-    for k in open_params:
+    for k in parameters['open']:
         kwargs = _enrich(kwargs, options, k)
 
     kwargs = _enrich(kwargs, options, "mode", mode)  # function parameter has higher priority
 
     kwargs = _converter(kwargs, "buffering", int, name4log)
     kwargs = _converter(kwargs, "closefd", bool, name4log)
```

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/json.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/json.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/pkg.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/pkg.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/omnicloud/airport/tools/type.py` & `omnicloud_airport-0.0.2.dev1/omnicloud/airport/tools/type.py`

 * *Files identical despite different names*

### Comparing `omnicloud_airport-0.0.1rc7/pyproject.toml` & `omnicloud_airport-0.0.2.dev1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "omnicloud-airport"
-version = "0.0.1-pre07"
+version = "0.0.2.dev1"
 description = "platform for interacting with omnicloud"
 keywords = ["omnicloud", "supercloud", "multicloud", "cloud computing", "migration"]
 authors = ["Iurii Tarasenko <iurii@omnicloud.world>"]
 readme = "README.md"
 packages = [{include = "omnicloud"}]
 
 homepage = "https://omnicloud.world/airport"
@@ -19,22 +19,23 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License"
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
+pyyaml = "^6.0"
+update = "^0.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 duty = "^0.9.0"
 ipykernel = "^6.22.0"
 pylint = "^2.17.0"
 flake8 = "^6.0.0"
-pyyaml = "^6.0"
 pyyaml-env-tag = "^0.1"
 omnicloud-tools = "^0.0.1rc1"
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.mkdocs.dependencies]
 mkdocs = "^1.4.2"
```

### Comparing `omnicloud_airport-0.0.1rc7/PKG-INFO` & `omnicloud_airport-0.0.2.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: omnicloud-airport
-Version: 0.0.1rc7
+Version: 0.0.2.dev1
 Summary: platform for interacting with omnicloud
 Home-page: https://omnicloud.world/airport
 Keywords: omnicloud,supercloud,multicloud,cloud computing,migration
 Author: Iurii Tarasenko
 Author-email: iurii@omnicloud.world
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: update (>=0.0.1,<0.0.2)
 Project-URL: Documentation, https://docs.omnicloud.world/py-airport
 Project-URL: Repository, https://github.com/omnicloudworld/py.airport
 Description-Content-Type: text/markdown
 
 
 # Omnicloud.Airport
```

