# Comparing `tmp/upsolver_sdk_python-0.1.6.tar.gz` & `tmp/upsolver_sdk_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsolver_sdk_python-0.1.6.tar", max compression
+gzip compressed data, was "upsolver_sdk_python-0.1.7.tar", max compression
```

## Comparing `upsolver_sdk_python-0.1.6.tar` & `upsolver_sdk_python-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     5010 2023-03-26 08:04:33.295758 upsolver_sdk_python-0.1.6/README.md
--rw-r--r--   0        0        0      651 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       97 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/upsolver/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/upsolver/client/__init__.py
--rw-r--r--   0        0        0      825 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/upsolver/client/auth_filler.py
--rw-r--r--   0        0        0     3673 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/upsolver/client/exceptions.py
--rw-r--r--   0        0        0     4153 2023-03-26 08:04:33.307758 upsolver_sdk_python-0.1.6/upsolver/client/poller.py
--rw-r--r--   0        0        0      958 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/client/query.py
--rw-r--r--   0        0        0     4204 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/client/requester.py
--rw-r--r--   0        0        0     1108 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/client/response.py
--rw-r--r--   0        0        0      938 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/README.md
--rw-r--r--   0        0        0      131 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/__init__.py
--rw-r--r--   0        0        0     2222 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/connection.py
--rw-r--r--   0        0        0     7767 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/cursor.py
--rw-r--r--   0        0        0     1967 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/examples.py
--rw-r--r--   0        0        0     1423 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/type_constructors.py
--rw-r--r--   0        0        0     1609 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/types_definitions.py
--rw-r--r--   0        0        0     3144 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/dbapi/utils.py
--rw-r--r--   0        0        0        0 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/sdk/__init__.py
--rw-r--r--   0        0        0     1309 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/sdk/client.py
--rw-r--r--   0        0        0      454 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/sdk/utils.py
--rw-r--r--   0        0        0     2557 2023-03-26 08:04:33.311758 upsolver_sdk_python-0.1.6/upsolver/utils.py
--rw-r--r--   0        0        0     5659 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5071 2023-04-21 12:19:24.202781 upsolver_sdk_python-0.1.7/README.md
+-rw-r--r--   0        0        0      651 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/auth_filler.py
+-rw-r--r--   0        0        0     3673 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/exceptions.py
+-rw-r--r--   0        0        0     4153 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/poller.py
+-rw-r--r--   0        0        0     1185 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/query.py
+-rw-r--r--   0        0        0     4204 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/requester.py
+-rw-r--r--   0        0        0     1108 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/response.py
+-rw-r--r--   0        0        0      938 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/README.md
+-rw-r--r--   0        0        0      131 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/__init__.py
+-rw-r--r--   0        0        0     2222 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/connection.py
+-rw-r--r--   0        0        0     7851 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/cursor.py
+-rw-r--r--   0        0        0     1967 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/examples.py
+-rw-r--r--   0        0        0     1423 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/type_constructors.py
+-rw-r--r--   0        0        0     1609 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/types_definitions.py
+-rw-r--r--   0        0        0     3144 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/__init__.py
+-rw-r--r--   0        0        0     1309 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/client.py
+-rw-r--r--   0        0        0      454 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/utils.py
+-rw-r--r--   0        0        0     2557 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/utils.py
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.7/PKG-INFO
```

### Comparing `upsolver_sdk_python-0.1.6/README.md` & `upsolver_sdk_python-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -153,8 +153,8 @@
 
 [Documentation](https://docs.upsolver.com/sqlake/sql-command-reference) of Upsolver SQL
 
 [upsolver-sdk-python](https://github.com/Upsolver/upsolver-sdk-python) - GitHub repository with upsolver SDK for Python language
 
 [SQLake workbench](https://sqlake.upsolver.com/) main page
 
-[Python examples from this README](doc/dbapi-ex.py)
+[Python examples from this README](https://github.com/Upsolver/upsolver-sdk-python/blob/develop/doc/dbapi-ex.py)
```

### Comparing `upsolver_sdk_python-0.1.6/pyproject.toml` & `upsolver_sdk_python-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upsolver-sdk-python"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python SDK for Upsolver"
 authors = ["Upsolver Team <info@upsolver.com>"]
 
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "upsolver/__init__.py"},
```

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/auth_filler.py` & `upsolver_sdk_python-0.1.7/upsolver/client/auth_filler.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/exceptions.py` & `upsolver_sdk_python-0.1.7/upsolver/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/poller.py` & `upsolver_sdk_python-0.1.7/upsolver/client/poller.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/query.py` & `upsolver_sdk_python-0.1.7/upsolver/client/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import Iterator
 from upsolver.client.poller import ResponsePollerBuilder
 from upsolver.client.requester import Requester
 from upsolver.client.exceptions import NotSupportedError
 
 ExecutionResult = list
 
+preferredQueryEngine = {"displayName": "Upsolver",
+                            "engine": {
+                                "clazz": "GetAvailableQueryEnginesUseCase$QueryEngine"}}
+
 class RestQueryApi():
     def __init__(self, requester: Requester, poller_builder: ResponsePollerBuilder):
         self.requester = requester
         self.poller_builder = poller_builder
 
     def check_syntax(self, expression: str) -> list:
         raise NotSupportedError()
 
     def execute(self, query: str, timeout_sec: float) -> Iterator[ExecutionResult]:
         assert len(query) > 0
         poller = self.poller_builder(timeout_sec)
 
         (data, next_path) = poller(
             self.requester,
-            self.requester.post('query', json={'sql': query})
+            self.requester.post('query', json={'sql': query, 'preferredQueryEngine': preferredQueryEngine})
         )
         yield data
 
         while next_path is not None:
             (data, next_path) = poller(self.requester, self.requester.get(next_path))
             yield data
```

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/requester.py` & `upsolver_sdk_python-0.1.7/upsolver/client/requester.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/client/response.py` & `upsolver_sdk_python-0.1.7/upsolver/client/response.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/README.md` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/README.md`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/connection.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/cursor.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         if not p.exists():
             raise InterfaceError(f'Failed to execute the operation because {file_path} is invalid')
         operation = p.read_text()
         return self.execute(operation)
 
     def _prepare_query_results(self, query_response):
         first_response = next(query_response)
+        logger.debug(f"{self.__class__.__name__} Query_response: {first_response}")
         if 'data' in first_response:
             self._rowcount = -1 if first_response.get('has_next_page', True) else len(first_response['data'])
             self._description = [(c['name'], c['columnType'].get('clazz'), None, None, None, None, None)
                                  for c in first_response['columns']]
         else:
             self._rowcount = -1
             self._description = None
```

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/examples.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/examples.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/type_constructors.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/type_constructors.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/types_definitions.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/types_definitions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/dbapi/utils.py` & `upsolver_sdk_python-0.1.7/upsolver/dbapi/utils.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/sdk/client.py` & `upsolver_sdk_python-0.1.7/upsolver/sdk/client.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/upsolver/utils.py` & `upsolver_sdk_python-0.1.7/upsolver/utils.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.6/PKG-INFO` & `upsolver_sdk_python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsolver-sdk-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python SDK for Upsolver
 License: MIT
 Author: Upsolver Team
 Author-email: info@upsolver.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -172,9 +172,9 @@
 
 [Documentation](https://docs.upsolver.com/sqlake/sql-command-reference) of Upsolver SQL
 
 [upsolver-sdk-python](https://github.com/Upsolver/upsolver-sdk-python) - GitHub repository with upsolver SDK for Python language
 
 [SQLake workbench](https://sqlake.upsolver.com/) main page
 
-[Python examples from this README](doc/dbapi-ex.py)
+[Python examples from this README](https://github.com/Upsolver/upsolver-sdk-python/blob/develop/doc/dbapi-ex.py)
```

