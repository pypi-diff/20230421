# Comparing `tmp/jupyspace_api-0.0.3.tar.gz` & `tmp/jupyspace_api-0.0.4.tar.gz`

## Comparing `jupyspace_api-0.0.3.tar` & `jupyspace_api-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/app.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/exceptions.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/main.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/router.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/space/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/jupyspace_api/space/models.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/README.md
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 jupyspace_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/app.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/exceptions.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/main.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/router.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/space/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/jupyspace_api/space/models.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/README.md
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 jupyspace_api-0.0.4/PKG-INFO
```

### Comparing `jupyspace_api-0.0.3/jupyspace_api/app.py` & `jupyspace_api-0.0.4/jupyspace_api/app.py`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/jupyspace_api/main.py` & `jupyspace_api-0.0.4/jupyspace_api/main.py`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/jupyspace_api/space/__init__.py` & `jupyspace_api-0.0.4/jupyspace_api/space/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/jupyspace_api/space/models.py` & `jupyspace_api-0.0.4/jupyspace_api/space/models.py`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/.gitignore` & `jupyspace_api-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/LICENSE.txt` & `jupyspace_api-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/pyproject.toml` & `jupyspace_api-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyspace_api-0.0.3/PKG-INFO` & `jupyspace_api-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyspace_api
-Version: 0.0.3
+Version: 0.0.4
 Summary: The public API for Jupyspace
 Project-URL: Source, https://github.com/davidbrochart/jupyspace/jupyspace_api
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Keywords: api,jupyspace
 Classifier: Development Status :: 4 - Beta
```

