# Comparing `tmp/notion-database-20220628.6.tar.gz` & `tmp/notion-database-20220628.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-database-20220628.6.tar", last modified: Wed Mar  1 13:04:53 2023, max compression
+gzip compressed data, was "notion-database-20220628.7.tar", last modified: Fri Apr 21 14:11:10 2023, max compression
```

## Comparing `notion-database-20220628.6.tar` & `notion-database-20220628.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-03-01 13:04:53.049202 notion-database-20220628.6/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    35148 2023-02-10 08:27:15.000000 notion-database-20220628.6/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-03-01 13:04:53.048872 notion-database-20220628.6/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1427 2023-02-10 08:27:15.000000 notion-database-20220628.6/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)       38 2023-03-01 13:04:53.049356 notion-database-20220628.6/setup.cfg
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1038 2023-03-01 13:03:39.000000 notion-database-20220628.6/setup.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-03-01 13:04:53.040151 notion-database-20220628.6/src/
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-03-01 13:04:53.046095 notion-database-20220628.6/src/notion_database/
--rw-r--r--   0 minwook-shin   (501) staff       (20)       30 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11957 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/children.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      497 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/color.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4843 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/database.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2661 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/page.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     5642 2023-03-01 13:03:39.000000 notion-database-20220628.6/src/notion_database/properties.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      459 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/query.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1266 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/request.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2816 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/notion_database/search.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-03-01 13:04:53.047802 notion-database-20220628.6/src/notion_database.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-03-01 13:04:52.000000 notion-database-20220628.6/src/notion_database.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      562 2023-03-01 13:04:52.000000 notion-database-20220628.6/src/notion_database.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-03-01 13:04:52.000000 notion-database-20220628.6/src/notion_database.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       42 2023-03-01 13:04:52.000000 notion-database-20220628.6/src/notion_database.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       22 2023-03-01 13:04:52.000000 notion-database-20220628.6/src/notion_database.egg-info/top_level.txt
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-03-01 13:04:53.048410 notion-database-20220628.6/src/utils/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/utils/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)      469 2023-02-10 08:27:15.000000 notion-database-20220628.6/src/utils/deprecate.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.011622 notion-database-20220628.7/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    35148 2023-02-10 08:27:15.000000 notion-database-20220628.7/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:11:10.011260 notion-database-20220628.7/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1427 2023-02-10 08:27:15.000000 notion-database-20220628.7/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       38 2023-04-21 14:11:10.011767 notion-database-20220628.7/setup.cfg
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1038 2023-04-21 13:57:04.000000 notion-database-20220628.7/setup.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:09.997581 notion-database-20220628.7/src/
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.007270 notion-database-20220628.7/src/notion_database/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       30 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11957 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/children.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      497 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/color.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      641 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/cover.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     5340 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/database.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      979 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/icon.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3134 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/page.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     5722 2023-04-21 13:57:04.000000 notion-database-20220628.7/src/notion_database/properties.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      459 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/query.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1266 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/request.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2816 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/notion_database/search.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.009696 notion-database-20220628.7/src/notion_database.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1999 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      619 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       42 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       22 2023-04-21 14:11:09.000000 notion-database-20220628.7/src/notion_database.egg-info/top_level.txt
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-04-21 14:11:10.010432 notion-database-20220628.7/src/utils/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/utils/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      469 2023-02-10 08:27:15.000000 notion-database-20220628.7/src/utils/deprecate.py
```

### Comparing `notion-database-20220628.6/LICENSE` & `notion-database-20220628.7/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.6/PKG-INFO` & `notion-database-20220628.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-database
-Version: 20220628.6
+Version: 20220628.7
 Summary:  Notion API Database Python Implementation
 Home-page: https://github.com/minwook-shin/notion-database
 Author: minwook-shin
 Author-email: minwook0106@gmail.com
 Project-URL: Bug Tracker, https://github.com/minwook-shin/notion-database/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notion-database-20220628.6/README.md` & `notion-database-20220628.7/README.md`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.6/setup.py` & `notion-database-20220628.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from src.notion_database import NOTION_VERSION
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="notion-database",
-    version=NOTION_VERSION.replace("-", "") + ".6",
+    version=NOTION_VERSION.replace("-", "") + ".7",
     author="minwook-shin",
     author_email="minwook0106@gmail.com",
     description=" Notion API Database Python Implementation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/minwook-shin/notion-database",
     project_urls={
```

### Comparing `notion-database-20220628.6/src/notion_database/children.py` & `notion-database-20220628.7/src/notion_database/children.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.6/src/notion_database/database.py` & `notion-database-20220628.7/src/notion_database/database.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from utils import deprecate
 
 from notion_database.properties import Properties
 from notion_database.request import Request
 
+from src.notion_database.cover import Cover
+from src.notion_database.icon import Icon
+
 
 class Database:
     def __init__(self, integrations_token):
         """
         init
 
         :param integrations_token: Notion Internal Integration Token
@@ -75,21 +78,23 @@
 
         :param page_size: The number of items from the full list desired in the response.
         :return:
         """
         url = self.url + f"?page_size={str(page_size)}"
         self.result = self.request.call_api_get(url)
 
-    def create_database(self, page_id, title, properties=None):
+    def create_database(self, page_id, title, properties=None, cover: Cover = None, icon: Icon = None):
         """
         Create a database
 
         :param page_id: Notion Page ID
         :param title: Title of database as it appears in Notion
         :param properties: Property schema of database
+        :param cover:
+        :param icon:
         :return:
         """
         if properties is None:
             properties = Properties()
         properties = properties
         body = {
             "parent": {
@@ -103,24 +108,31 @@
                         "content": title,
                         "link": None
                     }
                 }
             ],
             "properties": properties.result
         }
+        if cover:
+            body.update(cover.result)
+        if icon:
+            body.update(icon.result)
         self.result = self.request.call_api_post(self.url, body)
 
-    def update_database(self, database_id, title=None, remove_properties=None, add_properties=None):
+    def update_database(self, database_id, title=None, remove_properties=None, add_properties=None,
+                        cover: Cover = None, icon: Icon = None):
         """
         Update database
 
         :param database_id: Identifier for a Notion database
         :param title: Title of database as it appears in Notion
         :param remove_properties: Removal Property schema of database
         :param add_properties: Property schema of database
+        :param cover:
+        :param icon:
         :return:
         """
         if add_properties is None:
             add_properties = Properties()
         body = {
             "properties": {}
         }
@@ -130,14 +142,18 @@
                     "type": "text",
                     "text": {
                         "content": title,
                         "link": None
                     }
                 }
             ]
+        if cover:
+            body.update(cover.result)
+        if icon:
+            body.update(icon.result)
         if remove_properties:
             body["properties"].update({i["id"]: None for i in remove_properties})
             self.result = self.request.call_api_patch(self.url + "/" + database_id, body)
             body["properties"] = {}
         if add_properties:
             body["properties"].update(add_properties.result)
             self.result = self.request.call_api_patch(self.url + "/" + database_id, body)
```

### Comparing `notion-database-20220628.6/src/notion_database/page.py` & `notion-database-20220628.7/src/notion_database/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 
 from notion_database.children import Children
 from notion_database.properties import Properties
 from notion_database.request import Request
 
+from src.notion_database.cover import Cover
+from src.notion_database.icon import Icon
+
 LOGGER = logging.getLogger("Notion-Database")
 
 
 class Page:
     def __init__(self, integrations_token):
         """
         init
@@ -23,21 +26,23 @@
         Retrieve a page
 
         :param page_id: Identifier for a Notion page
         :return:
         """
         self.result = self.request.call_api_get(self.url + "/" + page_id)
 
-    def create_page(self, database_id, properties=None, children=None):
+    def create_page(self, database_id, properties=None, children=None, cover: Cover = None, icon: Icon = None):
         """
         Create a page
 
         :param database_id: Identifier for a Notion database
         :param properties: Property values of this page
         :param children: Page content for the new page
+        :param cover:
+        :param icon:
         :return:
         """
         if children is None:
             children = Children()
         if properties is None:
             properties = Properties()
         properties = properties
@@ -45,31 +50,41 @@
         body = {
             "parent": {
                 "database_id": database_id
             },
             "properties": properties.result,
             "children": children.result
         }
+        if cover:
+            body.update(cover.result)
+        if icon:
+            body.update(icon.result)
         self.result = self.request.call_api_post(self.url, body)
 
         self.check_field()
 
-    def update_page(self, page_id, properties=None):
+    def update_page(self, page_id, properties=None, cover: Cover = None, icon: Icon = None):
         """
         Update page
 
         :param page_id: Identifier for a Notion page
         :param properties: Property values to update for this page
+        :param cover:
+        :param icon:
         :return:
         """
         if properties is None:
             properties = Properties()
         body = {
             "properties": properties.result,
         }
+        if cover:
+            body.update(cover.result)
+        if icon:
+            body.update(icon.result)
         self.result = self.request.call_api_patch(self.url + "/" + page_id, body)
 
         self.check_field()
 
     def archive_page(self, page_id, archived):
         """
         Archive page
```

### Comparing `notion-database-20220628.6/src/notion_database/properties.py` & `notion-database-20220628.7/src/notion_database/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
         """
         title configuration
 
         :param col: column name
         :param text: page text. If no text is given, for database only.
         :return:
         """
-        if text:
+        if (text is not None) and isinstance(text, str):
             text = [{"text": {"content": text}}]
         else:
             text = {}
         self.result.update({col: {"title": text}})
 
     def set_rich_text(self, col, text=None):
         """
         rich_text configuration
 
         :param col: column name
         :param text: page text. If no text is given, for database only.
         :return:
         """
-        if text:
+        if (text is not None) and isinstance(text, str):
             text = [{"text": {"content": text}}]
         else:
             text = {}
         self.result.update({col: {"rich_text": text}})
 
     def set_number(self, col, text=None):
         """
```

### Comparing `notion-database-20220628.6/src/notion_database/request.py` & `notion-database-20220628.7/src/notion_database/request.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.6/src/notion_database/search.py` & `notion-database-20220628.7/src/notion_database/search.py`

 * *Files identical despite different names*

### Comparing `notion-database-20220628.6/src/notion_database.egg-info/PKG-INFO` & `notion-database-20220628.7/src/notion_database.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-database
-Version: 20220628.6
+Version: 20220628.7
 Summary:  Notion API Database Python Implementation
 Home-page: https://github.com/minwook-shin/notion-database
 Author: minwook-shin
 Author-email: minwook0106@gmail.com
 Project-URL: Bug Tracker, https://github.com/minwook-shin/notion-database/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `notion-database-20220628.6/src/notion_database.egg-info/SOURCES.txt` & `notion-database-20220628.7/src/notion_database.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 setup.py
 src/notion_database/__init__.py
 src/notion_database/children.py
 src/notion_database/color.py
+src/notion_database/cover.py
 src/notion_database/database.py
+src/notion_database/icon.py
 src/notion_database/page.py
 src/notion_database/properties.py
 src/notion_database/query.py
 src/notion_database/request.py
 src/notion_database/search.py
 src/notion_database.egg-info/PKG-INFO
 src/notion_database.egg-info/SOURCES.txt
```

