# Comparing `tmp/symdexer-0.2.7.tar.gz` & `tmp/symdexer-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-w72jevhj\symdexer-0.2.7.tar", last modified: Thu Apr 20 20:09:43 2023, max compression
+gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-gyn7ct2f\symdexer-0.2.8.tar", last modified: Fri Apr 21 01:44:53 2023, max compression
```

## Comparing `symdexer-0.2.7.tar` & `symdexer-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:09:43.000000 symdexer-0.2.7/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0      634 2023-04-20 20:09:43.000000 symdexer-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.7/README.md
--rw-rw-rw-   0        0        0      592 2023-04-20 20:07:32.000000 symdexer-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 20:09:43.000000 symdexer-0.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.7/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-20 19:57:17.000000 symdexer-0.2.7/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0       38 2023-04-20 20:08:19.000000 symdexer-0.2.7/src/symdexer/__version__.py
--rw-rw-rw-   0        0        0     3774 2023-04-20 19:53:13.000000 symdexer-0.2.7/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     1049 2023-04-20 00:08:33.000000 symdexer-0.2.7/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     3565 2023-04-20 19:56:53.000000 symdexer-0.2.7/src/symdexer/parser.py
--rw-rw-rw-   0        0        0     1038 2023-04-20 19:11:11.000000 symdexer-0.2.7/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 20:09:43.000000 symdexer-0.2.7/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      634 2023-04-21 01:44:53.000000 symdexer-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.8/README.md
+-rw-rw-rw-   0        0        0      592 2023-04-21 01:44:09.000000 symdexer-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:44:53.000000 symdexer-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.8/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-04-21 01:43:55.000000 symdexer-0.2.8/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0       38 2023-04-21 01:44:17.000000 symdexer-0.2.8/src/symdexer/__version__.py
+-rw-rw-rw-   0        0        0     3686 2023-04-21 01:43:32.000000 symdexer-0.2.8/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     1049 2023-04-20 00:08:33.000000 symdexer-0.2.8/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     3565 2023-04-20 19:56:53.000000 symdexer-0.2.8/src/symdexer/parser.py
+-rw-rw-rw-   0        0        0     1038 2023-04-20 19:11:11.000000 symdexer-0.2.8/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/top_level.txt
```

### Comparing `symdexer-0.2.7/LICENSE.txt` & `symdexer-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.7/PKG-INFO` & `symdexer-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.7
+Version: 0.2.8
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `symdexer-0.2.7/pyproject.toml` & `symdexer-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symdexer-0.2.7/src/symdexer/__main__.py` & `symdexer-0.2.8/src/symdexer/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def index_command(args: Arguments) -> Iterator[str]:
     if args.reset and args.cache.is_file():
         args.cache.unlink()
 
     with Cache(args.cache) as cache:
-        if not args.cache.exists():
+        if args.reset:
             cache.init()
 
         for module in cache.update(args.packages):
             yield f"Indexing {module.name}"
 
     yield "Done indexing"
```

### Comparing `symdexer-0.2.7/src/symdexer/cache.py` & `symdexer-0.2.8/src/symdexer/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 
     def __exit__(self, *args, **kwargs):
         self.db.__exit__(*args, **kwargs)
 
     def init(self):
         self.db.executescript(
             """
-            DROP TABLE IF EXISTS Module;
-
-            DROP TABLE IF EXISTS Symbol;
-
             CREATE TABLE Module (
                 name TEXT PRIMARY KEY,
                 path TEXT NOT NULL,
                 changed NUMBER NOT NULL
             );
 
             CREATE TABLE Symbol (
```

### Comparing `symdexer-0.2.7/src/symdexer/modules.py` & `symdexer-0.2.8/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.7/src/symdexer/parser.py` & `symdexer-0.2.8/src/symdexer/parser.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.7/src/symdexer/symbols.py` & `symdexer-0.2.8/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.7/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.8/src/symdexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.7
+Version: 0.2.8
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

