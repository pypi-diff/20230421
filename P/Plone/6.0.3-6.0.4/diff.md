# Comparing `tmp/Plone-6.0.3.tar.gz` & `tmp/Plone-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Plone-6.0.3.tar", last modified: Thu Mar 23 12:24:23 2023, max compression
+gzip compressed data, was "Plone-6.0.4.tar", last modified: Fri Apr 21 14:48:07 2023, max compression
```

## Comparing `Plone-6.0.3.tar` & `Plone-6.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.234242 Plone-6.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)     6573 2023-03-23 12:24:22.000000 Plone-6.0.3/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       95 2023-03-23 12:24:22.000000 Plone-6.0.3/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)       24 2023-03-23 12:24:22.000000 Plone-6.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14393 2023-03-23 12:24:23.234400 Plone-6.0.3/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.232150 Plone-6.0.3/Plone.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14393 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      324 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-23 12:24:23.000000 Plone-6.0.3/Plone.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     6411 2023-03-23 12:24:22.000000 Plone-6.0.3/README.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-23 12:24:23.233880 Plone-6.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/CREDITS.txt
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.ZPL
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1493 2023-03-23 12:24:22.000000 Plone-6.0.3/docs/UPGRADE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1531 2023-03-23 12:24:23.234995 Plone-6.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-03-23 12:24:22.000000 Plone-6.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:48:07.428978 Plone-6.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)     6639 2023-04-21 14:48:06.000000 Plone-6.0.4/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2023-04-21 14:48:06.000000 Plone-6.0.4/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-04-21 14:48:06.000000 Plone-6.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    14459 2023-04-21 14:48:07.429162 Plone-6.0.4/PKG-INFO
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:48:07.427186 Plone-6.0.4/Plone.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    14459 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      324 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-21 14:48:07.000000 Plone-6.0.4/Plone.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     6411 2023-04-21 14:48:06.000000 Plone-6.0.4/README.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-21 14:48:07.428729 Plone-6.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     6320 2023-04-21 14:48:06.000000 Plone-6.0.4/docs/CREDITS.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-21 14:48:06.000000 Plone-6.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)     2070 2023-04-21 14:48:06.000000 Plone-6.0.4/docs/LICENSE.ZPL
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2023-04-21 14:48:06.000000 Plone-6.0.4/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1493 2023-04-21 14:48:06.000000 Plone-6.0.4/docs/UPGRADE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1531 2023-04-21 14:48:07.429829 Plone-6.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-04-21 14:48:06.000000 Plone-6.0.4/setup.py
```

### Comparing `Plone-6.0.3/CHANGES.md` & `Plone-6.0.4/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## 6.0.4 (2023-04-21)
+
+Bug fixes:
+
+- Release 6.0.4.
+  [maurits]
+
+
 ## 6.0.3 (2023-03-23)
 
 Bug fixes:
 
 - Release 6.0.3.
   [maurits]
```

### Comparing `Plone-6.0.3/PKG-INFO` & `Plone-6.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.0.3
+Version: 6.0.4
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -173,14 +173,22 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.0.4 (2023-04-21)
+
+Bug fixes:
+
+- Release 6.0.4.
+  [maurits]
+
+
 ## 6.0.3 (2023-03-23)
 
 Bug fixes:
 
 - Release 6.0.3.
   [maurits]
```

### Comparing `Plone-6.0.3/Plone.egg-info/PKG-INFO` & `Plone-6.0.4/Plone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Plone
-Version: 6.0.3
+Version: 6.0.4
 Summary: The Plone Content Management System
 Home-page: https://plone.org/
 Author: Plone Foundation
 Author-email: releaseteam@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -173,14 +173,22 @@
 <h2 align="center">
 License
 </h2>
 The project is licensed under the GPLv2.
 
 # Changelog
 
+## 6.0.4 (2023-04-21)
+
+Bug fixes:
+
+- Release 6.0.4.
+  [maurits]
+
+
 ## 6.0.3 (2023-03-23)
 
 Bug fixes:
 
 - Release 6.0.3.
   [maurits]
```

### Comparing `Plone-6.0.3/README.md` & `Plone-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/docs/CREDITS.txt` & `Plone-6.0.4/docs/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/docs/LICENSE.GPL` & `Plone-6.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/docs/LICENSE.ZPL` & `Plone-6.0.4/docs/LICENSE.ZPL`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/docs/LICENSE.txt` & `Plone-6.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/docs/UPGRADE.txt` & `Plone-6.0.4/docs/UPGRADE.txt`

 * *Files identical despite different names*

### Comparing `Plone-6.0.3/setup.cfg` & `Plone-6.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 6.0.3
+version = 6.0.4
 name = Plone
 description = The Plone Content Management System
 long_description = file: README.md, CHANGES.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
```

