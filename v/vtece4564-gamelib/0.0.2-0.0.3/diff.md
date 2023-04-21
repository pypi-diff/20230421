# Comparing `tmp/vtece4564-gamelib-0.0.2.tar.gz` & `tmp/vtece4564-gamelib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtece4564-gamelib-0.0.2.tar", last modified: Fri Apr 21 19:24:32 2023, max compression
+gzip compressed data, was "vtece4564-gamelib-0.0.3.tar", last modified: Fri Apr 21 19:28:28 2023, max compression
```

## Comparing `vtece4564-gamelib-0.0.2.tar` & `vtece4564-gamelib-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.512395 vtece4564-gamelib-0.0.2/
--rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 19:24:32.512566 vtece4564-gamelib-0.0.2/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)      435 2023-04-21 18:13:29.000000 vtece4564-gamelib-0.0.2/README.md
--rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.2/pyproject.toml
--rw-r--r--   0 ceharris   (501) staff       (20)      737 2023-04-21 19:24:32.513608 vtece4564-gamelib-0.0.2/setup.cfg
--rw-r--r--   0 ceharris   (501) staff       (20)      146 2023-04-21 18:23:19.000000 vtece4564-gamelib-0.0.2/setup.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.497615 vtece4564-gamelib-0.0.2/src/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.497706 vtece4564-gamelib-0.0.2/src/main/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.498937 vtece4564-gamelib-0.0.2/src/main/python/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.503012 vtece4564-gamelib-0.0.2/src/main/python/gameauth/
--rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/__main__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/key_util.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1385 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/password.py
--rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/token.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/token_generator.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.2/src/main/python/gameauth/token_validator.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.503291 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/
--rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/__init__.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.504788 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/
--rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/game_client.py
--rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3804 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/tcp_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/ws_connection.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.506147 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/
--rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/tcp_listener.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/ws_listener.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.507007 vtece4564-gamelib-0.0.2/src/main/python/gamedb/
--rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/game_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.508467 vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/
--rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/json_db.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2141 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.509938 vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/
--rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/user_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.2/src/main/python/gamedb/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:24:32.512053 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/
--rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 19:24:32.000000 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)     1494 2023-04-21 19:24:32.000000 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
--rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-21 19:24:32.000000 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       38 2023-04-21 19:24:32.000000 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/requires.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-21 19:24:32.000000 vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.720940 vtece4564-gamelib-0.0.3/
+-rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 19:28:28.721113 vtece4564-gamelib-0.0.3/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)      435 2023-04-21 18:13:29.000000 vtece4564-gamelib-0.0.3/README.md
+-rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.3/pyproject.toml
+-rw-r--r--   0 ceharris   (501) staff       (20)      737 2023-04-21 19:28:28.722193 vtece4564-gamelib-0.0.3/setup.cfg
+-rw-r--r--   0 ceharris   (501) staff       (20)      146 2023-04-21 18:23:19.000000 vtece4564-gamelib-0.0.3/setup.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.703429 vtece4564-gamelib-0.0.3/src/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.703576 vtece4564-gamelib-0.0.3/src/main/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.705078 vtece4564-gamelib-0.0.3/src/main/python/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.710157 vtece4564-gamelib-0.0.3/src/main/python/gameauth/
+-rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/__main__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/key_util.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1385 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/password.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/token.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/token_generator.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.3/src/main/python/gameauth/token_validator.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.710740 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/
+-rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/__init__.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.712400 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/
+-rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/game_client.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3804 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/tcp_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/ws_connection.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.713774 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/
+-rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/tcp_listener.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/ws_listener.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.714746 vtece4564-gamelib-0.0.3/src/main/python/gamedb/
+-rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/game_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.716205 vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/
+-rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/json_db.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2299 2023-04-21 19:28:13.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.717713 vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/
+-rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/user_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.3/src/main/python/gamedb/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-21 19:28:28.720606 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/
+-rw-r--r--   0 ceharris   (501) staff       (20)      940 2023-04-21 19:28:28.000000 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)     1494 2023-04-21 19:28:28.000000 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-21 19:28:28.000000 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       38 2023-04-21 19:28:28.000000 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/requires.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-21 19:28:28.000000 vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
```

### Comparing `vtece4564-gamelib-0.0.2/PKG-INFO` & `vtece4564-gamelib-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-gamelib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A support library for the ECE 4564 Final Project
 Home-page: https://code.vt.edu/ece4564/gamelib
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://code.vt.edu/ece4564/gamelib/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtece4564-gamelib-0.0.2/setup.cfg` & `vtece4564-gamelib-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtece4564-gamelib
-version = 0.0.2
+version = 0.0.3
 author = Carl Harris
 author_email = ceharris414@gmail.com
 description = A support library for the ECE 4564 Final Project
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.vt.edu/ece4564/gamelib
 project_urls =
```

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gameauth/__main__.py` & `vtece4564-gamelib-0.0.3/src/main/python/gameauth/__main__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gameauth/key_util.py` & `vtece4564-gamelib-0.0.3/src/main/python/gameauth/key_util.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gameauth/password.py` & `vtece4564-gamelib-0.0.3/src/main/python/gameauth/password.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gameauth/token_generator.py` & `vtece4564-gamelib-0.0.3/src/main/python/gameauth/token_generator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gameauth/token_validator.py` & `vtece4564-gamelib-0.0.3/src/main/python/gameauth/token_validator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/game_client.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/game_client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/tcp_connection.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/client/ws_connection.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/client/ws_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/game_connection.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/game_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/tcp_listener.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/tcp_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamecomm/server/ws_listener.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamecomm/server/ws_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/game_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/game_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/json_db.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/json_db.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/json/user_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/json/user_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from datetime import datetime
 from typing import Dict
 
 
 from ..user_repository import User, UserRepository, NoSuchUserError, DuplicateUserIdError
 from .json_db import JsonDatabase
 
 
@@ -15,24 +16,27 @@
 logger = logging.getLogger(__name__)
 
 
 class JsonUser(User):
 
     @classmethod
     def from_dict(cls, rec: dict):
-        record = User(rec.get(_UID_KEY), rec.get(_PASSWORD_KEY), is_encrypted=True, creation_date=rec.get(_CREATION_DATE_KEY))
+        record = User(uid=rec.get(_UID_KEY),
+                      password=rec.get(_PASSWORD_KEY),
+                      is_encrypted=True,
+                      creation_date=datetime.fromisoformat(rec.get(_CREATION_DATE_KEY)))
         record.nickname = rec.get(_NICKNAME_KEY)
         record.full_name = rec.get(_FULL_NAME_KEY)
         return record
 
     def to_dict(self) -> Dict:
         record = {
             _UID_KEY: self.uid,
             _PASSWORD_KEY: self.password,
-            _CREATION_DATE_KEY: self.creation_date,
+            _CREATION_DATE_KEY: self.creation_date.astimezone().isoformat(),
         }
         if self.full_name:
             record.update({_FULL_NAME_KEY: self.full_name})
         if self.nickname:
             record.update({_NICKNAME_KEY: self.nickname})
         return record
```

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/game_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/mongo/user_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/mongo/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/gamedb/user_repository.py` & `vtece4564-gamelib-0.0.3/src/main/python/gamedb/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO` & `vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-gamelib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A support library for the ECE 4564 Final Project
 Home-page: https://code.vt.edu/ece4564/gamelib
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://code.vt.edu/ece4564/gamelib/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtece4564-gamelib-0.0.2/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt` & `vtece4564-gamelib-0.0.3/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

