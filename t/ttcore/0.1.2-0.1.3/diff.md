# Comparing `tmp/ttcore-0.1.2.tar.gz` & `tmp/ttcore-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttcore-0.1.2.tar", last modified: Mon Apr  3 19:04:12 2023, max compression
+gzip compressed data, was "ttcore-0.1.3.tar", last modified: Fri Apr 21 18:27:00 2023, max compression
```

## Comparing `ttcore-0.1.2.tar` & `ttcore-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-03 19:04:12.137369 ttcore-0.1.2/
--rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.2/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      633 2023-04-03 19:04:12.137369 ttcore-0.1.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      200 2023-04-03 19:04:12.137369 ttcore-0.1.2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      813 2023-04-03 18:50:11.000000 ttcore-0.1.2/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-03 19:04:12.136369 ttcore-0.1.2/ttcore/
--rw-r--r--   0 user      (1000) user      (1000)    11553 2023-04-03 14:30:07.000000 ttcore-0.1.2/ttcore/bottle.py
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.2/ttcore/ip.py
--rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.2/ttcore/mailers.py
--rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.2/ttcore/messages.py
--rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.2/ttcore/peewee.py
--rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.2/ttcore/utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-03 19:04:12.137369 ttcore-0.1.2/ttcore.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      633 2023-04-03 19:04:12.000000 ttcore-0.1.2/ttcore.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      314 2023-04-03 19:04:12.000000 ttcore-0.1.2/ttcore.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-03 19:04:12.000000 ttcore-0.1.2/ttcore.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-03 19:04:12.000000 ttcore-0.1.2/ttcore.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-04-03 19:04:12.000000 ttcore-0.1.2/ttcore.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.2/ttcore.egg-info/zip-safe
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-21 18:27:00.051792 ttcore-0.1.3/
+-rw-rw-r--   0 user      (1000) user      (1000)    11358 2023-03-30 08:55:21.000000 ttcore-0.1.3/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)      633 2023-04-21 18:27:00.051792 ttcore-0.1.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      112 2023-03-30 08:58:11.000000 ttcore-0.1.3/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      200 2023-04-21 18:27:00.052792 ttcore-0.1.3/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      813 2023-04-21 18:26:51.000000 ttcore-0.1.3/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-21 18:27:00.048792 ttcore-0.1.3/ttcore/
+-rw-r--r--   0 user      (1000) user      (1000)    11508 2023-04-21 18:26:51.000000 ttcore-0.1.3/ttcore/bottle.py
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-03-30 08:55:53.000000 ttcore-0.1.3/ttcore/ip.py
+-rw-r--r--   0 user      (1000) user      (1000)     2801 2023-04-03 18:50:11.000000 ttcore-0.1.3/ttcore/mailers.py
+-rw-r--r--   0 user      (1000) user      (1000)     1139 2023-04-03 14:30:07.000000 ttcore-0.1.3/ttcore/messages.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1029 2023-03-30 08:55:53.000000 ttcore-0.1.3/ttcore/peewee.py
+-rw-r--r--   0 user      (1000) user      (1000)     3486 2023-04-03 14:30:07.000000 ttcore-0.1.3/ttcore/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-21 18:27:00.051792 ttcore-0.1.3/ttcore.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      633 2023-04-21 18:27:00.000000 ttcore-0.1.3/ttcore.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      314 2023-04-21 18:27:00.000000 ttcore-0.1.3/ttcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-21 18:27:00.000000 ttcore-0.1.3/ttcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-04-21 18:27:00.000000 ttcore-0.1.3/ttcore.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-04-21 18:27:00.000000 ttcore-0.1.3/ttcore.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-30 11:51:08.000000 ttcore-0.1.3/ttcore.egg-info/zip-safe
```

### Comparing `ttcore-0.1.2/LICENSE.txt` & `ttcore-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.2/PKG-INFO` & `ttcore-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ttcore-0.1.2/setup.py` & `ttcore-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="ttcore",
-    version="0.1.2",
+    version="0.1.3",
     author="Martin F",
     author_email="pypi.org@tigerteamx.com",
     description="Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tigerteamx/ttcore",
     packages=['ttcore'],
```

### Comparing `ttcore-0.1.2/ttcore/bottle.py` & `ttcore-0.1.3/ttcore/bottle.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from functools import wraps
 from inspect import signature
 from dataclasses import dataclass
 from datetime import datetime
 from traceback import format_exc
 import inspect
 import time
+import os
+
 
 import peewee
-from bottle import request, post, get, hook, response, HTTPResponse, default_app, apps, route
+from bottle import request, post, get, hook, response, HTTPResponse, default_app, route, SimpleTemplate
 
 
 from .utils import mkdir, rmdir, read, is_ip4, dumps
 
 
 @dataclass
 class Context:
@@ -125,14 +127,15 @@
 def tpost(path, roles=None):
     def decorator(func):
         params = signature(func).parameters
         doc_params = _get_doc_params(params)
         _docs.append(dict(
             path=path,
             method='post',
+            func=func,
             params=doc_params,
         ))
 
         @wraps(func)
         @post(path)
         def wrapper(*args, **kwargs):
             if roles and not _auth(roles):
@@ -339,49 +342,46 @@
         except: # noqa
             print(
                 f"Error occured during mydocs setup {prop['name']} {format_exc()}"
             )
     return props
 
 
-def _get_doc_func(doc_path):
-    for route in apps().routes:
-        if route.rule == f"/{doc_path}":
-            return route.call
-    return
-
-
 def _get_rules(base, docs):
     rules = []
 
     for doc in docs:
-        doc_func = _get_doc_func(doc['path'])
+        doc_func = doc['func']
         rules.append(
             dict(
-                url=f"{base}/{doc['path']}",
+                url=f"{base}{doc['path']}",
                 path=doc["path"],
                 method=doc["method"],
                 doc=str(inspect.getdoc(doc_func) if inspect.getdoc(doc_func) else ""),
                 form=_nice_form(doc["params"])
             )
         )
 
     return rules
 
 
 def install_docs(path, base):
     # It is important that this is at init else it wont work
+    this_dir, this_filename = os.path.split(__file__)
+    docs_path = os.path.join(this_dir, "docs.html")
     rules = _get_rules(base, _docs)
 
     @get(path)
     def mydocs_view():
-        with open("docs.html", "r") as f:
-            html = f.read().replace("{{DOCS_URL}}", f'{path}.json')
-            html = html.replace("{{DOCS_JSON}}", dumps(dict(rules=rules, base=base)))
-            return html
+        with open(docs_path, "r") as f:
+            tmpl = SimpleTemplate(f.read())
+            return tmpl.render(
+                rules=rules,
+                base=base,
+            )
 
 
 def install_cors(hosts):
     @route("/<:re:.*>", method="OPTIONS")
     def enable_cors_generic_route():
         """
         This route takes priority over all others. So any request with an OPTIONS
```

### Comparing `ttcore-0.1.2/ttcore/mailers.py` & `ttcore-0.1.3/ttcore/mailers.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.2/ttcore/messages.py` & `ttcore-0.1.3/ttcore/messages.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.2/ttcore/peewee.py` & `ttcore-0.1.3/ttcore/peewee.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.2/ttcore/utils.py` & `ttcore-0.1.3/ttcore/utils.py`

 * *Files identical despite different names*

### Comparing `ttcore-0.1.2/ttcore.egg-info/PKG-INFO` & `ttcore-0.1.3/ttcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttcore
-Version: 0.1.2
+Version: 0.1.3
 Summary: Atomic Batteries Included. Used by https://tigerteamx.com to maximize producitivty.
 Home-page: https://github.com/tigerteamx/ttcore
 Author: Martin F
 Author-email: pypi.org@tigerteamx.com
 Keywords: productivity,bottlepy,peewee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

