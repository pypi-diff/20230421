# Comparing `tmp/emmett_rest-1.5.0.tar.gz` & `tmp/emmett_rest-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmett_rest-1.5.0.tar", max compression
+gzip compressed data, was "emmett_rest-1.5.1.tar", max compression
```

## Comparing `emmett_rest-1.5.0.tar` & `emmett_rest-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1022 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/CHANGES.md
--rw-r--r--   0        0        0     1486 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/LICENSE
--rw-r--r--   0        0        0    30802 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/README.md
--rw-r--r--   0        0        0      166 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/__init__.py
--rw-r--r--   0        0        0       22 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/__version__.py
--rw-r--r--   0        0        0     4394 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/ext.py
--rw-r--r--   0        0        0     3518 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/helpers.py
--rw-r--r--   0        0        0       25 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/__init__.py
--rw-r--r--   0        0        0     4559 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/api.py
--rw-r--r--   0        0        0        0 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/assets/__init__.py
--rw-r--r--   0        0        0     2694 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/assets/description.md
--rw-r--r--   0        0        0      573 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/assets/stoplight.html
--rw-r--r--   0        0        0    35890 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/generation.py
--rw-r--r--   0        0        0      598 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/helpers.py
--rw-r--r--   0        0        0     4895 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/mod.py
--rw-r--r--   0        0        0    10177 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/openapi/schemas.py
--rw-r--r--   0        0        0     5196 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/parsers.py
--rw-r--r--   0        0        0       35 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/queries/__init__.py
--rw-r--r--   0        0        0      587 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/queries/errors.py
--rw-r--r--   0        0        0     1927 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/queries/helpers.py
--rw-r--r--   0        0        0     6158 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/queries/parser.py
--rw-r--r--   0        0        0     2629 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/queries/validation.py
--rw-r--r--   0        0        0    32447 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/rest.py
--rw-r--r--   0        0        0     2356 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/serializers.py
--rw-r--r--   0        0        0      381 2023-03-19 16:38:33.195093 emmett_rest-1.5.0/emmett_rest/typing.py
--rw-r--r--   0        0        0     6987 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/emmett_rest/wrappers.py
--rw-r--r--   0        0        0     1483 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1750 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/conftest.py
--rw-r--r--   0        0        0     4372 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/test_endpoints.py
--rw-r--r--   0        0        0     1955 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/test_endpoints_additional.py
--rw-r--r--   0        0        0     2801 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/test_envelopes.py
--rw-r--r--   0        0        0     2429 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/test_meta.py
--rw-r--r--   0        0        0    10261 2023-03-19 16:38:33.199094 emmett_rest-1.5.0/tests/test_queries.py
--rw-r--r--   0        0        0    32257 1970-01-01 00:00:00.000000 emmett_rest-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/CHANGES.md
+-rw-r--r--   0        0        0     1486 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/LICENSE
+-rw-r--r--   0        0        0    30802 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/README.md
+-rw-r--r--   0        0        0      166 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/__version__.py
+-rw-r--r--   0        0        0     4394 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/ext.py
+-rw-r--r--   0        0        0     3518 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/helpers.py
+-rw-r--r--   0        0        0       25 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/api.py
+-rw-r--r--   0        0        0        0 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/assets/__init__.py
+-rw-r--r--   0        0        0     2694 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/assets/description.md
+-rw-r--r--   0        0        0      573 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/assets/stoplight.html
+-rw-r--r--   0        0        0    35890 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/generation.py
+-rw-r--r--   0        0        0      598 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/helpers.py
+-rw-r--r--   0        0        0     4895 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/mod.py
+-rw-r--r--   0        0        0    10177 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/openapi/schemas.py
+-rw-r--r--   0        0        0     5196 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/parsers.py
+-rw-r--r--   0        0        0       35 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/queries/__init__.py
+-rw-r--r--   0        0        0      587 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/queries/errors.py
+-rw-r--r--   0        0        0     1927 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/queries/helpers.py
+-rw-r--r--   0        0        0     6158 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/queries/parser.py
+-rw-r--r--   0        0        0     2700 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/queries/validation.py
+-rw-r--r--   0        0        0    32447 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/rest.py
+-rw-r--r--   0        0        0     2356 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/serializers.py
+-rw-r--r--   0        0        0      381 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/typing.py
+-rw-r--r--   0        0        0     6987 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/emmett_rest/wrappers.py
+-rw-r--r--   0        0        0     1483 2023-04-21 08:05:24.323500 emmett_rest-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1750 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     4372 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1955 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/test_endpoints_additional.py
+-rw-r--r--   0        0        0     2801 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/test_envelopes.py
+-rw-r--r--   0        0        0     2429 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/test_meta.py
+-rw-r--r--   0        0        0    10261 2023-04-21 08:05:24.327499 emmett_rest-1.5.1/tests/test_queries.py
+-rw-r--r--   0        0        0    32257 1970-01-01 00:00:00.000000 emmett_rest-1.5.1/PKG-INFO
```

### Comparing `emmett_rest-1.5.0/CHANGES.md` & `emmett_rest-1.5.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/LICENSE` & `emmett_rest-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/README.md` & `emmett_rest-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/ext.py` & `emmett_rest-1.5.1/emmett_rest/ext.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/helpers.py` & `emmett_rest-1.5.1/emmett_rest/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/api.py` & `emmett_rest-1.5.1/emmett_rest/openapi/api.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/assets/description.md` & `emmett_rest-1.5.1/emmett_rest/openapi/assets/description.md`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/assets/stoplight.html` & `emmett_rest-1.5.1/emmett_rest/openapi/assets/stoplight.html`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/generation.py` & `emmett_rest-1.5.1/emmett_rest/openapi/generation.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/helpers.py` & `emmett_rest-1.5.1/emmett_rest/openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/mod.py` & `emmett_rest-1.5.1/emmett_rest/openapi/mod.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/openapi/schemas.py` & `emmett_rest-1.5.1/emmett_rest/openapi/schemas.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/parsers.py` & `emmett_rest-1.5.1/emmett_rest/parsers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/queries/errors.py` & `emmett_rest-1.5.1/emmett_rest/queries/errors.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/queries/helpers.py` & `emmett_rest-1.5.1/emmett_rest/queries/helpers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/queries/parser.py` & `emmett_rest-1.5.1/emmett_rest/queries/parser.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/queries/validation.py` & `emmett_rest-1.5.1/emmett_rest/queries/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     '$le': op_validation_generator(int, float, datetime),
     '$ge': op_validation_generator(int, float, datetime),
     '$lte': op_validation_generator(int, float, datetime),
     '$gte': op_validation_generator(int, float, datetime),
     '$exists': op_validation_generator(bool),
     '$like': validate_default,
     '$ilike': validate_default,
+    '$contains': validate_default,
+    '$icontains': validate_default,
     '$regex': validate_default,
     '$iregex': validate_default,
     '$geo.contains': validate_geo,
     '$geo.equals': validate_geo,
     '$geo.intersects': validate_geo,
     '$geo.overlaps': validate_geo,
     '$geo.touches': validate_geo,
```

### Comparing `emmett_rest-1.5.0/emmett_rest/rest.py` & `emmett_rest-1.5.1/emmett_rest/rest.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/serializers.py` & `emmett_rest-1.5.1/emmett_rest/serializers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/emmett_rest/wrappers.py` & `emmett_rest-1.5.1/emmett_rest/wrappers.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/pyproject.toml` & `emmett_rest-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emmett-rest"
-version = "1.5.0"
+version = "1.5.1"
 description = "REST extension for Emmett framework"
 authors = ["Giovanni Barillari <gi0baro@d4net.org>"]
 license = "BSD-3-Clause"
 
 readme = "README.md"
 homepage = "https://github.com/emmett-framework/rest"
 repository = "https://github.com/emmett-framework/rest"
```

### Comparing `emmett_rest-1.5.0/tests/conftest.py` & `emmett_rest-1.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/tests/test_endpoints.py` & `emmett_rest-1.5.1/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/tests/test_endpoints_additional.py` & `emmett_rest-1.5.1/tests/test_endpoints_additional.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/tests/test_envelopes.py` & `emmett_rest-1.5.1/tests/test_envelopes.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/tests/test_meta.py` & `emmett_rest-1.5.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/tests/test_queries.py` & `emmett_rest-1.5.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `emmett_rest-1.5.0/PKG-INFO` & `emmett_rest-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emmett-rest
-Version: 1.5.0
+Version: 1.5.1
 Summary: REST extension for Emmett framework
 Home-page: https://github.com/emmett-framework/rest
 License: BSD-3-Clause
 Keywords: rest,web,emmett
 Author: Giovanni Barillari
 Author-email: gi0baro@d4net.org
 Requires-Python: >=3.8,<4.0
```

