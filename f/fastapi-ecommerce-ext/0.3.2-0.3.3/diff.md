# Comparing `tmp/fastapi_ecommerce_ext-0.3.2.tar.gz` & `tmp/fastapi_ecommerce_ext-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.3.2.tar", last modified: Fri Apr 21 03:21:52 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.3.3.tar", last modified: Fri Apr 21 03:31:07 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.3.2.tar` & `fastapi_ecommerce_ext-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:21:52.022812 fastapi_ecommerce_ext-0.3.2/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0      382 2023-04-21 03:21:52.022812 fastapi_ecommerce_ext-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:21:52.010815 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-21 03:21:52.021812 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1543 2023-04-20 17:10:01.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     2663 2023-04-21 03:21:49.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:21:52.019813 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      382 2023-04-21 03:21:51.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-21 03:21:51.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:21:51.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 03:21:51.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 03:21:51.000000 fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-21 03:21:52.023810 fastapi_ecommerce_ext-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-21 03:21:49.000000 fastapi_ecommerce_ext-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.804811 fastapi_ecommerce_ext-0.3.3/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:31:07.804811 fastapi_ecommerce_ext-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.791811 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.803812 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-21 03:31:05.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     2663 2023-04-21 03:21:49.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:31:07.800811 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      382 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-21 03:31:07.000000 fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-21 03:31:07.805811 fastapi_ecommerce_ext-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-21 03:31:05.000000 fastapi_ecommerce_ext-0.3.3/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.3.2/LICENSE.txt` & `fastapi_ecommerce_ext-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage()
         )
 
 
 def configure_logging(
-    logging_level: int, access_log_path: str, error_log_path: str
+    logging_level: int, access_log_path: str
 ) -> None:
     loggers = [
         logging.getLogger(name)
         for name in logging.root.manager.loggerDict
         if name.startswith("uvicorn") or name.startswith("gunicorn")
     ]
     for lg in loggers:
```

### Comparing `fastapi_ecommerce_ext-0.3.2/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.3.3/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.3.2/setup.py` & `fastapi_ecommerce_ext-0.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "0.3.2"
+version = "0.3.3"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```

