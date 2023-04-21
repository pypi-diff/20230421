# Comparing `tmp/databudgie-2.7.4.tar.gz` & `tmp/databudgie-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databudgie-2.7.4.tar", max compression
+gzip compressed data, was "databudgie-2.7.5.tar", max compression
```

## Comparing `databudgie-2.7.4.tar` & `databudgie-2.7.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     5139 2023-04-21 18:37:32.911767 databudgie-2.7.4/CHANGELOG.md
--rw-r--r--   0        0        0     1973 2023-04-21 18:37:32.911767 databudgie-2.7.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1053 2023-04-21 18:37:32.911767 databudgie-2.7.4/LICENSE
--rw-r--r--   0        0        0     1292 2023-04-21 18:37:32.911767 databudgie-2.7.4/README.md
--rw-r--r--   0        0        0     2879 2023-04-21 18:37:32.911767 databudgie-2.7.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/__init__.py
--rw-r--r--   0        0        0       69 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/__main__.py
--rw-r--r--   0        0        0       74 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/adapter/__init__.py
--rw-r--r--   0        0        0     7162 2023-04-21 18:37:32.911767 databudgie-2.7.4/src/databudgie/adapter/base.py
--rw-r--r--   0        0        0    10638 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/adapter/postgres.py
--rw-r--r--   0        0        0     7361 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/backup.py
--rw-r--r--   0        0        0      105 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/__init__.py
--rw-r--r--   0        0        0     2896 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/base.py
--rw-r--r--   0        0        0     6458 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/commands.py
--rw-r--r--   0        0        0     1473 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/config.py
--rw-r--r--   0        0        0      456 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/cli/setup.py
--rw-r--r--   0        0        0     1112 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/compression.py
--rw-r--r--   0        0        0    11862 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/config.py
--rw-r--r--   0        0        0      105 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/__init__.py
--rw-r--r--   0        0        0     2348 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/manager.py
--rw-r--r--   0        0        0     1602 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/manifest/sqlalchemy.py
--rw-r--r--   0        0        0      565 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/match.py
--rw-r--r--   0        0        0     1564 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/output.py
--rw-r--r--   0        0        0        0 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/py.typed
--rw-r--r--   0        0        0     8408 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/restore.py
--rw-r--r--   0        0        0     1948 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/s3.py
--rw-r--r--   0        0        0    11806 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/storage.py
--rw-r--r--   0        0        0     4586 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/table_op.py
--rw-r--r--   0        0        0     2320 2023-04-21 18:37:32.915767 databudgie-2.7.4/src/databudgie/utils.py
--rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 databudgie-2.7.4/setup.py
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 databudgie-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0     5139 2023-04-21 19:04:42.269454 databudgie-2.7.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1973 2023-04-21 19:04:42.269454 databudgie-2.7.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1053 2023-04-21 19:04:42.269454 databudgie-2.7.5/LICENSE
+-rw-r--r--   0        0        0     1292 2023-04-21 19:04:42.269454 databudgie-2.7.5/README.md
+-rw-r--r--   0        0        0     2879 2023-04-21 19:04:42.269454 databudgie-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-21 19:04:42.269454 databudgie-2.7.5/src/databudgie/__init__.py
+-rw-r--r--   0        0        0       69 2023-04-21 19:04:42.269454 databudgie-2.7.5/src/databudgie/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/__init__.py
+-rw-r--r--   0        0        0     7162 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/base.py
+-rw-r--r--   0        0        0    10638 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/adapter/postgres.py
+-rw-r--r--   0        0        0     7361 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/backup.py
+-rw-r--r--   0        0        0      105 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/__init__.py
+-rw-r--r--   0        0        0     2896 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/base.py
+-rw-r--r--   0        0        0     6458 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/commands.py
+-rw-r--r--   0        0        0     1473 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/config.py
+-rw-r--r--   0        0        0      456 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/cli/setup.py
+-rw-r--r--   0        0        0     1112 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/compression.py
+-rw-r--r--   0        0        0    11862 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/config.py
+-rw-r--r--   0        0        0      105 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/__init__.py
+-rw-r--r--   0        0        0     2348 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/manager.py
+-rw-r--r--   0        0        0     1602 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/manifest/sqlalchemy.py
+-rw-r--r--   0        0        0      565 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/match.py
+-rw-r--r--   0        0        0     1564 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/output.py
+-rw-r--r--   0        0        0        0 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/py.typed
+-rw-r--r--   0        0        0     8408 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/restore.py
+-rw-r--r--   0        0        0     1948 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/s3.py
+-rw-r--r--   0        0        0    11806 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/storage.py
+-rw-r--r--   0        0        0     4586 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/table_op.py
+-rw-r--r--   0        0        0     2462 2023-04-21 19:04:42.273454 databudgie-2.7.5/src/databudgie/utils.py
+-rw-r--r--   0        0        0     2589 1970-01-01 00:00:00.000000 databudgie-2.7.5/setup.py
+-rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 databudgie-2.7.5/PKG-INFO
```

### Comparing `databudgie-2.7.4/CHANGELOG.md` & `databudgie-2.7.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/CONTRIBUTING.md` & `databudgie-2.7.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/LICENSE` & `databudgie-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/README.md` & `databudgie-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/pyproject.toml` & `databudgie-2.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databudgie"
-version = "2.7.4"
+version = "2.7.5"
 packages = [
     { include = "databudgie", from = "src" },
 ]
 
 authors = [
   "Andrew Sosa <andrewso@known.is>",
   "Dan Cardin <ddcardin@gmail.com>",
```

### Comparing `databudgie-2.7.4/src/databudgie/adapter/base.py` & `databudgie-2.7.5/src/databudgie/adapter/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/adapter/postgres.py` & `databudgie-2.7.5/src/databudgie/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/backup.py` & `databudgie-2.7.5/src/databudgie/backup.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/cli/base.py` & `databudgie-2.7.5/src/databudgie/cli/base.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/cli/commands.py` & `databudgie-2.7.5/src/databudgie/cli/commands.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/cli/config.py` & `databudgie-2.7.5/src/databudgie/cli/config.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/compression.py` & `databudgie-2.7.5/src/databudgie/compression.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/config.py` & `databudgie-2.7.5/src/databudgie/config.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/manifest/manager.py` & `databudgie-2.7.5/src/databudgie/manifest/manager.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/manifest/sqlalchemy.py` & `databudgie-2.7.5/src/databudgie/manifest/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/match.py` & `databudgie-2.7.5/src/databudgie/match.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/output.py` & `databudgie-2.7.5/src/databudgie/output.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/restore.py` & `databudgie-2.7.5/src/databudgie/restore.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/s3.py` & `databudgie-2.7.5/src/databudgie/s3.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/storage.py` & `databudgie-2.7.5/src/databudgie/storage.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/table_op.py` & `databudgie-2.7.5/src/databudgie/table_op.py`

 * *Files identical despite different names*

### Comparing `databudgie-2.7.4/src/databudgie/utils.py` & `databudgie-2.7.5/src/databudgie/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,9 +78,17 @@
     if not real_components:
         return ""
 
     if len(real_components) == 1:
         return real_components[0]
 
     first_component, *rest_components = real_components
-    normalized_components = [S3Location(c).key if is_s3_path(c) else c for c in rest_components]
+    normalized_components = []
+    for c in rest_components:
+        if is_s3_path(c):
+            normalized_c = S3Location(c).key
+        else:
+            normalized_c = c.strip("/")
+
+        normalized_components.append(normalized_c)
+
     return os.path.join(first_component, *normalized_components)
```

### Comparing `databudgie-2.7.4/setup.py` & `databudgie-2.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'sentry': ['sentry-sdk']}
 
 entry_points = \
 {'console_scripts': ['databudgie = databudgie.__main__:run']}
 
 setup_kwargs = {
     'name': 'databudgie',
-    'version': '2.7.4',
+    'version': '2.7.5',
     'description': 'Ergonomic and flexible tool for database backup and restore',
     'long_description': '# Databudgie\n\n![Github Actions Build](https://github.com/schireson/databudgie/actions/workflows/build.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/schireson/databudgie/badge.svg?branch=main&t=6I0aU6)](https://coveralls.io/github/schireson/databudgie?branch=main)\n[![Documentation\nStatus](https://readthedocs.org/projects/databudgie/badge/?version=latest)](https://databudgie.readthedocs.io)\n\n![](docs/source/_static/databudgie.png)\n\nDatabudgie is a CLI & library for database performing targeted backup and restore\nof database tables or arbitrary queries against database tables.\n\n# Usage\n\nA minimal config file might look like:\n\n```yaml\n# config.databudgie.yml\nbackup:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      query: "select * from {table} where store_id > 4"\n      location: s3://my-s3-bucket/databudgie/public.product\nrestore:\n  url: postgresql://postgres:postgres@localhost:5432/postgres\n  tables:\n    - name: public.product\n      location: s3://my-s3-bucket/databudgie/public.product\n```\n\nWith that config in place, backing up the defined tables (using the specified config)\nis as simple as `databudgie backup`; and restore `databudgie restore`.\n\n## Installation\n\n```bash\npip install databudgie\n```\n',
     'author': 'Andrew Sosa',
     'author_email': 'andrewso@known.is',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/databudgie',
```

### Comparing `databudgie-2.7.4/PKG-INFO` & `databudgie-2.7.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databudgie
-Version: 2.7.4
+Version: 2.7.5
 Summary: Ergonomic and flexible tool for database backup and restore
 Home-page: https://github.com/schireson/databudgie
 License: MIT
 Keywords: sqlalchemy,postgres,database,etl,s3
 Author: Andrew Sosa
 Author-email: andrewso@known.is
 Requires-Python: >=3.7,<4
```

