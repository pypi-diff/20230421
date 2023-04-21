# Comparing `tmp/FunctionStoredController-0.0.8.tar.gz` & `tmp/FunctionStoredController-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunctionStoredController-0.0.8.tar", last modified: Thu Apr 20 17:23:47 2023, max compression
+gzip compressed data, was "FunctionStoredController-0.0.9.tar", last modified: Fri Apr 21 02:40:50 2023, max compression
```

## Comparing `FunctionStoredController-0.0.8.tar` & `FunctionStoredController-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       59 2022-12-31 08:27:33.620967 FunctionStoredController-0.0.8/.gitignore
--rw-r--r--   0        0        0     1099 2023-01-15 14:19:46.299275 FunctionStoredController-0.0.8/LICENSE
--rw-r--r--   0        0        0      516 2023-02-02 16:38:17.032194 FunctionStoredController-0.0.8/Pipfile
--rw-r--r--   0        0        0    23049 2023-02-02 16:38:27.637616 FunctionStoredController-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0     4865 2023-02-02 16:06:54.334179 FunctionStoredController-0.0.8/README.md
--rw-r--r--   0        0        0        0 2022-12-30 17:17:31.605087 FunctionStoredController-0.0.8/__init__.py
--rw-r--r--   0        0        0        0 2022-12-30 17:17:31.605087 FunctionStoredController-0.0.8/controller/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 13:47:27.222000 FunctionStoredController-0.0.8/controller/core/__init__.py
--rw-r--r--   0        0        0     3668 2023-04-20 16:29:54.251833 FunctionStoredController-0.0.8/controller/core/db.py
--rw-r--r--   0        0        0     1408 2023-03-30 16:47:12.414156 FunctionStoredController-0.0.8/controller/core/fields.py
--rw-r--r--   0        0        0      203 2023-03-11 13:47:27.223000 FunctionStoredController-0.0.8/controller/core/functions.py
--rw-r--r--   0        0        0     3124 2023-03-30 16:11:02.040621 FunctionStoredController-0.0.8/controller/core/models.py
--rw-r--r--   0        0        0        0 2023-03-11 13:47:27.224000 FunctionStoredController-0.0.8/controller/django/__init__.py
--rw-r--r--   0        0        0      440 2023-03-29 15:29:14.003829 FunctionStoredController-0.0.8/controller/django/db.py
--rw-r--r--   0        0        0      185 2023-03-11 13:47:27.225000 FunctionStoredController-0.0.8/controller/django/fields.py
--rw-r--r--   0        0        0      404 2023-03-29 12:31:34.726000 FunctionStoredController-0.0.8/controller/django/middleware.py
--rw-r--r--   0        0        0     1622 2023-03-29 06:40:04.918000 FunctionStoredController-0.0.8/controller/django/models.py
--rw-r--r--   0        0        0      604 2023-04-20 17:22:48.968557 FunctionStoredController-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      581 2023-02-02 16:37:42.084634 FunctionStoredController-0.0.8/requirements.txt
--rw-r--r--   0        0        0     5075 1970-01-01 00:00:00.000000 FunctionStoredController-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       59 2022-12-31 08:27:33.620967 FunctionStoredController-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1099 2023-01-15 14:19:46.299275 FunctionStoredController-0.0.9/LICENSE
+-rw-r--r--   0        0        0      516 2023-02-02 16:38:17.032194 FunctionStoredController-0.0.9/Pipfile
+-rw-r--r--   0        0        0    23049 2023-02-02 16:38:27.637616 FunctionStoredController-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0     4865 2023-02-02 16:06:54.334179 FunctionStoredController-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-12-30 17:17:31.605087 FunctionStoredController-0.0.9/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-30 17:17:31.605087 FunctionStoredController-0.0.9/controller/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-11 13:47:27.222000 FunctionStoredController-0.0.9/controller/core/__init__.py
+-rw-r--r--   0        0        0     3634 2023-04-21 02:40:11.979078 FunctionStoredController-0.0.9/controller/core/db.py
+-rw-r--r--   0        0        0     1408 2023-03-30 16:47:12.414156 FunctionStoredController-0.0.9/controller/core/fields.py
+-rw-r--r--   0        0        0      203 2023-03-11 13:47:27.223000 FunctionStoredController-0.0.9/controller/core/functions.py
+-rw-r--r--   0        0        0     3124 2023-03-30 16:11:02.040621 FunctionStoredController-0.0.9/controller/core/models.py
+-rw-r--r--   0        0        0        0 2023-03-11 13:47:27.224000 FunctionStoredController-0.0.9/controller/django/__init__.py
+-rw-r--r--   0        0        0      440 2023-03-29 15:29:14.003829 FunctionStoredController-0.0.9/controller/django/db.py
+-rw-r--r--   0        0        0      185 2023-03-11 13:47:27.225000 FunctionStoredController-0.0.9/controller/django/fields.py
+-rw-r--r--   0        0        0      404 2023-03-29 12:31:34.726000 FunctionStoredController-0.0.9/controller/django/middleware.py
+-rw-r--r--   0        0        0     1622 2023-03-29 06:40:04.918000 FunctionStoredController-0.0.9/controller/django/models.py
+-rw-r--r--   0        0        0      604 2023-04-21 02:40:23.123296 FunctionStoredController-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      581 2023-02-02 16:37:42.084634 FunctionStoredController-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     5075 1970-01-01 00:00:00.000000 FunctionStoredController-0.0.9/PKG-INFO
```

### Comparing `FunctionStoredController-0.0.8/LICENSE` & `FunctionStoredController-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/Pipfile` & `FunctionStoredController-0.0.9/Pipfile`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/Pipfile.lock` & `FunctionStoredController-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/README.md` & `FunctionStoredController-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/controller/core/db.py` & `FunctionStoredController-0.0.9/controller/core/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,30 +8,28 @@
     def __query(self, callback, response_limit: int):
         """Выполнение запроса по получению"""
 
         def to_dict(item):
             if item:
                 return dict(zip(columns, item))
             return {}
-        try:
-            with self.conn.cursor() as cursor:
-                callback(cursor)
-                columns = [col.name for col in cursor.description or []]
-                if response_limit == 1:
-                    try:
-                        response = to_dict(cursor.fetchone())
-                    except Exception as e:
-                        return None
-                elif response_limit <= 0:
-                    response = list(map(to_dict, cursor.fetchall()))
-                else:
-                    response = list(map(to_dict, cursor.fetchmany(response_limit)))
-                return response
-        except Exception:
-            pass
+
+        with self.conn.cursor() as cursor:
+            callback(cursor)
+            columns = [col.name for col in cursor.description or []]
+            if response_limit == 1:
+                try:
+                    response = to_dict(cursor.fetchone())
+                except Exception as e:
+                    return None
+            elif response_limit <= 0:
+                response = list(map(to_dict, cursor.fetchall()))
+            else:
+                response = list(map(to_dict, cursor.fetchmany(response_limit)))
+            return response
 
     @staticmethod
     def error_to_sql(value):
         if value is None:
             return 'null'
         if not isinstance(value, str):
             return str(value)
@@ -56,15 +54,18 @@
         return self.__query(
             lambda cursor: self.__create_query_execute(cursor, f'SELECT {aggregate} FROM ', func_name, *args),
             response_limit)
 
     def procedure(self, *args, func_name: str):
         def call_procedure(cursor):
             self.__create_query_execute(cursor, 'call ', func_name, *args)
-            self.conn.commit()
+            try:
+                self.conn.commit()
+            except Exception:
+                pass
 
         return self.__query(call_procedure, response_limit=1)
 
 
 class DataBase(AbstractDataBase):
     def __init__(self,
                  db_name: str,
```

### Comparing `FunctionStoredController-0.0.8/controller/core/fields.py` & `FunctionStoredController-0.0.9/controller/core/fields.py`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/controller/core/models.py` & `FunctionStoredController-0.0.9/controller/core/models.py`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/controller/django/models.py` & `FunctionStoredController-0.0.9/controller/django/models.py`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/pyproject.toml` & `FunctionStoredController-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "FunctionStoredController"
-version = '0.0.8'
+version = '0.0.9'
 description = "Контроллер для работы с хранимыми процедурами"
 authors = [{name = "DigoErisdar", email = "danil.galkin2017@mail.ru"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 
 [project.urls]
```

### Comparing `FunctionStoredController-0.0.8/requirements.txt` & `FunctionStoredController-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `FunctionStoredController-0.0.8/PKG-INFO` & `FunctionStoredController-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunctionStoredController
-Version: 0.0.8
+Version: 0.0.9
 Summary: Контроллер для работы с хранимыми процедурами
 Author-email: DigoErisdar <danil.galkin2017@mail.ru>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/DigoErisdar/Controller
 
 # Контроллер для работы с хранимыми процедурами
```

