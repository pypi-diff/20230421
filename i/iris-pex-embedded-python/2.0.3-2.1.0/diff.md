# Comparing `tmp/iris_pex_embedded_python-2.0.3.tar.gz` & `tmp/iris_pex_embedded_python-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.0.3.tar", last modified: Tue Apr 18 12:22:09 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.1.0.tar", last modified: Fri Apr 21 09:04:54 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.0.3.tar` & `iris_pex_embedded_python-2.1.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.649999 iris_pex_embedded_python-2.0.3/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.0.3/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-18 12:22:09.649116 iris_pex_embedded_python-2.0.3/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.3/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.0.3/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-18 12:22:09.650279 iris_pex_embedded_python-2.0.3/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-18 12:20:55.000000 iris_pex_embedded_python-2.0.3/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.596010 iris_pex_embedded_python-2.0.3/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.595276 iris_pex_embedded_python-2.0.3/src/grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.604141 iris_pex_embedded_python-2.0.3/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.633472 iris_pex_embedded_python-2.0.3/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112    19811 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112    14889 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     6966 2023-04-18 10:16:42.000000 iris_pex_embedded_python-2.0.3/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.644975 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112      845 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-18 12:22:09.000000 iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/top_level.txt
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-18 12:22:09.646683 iris_pex_embedded_python-2.0.3/test/
--rw-r--r--   0 grongier (902446405) 1252422112      273 2023-01-06 14:56:27.000000 iris_pex_embedded_python-2.0.3/test/test_selectt.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.780011 iris_pex_embedded_python-2.1.0/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.1.0/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35813 2023-04-21 09:04:54.778885 iris_pex_embedded_python-2.1.0/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.0/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.0/pyproject.toml
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-04-21 09:04:54.780359 iris_pex_embedded_python-2.1.0/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2016 2023-04-21 09:04:29.000000 iris_pex_embedded_python-2.1.0/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.718939 iris_pex_embedded_python-2.1.0/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.717984 iris_pex_embedded_python-2.1.0/src/grongier/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.728873 iris_pex_embedded_python-2.1.0/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.765183 iris_pex_embedded_python-2.1.0/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20029 2023-04-21 08:44:33.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7063 2023-04-21 08:18:02.000000 iris_pex_embedded_python-2.1.0/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 09:04:54.776736 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35813 2023-04-21 09:04:54.000000 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      824 2023-04-21 09:04:54.000000 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-04-21 09:04:54.000000 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       14 2023-04-21 09:04:54.000000 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-04-21 09:04:54.000000 iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.0.3/LICENSE` & `iris_pex_embedded_python-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/PKG-INFO` & `iris_pex_embedded_python-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.0.3
+Version: 2.1.0
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.0.3/README.md` & `iris_pex_embedded_python-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/setup.py` & `iris_pex_embedded_python-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.0.3',
+        version='2.1.0',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,18 @@
         :param message: The message to be serialized
         :return: The serialized message
         """
         if (message is not None and self._is_message_instance(message)):
             return self._serialize_message(message)
         elif (message is not None and self._is_pickle_message_instance(message)):
             return self._serialize_pickle_message(message)
-        else:
+        elif (message is not None and self._is_iris_object_instance(message)):
             return message
+        else:
+            raise TypeError("The message must be an instance of a class that is a subclass of Message or IRISObject %Persistent class.")
 
     def _serialize_message(self,message):
         """ Converts a python dataclass message into an iris grongier.pex.message.
 
         Parameters:
         message: The message to serialize, an instance of a class that is a subclass of Message.
```

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,20 @@
         return False
 
     @classmethod
     def _is_pickle_message_instance(cls, obj):
         if cls._is_pickel_message_class(type(obj)):
             return True
         return False
+    
+    @classmethod
+    def _is_iris_object_instance(cls, obj):
+        if (obj is not None and type(obj).__module__.find('iris') == 0) and obj._IsA("%Persistent"):
+            return True
+        return False
 
     @classmethod
     def _is_message_class(cls, klass):
         name = klass.__module__ + '.' + klass.__qualname__
         if name == "grongier.pex.Message": 
             return True
         for c in klass.__bases__:
```

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.0.3/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.1.0/src/grongier/pex/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,19 +107,20 @@
             for klass in classes:
                 extend = ''
                 if len(klass.bases) == 1:
                     if hasattr(klass.bases[0],'id'):
                         extend = klass.bases[0].id
                     else:
                         extend = klass.bases[0].attr
-                #if extends BusinessOperation,BusinessProcess,BusinessService
                 if  extend in ('BusinessOperation','BusinessProcess','BusinessService','DuplexService','DuplexProcess','DuplexOperation','InboundAdapter','OutboundAdapter'):
                     module = _Utils.filename_to_module(filename)
-                    _Utils.register_component(module, klass.name, path, overwrite, f"{iris_package_name}.{module}.{klass.name}")
-
+                    iris_class_name = f"{iris_package_name}.{module}.{klass.name}"
+                    # strip "_" for iris class name
+                    iris_class_name = iris_class_name.replace('_','')
+                    _Utils.register_component(module, klass.name, path, overwrite, iris_class_name)
     @staticmethod
     def register_package(package:str,path:str,overwrite:int,iris_package_name:str):
         """
         It takes a package name, a path to the package, a flag to overwrite existing files, and the name of
         the iris package to register the files to. It then loops through all the files in the package and
         registers them to the iris package
```

### Comparing `iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.0.3
+Version: 2.1.0
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.0.3/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.1.0/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,8 @@
 src/grongier/pex/_private_session_duplex.py
 src/grongier/pex/_private_session_process.py
 src/grongier/pex/_utils.py
 src/iris_pex_embedded_python.egg-info/PKG-INFO
 src/iris_pex_embedded_python.egg-info/SOURCES.txt
 src/iris_pex_embedded_python.egg-info/dependency_links.txt
 src/iris_pex_embedded_python.egg-info/requires.txt
-src/iris_pex_embedded_python.egg-info/top_level.txt
-test/test_selectt.py
+src/iris_pex_embedded_python.egg-info/top_level.txt
```

