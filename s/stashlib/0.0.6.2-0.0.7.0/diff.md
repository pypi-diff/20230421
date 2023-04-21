# Comparing `tmp/stashlib-0.0.6.2.tar.gz` & `tmp/stashlib-0.0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashlib-0.0.6.2.tar", last modified: Sun Apr  9 09:29:13 2023, max compression
+gzip compressed data, was "stashlib-0.0.7.0.tar", last modified: Fri Apr 21 08:00:35 2023, max compression
```

## Comparing `stashlib-0.0.6.2.tar` & `stashlib-0.0.7.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.469732 stashlib-0.0.6.2/
--rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/LICENSE
--rw-rw-rw-   0        0        0      988 2023-04-09 09:29:13.470732 stashlib-0.0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/README.md
--rw-rw-rw-   0        0        0     1135 2023-04-09 09:29:13.471731 stashlib-0.0.6.2/setup.cfg
--rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.395624 stashlib-0.0.6.2/stash/
--rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.6.2/stash/__init__.py
--rw-rw-rw-   0        0        0     6422 2023-04-09 09:26:26.000000 stashlib-0.0.6.2/stash/_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.420745 stashlib-0.0.6.2/stash/codecs/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/__init__.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/brotli.py
--rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/bzip2.py
--rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/codec.py
--rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/gzip.py
--rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lz4.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzf.py
--rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzma.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzo.py
--rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/passthru.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/snappy.py
--rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zlib.py
--rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zopfli.py
--rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zstd.py
--rw-rw-rw-   0        0        0      395 2023-04-09 09:27:23.000000 stashlib-0.0.6.2/stash/consts.py
--rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/defaults.py
--rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/manager.py
--rw-rw-rw-   0        0        0     1395 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/options.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.439762 stashlib-0.0.6.2/stash/serializers/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/__init__.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/bson.py
--rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/cbor.py
--rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/default.py
--rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/json.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/msgpack.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/orjson.py
--rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/rapidjson.py
--rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/serializer.py
--rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/simplejson.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/ujson.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.456751 stashlib-0.0.6.2/stash/storages/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/dbm_.py
--rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/filesystem.py
--rw-rw-rw-   0        0        0      411 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/leveldb.py
--rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/lmdb.py
--rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/lsmdb.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/memory.py
--rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/mongodb.py
--rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/null.py
--rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/redis.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/storage.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.461735 stashlib-0.0.6.2/stash/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/checksum.py
--rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/nested_path.py
-drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.467733 stashlib-0.0.6.2/stashlib.egg-info/
--rw-rw-rw-   0        0        0      988 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.921607 stashlib-0.0.7.0/
+-rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      988 2023-04-21 08:00:35.921607 stashlib-0.0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/README.md
+-rw-rw-rw-   0        0        0     1135 2023-04-21 08:00:35.922609 stashlib-0.0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.842635 stashlib-0.0.7.0/stash/
+-rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.7.0/stash/__init__.py
+-rw-rw-rw-   0        0        0     6932 2023-04-21 07:57:58.000000 stashlib-0.0.7.0/stash/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.867626 stashlib-0.0.7.0/stash/codecs/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/__init__.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/brotli.py
+-rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/bzip2.py
+-rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/codec.py
+-rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/gzip.py
+-rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lz4.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzf.py
+-rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzma.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzo.py
+-rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/passthru.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/snappy.py
+-rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zlib.py
+-rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zopfli.py
+-rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zstd.py
+-rw-rw-rw-   0        0        0      395 2023-04-21 07:56:03.000000 stashlib-0.0.7.0/stash/consts.py
+-rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/defaults.py
+-rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/manager.py
+-rw-rw-rw-   0        0        0     1395 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/options.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.887621 stashlib-0.0.7.0/stash/serializers/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/bson.py
+-rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/cbor.py
+-rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/default.py
+-rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/json.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/msgpack.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/orjson.py
+-rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/rapidjson.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/serializer.py
+-rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/simplejson.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/ujson.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.906614 stashlib-0.0.7.0/stash/storages/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/dbm_.py
+-rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/filesystem.py
+-rw-rw-rw-   0        0        0     1359 2023-04-21 07:55:23.000000 stashlib-0.0.7.0/stash/storages/leveldb.py
+-rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/lmdb.py
+-rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/lsmdb.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/memory.py
+-rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/mongodb.py
+-rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/null.py
+-rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/redis.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/storage.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.910614 stashlib-0.0.7.0/stash/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/checksum.py
+-rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/nested_path.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.919608 stashlib-0.0.7.0/stashlib.egg-info/
+-rw-rw-rw-   0        0        0      988 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/top_level.txt
```

### Comparing `stashlib-0.0.6.2/LICENSE` & `stashlib-0.0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/PKG-INFO` & `stashlib-0.0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.6.2
+Version: 0.0.7.0
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.6.2/setup.cfg` & `stashlib-0.0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/__init__.py` & `stashlib-0.0.7.0/stash/__init__.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/_helpers.py` & `stashlib-0.0.7.0/stash/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 import functools
 
+from stash.consts import SIZE_KB, SIZE_MB, SIZE_GB
 from stash.manager import StashManager
 from stash.options import StashOptions
 
 
+def size_kb(n: int) -> int:
+    return SIZE_KB * n
+
+
+def size_mb(n: int) -> int:
+    return SIZE_MB * n
+
+
+def size_gb(n: int) -> int:
+    return SIZE_GB * n
+
+
 def _init_cache(storage, codec, options: StashOptions) -> StashManager:
     cache_man = StashManager(storage=storage, codec=codec, options=options)
     return cache_man
 
 
 def _init_fs_cache(codec, options: StashOptions) -> StashManager:
     from .storages.filesystem import FileSystemStorage
@@ -179,14 +192,22 @@
     from .storages.lsmdb import LsmDbStorage
     from .codecs.passthru import PassthruCodec
 
     storage = LsmDbStorage(options=options)
     return _init_cache(storage, codec=PassthruCodec(), options=options)
 
 
+def get_leveldb_stash(options: StashOptions) -> StashManager:
+    from .storages.leveldb import LeveldbStorage
+    from .codecs.passthru import PassthruCodec
+
+    storage = LeveldbStorage(options=options)
+    return _init_cache(storage, codec=PassthruCodec(), options=options)
+
+
 def stash(stash: StashManager = None):
     stash_ = stash
 
     def decorator(function):
         stash = stash_
         if stash is None:
             stash = get_fs_stash(StashOptions())
```

### Comparing `stashlib-0.0.6.2/stash/manager.py` & `stashlib-0.0.7.0/stash/manager.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/options.py` & `stashlib-0.0.7.0/stash/options.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/dbm_.py` & `stashlib-0.0.7.0/stash/storages/dbm_.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/filesystem.py` & `stashlib-0.0.7.0/stash/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/lmdb.py` & `stashlib-0.0.7.0/stash/storages/lmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/lsmdb.py` & `stashlib-0.0.7.0/stash/storages/lsmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/memory.py` & `stashlib-0.0.7.0/stash/storages/memory.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/mongodb.py` & `stashlib-0.0.7.0/stash/storages/mongodb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/redis.py` & `stashlib-0.0.7.0/stash/storages/redis.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/storages/storage.py` & `stashlib-0.0.7.0/stash/storages/storage.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/utils/checksum.py` & `stashlib-0.0.7.0/stash/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stash/utils/nested_path.py` & `stashlib-0.0.7.0/stash/utils/nested_path.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.2/stashlib.egg-info/PKG-INFO` & `stashlib-0.0.7.0/stashlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.6.2
+Version: 0.0.7.0
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.6.2/stashlib.egg-info/SOURCES.txt` & `stashlib-0.0.7.0/stashlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

