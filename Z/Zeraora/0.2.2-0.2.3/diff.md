# Comparing `tmp/Zeraora-0.2.2.tar.gz` & `tmp/Zeraora-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.2.2.tar", last modified: Fri Apr 21 08:01:18 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.2.3.tar", last modified: Fri Apr 21 10:09:37 2023, max compression
```

## Comparing `Zeraora-0.2.2.tar` & `Zeraora-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 08:01:18.000000 Zeraora-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 08:01:04.000000 Zeraora-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 08:01:18.000000 Zeraora-0.2.2/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:01:18.000000 Zeraora-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 08:01:04.000000 Zeraora-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:01:18.000000 Zeraora-0.2.2/zeraora/djangobase/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/djangobase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/djangobase/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-04-21 08:01:04.000000 Zeraora-0.2.2/zeraora/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 10:09:37.000000 Zeraora-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-21 10:09:26.000000 Zeraora-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-21 10:09:37.000000 Zeraora-0.2.3/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 10:09:36.000000 Zeraora-0.2.3/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:09:37.000000 Zeraora-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-21 10:09:26.000000 Zeraora-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:09:37.000000 Zeraora-0.2.3/zeraora/djangobase/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/djangobase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/djangobase/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-21 10:09:26.000000 Zeraora-0.2.3/zeraora/typing.py
```

### Comparing `Zeraora-0.2.2/PKG-INFO` & `Zeraora-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.2
+Version: 0.2.3
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.2/README.md` & `Zeraora-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/Zeraora.egg-info/PKG-INFO` & `Zeraora-0.2.3/Zeraora.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zeraora
-Version: 0.2.2
+Version: 0.2.3
 Summary: 一个包含原创工具类及快捷函数的工具库。A original utility Python package.
 Home-page: https://github.com/aixcyi/zeraora
 Author: aixcyi
 Author-email: 75880483+aixcyi@users.noreply.github.com
 License: MIT
 Project-URL: Source, https://github.com/aixcyi/zeraora
 Project-URL: Tracker, https://github.com/aixcyi/zeraora/issues
```

### Comparing `Zeraora-0.2.2/setup.py` & `Zeraora-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/charsets.py` & `Zeraora-0.2.3/zeraora/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/decorators.py` & `Zeraora-0.2.3/zeraora/decorators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/djangobase/mixins.py` & `Zeraora-0.2.3/zeraora/djangobase/mixins.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/generators.py` & `Zeraora-0.2.3/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/time.py` & `Zeraora-0.2.3/zeraora/time.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.2.2/zeraora/typing.py` & `Zeraora-0.2.3/zeraora/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,28 +115,29 @@
         *errs: Union[Exception, Type[Exception]],
         default=None,
 ):
     """
     使用mapper将raw转换为所需的值，当出现异常时返回default。
 
     默认捕获以下异常，可以通过errs参数追加更多异常：
+        - TypeError
         - ValueError
         - KeyboardInterrupt
 
     :param mapper: 类型转换器。如果转换器不可调用，将直接返回默认值。
     :param raw: 被转换的值。
     :param errs: 需要捕获的其它异常类或异常对象。应当提供可被 except 语句接受的值。
     :param default: 默认值。即使不提供也会默认返回 None 而不会抛出异常。
     :return: 转换后的值。如若捕获到特定异常将返回默认值。
     """
     if not callable(mapper):
         return default
     try:
         return mapper(raw)
-    except (ValueError, KeyboardInterrupt) + errs:
+    except (TypeError, ValueError, KeyboardInterrupt) + errs:
         return default
 
 
 def represent(value) -> str:
     """
     将任意值转换为一个易于阅读的字符串。
```

