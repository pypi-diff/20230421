# Comparing `tmp/brease-sdk-1.0.0.tar.gz` & `tmp/brease-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brease-sdk-1.0.0.tar", last modified: Wed Apr 19 00:43:22 2023, max compression
+gzip compressed data, was "brease-sdk-1.1.0.tar", last modified: Fri Apr 21 00:41:45 2023, max compression
```

## Comparing `brease-sdk-1.0.0.tar` & `brease-sdk-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2432 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.906899 brease-sdk-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/brease_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-19 00:43:22.000000 brease-sdk-1.0.0/src/brease_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-19 00:43:22.000000 brease-sdk-1.0.0/src/brease_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:43:22.000000 brease-sdk-1.0.0/src/brease_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-19 00:43:22.000000 brease-sdk-1.0.0/src/brease_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 00:43:22.000000 brease-sdk-1.0.0/src/brease_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/contextid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/addrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/evaluaterules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/getallrules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/removerule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/operations/replacerule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/addruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/apiaddruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/apiallrulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/apievaluaterulesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      608 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/apireplaceruleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/condition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/conditionbasekey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/conditionbaseref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/conditiontype_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/evaluaterulesinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/expressionarray.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/modelsevaluationresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/modelsrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/modelstarget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/models/shared/replaceruleinput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:43:22.910899 brease-sdk-1.0.0/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-19 00:43:12.000000 brease-sdk-1.0.0/src/sdk/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2432 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/brease_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-21 00:41:45.000000 brease-sdk-1.1.0/src/brease_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6362 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/contextid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.295965 brease-sdk-1.1.0/src/sdk/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/addrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/evaluaterules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/getallrules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/removerule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1416 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/operations/replacerule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1043 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/addruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      604 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apiaddruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apiallrulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      670 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apievaluaterulesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      608 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/apireplaceruleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/condition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditionbasekey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      678 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditionbaseref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/conditiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      940 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/evaluaterulesinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/expressionarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelsevaluationresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelsrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/modelstarget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/models/shared/replaceruleinput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:41:45.299965 brease-sdk-1.1.0/src/sdk/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-21 00:41:31.000000 brease-sdk-1.1.0/src/sdk/utils/utils.py
```

### Comparing `brease-sdk-1.0.0/LICENSE.md` & `brease-sdk-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/PKG-INFO` & `brease-sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `brease-sdk-1.0.0/README.md` & `brease-sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/setup.py` & `brease-sdk-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="brease-sdk",
-    version="1.0.0",
+    version="1.1.0",
     author="dotindustries",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `brease-sdk-1.0.0/src/brease_sdk.egg-info/PKG-INFO` & `brease-sdk-1.1.0/src/brease_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brease-sdk
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: dotindustries
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `brease-sdk-1.0.0/src/brease_sdk.egg-info/SOURCES.txt` & `brease-sdk-1.1.0/src/brease_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/contextid.py` & `brease-sdk-1.1.0/src/sdk/contextid.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/__init__.py` & `brease-sdk-1.1.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/addrule.py` & `brease-sdk-1.1.0/src/sdk/models/operations/addrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/evaluaterules.py` & `brease-sdk-1.1.0/src/sdk/models/operations/evaluaterules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/getallrules.py` & `brease-sdk-1.1.0/src/sdk/models/operations/getallrules.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/removerule.py` & `brease-sdk-1.1.0/src/sdk/models/operations/removerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/operations/replacerule.py` & `brease-sdk-1.1.0/src/sdk/models/operations/replacerule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/__init__.py` & `brease-sdk-1.1.0/src/sdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/addruleinput.py` & `brease-sdk-1.1.0/src/sdk/models/shared/addruleinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/apiaddruleresponse.py` & `brease-sdk-1.1.0/src/sdk/models/shared/apiaddruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/apiallrulesresponse.py` & `brease-sdk-1.1.0/src/sdk/models/shared/apiallrulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/apievaluaterulesresponse.py` & `brease-sdk-1.1.0/src/sdk/models/shared/apievaluaterulesresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/apireplaceruleresponse.py` & `brease-sdk-1.1.0/src/sdk/models/shared/apireplaceruleresponse.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/condition.py` & `brease-sdk-1.1.0/src/sdk/models/shared/condition.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/conditionbaseref.py` & `brease-sdk-1.1.0/src/sdk/models/shared/conditionbaseref.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/evaluaterulesinput.py` & `brease-sdk-1.1.0/src/sdk/models/shared/evaluaterulesinput.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/expressionarray.py` & `brease-sdk-1.1.0/src/sdk/models/shared/expressionarray.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/modelsevaluationresult.py` & `brease-sdk-1.1.0/src/sdk/models/shared/modelsevaluationresult.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/modelsrule.py` & `brease-sdk-1.1.0/src/sdk/models/shared/modelsrule.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/models/shared/modelstarget.py` & `brease-sdk-1.1.0/src/sdk/models/shared/modelstarget.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/sdk.py` & `brease-sdk-1.1.0/src/sdk/sdk.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     context_id: ContextID
     r"""Rule domain context"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.0.0"
-    _gen_version: str = "2.18.2"
+    _sdk_version: str = "1.1.0"
+    _gen_version: str = "2.19.1"
 
     def __init__(self,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
```

### Comparing `brease-sdk-1.0.0/src/sdk/utils/retries.py` & `brease-sdk-1.1.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `brease-sdk-1.0.0/src/sdk/utils/utils.py` & `brease-sdk-1.1.0/src/sdk/utils/utils.py`

 * *Files identical despite different names*

