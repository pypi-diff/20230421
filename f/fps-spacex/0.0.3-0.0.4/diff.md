# Comparing `tmp/fps_spacex-0.0.3.tar.gz` & `tmp/fps_spacex-0.0.4.tar.gz`

## Comparing `fps_spacex-0.0.3.tar` & `fps_spacex-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/main.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/routes.py
--rw-r--r--   0        0        0    42581 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/static/htmx.min.js
--rw-r--r--   0        0        0   356447 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/static/tailwindcss.min.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/create_environment.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/create_server.html
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/edit_environment.html
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/edit_server.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/environment.html
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/environments.html
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/index.html
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/search_environments.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/searched_environments.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/server.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/fps_spacex/templates/servers.html
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/README.md
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fps_spacex-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/main.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/routes.py
+-rw-r--r--   0        0        0    42581 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/static/htmx.min.js
+-rw-r--r--   0        0        0   356447 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/static/tailwindcss.min.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/create_environment.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/create_server.html
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/edit_environment.html
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/edit_server.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/environment.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/environments.html
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/index.html
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/search_environments.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/searched_environments.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/server.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/fps_spacex/templates/servers.html
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/README.md
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fps_spacex-0.0.4/PKG-INFO
```

### Comparing `fps_spacex-0.0.3/fps_spacex/routes.py` & `fps_spacex-0.0.4/fps_spacex/routes.py`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/static/htmx.min.js` & `fps_spacex-0.0.4/fps_spacex/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/static/tailwindcss.min.js` & `fps_spacex-0.0.4/fps_spacex/static/tailwindcss.min.js`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/edit_environment.html` & `fps_spacex-0.0.4/fps_spacex/templates/edit_environment.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/edit_server.html` & `fps_spacex-0.0.4/fps_spacex/templates/edit_server.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/environment.html` & `fps_spacex-0.0.4/fps_spacex/templates/environment.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/environments.html` & `fps_spacex-0.0.4/fps_spacex/templates/environments.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/search_environments.html` & `fps_spacex-0.0.4/fps_spacex/templates/search_environments.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/fps_spacex/templates/server.html` & `fps_spacex-0.0.4/fps_spacex/templates/server.html`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/.gitignore` & `fps_spacex-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/LICENSE.txt` & `fps_spacex-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/pyproject.toml` & `fps_spacex-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_spacex-0.0.3/PKG-INFO` & `fps_spacex-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps-spacex
-Version: 0.0.3
+Version: 0.0.4
 Summary: JupySpace's user interface
 Project-URL: Source, https://github.com/davidbrochart/jupyspace/plugins/fps-spacex
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

