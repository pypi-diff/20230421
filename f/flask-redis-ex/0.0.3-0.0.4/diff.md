# Comparing `tmp/flask_redis_ex-0.0.3-py3-none-any.whl.zip` & `tmp/flask_redis_ex-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2581 bytes, number of entries: 6
--rw-rw-r--  2.0 unx      499 b- defN 23-Apr-19 23:52 flask_redis_ex/__init__.py
--rw-rw-r--  2.0 unx     1086 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      604 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      502 b- defN 23-Apr-20 00:58 flask_redis_ex-0.0.3.dist-info/RECORD
-6 files, 2798 bytes uncompressed, 1663 bytes compressed:  40.6%
+Zip file size: 2954 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     1282 b- defN 23-Apr-20 05:43 flask_redis_ex/__init__.py
+-rw-rw-r--  2.0 unx     1086 b- defN 23-Apr-21 15:42 flask_redis_ex-0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      954 b- defN 23-Apr-21 15:42 flask_redis_ex-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-21 15:42 flask_redis_ex-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-21 15:42 flask_redis_ex-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      503 b- defN 23-Apr-21 15:42 flask_redis_ex-0.0.4.dist-info/RECORD
+6 files, 3932 bytes uncompressed, 2036 bytes compressed:  48.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: flask_redis_ex/__init__.py
 Comment: 
 
-Filename: flask_redis_ex-0.0.3.dist-info/LICENSE
+Filename: flask_redis_ex-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: flask_redis_ex-0.0.3.dist-info/METADATA
+Filename: flask_redis_ex-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: flask_redis_ex-0.0.3.dist-info/WHEEL
+Filename: flask_redis_ex-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: flask_redis_ex-0.0.3.dist-info/top_level.txt
+Filename: flask_redis_ex-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_redis_ex-0.0.3.dist-info/RECORD
+Filename: flask_redis_ex-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_redis_ex/__init__.py

```diff
@@ -1,18 +1,48 @@
-from flask import current_app
+from flask import current_app, Flask
 from werkzeug.local import LocalProxy
 
 import redis
 
 
+def create_redis_from(app: Flask):
+    redis_url = app.config.get("REDIS_URL")
+    redis_decode = app.config.get("REDIS_DECODE", False)
+    if redis_url is None:
+        raise RuntimeError("REDIS_URL is not configured")
+    return redis.from_url(redis_url, decode_responses=redis_decode)
+
+
+class RedisFlask():
+
+    def __init__(self, app: Flask = None, redis: redis.Redis = None) -> None:
+        self.redis = redis
+        if app is not None:
+            self.init_app(app)
+        pass
+
+    def init_app(self, app: Flask):
+        if self.redis is None:
+            self.redis = create_redis_from(app)
+
+        app.extensions["redis_flask"] = self
+
+        @app.teardown_appcontext
+        def close(response_or_exc):
+            if self.redis is not None:
+                self.redis.close()
+            pass
+        pass
+    pass
+
+
 def _get_client():
+    if "redis_flask" in current_app.extensions:
+        return current_app.extensions["redis_flask"].redis
+
     key = "redis_client"
     if key not in current_app.extensions:
-        config = current_app.config
-        redis_url = config.get("REDIS_URL")
-        if redis_url is None:
-            raise RuntimeError("REDIS_URL is not configured")
-        current_app.extensions[key] = redis.from_url(redis_url)
+        current_app.extensions[key] = create_redis_from(current_app)
     return current_app.extensions[key]
 
 
 redis_client: redis.Redis = LocalProxy(_get_client)
```

## Comparing `flask_redis_ex-0.0.3.dist-info/LICENSE` & `flask_redis_ex-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

