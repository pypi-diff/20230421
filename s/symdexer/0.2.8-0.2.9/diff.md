# Comparing `tmp/symdexer-0.2.8.tar.gz` & `tmp/symdexer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\AntiMach\Desktop\symdexer\dist\.tmp-gyn7ct2f\symdexer-0.2.8.tar", last modified: Fri Apr 21 01:44:53 2023, max compression
+gzip compressed data, was "symdexer-0.2.9.tar", last modified: Fri Apr 21 10:26:46 2023, max compression
```

## Comparing `symdexer-0.2.8.tar` & `symdexer-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/
--rw-rw-rw-   0        0        0     1090 2023-04-13 01:46:40.000000 symdexer-0.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0      634 2023-04-21 01:44:53.000000 symdexer-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-04-14 20:55:22.000000 symdexer-0.2.8/README.md
--rw-rw-rw-   0        0        0      592 2023-04-21 01:44:09.000000 symdexer-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 01:44:53.000000 symdexer-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer/
--rw-rw-rw-   0        0        0        0 2023-04-13 01:32:58.000000 symdexer-0.2.8/src/symdexer/__init__.py
--rw-rw-rw-   0        0        0     1607 2023-04-21 01:43:55.000000 symdexer-0.2.8/src/symdexer/__main__.py
--rw-rw-rw-   0        0        0       38 2023-04-21 01:44:17.000000 symdexer-0.2.8/src/symdexer/__version__.py
--rw-rw-rw-   0        0        0     3686 2023-04-21 01:43:32.000000 symdexer-0.2.8/src/symdexer/cache.py
--rw-rw-rw-   0        0        0     1049 2023-04-20 00:08:33.000000 symdexer-0.2.8/src/symdexer/modules.py
--rw-rw-rw-   0        0        0     3565 2023-04-20 19:56:53.000000 symdexer-0.2.8/src/symdexer/parser.py
--rw-rw-rw-   0        0        0     1038 2023-04-20 19:11:11.000000 symdexer-0.2.8/src/symdexer/symbols.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 01:44:53.000000 symdexer-0.2.8/src/symdexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 10:26:46.829898 symdexer-0.2.9/
+-rw-rw-rw-   0        0        0     1090 2023-04-13 09:20:48.000000 symdexer-0.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      634 2023-04-21 10:26:46.828903 symdexer-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-04-20 08:34:32.000000 symdexer-0.2.9/README.md
+-rw-rw-rw-   0        0        0      592 2023-04-21 10:25:57.000000 symdexer-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 10:26:46.829898 symdexer-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 10:26:46.760893 symdexer-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 10:26:46.797894 symdexer-0.2.9/src/symdexer/
+-rw-rw-rw-   0        0        0        0 2023-04-13 09:20:48.000000 symdexer-0.2.9/src/symdexer/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-04-21 10:25:45.000000 symdexer-0.2.9/src/symdexer/__main__.py
+-rw-rw-rw-   0        0        0       38 2023-04-21 10:26:02.000000 symdexer-0.2.9/src/symdexer/__version__.py
+-rw-rw-rw-   0        0        0     3731 2023-04-21 10:25:42.000000 symdexer-0.2.9/src/symdexer/cache.py
+-rw-rw-rw-   0        0        0     1049 2023-04-20 08:34:32.000000 symdexer-0.2.9/src/symdexer/modules.py
+-rw-rw-rw-   0        0        0     3565 2023-04-21 08:40:51.000000 symdexer-0.2.9/src/symdexer/parser.py
+-rw-rw-rw-   0        0        0     1038 2023-04-21 08:40:51.000000 symdexer-0.2.9/src/symdexer/symbols.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:26:46.825897 symdexer-0.2.9/src/symdexer.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-21 10:26:46.000000 symdexer-0.2.9/src/symdexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-21 10:26:46.000000 symdexer-0.2.9/src/symdexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:26:46.000000 symdexer-0.2.9/src/symdexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-21 10:26:46.000000 symdexer-0.2.9/src/symdexer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 10:26:46.000000 symdexer-0.2.9/src/symdexer.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `symdexer-0.2.8/LICENSE.txt` & `symdexer-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.8/PKG-INFO` & `symdexer-0.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.8
+Version: 0.2.9
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `symdexer-0.2.8/pyproject.toml` & `symdexer-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symdexer"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="AntiMach", email="themachinumps@gmail.com" },
 ]
 description = "A CLI for finding and indexing symbols"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `symdexer-0.2.8/src/symdexer/__main__.py` & `symdexer-0.2.9/src/symdexer/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 
 
 def index_command(args: Arguments) -> Iterator[str]:
     if args.reset and args.cache.is_file():
         args.cache.unlink()
 
     with Cache(args.cache) as cache:
-        if args.reset:
-            cache.init()
-
         for module in cache.update(args.packages):
             yield f"Indexing {module.name}"
 
     yield "Done indexing"
 
 
 def import_command(args: Arguments) -> Iterator[str]:
```

### Comparing `symdexer-0.2.8/src/symdexer/cache.py` & `symdexer-0.2.9/src/symdexer/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,57 +8,56 @@
 from symdexer.modules import walk_modules, Module
 
 
 class Cache:
     def __init__(self, path: Path):
         self.path = path
 
-    def __enter__(self):
-        self.db = sqlite3.connect(self.path).__enter__()
-        return self
-
-    def __exit__(self, *args, **kwargs):
-        self.db.__exit__(*args, **kwargs)
-
-    def init(self):
         self.db.executescript(
             """
-            CREATE TABLE Module (
+            CREATE TABLE IF NOT EXISTS Module (
                 name TEXT PRIMARY KEY,
                 path TEXT NOT NULL,
                 changed NUMBER NOT NULL
             );
 
-            CREATE TABLE Symbol (
+            CREATE TABLE IF NOT EXISTS Symbol (
                 name TEXT NOT NULL,
                 type TEXT NOT NULL,
                 module TEXT NOT NULL REFERENCES Module(name) ON UPDATE CASCADE,
                 UNIQUE (name, type, module)
             );
             """
         )
 
+    def __enter__(self):
+        self.db = sqlite3.connect(self.path).__enter__()
+        return self
+
+    def __exit__(self, *args, **kwargs):
+        self.db.__exit__(*args, **kwargs)
+
     def update(self, packages: list[Path]) -> Iterator[Module]:
         for path in packages:
             for module in walk_modules(path):
-                yield module
-                self._index_module(module)
+                if self._index_module(module):
+                    yield module
 
         self.db.commit()
 
     def _index_module(self, module: Module):
         if self.db.execute(
             """
             SELECT path, changed
-            FROM module
-            WHERE name = ? AND (path != ? OR changed != ?)
+            FROM Module
+            WHERE name = ? AND (path == ? AND changed == ?)
             """,
             module.info,
         ).fetchall():
-            return
+            return False
 
         self.db.execute(
             """
             INSERT OR REPLACE INTO Module (name, path, changed)
             VALUES (?, ? ,?)
             """,
             module.info,
@@ -69,14 +68,16 @@
                 """
                 INSERT OR REPLACE INTO Symbol (name, type, module)
                 VALUES (?, ? ,?)
                 """,
                 (symbol, sym_type, module.name),
             )
 
+        return True
+
     def ungrouped(self, symbols: list[str], types: list[str], fuzzy: str) -> Iterator[tuple[str, str, str]]:
         if fuzzy:
             symbols = [f"%{s}%" for s in symbols]
             symbol_t = "Symbol.name LIKE ?"
         else:
             symbol_t = "Symbol.name = ?"
```

### Comparing `symdexer-0.2.8/src/symdexer/modules.py` & `symdexer-0.2.9/src/symdexer/modules.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.8/src/symdexer/parser.py` & `symdexer-0.2.9/src/symdexer/parser.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.8/src/symdexer/symbols.py` & `symdexer-0.2.9/src/symdexer/symbols.py`

 * *Files identical despite different names*

### Comparing `symdexer-0.2.8/src/symdexer.egg-info/PKG-INFO` & `symdexer-0.2.9/src/symdexer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symdexer
-Version: 0.2.8
+Version: 0.2.9
 Summary: A CLI for finding and indexing symbols
 Author-email: AntiMach <themachinumps@gmail.com>
 Project-URL: Homepage, https://github.com/antimach/symdexer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

