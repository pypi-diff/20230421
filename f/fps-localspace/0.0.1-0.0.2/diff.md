# Comparing `tmp/fps_localspace-0.0.1.tar.gz` & `tmp/fps_localspace-0.0.2.tar.gz`

## Comparing `fps_localspace-0.0.1.tar` & `fps_localspace-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/models.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/routes.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/subprocess.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/fps_localspace/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/README.md
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 fps_localspace-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/__init__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/main.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/micromamba.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/routes.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/subprocess.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/fps_localspace/utils.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/README.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 fps_localspace-0.0.2/PKG-INFO
```

### Comparing `fps_localspace-0.0.1/fps_localspace/subprocess.py` & `fps_localspace-0.0.2/fps_localspace/subprocess.py`

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

### Comparing `fps_localspace-0.0.1/LICENSE.txt` & `fps_localspace-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fps_localspace-0.0.1/README.md` & `fps_localspace-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fps_localspace-0.0.1/pyproject.toml` & `fps_localspace-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -20,21 +20,22 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "fps>=0.0.19",
+  "sqlmodel",
+  "jupyspace-api",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace#readme"
 Issues = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace/issues"
 Source = "https://github.com/davidbrochart/jupyspace/plugins/fps-localspace"
 
-[project.entry-points.fps_router]
-fps-localspace = "fps_localspace.routes"
+[project.entry-points."asphalt.components"]
+space = "fps_localspace.main:LocalspaceComponent"
 
 [tool.hatch.version]
-path = "fps_localspace/__about__.py"
+path = "fps_localspace/__init__.py"
```

### Comparing `fps_localspace-0.0.1/PKG-INFO` & `fps_localspace-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: fps-localspace
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/davidbrochart/jupyspace/plugins/fps-localspace#readme
 Project-URL: Issues, https://github.com/davidbrochart/jupyspace/plugins/fps-localspace/issues
 Project-URL: Source, https://github.com/davidbrochart/jupyspace/plugins/fps-localspace
 Author-email: David Brochart <david.brochart@gmail.com>
+License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Requires-Dist: fps>=0.0.19
+Requires-Dist: jupyspace-api
+Requires-Dist: sqlmodel
 Description-Content-Type: text/markdown
 
 # fps-localspace
 
 [![PyPI - Version](https://img.shields.io/pypi/v/fps-localspace.svg)](https://pypi.org/project/fps-localspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fps-localspace.svg)](https://pypi.org/project/fps-localspace)
```

