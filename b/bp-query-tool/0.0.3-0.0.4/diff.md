# Comparing `tmp/bp_query_tool-0.0.3.tar.gz` & `tmp/bp_query_tool-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_query_tool-0.0.3.tar", last modified: Fri Apr 21 05:58:47 2023, max compression
+gzip compressed data, was "bp_query_tool-0.0.4.tar", last modified: Fri Apr 21 09:42:00 2023, max compression
```

## Comparing `bp_query_tool-0.0.3.tar` & `bp_query_tool-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.873684 bp_query_tool-0.0.3/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.3/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.3/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 05:58:47.873279 bp_query_tool-0.0.3/PKG-INFO
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.864910 bp_query_tool-0.0.3/bp_query_tool.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-21 05:58:47.000000 bp_query_tool-0.0.3/bp_query_tool.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.865329 bp_query_tool-0.0.3/query_tool/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.3/query_tool/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.860699 bp_query_tool-0.0.3/query_tool/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.866135 bp_query_tool-0.0.3/query_tool/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.869004 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044744 2023-04-17 07:29:32.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-99e5fe3f.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-17 07:29:32.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-17 07:29:52.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-17 07:29:31.000000 bp_query_tool-0.0.3/query_tool/frontend/dist/vite.svg
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 05:58:47.872493 bp_query_tool-0.0.3/query_tool/services/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/dimension_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/entities_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/filters_service.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/query_tool_factory.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/query_tool_service.py
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.3/query_tool/services/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 05:58:47.873860 bp_query_tool-0.0.3/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-21 05:56:28.000000 bp_query_tool-0.0.3/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.698653 bp_query_tool-0.0.4/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-03 17:08:00.000000 bp_query_tool-0.0.4/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       45 2023-04-05 19:58:10.000000 bp_query_tool-0.0.4/MANIFEST.in
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 09:42:00.698238 bp_query_tool-0.0.4/PKG-INFO
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.688900 bp_query_tool-0.0.4/bp_query_tool.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      312 2023-04-21 09:42:00.000000 bp_query_tool-0.0.4/bp_query_tool.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      674 2023-04-21 09:42:00.000000 bp_query_tool-0.0.4/bp_query_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-21 09:42:00.000000 bp_query_tool-0.0.4/bp_query_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-21 09:42:00.000000 bp_query_tool-0.0.4/bp_query_tool.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       11 2023-04-21 09:42:00.000000 bp_query_tool-0.0.4/bp_query_tool.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.689289 bp_query_tool-0.0.4/query_tool/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     3587 2023-04-13 18:16:00.000000 bp_query_tool-0.0.4/query_tool/__init__.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.684050 bp_query_tool-0.0.4/query_tool/frontend/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.690097 bp_query_tool-0.0.4/query_tool/frontend/dist/
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.693293 bp_query_tool-0.0.4/query_tool/frontend/dist/assets/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1044762 2023-04-21 09:39:39.000000 bp_query_tool-0.0.4/query_tool/frontend/dist/assets/index-9cb700e1.js
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-04-21 09:39:39.000000 bp_query_tool-0.0.4/query_tool/frontend/dist/assets/index-d081bea5.css
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      463 2023-04-21 09:39:55.000000 bp_query_tool-0.0.4/query_tool/frontend/dist/index.html
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-04-21 09:39:38.000000 bp_query_tool-0.0.4/query_tool/frontend/dist/vite.svg
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-21 09:42:00.697359 bp_query_tool-0.0.4/query_tool/services/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1438 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/dimension_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3941 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/entities_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3653 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/filters_service.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      437 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/query_tool_factory.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1987 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/query_tool_service.py
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-03 16:47:55.000000 bp_query_tool-0.0.4/query_tool/services/register.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-21 09:42:00.698775 bp_query_tool-0.0.4/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      646 2023-04-21 09:40:28.000000 bp_query_tool-0.0.4/setup.py
```

### Comparing `bp_query_tool-0.0.3/LICENSE` & `bp_query_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/bp_query_tool.egg-info/SOURCES.txt` & `bp_query_tool-0.0.4/bp_query_tool.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 bp_query_tool.egg-info/SOURCES.txt
 bp_query_tool.egg-info/dependency_links.txt
 bp_query_tool.egg-info/requires.txt
 bp_query_tool.egg-info/top_level.txt
 query_tool/__init__.py
 query_tool/frontend/dist/index.html
 query_tool/frontend/dist/vite.svg
-query_tool/frontend/dist/assets/index-99e5fe3f.js
+query_tool/frontend/dist/assets/index-9cb700e1.js
 query_tool/frontend/dist/assets/index-d081bea5.css
 query_tool/services/__init__.py
 query_tool/services/dimension_service.py
 query_tool/services/entities_service.py
 query_tool/services/filters_service.py
 query_tool/services/query_tool_factory.py
 query_tool/services/query_tool_service.py
```

### Comparing `bp_query_tool-0.0.3/query_tool/__init__.py` & `bp_query_tool-0.0.4/query_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/frontend/dist/assets/index-99e5fe3f.js` & `bp_query_tool-0.0.4/query_tool/frontend/dist/assets/index-9cb700e1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -45782,14 +45782,15 @@
                         })
                     })
                 })]
             })]
         })
     },
     $Ee = e => U(hc, {
+        disableGutters: !0,
         component: "div",
         maxWidth: !1,
         sx: {
             ...e == null ? void 0 : e.style
         },
         children: U(WEe, {
             ...e
```

### Comparing `bp_query_tool-0.0.3/query_tool/frontend/dist/vite.svg` & `bp_query_tool-0.0.4/query_tool/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/services/dimension_service.py` & `bp_query_tool-0.0.4/query_tool/services/dimension_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/services/entities_service.py` & `bp_query_tool-0.0.4/query_tool/services/entities_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/services/filters_service.py` & `bp_query_tool-0.0.4/query_tool/services/filters_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/services/query_tool_service.py` & `bp_query_tool-0.0.4/query_tool/services/query_tool_service.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/query_tool/services/register.py` & `bp_query_tool-0.0.4/query_tool/services/register.py`

 * *Files identical despite different names*

### Comparing `bp_query_tool-0.0.3/setup.py` & `bp_query_tool-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_query_tool",
-    version="0.0.3",
+    version="0.0.4",
     author="Bluepinapple",
     author_email="vivek.sthul@bluepinapple.com",
     description="Query tool to generate query from selection",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

