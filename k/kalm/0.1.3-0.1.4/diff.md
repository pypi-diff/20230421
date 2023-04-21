# Comparing `tmp/kalm-0.1.3.tar.gz` & `tmp/kalm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.1.3.tar", last modified: Fri Apr 21 10:37:45 2023, max compression
+gzip compressed data, was "kalm-0.1.4.tar", last modified: Fri Apr 21 10:38:42 2023, max compression
```

## Comparing `kalm-0.1.3.tar` & `kalm-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.586672 kalm-0.1.3/
--rw-rw-r--   0 jho       (1000) jho       (1000)     1081 2023-04-21 06:37:05.000000 kalm-0.1.3/LICENSE.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:37:45.586672 kalm-0.1.3/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      705 2023-04-21 06:37:05.000000 kalm-0.1.3/README.md
--rw-rw-r--   0 jho       (1000) jho       (1000)     1272 2023-04-21 10:37:41.000000 kalm-0.1.3/pyproject.toml
--rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:37:45.586672 kalm-0.1.3/setup.cfg
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.584672 kalm-0.1.3/src/
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.585672 kalm-0.1.3/src/kalm/
--rw-rw-r--   0 jho       (1000) jho       (1000)    10449 2023-04-21 06:51:36.000000 kalm-0.1.3/src/kalm/__init__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)    31998 2023-04-21 06:53:06.000000 kalm-0.1.3/src/kalm/kalm.py
--rw-rw-r--   0 jho       (1000) jho       (1000)     1296 2023-04-21 06:37:05.000000 kalm-0.1.3/src/kalm/netbox.py
--rw-rw-r--   0 jho       (1000) jho       (1000)        9 2023-04-21 06:37:05.000000 kalm-0.1.3/src/kalm/package_data.dat
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:41:48.000000 kalm-0.1.3/src/kalm/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.586672 kalm-0.1.3/src/kalm.egg-info/
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      377 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/SOURCES.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/dependency_links.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       35 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/entry_points.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       67 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/requires.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       13 2023-04-21 10:37:45.000000 kalm-0.1.3/src/kalm.egg-info/top_level.txt
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.586672 kalm-0.1.3/src/toolbox/
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:46:41.000000 kalm-0.1.3/src/toolbox/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:37:45.586672 kalm-0.1.3/tests/
--rw-rw-r--   0 jho       (1000) jho       (1000)      417 2023-04-21 06:37:05.000000 kalm-0.1.3/tests/test_simple.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1081 2023-04-21 06:37:05.000000 kalm-0.1.4/LICENSE.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:38:42.318096 kalm-0.1.4/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)      705 2023-04-21 06:37:05.000000 kalm-0.1.4/README.md
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1282 2023-04-21 10:38:35.000000 kalm-0.1.4/pyproject.toml
+-rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:38:42.318096 kalm-0.1.4/setup.cfg
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.316096 kalm-0.1.4/src/
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.317096 kalm-0.1.4/src/kalm/
+-rw-rw-r--   0 jho       (1000) jho       (1000)    10449 2023-04-21 06:51:36.000000 kalm-0.1.4/src/kalm/__init__.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)    31998 2023-04-21 06:53:06.000000 kalm-0.1.4/src/kalm/kalm.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)     1296 2023-04-21 06:37:05.000000 kalm-0.1.4/src/kalm/netbox.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)        9 2023-04-21 06:37:05.000000 kalm-0.1.4/src/kalm/package_data.dat
+-rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:41:48.000000 kalm-0.1.4/src/kalm/toolbox.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/src/kalm.egg-info/
+-rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)      377 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/SOURCES.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/dependency_links.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       35 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/entry_points.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/requires.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       13 2023-04-21 10:38:42.000000 kalm-0.1.4/src/kalm.egg-info/top_level.txt
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/src/toolbox/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:46:41.000000 kalm-0.1.4/src/toolbox/toolbox.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:38:42.318096 kalm-0.1.4/tests/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      417 2023-04-21 06:37:05.000000 kalm-0.1.4/tests/test_simple.py
```

### Comparing `kalm-0.1.3/LICENSE.txt` & `kalm-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.1.3/PKG-INFO` & `kalm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Jakob Holst <jho@miracle.dk>
 Maintainer-email: Jakob Holst <jho@miracle.dk>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `kalm-0.1.3/README.md` & `kalm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kalm-0.1.3/pyproject.toml` & `kalm-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kalm"  
-version = "0.1.3" 
+version = "0.1.4" 
 description = "" 
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
@@ -25,14 +25,15 @@
   "Programming Language :: Python :: 3",
 ]
 
 dependencies = [ # Optional
   "redis",
   "pynetbox",
   "wheel",
+  "hvac",
   "netbox"
 ]
 
 [project.optional-dependencies] # Optional
 dev = ["check-manifest"]
 test = ["coverage"]
```

### Comparing `kalm-0.1.3/src/kalm/__init__.py` & `kalm-0.1.4/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.1.3/src/kalm/kalm.py` & `kalm-0.1.4/src/kalm/kalm.py`

 * *Files identical despite different names*

### Comparing `kalm-0.1.3/src/kalm/netbox.py` & `kalm-0.1.4/src/kalm/netbox.py`

 * *Files identical despite different names*

### Comparing `kalm-0.1.3/src/kalm.egg-info/PKG-INFO` & `kalm-0.1.4/src/kalm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalm
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Jakob Holst <jho@miracle.dk>
 Maintainer-email: Jakob Holst <jho@miracle.dk>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

