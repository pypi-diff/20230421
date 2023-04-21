# Comparing `tmp/surrealdb-0.3.0.tar.gz` & `tmp/surrealdb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealdb-0.3.0.tar", max compression
+gzip compressed data, was "surrealdb-0.3.1.tar", max compression
```

## Comparing `surrealdb-0.3.0.tar` & `surrealdb-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11341 2021-12-09 08:04:59.357893 surrealdb-0.3.0/LICENSE
--rw-r--r--   0        0        0     5599 2023-03-27 13:37:36.264433 surrealdb-0.3.0/README.md
--rw-r--r--   0        0        0     1885 2023-03-27 13:37:58.385104 surrealdb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      653 2023-03-27 13:37:36.265642 surrealdb-0.3.0/surrealdb/__init__.py
--rw-r--r--   0        0        0    11693 2023-03-27 13:37:36.265802 surrealdb-0.3.0/surrealdb/http.py
--rw-r--r--   0        0        0        0 2022-09-18 17:35:30.759418 surrealdb-0.3.0/surrealdb/py.typed
--rw-r--r--   0        0        0    23318 2023-03-27 13:37:36.266001 surrealdb-0.3.0/surrealdb/ws.py
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 surrealdb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2021-12-09 08:04:59.357893 surrealdb-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5599 2023-03-27 13:37:36.264433 surrealdb-0.3.1/README.md
+-rw-r--r--   0        0        0     2289 2023-04-21 09:04:43.300275 surrealdb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      653 2023-04-21 09:04:43.300413 surrealdb-0.3.1/surrealdb/__init__.py
+-rw-r--r--   0        0        0    11322 2023-04-21 09:04:43.300563 surrealdb-0.3.1/surrealdb/http.py
+-rw-r--r--   0        0        0        0 2022-09-18 17:35:30.759418 surrealdb-0.3.1/surrealdb/py.typed
+-rw-r--r--   0        0        0    23338 2023-04-21 09:04:43.300733 surrealdb-0.3.1/surrealdb/ws.py
+-rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 surrealdb-0.3.1/PKG-INFO
```

### Comparing `surrealdb-0.3.0/LICENSE` & `surrealdb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealdb-0.3.0/README.md` & `surrealdb-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `surrealdb-0.3.0/pyproject.toml` & `surrealdb-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surrealdb"
-version = "0.3.0"
+version = "0.3.1"
 description = "The official SurrealDB library for Python."
 readme = "README.md"
 authors = ["SurrealDB"]
 license = "Apache-2.0"
 repository = "https://github.com/surrealdb/surrealdb.py"
 documentation = "https://surrealdb.com/docs/integration/libraries/python"
 
@@ -64,15 +64,24 @@
 )/
 '''
 
 [tool.ruff]
 select = ["I", "D", "N", "UP"]
 line-length = 88
 
-ignore = ["D212", "D107", "D100", "D104", "D107", "N818", "D401", "D205"]
+ignore = [
+    "D100",  # Missing docstring in public module
+    "D104",  # Missing docstring in public package
+    "D107",  # Missing docstring in __init__
+    "D205",  # 1 blank line required between summary line and description
+    "D212",  # Multi-line docstring summary should start at the first line	
+    "N805",  # First argument of a method should be named self
+    "N818",  # Exception name ... should be named with an Error suffix
+    "UP035"  # Typing deprecations
+]
 
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".hg",
```

### Comparing `surrealdb-0.3.0/surrealdb/__init__.py` & `surrealdb-0.3.1/surrealdb/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from .ws import Surreal
 from .http import SurrealHTTP
+from .ws import Surreal
 
 __all__ = ("Surreal", "SurrealHTTP")
```

### Comparing `surrealdb-0.3.0/surrealdb/http.py` & `surrealdb-0.3.1/surrealdb/http.py`

 * *Files 6% similar despite different names*

```diff
@@ -199,21 +199,21 @@
         Examples:
             Select all records from a table (or other entity)
                 people = await db.select('person')
 
             Select a specific record from a table (or other entity)
                 person = await db.select('person:h5wxrf2ewk8xjxosxtyc')
         """
-        if ":" in thing:
-            table, id = thing.split(":")
-            response = await self._request(method="GET", uri=f"/key/{table}/{id}")
-            if not response:
-                raise SurrealException(f"Key {id} not found in table {table}")
-        else:
-            response = await self._request(method="GET", uri=f"/key/{thing}")
+        table, record_id = thing.split(":") if ":" in thing else (thing, None)
+        response = await self._request(
+            method="GET",
+            uri=f"/key/{table}/{record_id}" if record_id else f"/key/{table}",
+        )
+        if not response and record_id is not None:
+            raise SurrealException(f"Key {record_id} not found in table {table}")
         return response[0]['result']
 
     async def create(self, thing: str, data: Optional[Dict[str, Any]] = None) -> str:
         """Create a record in the database.
 
         This function will run the following query in the database:
         create $thing content $data
@@ -231,28 +231,24 @@
                     'name': 'Tobie',
                     'settings': {
                         'active': true,
                         'marketing': true,
                         },
                 })
         """
-        if ":" in thing:
-            table, id = thing.split(":")
-            response = await self._request(
-                method="POST",
-                uri=f"/key/{table}/{id}",
-                data=json.dumps(data),
-            )
-        else:
-            response = await self._request(
-                method="POST",
-                uri=f"/key/{thing}",
-                data=json.dumps(data),
-            )
+        table, record_id = thing.split(":") if ":" in thing else (thing, None)
+        response = await self._request(
+            method="POST",
+            uri=f"/key/{table}/{record_id}" if record_id else f"/key/{table}",
+            data=json.dumps(data, ensure_ascii=False),
+        )
+        if not response and record_id is not None:
+            raise SurrealException(f"Key {record_id} not found in table {table}")
         return response[0]['result']
+    
 
     async def update(self, thing: str, data: Any) -> Dict[str, Any]:
         """Updates all records in a table, or a specific record, in the database.
 
         This function replaces the current document / record data with the
         specified data.
 
@@ -272,28 +268,20 @@
                     'name': 'Tobie',
                     'settings': {
                         'active': true,
                         'marketing': true,
                         },
                 })
         """
-        if ":" in thing:
-            table, id = thing.split(":")
-            response = await self._request(
-                method="PUT",
-                uri=f"/key/{table}/{id}",
-                data=json.dumps(data),
-            )
-        else:
-            table, id = thing.split(":")
-            response = await self._request(
-                method="PUT",
-                uri=f"/key/{thing}",  # need to test if this works
-                data=json.dumps(data),
-            )
+        table, record_id = thing.split(":") if ":" in thing else (thing, None)
+        response = await self._request(
+            method="PUT",
+            uri=f"/key/{table}/{record_id}" if record_id else f"/key/{table}",
+            data=json.dumps(data, ensure_ascii=False),
+        )
         return response[0]['result']
 
     async def patch(self, thing: str, data: Any) -> Dict[str, Any]:
         """Applies JSON Patch changes to all records, or a specific record, in the database.
 
         This function patches the current document / record data with
         the specified JSON Patch data.
@@ -313,28 +301,20 @@
             Update a record with a specific ID
             person = await db.patch('person:tobie', [
                 { 'op': "replace", 'path': "/settings/active", 'value': False },
                 { 'op': "add", "path": "/tags", "value": ["developer", "engineer"] },
                 { 'op': "remove", "path": "/temp" },
             ])
         """
-        if ":" in thing:
-            table, id = thing.split(":")
-            response = await self._request(
-                method="PATCH",
-                uri=f"/key/{table}/{id}",
-                data=json.dumps(data),
-            )
-        else:
-            table, id = thing.split(":")
-            response = await self._request(
-                method="PATCH",
-                uri=f"/key/{thing}",  # need to test if this works
-                data=json.dumps(data),
-            )
+        table, record_id = thing.split(":") if ":" in thing else (thing, None)
+        response = await self._request(
+            method="PATCH",
+            uri=f"/key/{table}/{record_id}" if record_id else f"/key/{table}",
+            data=json.dumps(data, ensure_ascii=False),
+        )
         return response[0]['result']
 
     async def delete(self, thing: str) -> None:
         """Deletes all records in a table, or a specific record, from the database.
 
         This function will run the following query in the database:
         delete * from $thing
@@ -344,13 +324,13 @@
 
         Examples:
             Delete all records from a table
                 await db.delete('person')
             Delete a specific record from a table
                 await db.delete('person:h5wxrf2ewk8xjxosxtyc')
         """
-        if ":" in thing:
-            table, id = thing.split(":")
-            response = await self._request(method="DELETE", uri=f"/key/{table}/{id}")
-        else:
-            response = await self._request(method="DELETE", uri=f"/key/{thing}")
+        table, record_id = thing.split(":") if ":" in thing else (thing, None)
+        response = await self._request(
+            method="DELETE",
+            uri=f"/key/{table}/{record_id}" if record_id else f"/key/{table}",
+        )
         return response
```

### Comparing `surrealdb-0.3.0/surrealdb/ws.py` & `surrealdb-0.3.1/surrealdb/ws.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,15 +711,15 @@
         Args:
             request: The request to send.
 
         Raises:
             Exception: If the client is not connected to the Surreal server.
         """
         self._validate_connection()
-        await self.ws.send(json.dumps(request.dict()))  # type: ignore
+        await self.ws.send(json.dumps(request.dict(), ensure_ascii=False))  # type: ignore
 
     async def _recv(self) -> Union[ResponseSuccess, ResponseError]:
         """Receives a response from the Surreal server.
 
         Returns:
             The response from the Surreal server.
```

### Comparing `surrealdb-0.3.0/PKG-INFO` & `surrealdb-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealdb
-Version: 0.3.0
+Version: 0.3.1
 Summary: The official SurrealDB library for Python.
 Home-page: https://github.com/surrealdb/surrealdb.py
 License: Apache-2.0
 Keywords: SurrealDB,Database
 Author: SurrealDB
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: surrealdb Version: 0.3.0 Summary: The official
+Metadata-Version: 2.1 Name: surrealdb Version: 0.3.1 Summary: The official
 SurrealDB library for Python. Home-page: https://github.com/surrealdb/
 surrealdb.py License: Apache-2.0 Keywords: SurrealDB,Database Author: SurrealDB
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

