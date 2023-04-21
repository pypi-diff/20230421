# Comparing `tmp/jupyspace-0.0.1.tar.gz` & `tmp/jupyspace-0.0.2.tar.gz`

## Comparing `jupyspace-0.0.1.tar` & `jupyspace-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,49 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyspace-0.0.1/fps.log
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyspace-0.0.1/fps_cli_args.toml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jupyspace-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyspace-0.0.1/jupyspace/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.1/jupyspace/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/README.md
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/pyproject.toml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/models.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/routes.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/subprocess.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.1/plugins/fps-localspace/tests/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyspace-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 jupyspace-0.0.1/tests/test_localspace.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupyspace-0.0.1/README.md
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 jupyspace-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyspace-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyspace-0.0.2/config.yaml
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyspace-0.0.2/dev-environment.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyspace-0.0.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/LICENSE.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/pyproject.toml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/app.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/exceptions.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/main.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/router.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/space/__init__.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/space/models.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyspace-0.0.2/jupyspace_api/jupyspace_api/spacex/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/README.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/__init__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/main.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/micromamba.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/routes.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/subprocess.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/localspace/fps_localspace/utils.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/LICENSE.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/README.md
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/main.py
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/routes.py
+-rw-r--r--   0        0        0    42581 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/static/htmx.min.js
+-rw-r--r--   0        0        0   356447 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/static/tailwindcss.min.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/create_environment.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/create_server.html
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/edit_environment.html
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/edit_server.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/environment.html
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/environments.html
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/index.html
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/search_environments.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/searched_environments.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/server.html
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyspace-0.0.2/plugins/spacex/fps_spacex/templates/servers.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyspace-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 jupyspace-0.0.2/tests/test_localspace.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jupyspace-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 jupyspace-0.0.2/README.md
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 jupyspace-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 jupyspace-0.0.2/PKG-INFO
```

### Comparing `jupyspace-0.0.1/plugins/fps-localspace/LICENSE.txt` & `jupyspace-0.0.2/jupyspace_api/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.1/plugins/fps-localspace/README.md` & `jupyspace-0.0.2/plugins/localspace/README.md`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.1/plugins/fps-localspace/pyproject.toml` & `jupyspace-0.0.2/plugins/spacex/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps-localspace"
-description = ''
+name = "fps-spacex"
+description = "JupySpace's user interface"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "David Brochart", email = "david.brochart@gmail.com" },
 ]
@@ -20,21 +20,20 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "fps>=0.0.19",
+  "jupyspace-api",
+  "jinja2",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace#readme"
-Issues = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace/issues"
-Source = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace"
+Source = "https://github.com/davidbrochart/jupyspace/plugins/fps-spacex"
 
-[project.entry-points.fps_router]
-fps-localspace = "fps_localspace.routes"
+[project.entry-points."asphalt.components"]
+spacex = "fps_spacex.main:SpacexComponent"
 
 [tool.hatch.version]
-path = "fps_localspace/__about__.py"
+path = "fps_spacex/__init__.py"
```

### Comparing `jupyspace-0.0.1/plugins/fps-localspace/fps_localspace/subprocess.py` & `jupyspace-0.0.2/plugins/localspace/fps_localspace/subprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 
 
 async def run_exec(*args, wait: bool = True):
-    proc = await asyncio.create_subprocess_exec(*args)
+    proc = await asyncio.create_subprocess_exec(*args, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE)
     if wait:
         returncode = await proc.wait()
         if returncode != 0:
             raise RuntimeError(f'Error executing: {" ".join(args)}')
     return proc
```

### Comparing `jupyspace-0.0.1/LICENSE.txt` & `jupyspace-0.0.2/plugins/localspace/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyspace-0.0.1/pyproject.toml` & `jupyspace-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,47 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyspace"
 description = ''
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "David Brochart", email = "david.brochart@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "fps[uvicorn]>=0.0.19",
+  "asphalt >=4.11.0,<5",
+  "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/davidbrochart/jupyspace#readme"
 Issues = "https://github.com/davidbrochart/jupyspace/issues"
 Source = "https://github.com/davidbrochart/jupyspace"
 
 [project.optional-dependencies]
 test = [
   "pytest",
-  "requests",
+  "pytest-asyncio",
+  "httpx",
 ]
 
-[project.scripts]
-jupyspace = "fps_uvicorn.cli:app"
+#[project.scripts]
+#jupyspace-server = "fps_uvicorn.cli:app"
+#jupyspace = "jupyspace.jupyspace:app_run"
 
 [tool.hatch.version]
-path = "jupyspace/__about__.py"
+path = "jupyspace/__init__.py"
```

