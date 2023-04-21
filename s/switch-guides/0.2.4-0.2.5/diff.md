# Comparing `tmp/switch_guides-0.2.4.tar.gz` & `tmp/switch_guides-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_guides-0.2.4.tar", last modified: Mon Feb 20 03:36:35 2023, max compression
+gzip compressed data, was "switch_guides-0.2.5.tar", last modified: Fri Apr 21 03:56:51 2023, max compression
```

## Comparing `switch_guides-0.2.4.tar` & `switch_guides-0.2.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-02-20 03:36:19.000000 switch_guides-0.2.4/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)     4654 2023-02-20 03:36:19.000000 switch_guides-0.2.4/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-02-20 03:36:19.000000 switch_guides-0.2.4/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-02-20 03:36:19.000000 switch_guides-0.2.4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5948 2023-02-20 03:36:35.973633 switch_guides-0.2.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-02-20 03:36:19.000000 switch_guides-0.2.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-02-20 03:36:19.000000 switch_guides-0.2.4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-02-20 03:36:35.977633 switch_guides-0.2.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1360 2023-02-20 03:36:19.000000 switch_guides-0.2.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/
--rw-r--r--   0 vsts      (1001) docker     (122)    15127 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/SwitchGuideTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      714 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/extensions/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1444 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/extensions/component/
--rw-r--r--   0 vsts      (1001) docker     (122)      365 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/component/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4558 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/component/form_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4576 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/extensions/component/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      495 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3337 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/enums.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4739 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/guide.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/literals.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9038 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/models/step.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)      766 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13031 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/pipeline/automation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)     3163 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/tasks/GuideDefinitionTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)      605 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/tasks/GuideRetrySupportTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7701 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10606 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/tasks/GuideStepDefinitionTask.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1014 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-02-20 03:36:19.000000 switch_guides-0.2.4/switch_guides/utils/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-20 03:36:35.973633 switch_guides-0.2.4/switch_guides.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5948 2023-02-20 03:36:35.000000 switch_guides-0.2.4/switch_guides.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1156 2023-02-20 03:36:35.000000 switch_guides-0.2.4/switch_guides.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-20 03:36:35.000000 switch_guides-0.2.4/switch_guides.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-02-20 03:36:35.000000 switch_guides-0.2.4/switch_guides.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-02-20 03:36:35.000000 switch_guides-0.2.4/switch_guides.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-04-21 03:56:37.000000 switch_guides-0.2.5/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)     4778 2023-04-21 03:56:37.000000 switch_guides-0.2.5/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-04-21 03:56:37.000000 switch_guides-0.2.5/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-04-21 03:56:37.000000 switch_guides-0.2.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6072 2023-04-21 03:56:51.643776 switch_guides-0.2.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      612 2023-04-21 03:56:37.000000 switch_guides-0.2.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-04-21 03:56:37.000000 switch_guides-0.2.5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-21 03:56:51.643776 switch_guides-0.2.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1360 2023-04-21 03:56:37.000000 switch_guides-0.2.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15127 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/SwitchGuideTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      714 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/extensions/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1444 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/extensions/component/
+-rw-r--r--   0 vsts      (1001) docker     (122)      365 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/component/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4558 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/component/form_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4576 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/extensions/component/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      495 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3337 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4739 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/guide.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/literals.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9589 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/models/step.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)      766 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13031 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/pipeline/automation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3163 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/tasks/GuideDefinitionTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      605 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/tasks/GuideRetrySupportTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7701 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10606 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/tasks/GuideStepDefinitionTask.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1014 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-04-21 03:56:37.000000 switch_guides-0.2.5/switch_guides/utils/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 03:56:51.643776 switch_guides-0.2.5/switch_guides.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6072 2023-04-21 03:56:51.000000 switch_guides-0.2.5/switch_guides.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1156 2023-04-21 03:56:51.000000 switch_guides-0.2.5/switch_guides.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-21 03:56:51.000000 switch_guides-0.2.5/switch_guides.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-04-21 03:56:51.000000 switch_guides-0.2.5/switch_guides.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       14 2023-04-21 03:56:51.000000 switch_guides-0.2.5/switch_guides.egg-info/top_level.txt
```

### Comparing `switch_guides-0.2.4/HISTORY.md` & `switch_guides-0.2.5/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # History
 
+## 0.2.5
+
+Added
+
+* Following attributes to `SwitchGuideStepData`
+  * request_data, request_timestamp, request_component_id
+
 ## 0.2.4
 
 Added
 
 * `options` attribute to `SwitchGuideStepProcessInput`
   * Allows Guide authors to provide additional options while processing the step
   * Attribute is optional and therefore Guide Step authors should take this into account
```

### Comparing `switch_guides-0.2.4/LICENCE` & `switch_guides-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/PKG-INFO` & `switch_guides-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_guides
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for building Platform Guides in Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,21 @@
 
 ```bash
 pip install switch-guides
 ```
 
 # History
 
+## 0.2.5
+
+Added
+
+* Following attributes to `SwitchGuideStepData`
+  * request_data, request_timestamp, request_component_id
+
 ## 0.2.4
 
 Added
 
 * `options` attribute to `SwitchGuideStepProcessInput`
   * Allows Guide authors to provide additional options while processing the step
   * Attribute is optional and therefore Guide Step authors should take this into account
```

### Comparing `switch_guides-0.2.4/README.md` & `switch_guides-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/setup.py` & `switch_guides-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A package for building Platform Guides in Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_guides",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(
         include=["switch_guides", "switch_guides.*"],
         exclude=["switch_guides.tests", "switch_guides.tests.*"]
     ),
     install_requires=['switch-api','pydantic==1.9.0'],
     python_requires=">=3.8.*",
     classifiers=[
```

### Comparing `switch_guides-0.2.4/switch_guides/SwitchGuideTask.py` & `switch_guides-0.2.5/switch_guides/SwitchGuideTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/__init__.py` & `switch_guides-0.2.5/switch_guides/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     'api',
     'step',
     'guide',
     'literals',
     'enums'
 ]
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
```

### Comparing `switch_guides-0.2.4/switch_guides/exceptions.py` & `switch_guides-0.2.5/switch_guides/exceptions.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/extensions/cache/cache.py` & `switch_guides-0.2.5/switch_guides/extensions/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/extensions/component/form_data.py` & `switch_guides-0.2.5/switch_guides/extensions/component/form_data.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/extensions/component/forms.py` & `switch_guides-0.2.5/switch_guides/extensions/component/forms.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/models/api.py` & `switch_guides-0.2.5/switch_guides/models/api.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/models/guide.py` & `switch_guides-0.2.5/switch_guides/models/guide.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/models/literals.py` & `switch_guides-0.2.5/switch_guides/models/literals.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/models/step.py` & `switch_guides-0.2.5/switch_guides/models/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,28 @@
     count: int = 0
     completionPercentage: int = 0
     numerator: int = 0
     denominator: int = 0
 
 
 class SwitchGuideStepData(dict):
-    pass
-
+    @property
+    def request_data(self) -> Optional[dict]:
+        """Data that was passed to the step when it was executed"""
+        return self.get('request_data', None)
+    
+    @property
+    def request_timestamp(self) -> Optional[str]:
+        """Timestamp in seconds since epoch when the request was made"""
+        return self.get('request_timestamp', None)
+    
+    @property
+    def request_component_id(self) -> Optional[str]:
+        """ID of the component that was used to execute the step"""
+        return self.get('request_component_id', None)
 
 class SwitchGuideStepStatusUiState(BaseModel):
     """Keep the step locked on the UI when True; otherwise unlock it.
     Attribute relevant for UI
     """
 
     lockStep: bool = False
```

### Comparing `switch_guides-0.2.4/switch_guides/pipeline/__init__.py` & `switch_guides-0.2.5/switch_guides/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/pipeline/automation.py` & `switch_guides-0.2.5/switch_guides/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/tasks/GuideDefinitionTask.py` & `switch_guides-0.2.5/switch_guides/tasks/GuideDefinitionTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/tasks/GuideRetrySupportTask.py` & `switch_guides-0.2.5/switch_guides/tasks/GuideRetrySupportTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py` & `switch_guides-0.2.5/switch_guides/tasks/GuideStepDefinitionBackgroundTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/tasks/GuideStepDefinitionTask.py` & `switch_guides-0.2.5/switch_guides/tasks/GuideStepDefinitionTask.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/tasks/__init__.py` & `switch_guides-0.2.5/switch_guides/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides/utils/utils.py` & `switch_guides-0.2.5/switch_guides/utils/utils.py`

 * *Files identical despite different names*

### Comparing `switch_guides-0.2.4/switch_guides.egg-info/PKG-INFO` & `switch_guides-0.2.5/switch_guides.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-guides
-Version: 0.2.4
+Version: 0.2.5
 Summary: A package for building Platform Guides in Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,21 @@
 
 ```bash
 pip install switch-guides
 ```
 
 # History
 
+## 0.2.5
+
+Added
+
+* Following attributes to `SwitchGuideStepData`
+  * request_data, request_timestamp, request_component_id
+
 ## 0.2.4
 
 Added
 
 * `options` attribute to `SwitchGuideStepProcessInput`
   * Allows Guide authors to provide additional options while processing the step
   * Attribute is optional and therefore Guide Step authors should take this into account
```

### Comparing `switch_guides-0.2.4/switch_guides.egg-info/SOURCES.txt` & `switch_guides-0.2.5/switch_guides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

