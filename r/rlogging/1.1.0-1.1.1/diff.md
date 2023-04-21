# Comparing `tmp/rlogging-1.1.0.tar.gz` & `tmp/rlogging-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.0.tar", max compression
+gzip compressed data, was "rlogging-1.1.1.tar", max compression
```

## Comparing `rlogging-1.1.0.tar` & `rlogging-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1393 2023-04-15 17:09:46.635115 rlogging-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      456 2023-04-05 07:19:05.449274 rlogging-1.1.0/readme.md
--rw-r--r--   0        0        0       65 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/__init__.py
--rw-r--r--   0        0        0     3236 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/adapters.py
--rw-r--r--   0        0        0      270 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/filters.py
--rw-r--r--   0        0        0     2339 2023-04-15 17:09:46.635115 rlogging-1.1.0/rlogging/formatters.py
--rw-r--r--   0        0        0      945 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      740 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      267 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-04-15 17:40:17.133327 rlogging-1.1.0/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-04-05 07:19:05.453274 rlogging-1.1.0/rlogging/namespaces.py
--rw-r--r--   0        0        0     1509 2023-04-15 17:09:46.639115 rlogging-1.1.0/rlogging/utils.py
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-04-21 20:02:47.376896 rlogging-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-04-21 20:02:47.376896 rlogging-1.1.1/readme.md
+-rw-r--r--   0        0        0       65 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/__init__.py
+-rw-r--r--   0        0        0     3208 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/adapters.py
+-rw-r--r--   0        0        0      270 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/filters.py
+-rw-r--r--   0        0        0     2339 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/formatters.py
+-rw-r--r--   0        0        0      945 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      740 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      125 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/admin.py
+-rw-r--r--   0        0        0      267 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1483 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0       72 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/models.py
+-rw-r--r--   0        0        0     2019 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2023-04-21 20:02:47.512896 rlogging-1.1.1/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1509 2023-04-21 20:02:47.376896 rlogging-1.1.1/rlogging/utils.py
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 rlogging-1.1.1/PKG-INFO
```

### Comparing `rlogging-1.1.0/pyproject.toml` & `rlogging-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/adapters.py` & `rlogging-1.1.1/rlogging/adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         return msg, kwargs
 
 
 class AppLoggerAdapter(RsLoggerAdapter):
     def queries(self, queries: list, *args, **kwargs):
         kwargs.setdefault('stacklevel', 4)
-        self.info(f'processing queries: {len(queries)}', *args, **kwargs)
+        self.info(f'processing queries: {len(queries)}', **kwargs)
 
 
 class HttpLoggerAdapter(AppLoggerAdapter):
     """Флоу для логирования веб запросов/ответов"""
 
     def request(
         self,
@@ -79,27 +79,27 @@
             'http': {
                 'url': url,
                 'method': method,
             }
         }
         self._extra_update(kwargs, extra)
 
-        self.info('http request', *args, **kwargs)
+        self.info('http request', **kwargs)
 
     def response(self, code: int, *args, **kwargs):
         kwargs.setdefault('stacklevel', 3)
 
         extra = {
             'http': {
                 'code': code,
             },
         }
         self._extra_update(kwargs, extra)
 
-        self.info('http response', *args, **kwargs)
+        self.info('http response', **kwargs)
 
     def processing(
         self,
         path: str,
         route: str,
         route_name: str,
         view: str,
@@ -120,8 +120,8 @@
                 'view_args': view_args,
                 'view_kwargs': view_kwargs,
                 'namespace': namespace,
             },
         }
         self._extra_update(kwargs, extra)
 
-        self.info('http process_view', *args, **kwargs)
+        self.info('http process_view', **kwargs)
```

### Comparing `rlogging-1.1.0/rlogging/formatters.py` & `rlogging-1.1.1/rlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/handlers.py` & `rlogging-1.1.1/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/integration/django/adapters.py` & `rlogging-1.1.1/rlogging/integration/django/adapters.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/integration/django/middleware.py` & `rlogging-1.1.1/rlogging/integration/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/integration/django/signals.py` & `rlogging-1.1.1/rlogging/integration/django/signals.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/rlogging/utils.py` & `rlogging-1.1.1/rlogging/utils.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.0/PKG-INFO` & `rlogging-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

