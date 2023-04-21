# Comparing `tmp/redis_simple_orm-1.2.5.tar.gz` & `tmp/redis_simple_orm-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-1.2.5.tar", last modified: Mon Apr 17 03:49:35 2023, max compression
+gzip compressed data, was "redis_simple_orm-1.2.6.tar", last modified: Fri Apr 21 04:26:02 2023, max compression
```

## Comparing `redis_simple_orm-1.2.5.tar` & `redis_simple_orm-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.177098 redis_simple_orm-1.2.5/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/RSO/aioredis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/aioredis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.181098 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 03:49:35.000000 redis_simple_orm-1.2.5/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:49:35.185098 redis_simple_orm-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-17 03:49:21.000000 redis_simple_orm-1.2.5/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/aioredis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/aioredis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.066245 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 04:26:02.000000 redis_simple_orm-1.2.6/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:26:02.070245 redis_simple_orm-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-21 04:25:39.000000 redis_simple_orm-1.2.6/tests/test_model.py
```

### Comparing `redis_simple_orm-1.2.5/LICENSE` & `redis_simple_orm-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/PKG-INFO` & `redis_simple_orm-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 1.2.5
+Version: 1.2.6
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-1.2.5/README.md` & `redis_simple_orm-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/RSO/aioredis/index.py` & `redis_simple_orm-1.2.6/RSO/aioredis/index.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,22 @@
 T = TypeVar('T')
 
 
 class HashIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls):
-        return f'{cls.__prefix__}::{cls.__model__.__model_name__}::'\
-               f'{cls.__index_name__}::{cls.__key__}'
+        model_prefix = cls.__model__.__model_name__
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}'
+        return redis_key
 
     @property
     def redis_key(self):
         model_prefix = self.__model__.__model_name__
         return f'{self.__prefix__}::{model_prefix}::{self.__index_name__}::'\
                f'{self.__key__}'
 
@@ -61,17 +67,21 @@
 
 
 class ListIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
         model_prefix = cls.__model__.__model_name__
-        first_part = f'{cls.__prefix__}::{model_prefix}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self):
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     async def save_index(self, redis: Pipeline):
@@ -135,17 +145,21 @@
 
 
 class SetIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
         model_prefix = cls.__model__.__model_name__
-        first_part = f'{cls.__prefix__}::{model_prefix}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self):
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     async def save_index(self, redis: Pipeline):
```

### Comparing `redis_simple_orm-1.2.5/RSO/aioredis/model.py` & `redis_simple_orm-1.2.6/RSO/aioredis/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/RSO/base.py` & `redis_simple_orm-1.2.6/RSO/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 
 REDIS_MODEL_PREFIX = 'simple_redis_orm'
 
 
 class BaseIndex:
     # prefix for redis key
-    __prefix__: str = REDIS_MODEL_PREFIX
-    __index_name__: str = 'index_base'
+    __prefix__: str
+    __index_name__: str = 'index'
     # Model class that using this index
     __model__: T
     __key__: str
 
     @property
     def _model_key_value(self):
         value = getattr(self.__model__, self.__model__.__key__)
@@ -28,20 +28,20 @@
     def create_from_model_class(cls, model_instance: Type["BaseModel"]):
         cls.__model__ = model_instance
         return cls()
 
 
 class BaseModel:
     # prefix for redis key
-    __prefix__: str = REDIS_MODEL_PREFIX
+    __prefix__: str
     # infix for redis key and model name
     __model_name__: str
     # Object property name that are to be redis key suffix
     __key__: str
-    __indexes__: List[BaseIndex] = []
+    __indexes__: List[BaseIndex]
 
     @classmethod
     def get_fields(cls) -> List[str]:
         return [f.name for f in fields(cls)]
 
     def __post_init__(self):
         for field, desc in self.__dataclass_fields__.items():
@@ -64,14 +64,16 @@
                 continue
             setattr(self, field, value)
 
     @classmethod
     def _to_redis_key(cls, value):
         if isinstance(value, UUID):
             value = str(value)
+        if cls.__prefix__ is None:
+            return f'{cls.__model_name__}:{value}'
         return f'{cls.__prefix__}::{cls.__model_name__}:{value}'
 
     @property
     def redis_key(self):
         return self._to_redis_key(getattr(self, self.__key__))
 
     def dict(self) -> dict:
```

### Comparing `redis_simple_orm-1.2.5/RSO/index.py` & `redis_simple_orm-1.2.6/RSO/index.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 
 T = TypeVar('T')
 
 
 class HashIndex(BaseIndex):
     @classmethod
     def _to_redis_key(cls) -> str:
-        return f'{cls.__prefix__}::{cls.__model__.__model_name__}::'\
-               f'{cls.__index_name__}::{cls.__key__}'
+        model_prefix = cls.__model__.__model_name__
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}'
+        return redis_key
 
     @property
     def redis_key(self) -> str:
         return self._to_redis_key()
 
     def save_index(self, redis: Union[Pipeline, Redis]) -> None:
         index_value = getattr(self.__model__, self.__key__)
@@ -40,17 +46,21 @@
         redis.hdel(self.redis_key, index_value)
 
 
 class ListIndex(BaseIndex):
     @classmethod
     def _to_redis_key(cls, value) -> str:
         model_prefix = cls.__model__.__model_name__
-        first_part = f'{cls.__prefix__}::{model_prefix}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self) -> str:
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     def save_index(self, redis: Union[Pipeline, Redis]) -> None:
@@ -110,17 +120,21 @@
 
 
 class SetIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value: Any) -> str:
         model_prefix = cls.__model__.__model_name__
-        first_part = f'{cls.__prefix__}::{model_prefix}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self) -> str:
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     def save_index(self, redis: Union[Pipeline, Redis]) -> None:
```

### Comparing `redis_simple_orm-1.2.5/RSO/model.py` & `redis_simple_orm-1.2.6/RSO/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/RSO/txredisapi/index.py` & `redis_simple_orm-1.2.6/RSO/txredisapi/index.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 
 T = TypeVar('T')
 
 
 class HashIndex(BaseIndex):
     @classmethod
     def _to_redis_key(cls) -> str:
-        return f'{cls.__prefix__}::{cls.__model__.__model_name__}::'\
-               f'{cls.__index_name__}::{cls.__key__}'
+        model_prefix = cls.__model__.__model_name__
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}'
+        return redis_key
 
     @property
     def redis_key(self) -> str:
         return self._to_redis_key()
 
     @inlineCallbacks
     def save_index(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
@@ -56,17 +62,21 @@
 
 
 class ListIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
         model_prefix = cls.__model__.__model_name__
-        first_part = f'{cls.__prefix__}::{model_prefix}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self):
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     @inlineCallbacks
@@ -148,30 +158,35 @@
             returnValue(result)
 
 
 class SetIndex(BaseIndex):
 
     @classmethod
     def _to_redis_key(cls, value):
-        first_part = f'{cls.__prefix__}::{cls.__model__.__model_name__}::'\
-                     f'{cls.__index_name__}::{cls.__key__}'
-        return f'{first_part}:{value}'
+        model_prefix = cls.__model__.__model_name__
+        if cls.__prefix__ is not None:
+            redis_key = f'{cls.__prefix__}::'
+        else:
+            redis_key = ''
+        redis_key = f'{redis_key}{model_prefix}::' \
+                    f'{cls.__index_name__}::{cls.__key__}:{value}'
+        return redis_key
 
     @property
     def redis_key(self):
         value = getattr(self.__model__, self.__key__)
         return self._to_redis_key(value)
 
     @inlineCallbacks
     def save_index(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
         if isinstance(redis, BaseRedisProtocol):
             redis.sadd(self.redis_key, self._model_key_value)
             returnValue(None)
         else:
-            yield redis.sadd(self.redis_key, self._model_key_value)
+            yield redis.sadd(self.redis_key, members=self._model_key_value)
 
     @classmethod
     @inlineCallbacks
     def get_members(cls, redis: ConnectionHandler, index_value):
         redis_key = cls._to_redis_key(index_value)
         result = yield redis.smembers(redis_key)
         return returnValue(result)
@@ -192,8 +207,8 @@
         for value in result:
             model_instance = yield model_class.search(redis, value)
             model_instances.append(model_instance)
         return model_instances
 
     @inlineCallbacks
     def remove_from_index(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
-        yield redis.srem(self.redis_key, self._model_key_value)
+        yield redis.srem(self.redis_key, members=self._model_key_value)
```

### Comparing `redis_simple_orm-1.2.5/RSO/txredisapi/model.py` & `redis_simple_orm-1.2.6/RSO/txredisapi/model.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-1.2.6/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 1.2.5
+Version: 1.2.6
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `redis_simple_orm-1.2.5/setup.py` & `redis_simple_orm-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/tests/test_example.py` & `redis_simple_orm-1.2.6/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.5/tests/test_index.py` & `redis_simple_orm-1.2.6/tests/test_index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 from datetime import date
 
+from tests.models.const import REDIS_MODEL_PREFIX
 from .models.redispy import (
     UserModel,
     SingleIndexEmail,
     SingleIndexUsername,
     SetIndexGroupID,
-    ListIndexQueue
+    ListIndexQueue,
+    NoPrefixUserModel,
+    NoPrefixSingleIndexUsername,
+    NoPrefixSetIndexGroupID,
+    NoPrefixListIndexQueue,
 )
 
 
 BIRTH_DATE = date.fromisoformat('1999-09-09')
 
 
 class TestHashIndex:
+    def test_redis_key(self):
+        # With prefix
+        user = UserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = SingleIndexUsername.create_from_model_class(user)
+        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
+        # Without prefix
+        user = NoPrefixUserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = NoPrefixSingleIndexUsername.create_from_model_class(user)
+        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
+
     def test_search_model(self, sync_redis):
         user = UserModel(
             user_id=1, username='username', email='test@email'
         )
         user.save(sync_redis)
 
         assert SingleIndexUsername.search_model(
@@ -55,14 +76,30 @@
         ) is None
         assert SingleIndexEmail.search_model(
             sync_redis, user.email, UserModel
         ) is None
 
 
 class TestListIndex:
+    def test_redis_key(self):
+        # With prefix
+        user = UserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = ListIndexQueue.create_from_model_class(user)
+        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
+        # Without prefix
+        user = NoPrefixUserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = NoPrefixListIndexQueue.create_from_model_class(user)
+        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
+
     def test_success(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
             group_id=2,
             queue_id=3,
@@ -146,14 +183,30 @@
         assert index.is_exist_on_list(sync_redis, user.user_id) is False
         assert len(ListIndexQueue.search_models(
             sync_redis, user.queue_id, UserModel
         )) == 0
 
 
 class TestSetIndex:
+
+    def test_redis_key(self):
+        # With prefix
+        user = UserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = SetIndexGroupID.create_from_model_class(user)
+        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
+        # Without prefix
+        user = NoPrefixUserModel(
+            user_id=1, username='username', email='test@email'
+        )
+        index = NoPrefixSetIndexGroupID.create_from_model_class(user)
+        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+
     def test_search_model(self, sync_redis):
         user = UserModel(
             user_id=1, username='username', group_id=10,
             email='test@email',
         )
         user.save(sync_redis)
```

### Comparing `redis_simple_orm-1.2.5/tests/test_model.py` & `redis_simple_orm-1.2.6/tests/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,39 @@
 from datetime import date
 
+from tests.models.const import REDIS_MODEL_PREFIX
 from .models.redispy import (
     UserModel,
     SingleIndexUsername,
     SingleIndexEmail,
-    SetIndexGroupID
+    SetIndexGroupID,
+    NoPrefixUserModel
 )
 
 
 class TestModelCreate:
+    def test_redis_key(self):
+        # With prefix
+        user = UserModel(
+            user_id=1, username='test', email='test@create.success',
+            group_id=10, birth_date=date.fromisoformat('1999-09-09')
+        )
+        assert user.redis_key.startswith(REDIS_MODEL_PREFIX), \
+            f'key={user.redis_key} prefix={UserModel.__prefix__} ' \
+            f'REDIS_MODEL_PREFIX={REDIS_MODEL_PREFIX}'
+
+        # Without prefix
+        user2 = NoPrefixUserModel(
+            user_id=1, username='test', email='test@create.success',
+            group_id=10, birth_date=date.fromisoformat('1999-09-09')
+        )
+        assert not user2.redis_key.startswith(REDIS_MODEL_PREFIX), \
+            f'key={user2.redis_key} prefix={UserModel.__prefix__} ' \
+            f'REDIS_MODEL_PREFIX={REDIS_MODEL_PREFIX}'
+
     def test_success(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
             group_id=10,
             birth_date=date.fromisoformat('1999-09-09')
```

