# Comparing `tmp/stashlib-0.0.7.0.tar.gz` & `tmp/stashlib-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashlib-0.0.7.0.tar", last modified: Fri Apr 21 08:00:35 2023, max compression
+gzip compressed data, was "stashlib-0.0.7.1.tar", last modified: Fri Apr 21 08:11:00 2023, max compression
```

## Comparing `stashlib-0.0.7.0.tar` & `stashlib-0.0.7.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.921607 stashlib-0.0.7.0/
--rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/LICENSE
--rw-rw-rw-   0        0        0      988 2023-04-21 08:00:35.921607 stashlib-0.0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/README.md
--rw-rw-rw-   0        0        0     1135 2023-04-21 08:00:35.922609 stashlib-0.0.7.0/setup.cfg
--rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.842635 stashlib-0.0.7.0/stash/
--rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.7.0/stash/__init__.py
--rw-rw-rw-   0        0        0     6932 2023-04-21 07:57:58.000000 stashlib-0.0.7.0/stash/_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.867626 stashlib-0.0.7.0/stash/codecs/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/__init__.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/brotli.py
--rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/bzip2.py
--rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/codec.py
--rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/gzip.py
--rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lz4.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzf.py
--rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzma.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/lzo.py
--rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/passthru.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/snappy.py
--rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zlib.py
--rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zopfli.py
--rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/codecs/zstd.py
--rw-rw-rw-   0        0        0      395 2023-04-21 07:56:03.000000 stashlib-0.0.7.0/stash/consts.py
--rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/defaults.py
--rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/manager.py
--rw-rw-rw-   0        0        0     1395 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/options.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.887621 stashlib-0.0.7.0/stash/serializers/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/__init__.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/bson.py
--rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/cbor.py
--rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/default.py
--rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/json.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/msgpack.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/orjson.py
--rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/rapidjson.py
--rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/serializer.py
--rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/simplejson.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/serializers/ujson.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.906614 stashlib-0.0.7.0/stash/storages/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/dbm_.py
--rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/filesystem.py
--rw-rw-rw-   0        0        0     1359 2023-04-21 07:55:23.000000 stashlib-0.0.7.0/stash/storages/leveldb.py
--rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/lmdb.py
--rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/lsmdb.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/memory.py
--rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/mongodb.py
--rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/null.py
--rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/redis.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/storages/storage.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.910614 stashlib-0.0.7.0/stash/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/checksum.py
--rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.7.0/stash/utils/nested_path.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:00:35.919608 stashlib-0.0.7.0/stashlib.egg-info/
--rw-rw-rw-   0        0        0      988 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 08:00:35.000000 stashlib-0.0.7.0/stashlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.497897 stashlib-0.0.7.1/
+-rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/LICENSE
+-rw-rw-rw-   0        0        0      988 2023-04-21 08:11:00.498896 stashlib-0.0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/README.md
+-rw-rw-rw-   0        0        0     1135 2023-04-21 08:11:00.500890 stashlib-0.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.404924 stashlib-0.0.7.1/stash/
+-rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.7.1/stash/__init__.py
+-rw-rw-rw-   0        0        0     6932 2023-04-21 07:57:58.000000 stashlib-0.0.7.1/stash/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.434912 stashlib-0.0.7.1/stash/codecs/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/__init__.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/brotli.py
+-rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/bzip2.py
+-rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/codec.py
+-rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/gzip.py
+-rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/lz4.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/lzf.py
+-rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/lzma.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/lzo.py
+-rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/passthru.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/snappy.py
+-rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/zlib.py
+-rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/zopfli.py
+-rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/codecs/zstd.py
+-rw-rw-rw-   0        0        0      395 2023-04-21 08:08:43.000000 stashlib-0.0.7.1/stash/consts.py
+-rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/defaults.py
+-rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/manager.py
+-rw-rw-rw-   0        0        0     1476 2023-04-21 08:06:35.000000 stashlib-0.0.7.1/stash/options.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.461903 stashlib-0.0.7.1/stash/serializers/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/bson.py
+-rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/cbor.py
+-rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/default.py
+-rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/json.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/msgpack.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/orjson.py
+-rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/rapidjson.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/serializer.py
+-rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/simplejson.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/serializers/ujson.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.480897 stashlib-0.0.7.1/stash/storages/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/dbm_.py
+-rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/filesystem.py
+-rw-rw-rw-   0        0        0     1363 2023-04-21 08:05:44.000000 stashlib-0.0.7.1/stash/storages/leveldb.py
+-rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/lmdb.py
+-rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/lsmdb.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/memory.py
+-rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/mongodb.py
+-rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/null.py
+-rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/redis.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/storages/storage.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.487894 stashlib-0.0.7.1/stash/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/utils/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/utils/checksum.py
+-rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.7.1/stash/utils/nested_path.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:11:00.496891 stashlib-0.0.7.1/stashlib.egg-info/
+-rw-rw-rw-   0        0        0      988 2023-04-21 08:11:00.000000 stashlib-0.0.7.1/stashlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-04-21 08:11:00.000000 stashlib-0.0.7.1/stashlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:11:00.000000 stashlib-0.0.7.1/stashlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 08:11:00.000000 stashlib-0.0.7.1/stashlib.egg-info/top_level.txt
```

### Comparing `stashlib-0.0.7.0/LICENSE` & `stashlib-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/PKG-INFO` & `stashlib-0.0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.7.0
+Version: 0.0.7.1
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.7.0/setup.cfg` & `stashlib-0.0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/__init__.py` & `stashlib-0.0.7.1/stash/__init__.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/_helpers.py` & `stashlib-0.0.7.1/stash/_helpers.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/manager.py` & `stashlib-0.0.7.1/stash/manager.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/options.py` & `stashlib-0.0.7.1/stash/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,18 @@
     "fs_cache_filename": defaults.CACHE_DEFAULT_FILENAME,
     "fs_cache_dir": defaults.CACHE_DEFAULT_PATH,
     "fs_cache_dir_level": defaults.CACHE_DEFAULT_DIR_LEVEL,
     "fs_cache_segment_size": defaults.CACHE_SEGMENT_SIZE,
     "fs_cache_file_ext": "",
     "logger": None,
     "lmdb_map_size": consts.SIZE_MB * 4,
-    "lmdb_filename": defaults.CACHE_DEFAULT_FILENAME,
+    "lmdb_filename": defaults.CACHE_DEFAULT_FILENAME + ".lmdb",
     "dbm_filename": defaults.CACHE_DEFAULT_FILENAME + ".dbm",
-    "lsmdb_filename": defaults.CACHE_DEFAULT_FILENAME + ".ldb",
+    "leveldb_filename": defaults.CACHE_DEFAULT_FILENAME + ".lvldb",
+    "lsmdb_filename": defaults.CACHE_DEFAULT_FILENAME + ".lsmdb",
     "redis_unix_socket_path": None,
     "redis_host": "localhost",
     "redis_port": 6379,
     "redis_db": 0,
     "redis_ssl": False,
     "redis_ssl_ca_certs": None,
 }
```

### Comparing `stashlib-0.0.7.0/stash/storages/dbm_.py` & `stashlib-0.0.7.1/stash/storages/dbm_.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/filesystem.py` & `stashlib-0.0.7.1/stash/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/leveldb.py` & `stashlib-0.0.7.1/stash/storages/leveldb.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class LeveldbStorage(Storage):
     def __init__(self, options: StashOptions):
         super().__init__(options)
         self._cache_max_age = self.options.cache_max_age
         self._logger = self.options.logger
-        dbpath = os.path.join(self.options.fs_cache_dir, options.dbm_filename)
+        dbpath = os.path.join(self.options.fs_cache_dir, options.leveldb_filename)
         self._db: LevelDB | None = LevelDB(path=dbpath, create_if_missing=True)
 
     @staticmethod
     def _encode_str(s: str) -> bytes:
         return to_bytes(s.strip())
 
     def close(self):
```

### Comparing `stashlib-0.0.7.0/stash/storages/lmdb.py` & `stashlib-0.0.7.1/stash/storages/lmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/lsmdb.py` & `stashlib-0.0.7.1/stash/storages/lsmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/memory.py` & `stashlib-0.0.7.1/stash/storages/memory.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/mongodb.py` & `stashlib-0.0.7.1/stash/storages/mongodb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/redis.py` & `stashlib-0.0.7.1/stash/storages/redis.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/storages/storage.py` & `stashlib-0.0.7.1/stash/storages/storage.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/utils/checksum.py` & `stashlib-0.0.7.1/stash/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stash/utils/nested_path.py` & `stashlib-0.0.7.1/stash/utils/nested_path.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.7.0/stashlib.egg-info/PKG-INFO` & `stashlib-0.0.7.1/stashlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.7.0
+Version: 0.0.7.1
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.7.0/stashlib.egg-info/SOURCES.txt` & `stashlib-0.0.7.1/stashlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

