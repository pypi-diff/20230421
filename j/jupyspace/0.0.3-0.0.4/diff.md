# Comparing `tmp/jupyspace-0.0.3.tar.gz` & `tmp/jupyspace-0.0.4.tar.gz`

## Comparing `jupyspace-0.0.3.tar` & `jupyspace-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 jupyspace-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyspace-0.0.3/config.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyspace-0.0.3/dev-environment.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyspace-0.0.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/LICENSE.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/README.md
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/app.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/exceptions.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/main.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/router.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/space/__init__.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyspace-0.0.3/jupyspace_api/jupyspace_api/space/models.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/README.md
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/__init__.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/main.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/micromamba.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/routes.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/subprocess.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/localspace/fps_localspace/utils.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/LICENSE.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/README.md
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/main.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/routes.py
--rw-r--r--   0        0        0    42581 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/static/htmx.min.js
--rw-r--r--   0        0        0   356447 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/static/tailwindcss.min.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/create_environment.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/create_server.html
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/edit_environment.html
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/edit_server.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/environment.html
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/environments.html
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/index.html
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/search_environments.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/searched_environments.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/server.html
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/servers.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 jupyspace-0.0.3/tests/test_localspace.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyspace-0.0.3/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyspace-0.0.3/README.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 jupyspace-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 jupyspace-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 jupyspace-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyspace-0.0.4/config.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyspace-0.0.4/dev-environment.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyspace-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/LICENSE.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/README.md
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/app.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/exceptions.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/main.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/router.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/space/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyspace-0.0.4/jupyspace_api/jupyspace_api/space/models.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/README.md
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/__init__.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/main.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/micromamba.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/routes.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/subprocess.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/localspace/fps_localspace/utils.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/LICENSE.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/README.md
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/main.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/routes.py
+-rw-r--r--   0        0        0    42581 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/static/htmx.min.js
+-rw-r--r--   0        0        0   356447 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/static/tailwindcss.min.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/create_environment.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/create_server.html
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/edit_environment.html
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/edit_server.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/environment.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/environments.html
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/index.html
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/search_environments.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/searched_environments.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/server.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/servers.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 jupyspace-0.0.4/tests/test_localspace.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 jupyspace-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jupyspace-0.0.4/README.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 jupyspace-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 jupyspace-0.0.4/PKG-INFO
```

### Comparing `jupyspace-0.0.3/CHANGELOG.md` & `jupyspace-0.0.4/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 # Changes in Jupyspace {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.0.4
+
+([Full Changelog](https://github.com/davidbrochart/jupyspace/compare/v0.0.3...1495da728601d22e9be567962addbf397c5c505f))
+
+### Merged PRs
+
+- Add CLI [#5](https://github.com/davidbrochart/jupyspace/pull/5) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/davidbrochart/jupyspace/graphs/contributors?from=2023-04-21&to=2023-04-21&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Adavidbrochart%2Fjupyspace+involves%3Adavidbrochart+updated%3A2023-04-21..2023-04-21&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.0.3
 
 ([Full Changelog](https://github.com/davidbrochart/jupyspace/compare/0.0.2...b44a7feead69173355c1518ab9bc8072d34f7627))
 
 ### Merged PRs
 
 - Check servers [#4](https://github.com/davidbrochart/jupyspace/pull/4) ([@davidbrochart](https://github.com/davidbrochart))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/davidbrochart/jupyspace/graphs/contributors?from=2023-04-20&to=2023-04-21&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Adavidbrochart%2Fjupyspace+involves%3Adavidbrochart+updated%3A2023-04-20..2023-04-21&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.0.2
```

### Comparing `jupyspace-0.0.3/.github/workflows/main.yml` & `jupyspace-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/LICENSE.txt` & `jupyspace-0.0.4/jupyspace_api/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/pyproject.toml` & `jupyspace-0.0.4/jupyspace_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/jupyspace_api/app.py` & `jupyspace-0.0.4/jupyspace_api/jupyspace_api/app.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/jupyspace_api/main.py` & `jupyspace-0.0.4/jupyspace_api/jupyspace_api/main.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/jupyspace_api/space/__init__.py` & `jupyspace-0.0.4/jupyspace_api/jupyspace_api/space/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/jupyspace_api/jupyspace_api/space/models.py` & `jupyspace-0.0.4/jupyspace_api/jupyspace_api/space/models.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/LICENSE.txt` & `jupyspace-0.0.4/plugins/localspace/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/README.md` & `jupyspace-0.0.4/plugins/localspace/README.md`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/pyproject.toml` & `jupyspace-0.0.4/plugins/localspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/fps_localspace/main.py` & `jupyspace-0.0.4/plugins/localspace/fps_localspace/main.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/fps_localspace/micromamba.py` & `jupyspace-0.0.4/plugins/localspace/fps_localspace/micromamba.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/fps_localspace/routes.py` & `jupyspace-0.0.4/plugins/localspace/fps_localspace/routes.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/localspace/fps_localspace/subprocess.py` & `jupyspace-0.0.4/plugins/localspace/fps_localspace/subprocess.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/LICENSE.txt` & `jupyspace-0.0.4/plugins/spacex/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/pyproject.toml` & `jupyspace-0.0.4/plugins/spacex/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/routes.py` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/routes.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/static/htmx.min.js` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/static/tailwindcss.min.js` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/static/tailwindcss.min.js`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/edit_environment.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/edit_environment.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/edit_server.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/edit_server.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/environment.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/environment.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/environments.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/environments.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/search_environments.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/search_environments.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/plugins/spacex/fps_spacex/templates/server.html` & `jupyspace-0.0.4/plugins/spacex/fps_spacex/templates/server.html`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/tests/test_localspace.py` & `jupyspace-0.0.4/tests/test_localspace.py`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/.gitignore` & `jupyspace-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/LICENSE.txt` & `jupyspace-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/README.md` & `jupyspace-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/pyproject.toml` & `jupyspace-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.3/PKG-INFO` & `jupyspace-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyspace
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/davidbrochart/jupyspace#readme
 Project-URL: Issues, https://github.com/davidbrochart/jupyspace/issues
 Project-URL: Source, https://github.com/davidbrochart/jupyspace
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Keywords: conda,jupyter
```

