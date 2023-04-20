# Comparing `tmp/async_faceit_api-0.1.0.tar.gz` & `tmp/async_faceit_api-0.1.1.tar.gz`

## Comparing `async_faceit_api-0.1.0.tar` & `async_faceit_api-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.gitattributes
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/AsyncFaceitApi.iml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/async_faceit_api.rst
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/make.bat
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/docs/modules.rst
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/src/async_faceit_api/__init__.py
--rw-r--r--   0        0        0    42627 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/src/async_faceit_api/api.py
--rw-r--r--   0        0        0    45723 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/src/async_faceit_api/dataclasses.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/src/async_faceit_api/enums.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/tests/example.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/tests/subclassing.py
--rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/tests/test.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/LICENSE
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 async_faceit_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/AsyncFaceitApi.iml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/async_faceit_api.rst
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/modules.rst
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/__init__.py
+-rw-r--r--   0        0        0    42627 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/api.py
+-rw-r--r--   0        0        0    45723 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/dataclasses.py
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/src/async_faceit_api/enums.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/example.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/subclassing.py
+-rw-r--r--   0        0        0     7353 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/tests/test.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 async_faceit_api-0.1.1/PKG-INFO
```

### Comparing `async_faceit_api-0.1.0/.idea/AsyncFaceitApi.iml` & `async_faceit_api-0.1.1/.idea/AsyncFaceitApi.iml`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/.idea/workspace.xml` & `async_faceit_api-0.1.1/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `async_faceit_api-0.1.0/.idea/workspace.xml` & `async_faceit_api-0.1.1/.idea/workspace.xml`

```diff
@@ -1,13 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-    </list>
+    <list default="true" id="7a343e8b-7b6d-4f78-a923-893771613ad2" name="Changes" comment=""/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
```

### Comparing `async_faceit_api-0.1.0/docs/Makefile` & `async_faceit_api-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/docs/async_faceit_api.rst` & `async_faceit_api-0.1.1/docs/async_faceit_api.rst`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/docs/conf.py` & `async_faceit_api-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/docs/make.bat` & `async_faceit_api-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/src/async_faceit_api/api.py` & `async_faceit_api-0.1.1/src/async_faceit_api/api.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/src/async_faceit_api/dataclasses.py` & `async_faceit_api-0.1.1/src/async_faceit_api/dataclasses.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/src/async_faceit_api/enums.py` & `async_faceit_api-0.1.1/src/async_faceit_api/enums.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/tests/subclassing.py` & `async_faceit_api-0.1.1/tests/subclassing.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/tests/test.py` & `async_faceit_api-0.1.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/.gitignore` & `async_faceit_api-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/LICENSE` & `async_faceit_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_faceit_api-0.1.0/README.md` & `async_faceit_api-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Async faceit API
 
 Async wrapper for the faceit API for csgo.
 
+[Here are the docs](https://async-faceit-api.readthedocs.io/en/latest/async_faceit_api.html)
+
 ### Error Handling
 
 Note that the async api methods return an object of type FaceitApiError 
 if the request was not successful. To distinguish between a successful 
 response and an error, you can easily use the object as a boolean expression:
 ```
     games = await api.games()
```

### Comparing `async_faceit_api-0.1.0/pyproject.toml` & `async_faceit_api-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "async_faceit_api"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Stuart", email="stuart.the.yellow.one@gmail.com" },
 ]
 description = "Async wrapper for the faceit API for csgo"
+documentation = "https://async-faceit-api.readthedocs.io/en/latest/index.html"
 readme = "README.md"
 requires-python = ">=3.10"
+dependencies = [
+  'aiohttp < 3.8.3',
+]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `async_faceit_api-0.1.0/PKG-INFO` & `async_faceit_api-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: async_faceit_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async wrapper for the faceit API for csgo
 Project-URL: Homepage, https://github.com/StuartTheYellowOne/async_faceit_api
 Project-URL: Bug Tracker, https://github.com/StuartTheYellowOne/async_faceit_api/issues
 Author-email: Stuart <stuart.the.yellow.one@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: aiohttp<3.8.3
 Description-Content-Type: text/markdown
 
 # Async faceit API
 
 Async wrapper for the faceit API for csgo.
 
+[Here are the docs](https://async-faceit-api.readthedocs.io/en/latest/async_faceit_api.html)
+
 ### Error Handling
 
 Note that the async api methods return an object of type FaceitApiError 
 if the request was not successful. To distinguish between a successful 
 response and an error, you can easily use the object as a boolean expression:
 ```
     games = await api.games()
```

