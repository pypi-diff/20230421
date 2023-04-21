# Comparing `tmp/redfish_service_validator-2.3.0.tar.gz` & `tmp/redfish_service_validator-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_service_validator-2.3.0.tar", last modified: Fri Mar 17 22:48:44 2023, max compression
+gzip compressed data, was "redfish_service_validator-2.3.1.tar", last modified: Fri Apr 21 19:24:05 2023, max compression
```

## Comparing `redfish_service_validator-2.3.0.tar` & `redfish_service_validator-2.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:48:44.832028 redfish_service_validator-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-03-17 22:48:44.832028 redfish_service_validator-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:48:44.832028 redfish_service_validator-2.3.0/redfish_service_validator/
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/RedfishLogo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11487 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/RedfishServiceValidator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16495 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/RedfishServiceValidatorGui.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47678 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/schema_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/traverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/validateRedfish.py
--rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/redfish_service_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 22:48:44.832028 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-17 22:48:44.000000 redfish_service_validator-2.3.0/redfish_service_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 22:48:44.832028 redfish_service_validator-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-17 22:48:32.000000 redfish_service_validator-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/redfish_service_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishLogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11487 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16495 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidatorGui.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47588 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14133 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/schema_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/validateRedfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20865 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/redfish_service_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 19:24:05.000000 redfish_service_validator-2.3.1/redfish_service_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 19:24:05.230904 redfish_service_validator-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-21 19:23:49.000000 redfish_service_validator-2.3.1/setup.py
```

### Comparing `redfish_service_validator-2.3.0/LICENSE.md` & `redfish_service_validator-2.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/PKG-INFO` & `redfish_service_validator-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.3.0
+Version: 2.3.1
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.3.0/README.md` & `redfish_service_validator-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/RedfishLogo.py` & `redfish_service_validator-2.3.1/redfish_service_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/RedfishServiceValidator.py` & `redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from redfish_service_validator.config import convert_config_to_args, convert_args_to_config
 from redfish_service_validator.validateResource import validateSingleURI, validateURITree
 import redfish_service_validator.schema as schema
 from redfish_service_validator import tohtml, schema_pack, traverse
 from urllib.parse import urlparse, urlunparse
 from collections import Counter
 
-tool_version = '2.3.0'
+tool_version = '2.3.1'
 
 # Set up the custom debug levels
 VERBOSE1=logging.INFO-1
 VERBOSE2=logging.INFO-2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/RedfishServiceValidatorGui.py` & `redfish_service_validator-2.3.1/redfish_service_validator/RedfishServiceValidatorGui.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/catalog.py` & `redfish_service_validator-2.3.1/redfish_service_validator/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -861,69 +861,70 @@
                 sub_obj.HasValidUri = True
                 sub_obj.HasValidUriStrict = False
                 sub_obj.properties = {x:y.populate(REDFISH_ABSENT) for x, y in sub_obj.properties.items()}
                 evals.append(sub_obj)
                 continue
 
             # Cast types if they're below their parent or are OemObjects
+            # Don't cast objects with odata.type that matches their current object type
             already_typed = False
             my_odata_type = sub_payload.get('@odata.type')
             if my_odata_type is not None and str(sub_obj.Type) == my_odata_type.strip('#'):
                 already_typed = True
             if sub_obj.Type.IsNav:
                 already_typed = True
 
-            # we can only cast if we have an odata type and valid schema
+            # If our item is an OemObject type and hasn't been casted to a type, then cast it
             if 'Resource.OemObject' in sub_obj.Type.getTypeTree() and not casted:
                 my_logger.verbose1(('Morphing OemObject', my_odata_type, sub_obj.Type))
                 if my_odata_type:
                     my_odata_type = my_odata_type.strip('#')
                     try:
                         type_obj = sub_obj.Type.catalog.getSchemaDocByClass(my_odata_type).getTypeInSchemaDoc(my_odata_type)
                         sub_obj = RedfishObject(type_obj, sub_obj.Name, sub_obj.parent).populate(sub_payload, check=check, casted=True)
                     except MissingSchemaError:
                         my_logger.warning("Couldn't get schema for object, skipping OemObject {}".format(sub_obj.Name))
                     except Exception as e:
                         my_logger.warning("Couldn't get schema for object (?), skipping OemObject {} : {}".format(sub_obj.Name, e))
                     evals.append(sub_obj)
                     continue
-            # or if we're a Resource or unversioned or v1_0_0 type
+            # Otherwise, if we're not casted, or we don't have an odata type, then cast it
             elif not casted and not already_typed:
                 my_ns, my_ns_unversioned = sub_obj.Type.Namespace, getNamespaceUnversioned(sub_obj.Type.Namespace)
-                try:
-                    min_version = min([tuple(splitVersionString(x.Namespace)) for x in sub_obj.Type.getTypeTree() if not x.IsPropertyType and my_ns_unversioned in x.Namespace])
-                    min_version = 'v' + '_'.join([str(x) for x in min_version])
-                except:
-                    my_logger.debug('Issue getting minimum version', exc_info=1)
-                    min_version = 'v1_0_0'
-                if my_ns in [my_ns_unversioned, my_ns_unversioned + '.v1_0_0', '.'.join([my_ns_unversioned, min_version])] or my_odata_type:
+                # if we have an odata type, use it as our upper limit
+                if my_odata_type:
+                    my_limit = getNamespace(my_odata_type).strip('#')
+                else:
                     my_limit = 'v9_9_9'
-                    if my_odata_type:
-                        my_limit = getNamespace(my_odata_type).strip('#')
-                    if sub_obj.parent and my_ns_unversioned not in 'Resource': # we always cast Resource objects
-                        parent = sub_obj
-                        while parent.parent and parent.parent.Type.Namespace.startswith(my_ns_unversioned + '.'):
-                            parent = parent.parent
-                            my_limit = parent.Type.Namespace
-                    my_type = sub_obj.Type.Type
-                    # get type order from bottom up of schema, check if my_type in that schema
-                    for top_ns, schema in reversed(list(sub_obj.Type.catalog.getSchemaDocByClass(my_ns).classes.items())):
-                        if my_type in schema.my_types:
-                            if splitVersionString(top_ns) <= splitVersionString(my_limit):
-                                my_ns = top_ns
-                                break
-                    # ISSUE: We can't cast under v1_0_0, get the next best Type
-                    if my_ns == my_ns_unversioned:
-                        my_ns = top_ns
-                    if my_ns not in sub_obj.Type.Namespace:
-                        my_logger.verbose1(('Morphing Complex', my_ns, my_type, my_limit))
-                        new_type_obj = sub_obj.Type.catalog.getSchemaDocByClass(my_ns).getTypeInSchemaDoc('.'.join([my_ns, my_type]))
-                        sub_obj = RedfishObject(new_type_obj, sub_obj.Name, sub_obj.parent).populate(sub_payload, check=check, casted=True)
-                        evals.append(sub_obj)
-                        continue
+                # If our item is not a Resource.Resource type, determine its parent's version limit for later...
+                # NOTE: Resource items always seem to be cast to highest type, not determined by its parent's type
+                #       not sure where this is backed up in documentation
+                if sub_obj.parent and my_ns_unversioned not in ['Resource']:
+                    parent = sub_obj
+                    while parent.parent and parent.parent.Type.Namespace.startswith(my_ns_unversioned + '.'):
+                        parent = parent.parent
+                        my_limit = parent.Type.Namespace
+                my_type = sub_obj.Type.Type
+                top_ns = my_ns
+                # get type order from bottom up of SchemaDoc
+                for top_ns, schema in reversed(list(sub_obj.Type.catalog.getSchemaDocByClass(my_ns).classes.items())):
+                    # if our object type is in schema... check for limit
+                    if my_type in schema.my_types:
+                        if splitVersionString(top_ns) <= splitVersionString(my_limit):
+                            my_ns = top_ns
+                            break
+                # ISSUE: We can't cast under v1_0_0, get the next best Type
+                if my_ns == my_ns_unversioned:
+                    my_ns = top_ns
+                if my_ns not in sub_obj.Type.Namespace:
+                    my_logger.verbose1(('Morphing Complex', my_ns, my_type, my_limit))
+                    new_type_obj = sub_obj.Type.catalog.getSchemaDocByClass(my_ns).getTypeInSchemaDoc('.'.join([my_ns, my_type]))
+                    sub_obj = RedfishObject(new_type_obj, sub_obj.Name, sub_obj.parent).populate(sub_payload, check=check, casted=True)
+                    evals.append(sub_obj)
+                    continue
 
             # Validate our Uri
             sub_obj.HasValidUri = True
             sub_obj.HasValidUriStrict = True
             allowable_uris = sub_obj.Type.getUris()
             # If we have expected URIs and @odata.id
             # And we AREN'T a navigation property
```

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/config.py` & `redfish_service_validator-2.3.1/redfish_service_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/helper.py` & `redfish_service_validator-2.3.1/redfish_service_validator/helper.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/metadata.py` & `redfish_service_validator-2.3.1/redfish_service_validator/metadata.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/schema.py` & `redfish_service_validator-2.3.1/redfish_service_validator/schema.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/schema_pack.py` & `redfish_service_validator-2.3.1/redfish_service_validator/schema_pack.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/tohtml.py` & `redfish_service_validator-2.3.1/redfish_service_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/traverse.py` & `redfish_service_validator-2.3.1/redfish_service_validator/traverse.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/validateRedfish.py` & `redfish_service_validator-2.3.1/redfish_service_validator/validateRedfish.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator/validateResource.py` & `redfish_service_validator-2.3.1/redfish_service_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator.egg-info/PKG-INFO` & `redfish_service_validator-2.3.1/redfish_service_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-service-validator
-Version: 2.3.0
+Version: 2.3.1
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.3.0/redfish_service_validator.egg-info/SOURCES.txt` & `redfish_service_validator-2.3.1/redfish_service_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.3.0/setup.py` & `redfish_service_validator-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_service_validator",
-    version="2.3.0",
+    version="2.3.1",
     description="Redfish Service Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

