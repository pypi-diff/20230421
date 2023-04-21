# Comparing `tmp/canonicalwebteam.discourse-5.4.0.tar.gz` & `tmp/canonicalwebteam.discourse-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam.discourse-5.4.0.tar", last modified: Mon Apr  3 13:23:07 2023, max compression
+gzip compressed data, was "canonicalwebteam.discourse-5.4.1.tar", last modified: Fri Apr 21 14:02:48 2023, max compression
```

## Comparing `canonicalwebteam.discourse-5.4.0.tar` & `canonicalwebteam.discourse-5.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.260186 canonicalwebteam.discourse-5.4.0/canonicalwebteam/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.260186 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27302 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.260186 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-03 13:23:07.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-03 13:23:07.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 13:23:07.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 13:23:07.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-03 13:23:07.000000 canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:07.264186 canonicalwebteam.discourse-5.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/fixtures/forum_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/test_engage_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-03 13:23:02.000000 canonicalwebteam.discourse-5.4.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.118363 canonicalwebteam.discourse-5.4.1/canonicalwebteam/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20665 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25660 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27552 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.118363 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:02:48.000000 canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:48.122362 canonicalwebteam.discourse-5.4.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/fixtures/forum_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_engage_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-04-21 14:02:43.000000 canonicalwebteam.discourse-5.4.1/tests/test_parser.py
```

### Comparing `canonicalwebteam.discourse-5.4.0/LICENSE` & `canonicalwebteam.discourse-5.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/PKG-INFO` & `canonicalwebteam.discourse-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.discourse
-Version: 5.4.0
+Version: 5.4.1
 Summary: Flask extension to integrate discourse content generated to docs to your website.
 Home-page: https://github.com/canonical/canonicalwebteam.discourse
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canonicalwebteam.discourse-5.4.0/README.md` & `canonicalwebteam.discourse-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/app.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/exceptions.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/exceptions.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/models.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/models.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/base_parser.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/docs.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Standard library
+import copy
 import os
 import re
 from urllib.parse import urlparse
 
 # Packages
 import dateutil.parser
 import humanize
@@ -25,17 +26,17 @@
         self,
         api,
         index_topic_id,
         url_prefix,
         tutorials_index_topic_id=None,
         tutorials_url_prefix=None,
     ):
-        self.active_topic = None
+        self.active_topic_id = None
         self.versions = []
-        self.navigations = []
+        self.navigations = {}
         self.url_map_versions = {}
 
         # Tutorials
         self.tutorials_url_map = {}
         self.tutorials_index_topic_id = tutorials_index_topic_id
         self.tutorials_url_prefix = tutorials_url_prefix
 
@@ -95,15 +96,15 @@
         - title: The title
         - body_html: The HTML content of the initial topic post
                         (with some post-processing)
         - updated: A human-readable date, relative to now
                     (e.g. "3 days ago")
         - forum_link: The link to the original forum post
         """
-        self.active_topic = topic
+        self.active_topic_id = topic["id"]
 
         updated_datetime = dateutil.parser.parse(
             topic["post_stream"]["posts"][0]["updated_at"]
         )
 
         topic_path = f"/t/{topic['slug']}/{topic['id']}".replace("—", "--")
 
@@ -268,15 +269,17 @@
 
                 if not pretty_path.startswith("/"):
                     pretty_path = "/" + pretty_path
                 if not pretty_path.startswith(url_prefix):
                     pretty_path = url_prefix + pretty_path
 
                 if not topic_match or not pretty_path.startswith(url_prefix):
-                    self.warnings.append("Could not parse URL map item {item}")
+                    self.warnings.append(
+                        f"Could not parse URL map item {item}"
+                    )
                     continue
 
                 topic_id = int(topic_match.groupdict()["topic_id"])
 
                 url_map[version_path][pretty_path] = topic_id
 
             # Add the reverse mappings as well, for efficiency
@@ -549,15 +552,18 @@
                     item["has_active_child"] = True
                     return True
 
         item["has_active_child"] = False
         return False
 
     def _generate_navigation(self, navigations, version_path):
-        navigation = navigations[version_path]
+        # we mutate the navigations[version_path] dictionary and so to
+        # avoid retaining state between document views, we need to
+        # take a (deep)copy.
+        navigation = copy.deepcopy(navigations[version_path])
 
         # Replace links with url_map
         for item in navigation["nav_items"]:
             if item["navlink_href"] and self._match_url_with_topic(
                 item["navlink_href"]
             ):
                 topic_id = self._get_url_topic_id(item["navlink_href"])
@@ -566,15 +572,15 @@
                     fragment = item["navlink_fragment"]
                     if fragment:
                         item["navlink_href"] = f"{href}#{fragment}"
                     else:
                         item["navlink_href"] = href
 
                 # Check if given item should be marked as active
-                if topic_id == self.active_topic["id"]:
+                if topic_id == self.active_topic_id:
                     item["is_active"] = True
 
         # Generate tree structure with levels
         navigation["nav_items"] = self._process_nav_levels(
             navigation["nav_items"]
         )
```

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam/discourse/parsers/tutorials.py` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam/discourse/parsers/tutorials.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/PKG-INFO` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.discourse
-Version: 5.4.0
+Version: 5.4.1
 Summary: Flask extension to integrate discourse content generated to docs to your website.
 Home-page: https://github.com/canonical/canonicalwebteam.discourse
 Author: Canonical webteam
 Author-email: webteam@canonical.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `canonicalwebteam.discourse-5.4.0/canonicalwebteam.discourse.egg-info/SOURCES.txt` & `canonicalwebteam.discourse-5.4.1/canonicalwebteam.discourse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/setup.py` & `canonicalwebteam.discourse-5.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from setuptools import setup, find_packages
 
 setup(
     name="canonicalwebteam.discourse",
-    version="5.4.0",
+    version="5.4.1",
     author="Canonical webteam",
     author_email="webteam@canonical.com",
     url="https://github.com/canonical/canonicalwebteam.discourse",
     description=(
         "Flask extension to integrate discourse content generated "
         "to docs to your website."
     ),
```

### Comparing `canonicalwebteam.discourse-5.4.0/tests/fixtures/forum_mock.py` & `canonicalwebteam.discourse-5.4.1/tests/fixtures/forum_mock.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/tests/test_app.py` & `canonicalwebteam.discourse-5.4.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/tests/test_engage_pages.py` & `canonicalwebteam.discourse-5.4.1/tests/test_engage_pages.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/tests/test_models.py` & `canonicalwebteam.discourse-5.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam.discourse-5.4.0/tests/test_parser.py` & `canonicalwebteam.discourse-5.4.1/tests/test_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -288,14 +288,68 @@
         page_a = navigation["nav_items"][0]
         self.assertEqual(page_a["path"], "/a")
         self.assertEqual(page_a["navlink_text"], "Page A")
         page_z = page_a["children"][0]
         self.assertEqual(page_z["path"], "/page-z")
         self.assertEqual(page_z["navlink_text"], "Page Z")
 
+    def test_active_topic(self):
+        for page_id in [10, 26]:
+            httpretty.register_uri(
+                httpretty.GET,
+                f"https://discourse.example.com/t/{page_id}.json",
+                body=json.dumps(
+                    {
+                        "id": page_id,
+                        "category_id": 2,
+                        "title": "A topic page",
+                        "slug": "a-page",
+                        "post_stream": {
+                            "posts": [
+                                {
+                                    "id": 3434,
+                                    "cooked": "<h1>Content</h1>",
+                                    "updated_at": "2023-04-01T12:34:56.789Z",
+                                }
+                            ]
+                        },
+                    }
+                ),
+                content_type="application/json",
+            )
+        self.assertEqual(self.parser.active_topic_id, 34)
+        root_navigation = self.parser.navigation
+
+        root_page_a = root_navigation["nav_items"][0]
+        self.assertFalse(root_page_a["is_active"])
+        self.assertFalse(root_page_a["has_active_child"])
+
+        # Simulate clicking on child page
+        self.parser.parse_topic(self.parser.api.get_topic(10))
+        self.assertEqual(self.parser.active_topic_id, 10)
+        child = self.parser.navigation["nav_items"][0]
+        self.assertTrue(child["is_active"])
+        self.assertFalse(child["has_active_child"])
+
+        # Simulate clicking on grand-child page
+        self.parser.parse_topic(self.parser.api.get_topic(26))
+        self.assertEqual(self.parser.active_topic_id, 26)
+        child = self.parser.navigation["nav_items"][0]
+        self.assertFalse(child["is_active"])
+        self.assertTrue(child["has_active_child"])
+        grandchild = child["children"][0]
+        self.assertTrue(grandchild["is_active"])
+        self.assertFalse(grandchild["has_active_child"])
+
+        # Simulate clicking on root
+        self.parser.parse_topic(self.parser.index_topic)
+        child = self.parser.navigation["nav_items"][0]
+        self.assertFalse(child["is_active"])
+        self.assertFalse(child["has_active_child"])
+
     def test_versions(self):
         versions = self.parser.versions
         self.assertEqual(len(versions), 1)
         version = versions[0]
         self.assertEqual(version["index"], int(self.parser.index_topic_id))
         self.assertEqual(version["path"], "")
         self.assertEqual(version["version"], "latest")
```

