# Comparing `tmp/mongo_db_operation-1.0.8.tar.gz` & `tmp/mongo_db_operation-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_db_operation-1.0.8.tar", max compression
+gzip compressed data, was "mongo_db_operation-1.0.9.tar", max compression
```

## Comparing `mongo_db_operation-1.0.8.tar` & `mongo_db_operation-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-19 13:31:34.962743 mongo_db_operation-1.0.8/LICENSE
--rw-r--r--   0        0        0     8943 2023-04-21 12:42:32.282215 mongo_db_operation-1.0.8/README.md
--rw-r--r--   0        0        0      643 2023-04-21 21:11:35.251001 mongo_db_operation-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 12:07:02.729459 mongo_db_operation-1.0.8/src/mongo_db_operation/__init__.py
--rw-r--r--   0        0        0      299 2023-04-21 12:07:02.729949 mongo_db_operation-1.0.8/src/mongo_db_operation/environment.py
--rw-r--r--   0        0        0     1958 2023-04-21 12:07:02.730318 mongo_db_operation-1.0.8/src/mongo_db_operation/mongo_client.py
--rw-r--r--   0        0        0     9803 1970-01-01 00:00:00.000000 mongo_db_operation-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-19 13:31:34.962743 mongo_db_operation-1.0.9/LICENSE
+-rw-r--r--   0        0        0     8943 2023-04-21 12:42:32.282215 mongo_db_operation-1.0.9/README.md
+-rw-r--r--   0        0        0      643 2023-04-21 21:18:43.421835 mongo_db_operation-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 12:07:02.729459 mongo_db_operation-1.0.9/src/mongo_db_operation/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-21 12:07:02.729949 mongo_db_operation-1.0.9/src/mongo_db_operation/environment.py
+-rw-r--r--   0        0        0     1982 2023-04-21 21:17:18.650122 mongo_db_operation-1.0.9/src/mongo_db_operation/mongo_client.py
+-rw-r--r--   0        0        0     9803 1970-01-01 00:00:00.000000 mongo_db_operation-1.0.9/PKG-INFO
```

### Comparing `mongo_db_operation-1.0.8/LICENSE` & `mongo_db_operation-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo_db_operation-1.0.8/README.md` & `mongo_db_operation-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mongo_db_operation-1.0.8/pyproject.toml` & `mongo_db_operation-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "mongo_db_operation"
-version = "1.0.8"
+version = "1.0.9"
 description = "A small package for CRUD operations for Mongo DB"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/mongo-db-operation"
 repository = "https://github.com/melihteke/mongo-db-operation"
 documentation = "https://github.com/melihteke/mongo-db-operation/blob/master/README.md"
```

### Comparing `mongo_db_operation-1.0.8/src/mongo_db_operation/mongo_client.py` & `mongo_db_operation-1.0.9/src/mongo_db_operation/mongo_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pymongo import MongoClient
 from bson.objectid import ObjectId
 
 class MongoDBOperation:
-    import environment
+    from mongo_db_operation import environment
     
     def __init__(self, uri=environment.DB_URI, db_name=environment.DB_NAME, collection_name=environment.DB_COLLECTION_NAME):
         try:
             self.client = MongoClient(uri)
             self.db = self.client.get_database(db_name)
             self.collection = self.db.get_collection(collection_name)
         except Exception as e:
```

### Comparing `mongo_db_operation-1.0.8/PKG-INFO` & `mongo_db_operation-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-db-operation
-Version: 1.0.8
+Version: 1.0.9
 Summary: A small package for CRUD operations for Mongo DB
 Home-page: https://github.com/melihteke/mongo-db-operation
 License: MIT
 Author: Melih Teke
 Author-email: me@mteke.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

