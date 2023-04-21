# Comparing `tmp/keepvariable-1.0.2.tar.gz` & `tmp/keepvariable-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.0.2.tar", last modified: Mon Apr 10 03:43:28 2023, max compression
+gzip compressed data, was "keepvariable-1.0.3.tar", last modified: Fri Apr 21 21:41:37 2023, max compression
```

## Comparing `keepvariable-1.0.2.tar` & `keepvariable-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.144216 keepvariable-1.0.2/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-04-10 03:43:28.144216 keepvariable-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.131251 keepvariable-1.0.2/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.0.2/keepvariable/__init__.py
--rw-rw-rw-   0        0        0     7343 2023-04-10 03:41:22.000000 keepvariable-1.0.2/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.0.2/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0      715 2023-04-10 03:41:38.000000 keepvariable-1.0.2/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-04-10 03:43:28.143219 keepvariable-1.0.2/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-10 03:43:28.000000 keepvariable-1.0.2/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 03:43:27.000000 keepvariable-1.0.2/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 03:43:28.144216 keepvariable-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-04-10 03:43:24.000000 keepvariable-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.069442 keepvariable-1.0.3/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-04-21 21:41:37.068445 keepvariable-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.035533 keepvariable-1.0.3/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.0.3/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0     7789 2023-04-21 21:40:36.000000 keepvariable-1.0.3/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.0.3/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1017 2023-04-21 21:27:03.000000 keepvariable-1.0.3/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.067448 keepvariable-1.0.3/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 21:41:37.069442 keepvariable-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-04-21 21:41:32.000000 keepvariable-1.0.3/setup.py
```

### Comparing `keepvariable-1.0.2/LICENSE` & `keepvariable-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.0.2/PKG-INFO` & `keepvariable-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.0.2/README.md` & `keepvariable-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.0.2/keepvariable/keepvariable_core.py` & `keepvariable-1.0.3/keepvariable/keepvariable_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 import ast
 import redis
 import json
 import pandas as pd
 import numpy as np
+import datetime
 
 def get_definition(jump_frames,*args,**kwargs):
     """Returns the definition of a function or a class from inside"""
     frame = inspect.currentframe()
     frame = inspect.getouterframes(frame)[jump_frames]
     try:
         string = inspect.getframeinfo(frame[0]).code_context[0].strip()
@@ -143,26 +144,33 @@
             final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame"}
             print(final_data)
             value=json.dumps(final_data)
         elif isinstance(value,np.ndarray):
             data=value.tolist()
             final_data={"data":data,"object_type":"np.ndarray"}
             value=json.dumps(final_data)
+        elif isinstance(value, datetime.datetime):
+            data=value.strftime("%Y-%m-%d %H:%M:%S")
+            final_data = {"data": data, "object_type": "datetime.datetime"}
+            value = json.dumps(final_data)
         return(value)
     
     def decode_loaded_value(self,value):
         try:
             value=json.loads(value)
             if "object_type" in value and isinstance(value,dict):
                 if value["object_type"]=="pd.DataFrame":
                     df=pd.DataFrame(value["data"],columns=value["columns"])
                     return(df)
                 elif value["object_type"]=="np.ndarray":
                     array=pd.DataFrame(value["data"]).values #to ensure 64bit values in array
                     return(array)
+                elif value["object_type"] == "datetime.datetime":
+                    datetime_value = datetime.datetime.strptime(value["data"],"%Y-%m-%d %H:%M:%S")
+                    return datetime_value
             return(value)
         except json.JSONDecodeError: #if type is str, it fails to decode
             return(value)
         
         
     def set(self,key,value):
         value=self.parse_saved_value(value)
@@ -196,8 +204,8 @@
         return(result)
         
     def get(self,key):
         value=self.redis.get(key)
         decoded_value=self.decode_loaded_value(value)
         return(decoded_value)
         
-        
+
```

### Comparing `keepvariable-1.0.2/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.0.3/keepvariable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.0.2/setup.py` & `keepvariable-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.0.2',
+    version='1.0.3',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-          ''
+          'redis'
      ],
     python_requires='>=3.6',
 )
```

