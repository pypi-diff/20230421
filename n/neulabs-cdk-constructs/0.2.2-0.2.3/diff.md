# Comparing `tmp/neulabs-cdk-constructs-0.2.2.tar.gz` & `tmp/neulabs-cdk-constructs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.2.2.tar", last modified: Wed Apr 12 08:02:42 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.2.3.tar", last modified: Fri Apr 21 10:58:12 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.2.2.tar` & `neulabs-cdk-constructs-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.694524 neulabs-cdk-constructs-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   325578 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221168 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    38906 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-12 08:02:27.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:02:42.698524 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-12 08:02:42.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 08:02:42.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:02:42.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 08:02:42.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 08:02:42.000000 neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.634312 neulabs-cdk-constructs-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.634312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.634312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   325807 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.634312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40775 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    38906 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.638312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-21 10:57:59.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:58:12.634312 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-21 10:58:12.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-21 10:58:12.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:58:12.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-21 10:58:12.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 10:58:12.000000 neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.2.2/LICENSE` & `neulabs-cdk-constructs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/PKG-INFO` & `neulabs-cdk-constructs-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.2.2
+Version: 0.2.3
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.3 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
 neulabscom/neulabs-cdk-constructs.git Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
```

### Comparing `neulabs-cdk-constructs-0.2.2/README.md` & `neulabs-cdk-constructs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/setup.py` & `neulabs-cdk-constructs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.2.2",
+    "version": "0.2.3",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.2.2.jsii.tgz"
+            "neulabs-cdk-constructs@0.2.3.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.2.2",
+    "0.2.3",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.2.2.jsii.tgz",
+    "neulabs-cdk-constructs@0.2.3.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         :param on_success: The destination for successful invocations. Default: - no destination
         :param retry_attempts: The maximum number of times to retry when the function returns an error. Minimum: 0 Maximum: 2 Default: 2
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f74ea4209ec411b0aa54f447882f7ec52bcf71d7bd9634932a0b9d0c069e374f)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = FunctionNodeProps(
+        __2 = FunctionNodeProps(
             stage=stage,
             with_base_environment=with_base_environment,
             with_base_tags=with_base_tags,
             aws_sdk_connection_reuse=aws_sdk_connection_reuse,
             bundling=bundling,
             deps_lock_file_path=deps_lock_file_path,
             entry=entry,
@@ -351,15 +351,15 @@
             vpc_subnets=vpc_subnets,
             max_event_age=max_event_age,
             on_failure=on_failure,
             on_success=on_success,
             retry_attempts=retry_attempts,
         )
 
-        jsii.create(self.__class__, self, [scope, id, props])
+        jsii.create(self.__class__, self, [scope, id, __2])
 
     @jsii.member(jsii_name="addBaseEnvironment")
     def add_base_environment(self) -> None:
         return typing.cast(None, jsii.invoke(self, "addBaseEnvironment", []))
 
     @jsii.member(jsii_name="addBaseTags")
     def add_base_tags(self) -> None:
```

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.2.2
+Version: 0.2.3
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: neulabs-cdk-constructs Version: 0.2.3 Summary:
 neulabs-cdk-constructs Home-page: https://github.com/neulabscom/neulabs-cdk-
 constructs.git Author: Neulabs
 neulabs.com> License: Apache-2.0 Project-URL: Source, https://github.com/
 neulabscom/neulabs-cdk-constructs.git Platform: UNKNOWN Classifier: Intended
 Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.7
```

### Comparing `neulabs-cdk-constructs-0.2.2/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.2.3/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.2.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.2.3.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

