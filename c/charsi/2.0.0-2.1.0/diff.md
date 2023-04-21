# Comparing `tmp/charsi-2.0.0.tar.gz` & `tmp/charsi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charsi-2.0.0.tar", max compression
+gzip compressed data, was "charsi-2.1.0.tar", max compression
```

## Comparing `charsi-2.0.0.tar` & `charsi-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1007 2023-04-20 07:29:24.095764 charsi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3580 2023-04-20 07:28:46.454655 charsi-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-2.0.0/src/charsi/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-2.0.0/src/charsi/__main__.py
--rw-r--r--   0        0        0      348 2023-04-19 12:44:19.623591 charsi-2.0.0/src/charsi/asset.py
--rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-2.0.0/src/charsi/commands/__init__.py
--rw-r--r--   0        0        0      896 2023-04-20 07:14:22.978166 charsi-2.0.0/src/charsi/commands/build.py
--rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-2.0.0/src/charsi/commands/build_manifest.py
--rw-r--r--   0        0        0     2602 2023-04-19 12:57:54.250514 charsi-2.0.0/src/charsi/instruction.py
--rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-2.0.0/src/charsi/manifest.py
--rw-r--r--   0        0        0     1294 2023-04-20 07:13:00.354859 charsi-2.0.0/src/charsi/recipe.py
--rw-r--r--   0        0        0     2132 2023-04-18 03:11:57.019672 charsi-2.0.0/src/charsi/strings.py
--rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-2.0.0/src/charsi/utils.py
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 charsi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1007 2023-04-21 09:56:58.581088 charsi-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3660 2023-04-21 09:54:48.275836 charsi-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 15:29:07.850456 charsi-2.1.0/src/charsi/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 22:39:49.537722 charsi-2.1.0/src/charsi/__main__.py
+-rw-r--r--   0        0        0      912 2023-04-20 12:21:17.407136 charsi-2.1.0/src/charsi/asset.py
+-rw-r--r--   0        0        0      141 2023-04-18 11:06:34.749797 charsi-2.1.0/src/charsi/commands/__init__.py
+-rw-r--r--   0        0        0     1126 2023-04-20 12:29:04.602490 charsi-2.1.0/src/charsi/commands/build.py
+-rw-r--r--   0        0        0      684 2023-04-18 12:19:40.780769 charsi-2.1.0/src/charsi/commands/build_manifest.py
+-rw-r--r--   0        0        0     2602 2023-04-19 12:57:54.250514 charsi-2.1.0/src/charsi/instruction.py
+-rw-r--r--   0        0        0     1278 2023-04-18 10:59:27.587548 charsi-2.1.0/src/charsi/manifest.py
+-rw-r--r--   0        0        0     1294 2023-04-20 07:13:00.354859 charsi-2.1.0/src/charsi/recipe.py
+-rw-r--r--   0        0        0     2380 2023-04-20 12:26:12.708529 charsi-2.1.0/src/charsi/strings.py
+-rw-r--r--   0        0        0      551 2023-04-18 12:27:45.093226 charsi-2.1.0/src/charsi/utils.py
+-rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 charsi-2.1.0/PKG-INFO
```

### Comparing `charsi-2.0.0/pyproject.toml` & `charsi-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charsi"
-version = "2.0.0"
+version = "2.1.0"
 description = "A command-line tool to help game modders build string resources for Diablo II: Resurrected."
 authors = ["HE Yaowen <he.yaowen@hotmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/he-yaowen/charsi"
 packages = [{include = "charsi", from = "src"}]
```

### Comparing `charsi-2.0.0/README.md` & `charsi-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -145,13 +145,17 @@
 
 * `/instructions/`: Lua scripts for instruction handlers
 
 ### Variables
 
 * `{origin}`: Placeholder for original text
 
+### Alias
+
+You can set alias to a bunch of keys by putting files in `/alias/`.
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

### Comparing `charsi-2.0.0/src/charsi/commands/build_manifest.py` & `charsi-2.1.0/src/charsi/commands/build_manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-2.0.0/src/charsi/instruction.py` & `charsi-2.1.0/src/charsi/instruction.py`

 * *Files identical despite different names*

### Comparing `charsi-2.0.0/src/charsi/manifest.py` & `charsi-2.1.0/src/charsi/manifest.py`

 * *Files identical despite different names*

### Comparing `charsi-2.0.0/src/charsi/recipe.py` & `charsi-2.1.0/src/charsi/recipe.py`

 * *Files identical despite different names*

### Comparing `charsi-2.0.0/src/charsi/strings.py` & `charsi-2.1.0/src/charsi/strings.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,26 +43,29 @@
     ruRU: str
     zhCN: str
 
 
 class GameStringTable:
     _strings: List[GameString]
     _indices: Dict[str, int]
+    _alias: Dict[str, str]
 
     def __init__(self):
         self._strings = []
         self._indices = {}
+        self._alias = {}
 
     @property
     def strings(self):
         return self._strings
 
     def load(self, fp: IO):
         self._strings = json.load(fp)
         self._indices = {self._strings[i]['Key']: i for i in range(0, len(self._strings))}
+        self._alias = {}
 
         return self
 
     def dump(self, fp: IO):
         json.dump(self._strings, fp, ensure_ascii=False, indent=2)
 
         return self
@@ -76,18 +79,24 @@
     def findall(self, query: str) -> List[dict]:
         if query.find(',') > -1:
             return reduce(lambda v, sl: v + sl, [self.findall(q.strip()) for q in query.split(',')], [])
 
         m = re.match(r'^\s*([\w\s]+)\s*~\s*([\w\s]+)\s*$', query)
 
         if not m:
+            if query in self._alias:
+                return self.findall(self._alias[query])
+
             return [self.find(query)]
 
         if (m.group(1) not in self._indices) or (m.group(2) not in self._indices):
             raise IndexError(query)
 
         start_index = self._indices[m.group(1)]
         end_index = self._indices[m.group(2)] + 1
         if start_index > end_index:
             raise IndexError(query)
 
         return self._strings[start_index:end_index]
+
+    def set_alias(self, table: Dict[str, str]):
+        self._alias = table
```

### Comparing `charsi-2.0.0/src/charsi/utils.py` & `charsi-2.1.0/src/charsi/utils.py`

 * *Files identical despite different names*

### Comparing `charsi-2.0.0/PKG-INFO` & `charsi-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charsi
-Version: 2.0.0
+Version: 2.1.0
 Summary: A command-line tool to help game modders build string resources for Diablo II: Resurrected.
 Home-page: https://github.com/he-yaowen/charsi
 License: GPL-3.0
 Author: HE Yaowen
 Author-email: he.yaowen@hotmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -164,14 +164,18 @@
 
 * `/instructions/`: Lua scripts for instruction handlers
 
 ### Variables
 
 * `{origin}`: Placeholder for original text
 
+### Alias
+
+You can set alias to a bunch of keys by putting files in `/alias/`.
+
 ## License
 
 Copyright (C) 2022 HE Yaowen <he.yaowen@hotmail.com>
 The GNU General Public License (GPL) version 3, see [COPYING](./COPYING).
 
 [1]: https://diablo2.blizzard.com
```

