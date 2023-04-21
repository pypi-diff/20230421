# Comparing `tmp/edge_orm-0.6.6.tar.gz` & `tmp/edge_orm-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.6.6.tar", max compression
+gzip compressed data, was "edge_orm-0.6.7.tar", max compression
```

## Comparing `edge_orm-0.6.6.tar` & `edge_orm-0.6.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.6.6/README.md
--rw-r--r--   0        0        0      806 2023-04-19 18:28:11.434516 edge_orm-0.6.6/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.6.6/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.6.6/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.6.6/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.6.6/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.6.6/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.6.6/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.6.6/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.6.6/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.6.6/edge_orm/node/models.py
--rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.6.6/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.6.6/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.6.6/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.6.6/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    42021 2023-04-19 18:44:00.826996 edge_orm-0.6.6/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.6.6/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.6.6/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.6.6/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.6.6/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.6.6/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.6.6/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.6.6/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.6.6/edge_orm/validators.py
--rw-r--r--   0        0        0      785 2023-04-19 18:44:56.067564 edge_orm-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.6.6/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.6.7/README.md
+-rw-r--r--   0        0        0      806 2023-04-19 18:28:11.434516 edge_orm-0.6.7/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.6.7/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.6.7/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.6.7/edge_orm/execute.py
+-rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.6.7/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.6.7/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.6.7/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.6.7/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.6.7/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.6.7/edge_orm/node/models.py
+-rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.6.7/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.6.7/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.6.7/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.6.7/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    42082 2023-04-21 19:01:50.518231 edge_orm-0.6.7/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5294 2023-02-08 20:21:01.356439 edge_orm-0.6.7/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.6.7/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.6.7/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.6.7/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.6.7/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.6.7/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.6.7/edge_orm/unset.py
+-rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.6.7/edge_orm/validators.py
+-rw-r--r--   0        0        0      785 2023-04-21 19:01:47.866609 edge_orm-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 edge_orm-0.6.7/setup.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.6.7/PKG-INFO
```

### Comparing `edge_orm-0.6.6/edge_orm/__init__.py` & `edge_orm-0.6.7/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/cache.py` & `edge_orm-0.6.7/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/execute.py` & `edge_orm-0.6.7/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/external/encoders.py` & `edge_orm-0.6.7/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/helpers.py` & `edge_orm-0.6.7/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/logs.py` & `edge_orm-0.6.7/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/node/models.py` & `edge_orm-0.6.7/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/resolver/merging.py` & `edge_orm-0.6.7/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/resolver/model.py` & `edge_orm-0.6.7/edge_orm/resolver/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,16 +486,16 @@
             return None
         return model_lst[0]
 
     async def count(self, client: edgedb.AsyncIOClient) -> int:
         query_str, variables = self.full_query_str_and_vars(
             include_select=False, prefix=""
         )
-
-        query_str = f"SELECT count({self.model_name} {query_str})"
+        query_str = query_str.replace("{ id } ", "")
+        query_str = f"SELECT count((select {self.model_name} {query_str}))"
         with span.span(
             op=f"edgedb.query.{self.model_name}", description=query_str[:200]
         ):
             c = await execute.query(
                 client=client,
                 query_str=query_str,
                 variables=variables,
```

### Comparing `edge_orm-0.6.6/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.6.7/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/resolver/utils.py` & `edge_orm-0.6.7/edge_orm/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/span.py` & `edge_orm-0.6.7/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/types_generator/introspection.py` & `edge_orm-0.6.7/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/types_generator/main.py` & `edge_orm-0.6.7/edge_orm/types_generator/main.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/unset.py` & `edge_orm-0.6.7/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/edge_orm/validators.py` & `edge_orm-0.6.7/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.6.6/pyproject.toml` & `edge_orm-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `edge_orm-0.6.6/setup.py` & `edge_orm-0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pydantic[email]>=1.10,<2.0']
 
 extras_require = \
 {'docs': ['mkdocs-material>=8.5.7,<9.0.0']}
 
 setup_kwargs = {
     'name': 'edge-orm',
-    'version': '0.6.6',
+    'version': '0.6.7',
     'description': '',
     'long_description': '# edge orm',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edge_orm-0.6.6/PKG-INFO` & `edge_orm-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.6.6
+Version: 0.6.7
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
```

