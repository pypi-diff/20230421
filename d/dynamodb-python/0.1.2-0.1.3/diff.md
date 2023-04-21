# Comparing `tmp/dynamodb_python-0.1.2.tar.gz` & `tmp/dynamodb_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodb_python-0.1.2.tar", max compression
+gzip compressed data, was "dynamodb_python-0.1.3.tar", max compression
```

## Comparing `dynamodb_python-0.1.2.tar` & `dynamodb_python-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1495 2023-02-07 13:09:44.924264 dynamodb_python-0.1.2/LICENSE
--rw-r--r--   0        0        0     1474 2023-02-09 13:37:18.852506 dynamodb_python-0.1.2/README.md
--rw-r--r--   0        0        0       56 2023-02-09 14:14:11.884881 dynamodb_python-0.1.2/dynamodb_python/__init__.py
--rw-r--r--   0        0        0     1468 2023-02-09 14:12:45.570078 dynamodb_python-0.1.2/dynamodb_python/dynamodb.py
--rw-r--r--   0        0        0    15906 2023-02-09 14:13:17.449260 dynamodb_python-0.1.2/dynamodb_python/table.py
--rw-r--r--   0        0        0     2738 2023-02-09 13:37:18.854234 dynamodb_python-0.1.2/dynamodb_python/utils.py
--rw-r--r--   0        0        0     1125 2023-02-09 14:03:45.540892 dynamodb_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2228 1970-01-01 00:00:00.000000 dynamodb_python-0.1.2/setup.py
--rw-r--r--   0        0        0     2038 1970-01-01 00:00:00.000000 dynamodb_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-02-07 13:09:44.924264 dynamodb_python-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1515 2023-02-09 14:31:06.781872 dynamodb_python-0.1.3/README.md
+-rw-r--r--   0        0        0       56 2023-02-09 14:14:11.884881 dynamodb_python-0.1.3/dynamodb_python/__init__.py
+-rw-r--r--   0        0        0     1468 2023-02-09 14:12:45.570078 dynamodb_python-0.1.3/dynamodb_python/dynamodb.py
+-rw-r--r--   0        0        0    15906 2023-02-09 14:13:17.449260 dynamodb_python-0.1.3/dynamodb_python/table.py
+-rw-r--r--   0        0        0     2738 2023-02-09 13:37:18.854234 dynamodb_python-0.1.3/dynamodb_python/utils.py
+-rw-r--r--   0        0        0     1126 2023-04-21 12:44:30.342866 dynamodb_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 dynamodb_python-0.1.3/PKG-INFO
```

### Comparing `dynamodb_python-0.1.2/LICENSE` & `dynamodb_python-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodb_python-0.1.2/README.md` & `dynamodb_python-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # dynamodb-python
 
 ## Installation
 
+```bash
+pip install dynamodb-python
+```
+
 ## Requirements
 
 ### Dependencies
 
 - python = "^3.9"
 - ddbcereal
 - botocore
```

### Comparing `dynamodb_python-0.1.2/dynamodb_python/dynamodb.py` & `dynamodb_python-0.1.3/dynamodb_python/dynamodb.py`

 * *Files identical despite different names*

### Comparing `dynamodb_python-0.1.2/dynamodb_python/table.py` & `dynamodb_python-0.1.3/dynamodb_python/table.py`

 * *Files identical despite different names*

### Comparing `dynamodb_python-0.1.2/dynamodb_python/utils.py` & `dynamodb_python-0.1.3/dynamodb_python/utils.py`

 * *Files identical despite different names*

### Comparing `dynamodb_python-0.1.2/pyproject.toml` & `dynamodb_python-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dynamodb-python"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["domas-v <domas.vaitmonas93@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dynamodb_python"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 ddbcereal = "^2.1.1"
 botocore = "^1.29.65"
 boto3 = "^1.26.65"
 requests = "^2.28.2"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dynamodb_python-0.1.2/PKG-INFO` & `dynamodb_python-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: dynamodb-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: domas-v
 Author-email: domas.vaitmonas93@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.65,<2.0.0)
 Requires-Dist: botocore (>=1.29.65,<2.0.0)
 Requires-Dist: ddbcereal (>=2.1.1,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # dynamodb-python
 
 ## Installation
 
+```bash
+pip install dynamodb-python
+```
+
 ## Requirements
 
 ### Dependencies
 
 - python = "^3.9"
 - ddbcereal
 - botocore
```

