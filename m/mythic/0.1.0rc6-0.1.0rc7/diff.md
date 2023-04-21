# Comparing `tmp/mythic-0.1.0rc6.tar.gz` & `tmp/mythic-0.1.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc6.tar", last modified: Thu Apr 20 16:27:24 2023, max compression
+gzip compressed data, was "mythic-0.1.0rc7.tar", last modified: Fri Apr 21 17:51:56 2023, max compression
```

## Comparing `mythic-0.1.0rc6.tar` & `mythic-0.1.0rc7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.871290 mythic-0.1.0rc6/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-20 16:27:24.870866 mythic-0.1.0rc6/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc6/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.868345 mythic-0.1.0rc6/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc6/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc6/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    95248 2023-04-20 16:26:24.000000 mythic-0.1.0rc6/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-20 16:27:07.000000 mythic-0.1.0rc6/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc6/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc6/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-20 16:27:24.870391 mythic-0.1.0rc6/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-20 16:27:24.000000 mythic-0.1.0rc6/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-20 16:27:24.871411 mythic-0.1.0rc6/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-20 16:26:50.000000 mythic-0.1.0rc6/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.575304 mythic-0.1.0rc7/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-21 17:51:56.574032 mythic-0.1.0rc7/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc7/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.571264 mythic-0.1.0rc7/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc7/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc7/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    95272 2023-04-21 17:51:11.000000 mythic-0.1.0rc7/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-21 17:51:52.000000 mythic-0.1.0rc7/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc7/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc7/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.573314 mythic-0.1.0rc7/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-21 17:51:56.575740 mythic-0.1.0rc7/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-21 17:51:43.000000 mythic-0.1.0rc7/setup.py
```

### Comparing `mythic-0.1.0rc6/PKG-INFO` & `mythic-0.1.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc6/README.md` & `mythic-0.1.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc6/mythic/graphql_queries.py` & `mythic-0.1.0rc7/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc6/mythic/mythic.py` & `mythic-0.1.0rc7/mythic/mythic.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,16 +474,17 @@
     ):
         yield t
     async for t in subscribe_new_tasks_and_updates(
         mythic=mythic,
         timeout=timeout,
         custom_return_attributes=custom_return_attributes,
         callback_display_id=callback_display_id,
+        batch_size=1
     ):
-        yield t
+        yield t[0]
 
 
 async def add_mitre_attack_to_task(
     mythic: mythic_classes.Mythic, task_display_id: int, mitre_attack_numbers: List[str]
 ) -> bool:
     """
     Adds the supplied MITRE ATT&CK techniques to the specified task.
```

### Comparing `mythic-0.1.0rc6/mythic/mythic_classes.py` & `mythic-0.1.0rc7/mythic/mythic_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.0rc6"
+        self.scripting_version = "0.1.0rc7"
         self.current_operation_id = 0
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
```

### Comparing `mythic-0.1.0rc6/mythic/mythic_utilities.py` & `mythic-0.1.0rc7/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc6/mythic.egg-info/PKG-INFO` & `mythic-0.1.0rc7/mythic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc6
+Version: 0.1.0rc7
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc6/setup.py` & `mythic-0.1.0rc7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc6",
+    version="0.1.0rc7",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

