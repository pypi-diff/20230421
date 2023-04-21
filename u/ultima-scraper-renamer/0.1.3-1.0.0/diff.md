# Comparing `tmp/ultima_scraper_renamer-0.1.3.tar.gz` & `tmp/ultima_scraper_renamer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_renamer-0.1.3.tar", max compression
+gzip compressed data, was "ultima_scraper_renamer-1.0.0.tar", max compression
```

## Comparing `ultima_scraper_renamer-0.1.3.tar` & `ultima_scraper_renamer-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-0.1.3/README.md
--rw-r--r--   0        0        0      674 2023-03-14 05:51:52.241665 ultima_scraper_renamer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/py.typed
--rw-r--r--   0        0        0     8793 2023-03-07 05:09:45.193613 ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/reformat.py
--rw-r--r--   0        0        0     8403 2023-03-12 13:33:36.003308 ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/renamer.py
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 ultima_scraper_renamer-0.1.3/setup.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 ultima_scraper_renamer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.0.0/README.md
+-rw-r--r--   0        0        0      674 2023-04-20 23:22:36.713797 ultima_scraper_renamer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/py.typed
+-rw-r--r--   0        0        0     8793 2023-03-07 05:09:45.193613 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/reformat.py
+-rw-r--r--   0        0        0     8413 2023-03-25 23:23:34.019541 ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/renamer.py
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.0.0/setup.py
+-rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.0.0/PKG-INFO
```

### Comparing `ultima_scraper_renamer-0.1.3/pyproject.toml` & `ultima_scraper_renamer-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ultima-scraper-renamer"
-version = "0.1.3"
+version = "1.0.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 readme = "README.md"
 packages = [{include = "ultima_scraper_renamer"}]
 include = ["ultima_scraper_renamer/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tqdm = "^4.64.1"
 orjson = "^3.8.3"
-ultima-scraper-api = "^0.1.3"
-ultima-scraper-collection = "^0.1.3"
+ultima-scraper-api = "^1.0.0"
+ultima-scraper-collection = "^1.0.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
```

### Comparing `ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/reformat.py` & `ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/reformat.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_renamer-0.1.3/ultima_scraper_renamer/renamer.py` & `ultima_scraper_renamer-1.0.0/ultima_scraper_renamer/renamer.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         date=datetime.today(),
         date_format=site_settings.date_format,
         text_length=site_settings.text_length,
         directory=directory_manager.root_metadata_directory,
     )
     p_r.api_type = api_type
     result: list[ApiModel] = database_session.query(api_table_).all()
-    metadata = getattr(subscription.temp_scraped, api_type)
+    metadata = getattr(subscription.scrape_manager.scraped, api_type)
 
     await fix_directories(
         result,
         subscription,
         directory_manager,
         database_session,
         api_type,
```

### Comparing `ultima_scraper_renamer-0.1.3/setup.py` & `ultima_scraper_renamer-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['orjson>=3.8.3,<4.0.0',
  'tqdm>=4.64.1,<5.0.0',
- 'ultima-scraper-api>=0.1.3,<0.2.0',
- 'ultima-scraper-collection>=0.1.3,<0.2.0']
+ 'ultima-scraper-api>=1.0.0,<2.0.0',
+ 'ultima-scraper-collection>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'ultima-scraper-renamer',
-    'version': '0.1.3',
+    'version': '1.0.0',
     'description': '',
     'long_description': '',
     'author': 'DIGITALCRIMINALS',
     'author_email': '89371864+digitalcriminals@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ultima_scraper_renamer-0.1.3/PKG-INFO` & `ultima_scraper_renamer-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-renamer
-Version: 0.1.3
+Version: 1.0.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=0.1.3,<0.2.0)
-Requires-Dist: ultima-scraper-collection (>=0.1.3,<0.2.0)
+Requires-Dist: ultima-scraper-api (>=1.0.0,<2.0.0)
+Requires-Dist: ultima-scraper-collection (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
```

