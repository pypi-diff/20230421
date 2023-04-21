# Comparing `tmp/locache-2.1.1.tar.gz` & `tmp/locache-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locache-2.1.1.tar", last modified: Tue Dec  6 14:48:26 2022, max compression
+gzip compressed data, was "locache-3.0.0.tar", last modified: Fri Apr 21 16:11:06 2023, max compression
```

## Comparing `locache-2.1.1.tar` & `locache-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2022-12-06 14:48:26.407054 locache-2.1.1/
--rw-r--r--   0 john       (504) staff       (20)     1069 2022-12-06 14:45:21.000000 locache-2.1.1/LICENCE.md
--rw-r--r--   0 john       (504) staff       (20)     3276 2022-12-06 14:48:26.406928 locache-2.1.1/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     2830 2022-12-06 14:45:21.000000 locache-2.1.1/README.md
-drwxr-xr-x   0 john       (504) staff       (20)        0 2022-12-06 14:48:26.406210 locache-2.1.1/locache/
--rw-r--r--   0 john       (504) staff       (20)     2246 2022-12-06 14:40:00.000000 locache-2.1.1/locache/LocalCache.py
--rw-r--r--   0 john       (504) staff       (20)     1502 2022-12-06 14:44:38.000000 locache-2.1.1/locache/__init__.py
--rw-r--r--   0 john       (504) staff       (20)      181 2022-10-20 10:03:53.000000 locache-2.1.1/locache/logging.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2022-12-06 14:48:26.406759 locache-2.1.1/locache.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     3276 2022-12-06 14:48:26.000000 locache-2.1.1/locache.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      214 2022-12-06 14:48:26.000000 locache-2.1.1/locache.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2022-12-06 14:48:26.000000 locache-2.1.1/locache.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)        8 2022-12-06 14:48:26.000000 locache-2.1.1/locache.egg-info/top_level.txt
--rw-r--r--   0 john       (504) staff       (20)       38 2022-12-06 14:48:26.407099 locache-2.1.1/setup.cfg
--rw-r--r--   0 john       (504) staff       (20)      714 2022-12-06 14:48:20.000000 locache-2.1.1/setup.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564981 locache-3.0.0/
+-rw-r--r--   0 john       (504) staff       (20)     1069 2022-12-06 14:45:21.000000 locache-3.0.0/LICENCE.md
+-rw-r--r--   0 john       (504) staff       (20)     3318 2023-04-21 16:11:06.564820 locache-3.0.0/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     2830 2022-12-06 14:45:21.000000 locache-3.0.0/README.md
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.563607 locache-3.0.0/locache/
+-rw-r--r--   0 john       (504) staff       (20)     4538 2023-04-21 16:09:53.000000 locache-3.0.0/locache/__init__.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564242 locache-3.0.0/locache.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     3318 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      231 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)       51 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)        8 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/top_level.txt
+-rw-r--r--   0 john       (504) staff       (20)     1042 2023-04-21 16:09:56.000000 locache-3.0.0/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-04-21 16:11:06.565030 locache-3.0.0/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564378 locache-3.0.0/tests/
+-rw-r--r--   0 john       (504) staff       (20)     2176 2023-04-21 15:08:42.000000 locache-3.0.0/tests/test_locache.py
```

### Comparing `locache-2.1.1/LICENCE.md` & `locache-3.0.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `locache-2.1.1/PKG-INFO` & `locache-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: locache
-Version: 2.1.1
+Version: 3.0.0
 Summary: Cache expensive function calls to disk.
-Home-page: https://github.com/jla-gardner/local-cache
-Author: John Gardner
-License: MIT
-Keywords: cache
+Author-email: John Gardner <gardner.john97@gmail.com>
+Project-URL: Homepage, https://github.com/jla-gardner/locache
+Keywords: cache,disk
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENCE.md
 
 # locache
 [![PyPI](https://img.shields.io/pypi/v/locache?style=for-the-badge)](https://pypi.org/project/locache/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/locache?color=green&label=Downloads&logo=Python&logoColor=white&style=for-the-badge)](https://pypistats.org/packages/locache)
 [![GitHub](https://img.shields.io/github/license/jla-gardner/local-cache?style=for-the-badge)](LICENCE.md)
```

### Comparing `locache-2.1.1/README.md` & `locache-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `locache-2.1.1/locache.egg-info/PKG-INFO` & `locache-3.0.0/locache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: locache
-Version: 2.1.1
+Version: 3.0.0
 Summary: Cache expensive function calls to disk.
-Home-page: https://github.com/jla-gardner/local-cache
-Author: John Gardner
-License: MIT
-Keywords: cache
+Author-email: John Gardner <gardner.john97@gmail.com>
+Project-URL: Homepage, https://github.com/jla-gardner/locache
+Keywords: cache,disk
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENCE.md
 
 # locache
 [![PyPI](https://img.shields.io/pypi/v/locache?style=for-the-badge)](https://pypi.org/project/locache/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/locache?color=green&label=Downloads&logo=Python&logoColor=white&style=for-the-badge)](https://pypistats.org/packages/locache)
 [![GitHub](https://img.shields.io/github/license/jla-gardner/local-cache?style=for-the-badge)](LICENCE.md)
```

