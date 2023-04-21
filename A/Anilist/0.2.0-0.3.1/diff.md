# Comparing `tmp/Anilist-0.2.0.tar.gz` & `tmp/Anilist-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Anilist-0.2.0.tar", last modified: Thu Apr 20 22:10:33 2023, max compression
+gzip compressed data, was "Anilist-0.3.1.tar", last modified: Fri Apr 21 03:22:07 2023, max compression
```

## Comparing `Anilist-0.2.0.tar` & `Anilist-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.741804 Anilist-0.2.0/
--rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      563 2023-04-20 22:10:33.740802 Anilist-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.2.0/README.md
--rw-rw-rw-   0        0        0      601 2023-04-20 22:10:03.000000 Anilist-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-20 22:10:33.742800 Anilist-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.695988 Anilist-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.710978 Anilist-0.2.0/src/Anilist/
--rw-rw-rw-   0        0        0      127 2023-04-20 21:56:55.000000 Anilist-0.2.0/src/Anilist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.732965 Anilist-0.2.0/src/Anilist/auth/
--rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.2.0/src/Anilist/auth/auth.py
--rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.2.0/src/Anilist/auth/code.py
--rw-rw-rw-   0        0        0      497 2023-04-19 21:18:07.000000 Anilist-0.2.0/src/Anilist/auth/token.py
--rw-rw-rw-   0        0        0     2166 2023-04-20 22:04:46.000000 Anilist-0.2.0/src/Anilist/client.py
--rw-rw-rw-   0        0        0       51 2023-04-19 21:07:09.000000 Anilist-0.2.0/src/Anilist/consts.py
--rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.2.0/src/Anilist/logging.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.735963 Anilist-0.2.0/src/Anilist/mutation/
--rw-rw-rw-   0        0        0        0 2023-04-19 21:32:11.000000 Anilist-0.2.0/src/Anilist/mutation/__init__.py
--rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.2.0/src/Anilist/mutation/media_list.py
--rw-rw-rw-   0        0        0      599 2023-04-20 21:27:29.000000 Anilist-0.2.0/src/Anilist/obj.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.738799 Anilist-0.2.0/src/Anilist/query/
--rw-rw-rw-   0        0        0        0 2023-04-19 23:42:28.000000 Anilist-0.2.0/src/Anilist/query/__init__.py
--rw-rw-rw-   0        0        0     1933 2023-04-20 21:27:54.000000 Anilist-0.2.0/src/Anilist/query/media_list.py
--rw-rw-rw-   0        0        0     1498 2023-04-20 21:17:57.000000 Anilist-0.2.0/src/Anilist/scheme.py
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.728967 Anilist-0.2.0/src/Anilist.egg-info/
--rw-rw-rw-   0        0        0      563 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-20 22:10:33.000000 Anilist-0.2.0/src/Anilist.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 22:10:33.739803 Anilist-0.2.0/tests/
--rw-rw-rw-   0        0        0      294 2023-04-20 22:04:12.000000 Anilist-0.2.0/tests/test_base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.211926 Anilist-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.124981 Anilist-0.3.1/Anilist/
+-rw-rw-rw-   0        0        0      127 2023-04-21 03:20:18.000000 Anilist-0.3.1/Anilist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.160957 Anilist-0.3.1/Anilist/auth/
+-rw-rw-rw-   0        0        0      719 2023-04-19 21:58:46.000000 Anilist-0.3.1/Anilist/auth/auth.py
+-rw-rw-rw-   0        0        0     1007 2023-04-19 23:18:58.000000 Anilist-0.3.1/Anilist/auth/code.py
+-rw-rw-rw-   0        0        0      497 2023-04-19 21:18:07.000000 Anilist-0.3.1/Anilist/auth/token.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.197934 Anilist-0.3.1/Anilist/client/
+-rw-rw-rw-   0        0        0       96 2023-04-21 03:19:41.000000 Anilist-0.3.1/Anilist/client/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-21 03:20:24.000000 Anilist-0.3.1/Anilist/client/client.py
+-rw-rw-rw-   0        0        0      365 2023-04-21 03:19:10.000000 Anilist-0.3.1/Anilist/client/mutation.py
+-rw-rw-rw-   0        0        0      577 2023-04-21 03:20:31.000000 Anilist-0.3.1/Anilist/client/query.py
+-rw-rw-rw-   0        0        0      190 2023-04-21 03:11:45.000000 Anilist-0.3.1/Anilist/consts.py
+-rw-rw-rw-   0        0        0     1571 2023-04-20 22:06:18.000000 Anilist-0.3.1/Anilist/logging.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.199933 Anilist-0.3.1/Anilist/mutation/
+-rw-rw-rw-   0        0        0        0 2023-04-19 21:32:11.000000 Anilist-0.3.1/Anilist/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1302 2023-04-19 23:39:31.000000 Anilist-0.3.1/Anilist/mutation/media_list.py
+-rw-rw-rw-   0        0        0      599 2023-04-20 21:27:29.000000 Anilist-0.3.1/Anilist/object.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.203930 Anilist-0.3.1/Anilist/query/
+-rw-rw-rw-   0        0        0        0 2023-04-19 23:42:28.000000 Anilist-0.3.1/Anilist/query/__init__.py
+-rw-rw-rw-   0        0        0     1933 2023-04-21 00:03:00.000000 Anilist-0.3.1/Anilist/query/media_list.py
+-rw-rw-rw-   0        0        0     2007 2023-04-21 03:14:07.000000 Anilist-0.3.1/Anilist/scheme.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.152962 Anilist-0.3.1/Anilist.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 03:22:07.000000 Anilist-0.3.1/Anilist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-04-20 22:07:52.000000 Anilist-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-04-21 03:22:07.210926 Anilist-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:05:02.000000 Anilist-0.3.1/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-21 03:07:29.000000 Anilist-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 03:22:07.211926 Anilist-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 03:22:07.208928 Anilist-0.3.1/tests/
+-rw-rw-rw-   0        0        0      383 2023-04-21 03:16:41.000000 Anilist-0.3.1/tests/test_base.py
```

### Comparing `Anilist-0.2.0/LICENSE` & `Anilist-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/PKG-INFO` & `Anilist-0.3.1/Anilist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.2.0
+Version: 0.3.1
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Anilist-0.2.0/pyproject.toml` & `Anilist-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Anilist"
-version = "0.2.0"
+version = "0.3.1"
 authors = [
   { name="Ann Mauduy-Decius", email="ann.mauduy.decius@gmail.com" },
 ]
 description = "Anilist API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `Anilist-0.2.0/src/Anilist/auth/auth.py` & `Anilist-0.3.1/Anilist/auth/auth.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist/auth/code.py` & `Anilist-0.3.1/Anilist/auth/code.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist/logging.py` & `Anilist-0.3.1/Anilist/logging.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist/mutation/media_list.py` & `Anilist-0.3.1/Anilist/mutation/media_list.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist/obj.py` & `Anilist-0.3.1/Anilist/object.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist/query/media_list.py` & `Anilist-0.3.1/Anilist/query/media_list.py`

 * *Files identical despite different names*

### Comparing `Anilist-0.2.0/src/Anilist.egg-info/PKG-INFO` & `Anilist-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Anilist
-Version: 0.2.0
+Version: 0.3.1
 Summary: Anilist API wrapper
 Author-email: Ann Mauduy-Decius <ann.mauduy.decius@gmail.com>
 Project-URL: Homepage, https://github.com/xxxAnn/Anilist.py
 Project-URL: Bug Tracker, https://github.com/xxxAnn/Anilist.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

