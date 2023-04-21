# Comparing `tmp/Anilist-0.1.0.tar.gz` & `tmp/Anilist-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.1.0.tar", last modified: Thu Apr 20 00:23:22 2023, max compression
+gzip compressed data, was "Anilist-0.2.0.tar", last modified: Thu Apr 20 22:10:33 2023, max compression
```

## Comparing `Anilist-0.1.0.tar` & `Anilist-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.258311 Anilist-0.1.0/
--rw-rw-rw-   0        0        0      494 2023-04-20 00:23:22.242321 Anilist-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-20 00:19:09.000000 Anilist-0.1.0/README.md
--rw-rw-rw-   0        0        0      601 2023-04-20 00:19:55.000000 Anilist-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 00:23:22.258311 Anilist-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.195351 Anilist-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.208341 Anilist-0.1.0/src/Anilist/
--rw-rw-rw-   0        0        0       90 2023-04-19 22:57:01.000000 Anilist-0.1.0/src/Anilist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.231328 Anilist-0.1.0/src/Anilist/auth/
--rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.1.0/src/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.1.0/src/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      497 2023-04-19 21:18:07.000000 Anilist-0.1.0/src/Anilist/auth/token.py
--rw-rw-rw-   0        0        0     1583 2023-04-20 00:00:36.000000 Anilist-0.1.0/src/Anilist/client.py
--rw-rw-rw-   0        0        0       51 2023-04-19 21:07:09.000000 Anilist-0.1.0/src/Anilist/consts.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.235325 Anilist-0.1.0/src/Anilist/mutation/
--rw-rw-rw-   0        0        0        0 2023-04-19 21:32:11.000000 Anilist-0.1.0/src/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.1.0/src/Anilist/mutation/media_list.py
--rw-rw-rw-   0        0        0      599 2023-04-20 00:05:42.000000 Anilist-0.1.0/src/Anilist/obj.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.239323 Anilist-0.1.0/src/Anilist/query/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:42:28.000000 Anilist-0.1.0/src/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0     1695 2023-04-20 00:06:44.000000 Anilist-0.1.0/src/Anilist/query/media_list.py
-drwxrwxrwx   0        0        0        0 2023-04-20 00:23:22.225332 Anilist-0.1.0/src/Anilist.egg-info/
--rw-rw-rw-   0        0        0      494 2023-04-20 00:23:22.000000 Anilist-0.1.0/src/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-20 00:23:22.000000 Anilist-0.1.0/src/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 00:23:22.000000 Anilist-0.1.0/src/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 00:23:22.000000 Anilist-0.1.0/src/Anilist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.741804 Anilist-0.2.0/
+-rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-04-20 22:10:33.740802 Anilist-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.2.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-20 22:10:03.000000 Anilist-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 22:10:33.742800 Anilist-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.695988 Anilist-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.710978 Anilist-0.2.0/src/Anilist/
+-rw-rw-rw-   0        0        0      127 2023-04-20 21:56:55.000000 Anilist-0.2.0/src/Anilist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.732965 Anilist-0.2.0/src/Anilist/auth/
+-rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.2.0/src/Anilist/auth/auth.py
+-rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.2.0/src/Anilist/auth/code.py
+-rw-rw-rw-   0        0        0      497 2023-04-19 21:18:07.000000 Anilist-0.2.0/src/Anilist/auth/token.py
+-rw-rw-rw-   0        0        0     2166 2023-04-20 22:04:46.000000 Anilist-0.2.0/src/Anilist/client.py
+-rw-rw-rw-   0        0        0       51 2023-04-19 21:07:09.000000 Anilist-0.2.0/src/Anilist/consts.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.2.0/src/Anilist/logging.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.735963 Anilist-0.2.0/src/Anilist/mutation/
+-rw-rw-rw-   0        0        0        0 2023-04-19 21:32:11.000000 Anilist-0.2.0/src/Anilist/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.2.0/src/Anilist/mutation/media_list.py
+-rw-rw-rw-   0        0        0      599 2023-04-20 21:27:29.000000 Anilist-0.2.0/src/Anilist/obj.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.738799 Anilist-0.2.0/src/Anilist/query/
+-rw-rw-rw-   0        0        0        0 2023-04-19 23:42:28.000000 Anilist-0.2.0/src/Anilist/query/__init__.py
+-rw-rw-rw-   0        0        0     1933 2023-04-20 21:27:54.000000 Anilist-0.2.0/src/Anilist/query/media_list.py
+-rw-rw-rw-   0        0        0     1498 2023-04-20 21:17:57.000000 Anilist-0.2.0/src/Anilist/scheme.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.728967 Anilist-0.2.0/src/Anilist.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.739803 Anilist-0.2.0/tests/
+-rw-rw-rw-   0        0        0      294 2023-04-20 22:04:12.000000 Anilist-0.2.0/tests/test_base.py
```

### Comparing `Anilist-0.1.0/pyproject.toml` & `Anilist-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Anilist"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
 ]
 description = "Anilist API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `Anilist-0.1.0/src/Anilist/auth/auth.py` & `Anilist-0.2.0/src/Anilist/auth/auth.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.1.0/src/Anilist/auth/code.py` & `Anilist-0.2.0/src/Anilist/auth/code.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.1.0/src/Anilist/mutation/media_list.py` & `Anilist-0.2.0/src/Anilist/mutation/media_list.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.1.0/src/Anilist/obj.py` & `Anilist-0.2.0/src/Anilist/obj.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.1.0/src/Anilist/query/media_list.py` & `Anilist-0.2.0/src/Anilist/query/media_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,48 @@
+from Anilist.scheme import MediaScheme, Scheme
 class MediaListQuery:
     
-    def __init__(self, client, username: str, per_page: int=10, starting_page: int = 1, languages=["english"]):
+    def __init__(self, client, username: str, per_page: int=10, starting_page: int = 1, languages=["english"], sizes=["extraLarge"]):
         self._username = username
         self._per_page = per_page
         self._starting_page = starting_page
         self._languages = languages
         self._client = client
+        self._sizes = sizes
         self._media_entries = []
+        self.DEFAULT_QUERY = [
+            MediaScheme().id, 
+            *[MediaScheme().title[lang] for lang in self._languages], 
+            *[MediaScheme().coverImage[size] for size in self._sizes]
+        ]
         # load a few important values
         self._base_query()
 
     @property
     def entries(self):
         return self._media_entries
+    
+    def query(self, *schs, default=True):
+    
+        if default:
+            schs = list(schs)
+            schs.extend(self.DEFAULT_QUERY)
 
-    def _base_query(self):
+        return self._query(*schs)
+    
+    def _query(self, *schs):
         query = """
-        query ($usr: String, $page: Int, $perPage: Int) {
-            Page (page: $page, perPage: $perPage) {
-                mediaList (userName: $usr) {
-                    media {
-                        id
-                        title {
-                            --REP--
-                        }
-                        coverImage {
-                            extraLarge
-                            large
-                            medium
-                        }
-                    }
-                }
-            }
-        }
-        """.replace("--REP--", '\n'.join(self._languages))
+        query ($usr: String, $page: Int, $perPage: Int) {{
+            Page (page: $page, perPage: $perPage) {{
+                mediaList (userName: $usr) {{
+                    {0}
+                }}
+            }}
+        }}
+        """.format(Scheme._construct(*schs))
 
         vars = {
             "usr": self._username,
             "page": self._starting_page,
             "perPage": self._per_page
         }
 
@@ -53,7 +58,10 @@
             if data == []:
                 break
 
             pg += 1
             vars["page"] = pg
 
         self._media_entries = temp
+
+    def _base_query(self):
+        self.query(default=True)
```

