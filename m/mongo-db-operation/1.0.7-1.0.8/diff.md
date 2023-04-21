# Comparing `tmp/mongo_db_operation-1.0.7.tar.gz` & `tmp/mongo_db_operation-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_db_operation-1.0.7.tar", max compression
+gzip compressed data, was "mongo_db_operation-1.0.8.tar", max compression
```

## Comparing `mongo_db_operation-1.0.7.tar` & `mongo_db_operation-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-19 13:31:34.962743 mongo_db_operation-1.0.7/LICENSE
--rw-r--r--   0        0        0     8943 2023-04-21 12:42:32.282215 mongo_db_operation-1.0.7/README.md
--rw-r--r--   0        0        0      619 2023-04-21 20:54:30.388329 mongo_db_operation-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 12:07:02.729459 mongo_db_operation-1.0.7/src/mongo_db_operation/__init__.py
--rw-r--r--   0        0        0      299 2023-04-21 12:07:02.729949 mongo_db_operation-1.0.7/src/mongo_db_operation/environment.py
--rw-r--r--   0        0        0     1958 2023-04-21 12:07:02.730318 mongo_db_operation-1.0.7/src/mongo_db_operation/mongo_client.py
--rw-r--r--   0        0        0     9814 1970-01-01 00:00:00.000000 mongo_db_operation-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-19 13:31:34.962743 mongo_db_operation-1.0.8/LICENSE
+-rw-r--r--   0        0        0     8943 2023-04-21 12:42:32.282215 mongo_db_operation-1.0.8/README.md
+-rw-r--r--   0        0        0      643 2023-04-21 21:11:35.251001 mongo_db_operation-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 12:07:02.729459 mongo_db_operation-1.0.8/src/mongo_db_operation/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-21 12:07:02.729949 mongo_db_operation-1.0.8/src/mongo_db_operation/environment.py
+-rw-r--r--   0        0        0     1958 2023-04-21 12:07:02.730318 mongo_db_operation-1.0.8/src/mongo_db_operation/mongo_client.py
+-rw-r--r--   0        0        0     9803 1970-01-01 00:00:00.000000 mongo_db_operation-1.0.8/PKG-INFO
```

### Comparing `mongo_db_operation-1.0.7/LICENSE` & `mongo_db_operation-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo_db_operation-1.0.7/README.md` & `mongo_db_operation-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mongo_db_operation-1.0.7/pyproject.toml` & `mongo_db_operation-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "mongo_db_operation"
-version = "1.0.7"
+version = "1.0.8"
 description = "A small package for CRUD operations for Mongo DB"
 authors = ["Melih Teke <me@mteke.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/melihteke/mongo-db-operation"
 repository = "https://github.com/melihteke/mongo-db-operation"
 documentation = "https://github.com/melihteke/mongo-db-operation/blob/master/README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pymongo = "^3.12.0"
+python-dotenv = "1.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
```

### Comparing `mongo_db_operation-1.0.7/src/mongo_db_operation/mongo_client.py` & `mongo_db_operation-1.0.8/src/mongo_db_operation/mongo_client.py`

 * *Files identical despite different names*

### Comparing `mongo_db_operation-1.0.7/PKG-INFO` & `mongo_db_operation-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mongo-db-operation
-Version: 1.0.7
+Version: 1.0.8
 Summary: A small package for CRUD operations for Mongo DB
 Home-page: https://github.com/melihteke/mongo-db-operation
 License: MIT
 Author: Melih Teke
 Author-email: me@mteke.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pymongo (>=3.12.0,<4.0.0)
+Requires-Dist: python-dotenv (==1.0.0)
 Project-URL: Documentation, https://github.com/melihteke/mongo-db-operation/blob/master/README.md
 Project-URL: Repository, https://github.com/melihteke/mongo-db-operation
 Description-Content-Type: text/markdown
 
 ## MongoDB Python CRUD Operations
 
 This project offers an easy-to-use Python interface that enables you to perform CRUD (Create, Read, Update, Delete) operations on a MongoDB database. It uses the PyMongo library and is designed to work seamlessly with a prebuilt MongoDB instance installed on your system or hosted elsewhere.
```

