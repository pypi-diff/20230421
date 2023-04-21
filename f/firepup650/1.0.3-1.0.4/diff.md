# Comparing `tmp/firepup650-1.0.3.tar.gz` & `tmp/firepup650-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firepup650-1.0.3.tar", last modified: Fri Apr 21 14:28:00 2023, max compression
+gzip compressed data, was "firepup650-1.0.4.tar", last modified: Fri Apr 21 14:43:26 2023, max compression
```

## Comparing `firepup650-1.0.3.tar` & `firepup650-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:28:00.184684 firepup650-1.0.3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1225 2023-04-21 14:28:00.184684 firepup650-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      294 2023-04-21 14:27:30.000000 firepup650-1.0.3/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-04-21 14:24:26.000000 firepup650-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-21 14:28:00.184684 firepup650-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:28:00.184684 firepup650-1.0.3/src/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:28:00.184684 firepup650-1.0.3/src/firepup650/
--rw-r--r--   0 runner    (1000) runner    (1000)     3302 2023-04-21 14:25:14.000000 firepup650-1.0.3/src/firepup650/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:28:00.184684 firepup650-1.0.3/src/firepup650.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1225 2023-04-21 14:27:59.000000 firepup650-1.0.3/src/firepup650.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-21 14:27:59.000000 firepup650-1.0.3/src/firepup650.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-21 14:27:59.000000 firepup650-1.0.3/src/firepup650.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-21 14:27:59.000000 firepup650-1.0.3/src/firepup650.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1072 2021-11-16 19:34:41.000000 firepup650-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-04-21 14:43:26.836159 firepup650-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-04-21 14:41:13.000000 firepup650-1.0.4/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      310 2023-04-21 14:24:26.000000 firepup650-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)      895 2023-04-21 14:43:26.836159 firepup650-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.832159 firepup650-1.0.4/src/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/src/firepup650/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3382 2023-04-21 14:40:17.000000 firepup650-1.0.4/src/firepup650/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-21 14:43:26.836159 firepup650-1.0.4/src/firepup650.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1274 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      221 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-21 14:43:26.000000 firepup650-1.0.4/src/firepup650.egg-info/top_level.txt
```

### Comparing `firepup650-1.0.3/LICENSE` & `firepup650-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `firepup650-1.0.3/PKG-INFO` & `firepup650-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.4:
+        Subscript errors
         ###### v.1.0.3:
         Dependant errors
         ###### v.1.0.2:
         Random shorthand (litterally)
         ###### v.1.0.1:
         Added animated typing function, sleep shorthand
         ###### v.1.0.0:
```

### Comparing `firepup650-1.0.3/setup.cfg` & `firepup650-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = firepup650
-version = 1.0.3
+version = 1.0.4
 author = Firepup650
 author_email = firepyp650@gmail.com
 description = Package containing various shorthand things I use, and a few imports I almost always use
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/F1repup650/firepup650-PYPI
 project_urls =
```

### Comparing `firepup650-1.0.3/src/firepup650/__init__.py` & `firepup650-1.0.4/src/firepup650/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -124,15 +124,19 @@
   
   # Returns:
     None
   
   # Raises:
     None"""
   r.seed(seed, version)
-def robj(sequence: any[object]) -> object:
+def robj(sequence: any) -> object:
   """# Function: robj
     Returns a random object from the provided sequence
   # Input:
     sequence: Sequence[object] - Any valid sequence
   
-  # """
+  # Returns:
+    object - A random object from the provided sequence
+  
+  # Raises:
+    None"""
   r.choice(sequence)
```

### Comparing `firepup650-1.0.3/src/firepup650.egg-info/PKG-INFO` & `firepup650-1.0.4/src/firepup650.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: firepup650
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package containing various shorthand things I use, and a few imports I almost always use
 Home-page: https://github.com/F1repup650/firepup650-PYPI
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/F1repup650/firepup650-PYPI/issues
 Project-URL: replit, https://replit.com/@Firepup650/firepup650-PYPI-Package
 Description: # Firepup650
         Package containing various shorthand things I use, and a few imports I almost always use
         #### Change log:
+        ###### v.1.0.4:
+        Subscript errors
         ###### v.1.0.3:
         Dependant errors
         ###### v.1.0.2:
         Random shorthand (litterally)
         ###### v.1.0.1:
         Added animated typing function, sleep shorthand
         ###### v.1.0.0:
```

