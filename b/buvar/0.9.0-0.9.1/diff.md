# Comparing `tmp/buvar-0.9.0.tar.gz` & `tmp/buvar-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buvar-0.9.0.tar", last modified: Tue Jul  9 21:10:27 2019, max compression
+gzip compressed data, was "buvar-0.9.1.tar", last modified: Tue Jul  9 21:14:36 2019, max compression
```

## Comparing `buvar-0.9.0.tar` & `buvar-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      251 2019-07-09 20:56:17.738909 buvar-0.9.0/COPYRIGHT
--rw-r--r--   0        0        0    11358 2019-07-09 20:56:17.738909 buvar-0.9.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1023 2019-07-09 20:56:17.738909 buvar-0.9.0/LICENSE-MIT
--rw-r--r--   0        0        0      492 2019-07-09 20:56:17.738909 buvar-0.9.0/build.py
--rw-r--r--   0        0        0      905 2019-07-09 21:10:14.799880 buvar-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/__init__.py
--rw-r--r--   0        0        0     3181 2019-06-18 23:42:16.866661 buvar-0.9.0/src/buvar/cli.py
--rw-r--r--   0        0        0     2564 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/components.py
--rw-r--r--   0        0        0     7435 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/config.py
--rw-r--r--   0        0        0     1936 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/context.py
--rw-r--r--   0        0        0     2467 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/di/__init__.py
--rw-r--r--   0        0        0     2054 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/di/adapter.py
--rw-r--r--   0        0        0     2894 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/di/c_resolve.pyx
--rw-r--r--   0        0        0     2867 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/di/resolve.py
--rw-r--r--   0        0        0     5185 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/log.py
--rw-r--r--   0        0        0    10598 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/plugin.py
--rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/plugins/__init__.py
--rw-r--r--   0        0        0     1009 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/plugins/aiohttp.py
--rw-r--r--   0        0        0      349 2019-07-09 20:56:17.742242 buvar-0.9.0/src/buvar/util.py
--rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      191 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/bar_plugin.py
--rw-r--r--   0        0        0       62 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/baz_plugin.py
--rw-r--r--   0        0        0      166 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/buvar.toml
--rw-r--r--   0        0        0      189 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      234 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/foo_plugin.py
--rw-r--r--   0        0        0      468 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/server_plugin.py
--rw-r--r--   0        0        0      680 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/test_components.py
--rw-r--r--   0        0        0     4030 2019-07-09 20:56:17.742242 buvar-0.9.0/tests/test_config.py
--rw-r--r--   0        0        0     2730 2019-07-09 20:56:17.745576 buvar-0.9.0/tests/test_di.py
--rw-r--r--   0        0        0     4795 2019-07-09 20:56:17.745576 buvar-0.9.0/tests/test_plugin.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 buvar-0.9.0/setup.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 buvar-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2019-07-09 20:56:17.738909 buvar-0.9.1/COPYRIGHT
+-rw-r--r--   0        0        0    11358 2019-07-09 20:56:17.738909 buvar-0.9.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     1023 2019-07-09 20:56:17.738909 buvar-0.9.1/LICENSE-MIT
+-rw-r--r--   0        0        0     3963 2019-07-09 21:04:47.333859 buvar-0.9.1/README.rst
+-rw-r--r--   0        0        0      492 2019-07-09 20:56:17.738909 buvar-0.9.1/build.py
+-rw-r--r--   0        0        0      974 2019-07-09 21:14:33.524302 buvar-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/__init__.py
+-rw-r--r--   0        0        0     3181 2019-06-18 23:42:16.866661 buvar-0.9.1/src/buvar/cli.py
+-rw-r--r--   0        0        0     2564 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/components.py
+-rw-r--r--   0        0        0     7435 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/config.py
+-rw-r--r--   0        0        0     1936 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/context.py
+-rw-r--r--   0        0        0     2467 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/di/__init__.py
+-rw-r--r--   0        0        0     2054 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/di/adapter.py
+-rw-r--r--   0        0        0     2894 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/di/c_resolve.pyx
+-rw-r--r--   0        0        0     2867 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/di/resolve.py
+-rw-r--r--   0        0        0     5185 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/log.py
+-rw-r--r--   0        0        0    10598 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/plugin.py
+-rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/plugins/__init__.py
+-rw-r--r--   0        0        0     1009 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/plugins/aiohttp.py
+-rw-r--r--   0        0        0      349 2019-07-09 20:56:17.742242 buvar-0.9.1/src/buvar/util.py
+-rw-r--r--   0        0        0        0 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0      191 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/bar_plugin.py
+-rw-r--r--   0        0        0       62 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/baz_plugin.py
+-rw-r--r--   0        0        0      166 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/buvar.toml
+-rw-r--r--   0        0        0      189 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0      234 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/foo_plugin.py
+-rw-r--r--   0        0        0      468 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/server_plugin.py
+-rw-r--r--   0        0        0      680 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/test_components.py
+-rw-r--r--   0        0        0     4030 2019-07-09 20:56:17.742242 buvar-0.9.1/tests/test_config.py
+-rw-r--r--   0        0        0     2730 2019-07-09 20:56:17.745576 buvar-0.9.1/tests/test_di.py
+-rw-r--r--   0        0        0     4795 2019-07-09 20:56:17.745576 buvar-0.9.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     5126 1970-01-01 00:00:00.000000 buvar-0.9.1/setup.py
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 buvar-0.9.1/PKG-INFO
```

### Comparing `buvar-0.9.0/LICENSE-APACHE` & `buvar-0.9.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/LICENSE-MIT` & `buvar-0.9.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/pyproject.toml` & `buvar-0.9.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 build = 'build.py'
 name = "buvar"
-version = "0.9.0"
-description = "General purpose config loader"
+version = "0.9.1"
+description = "General purpose asyncio service loader and dependency injector"
+readme = "README.rst"
 authors = ["Oliver Berger <diefans@gmail.com>"]
 license = "Apache-2.0"
-include = ['COPYRIGHT', 'tests/*']
+include = ['COPYRIGHT', 'tests/*', 'examples/*']
 
 [tool.poetry.scripts]
 buvar = 'buvar.cli:main'
 
 [tool.poetry.dependencies]
 python = "^3.6"
 orjson = "^2.0"
 tomlkit = "^0.5.3"
 toml = "^0.10"
 multidict = "^4.5"
 structlog = "^19.1"
 attrs = "^19.1"
-cattrs = "^0.9.0"
+cattrs = "^0.9.1"
 typing_inspect = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^4.6"
 pytest-randomly = "^3.0"
 pytest-watch = "^4.2"
 pytest-cache = "^1.0"
```

### Comparing `buvar-0.9.0/src/buvar/cli.py` & `buvar-0.9.1/src/buvar/cli.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/components.py` & `buvar-0.9.1/src/buvar/components.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/config.py` & `buvar-0.9.1/src/buvar/config.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/context.py` & `buvar-0.9.1/src/buvar/context.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/di/__init__.py` & `buvar-0.9.1/src/buvar/di/__init__.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/di/adapter.py` & `buvar-0.9.1/src/buvar/di/adapter.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/di/c_resolve.pyx` & `buvar-0.9.1/src/buvar/di/c_resolve.pyx`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/di/resolve.py` & `buvar-0.9.1/src/buvar/di/resolve.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/log.py` & `buvar-0.9.1/src/buvar/log.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/plugin.py` & `buvar-0.9.1/src/buvar/plugin.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/src/buvar/plugins/aiohttp.py` & `buvar-0.9.1/src/buvar/plugins/aiohttp.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/tests/test_components.py` & `buvar-0.9.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/tests/test_config.py` & `buvar-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/tests/test_di.py` & `buvar-0.9.1/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `buvar-0.9.0/tests/test_plugin.py` & `buvar-0.9.1/tests/test_plugin.py`

 * *Files identical despite different names*

