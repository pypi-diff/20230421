# Comparing `tmp/odoo_models_connect-0.1.8.tar.gz` & `tmp/odoo_models_connect-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_models_connect-0.1.8.tar", last modified: Wed Apr 19 14:04:03 2023, max compression
+gzip compressed data, was "odoo_models_connect-0.1.9.tar", last modified: Fri Apr 21 15:33:48 2023, max compression
```

## Comparing `odoo_models_connect-0.1.8.tar` & `odoo_models_connect-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.543528 odoo_models_connect-0.1.8/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-19 14:04:03.542008 odoo_models_connect-0.1.8/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4429 2023-04-18 21:27:49.000000 odoo_models_connect-0.1.8/README.md
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.531728 odoo_models_connect-0.1.8/odoo_models_connect/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       72 2023-04-17 14:13:42.000000 odoo_models_connect-0.1.8/odoo_models_connect/__init__.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.8/odoo_models_connect/connect_odoo.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      648 2023-04-12 11:53:38.000000 odoo_models_connect-0.1.8/odoo_models_connect/fields.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4124 2023-04-19 14:02:19.000000 odoo_models_connect-0.1.8/odoo_models_connect/models.py
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.539325 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      360 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/SOURCES.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/dependency_links.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/requires.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/top_level.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-19 14:04:03.544533 odoo_models_connect-0.1.8/setup.cfg
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-19 14:03:50.000000 odoo_models_connect-0.1.8/setup.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-21 15:33:48.490062 odoo_models_connect-0.1.9/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-21 15:33:48.489347 odoo_models_connect-0.1.9/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4429 2023-04-19 14:21:30.000000 odoo_models_connect-0.1.9/README.md
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-21 15:33:48.483086 odoo_models_connect-0.1.9/odoo_models_connect/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-19 14:21:24.000000 odoo_models_connect-0.1.9/odoo_models_connect/__init__.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.9/odoo_models_connect/connect_odoo.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      389 2023-04-21 15:32:56.000000 odoo_models_connect-0.1.9/odoo_models_connect/exceptions.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      629 2023-04-19 14:26:39.000000 odoo_models_connect-0.1.9/odoo_models_connect/fields.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4374 2023-04-21 15:32:42.000000 odoo_models_connect-0.1.9/odoo_models_connect/models.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-21 15:33:48.487977 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-21 15:33:48.000000 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      394 2023-04-21 15:33:48.000000 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-21 15:33:48.000000 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-21 15:33:48.000000 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/requires.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-21 15:33:48.000000 odoo_models_connect-0.1.9/odoo_models_connect.egg-info/top_level.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-21 15:33:48.490302 odoo_models_connect-0.1.9/setup.cfg
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-21 15:32:19.000000 odoo_models_connect-0.1.9/setup.py
```

### Comparing `odoo_models_connect-0.1.8/PKG-INFO` & `odoo_models_connect-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_models_connect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.8/README.md` & `odoo_models_connect-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.8/odoo_models_connect/connect_odoo.py` & `odoo_models_connect-0.1.9/odoo_models_connect/connect_odoo.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.8/odoo_models_connect/fields.py` & `odoo_models_connect-0.1.9/odoo_models_connect/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from abc import ABC
-
-class OdooField(ABC):
+class OdooField(object):
     _type = None
 
 class StringField(OdooField):
     _type = 'char'
 
 class BooleanField(OdooField):
     _type = 'bool'
@@ -31,8 +29,7 @@
     _type = 'many2one'
 
 class Many2manyField(OdooField):
     _type = 'many2many'
 
 class One2manyField(OdooField):
     _type = 'one2many'
-
```

### Comparing `odoo_models_connect-0.1.8/odoo_models_connect/models.py` & `odoo_models_connect-0.1.9/odoo_models_connect/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import xmlrpc.client
 from xmlrpc.client import Error
 from .fields import OdooField
 from dotenv import dotenv_values
 from abc import ABC, abstractmethod
 import os
 from dotenv import load_dotenv
+from .exceptions import (
+    ObjectDoesNotExist,
+    IDRequiredException,
+    EnvVariablesException,
+)
 
 
 def load_env_vars(env_path):
     if not os.path.exists(env_path):
         raise FileNotFoundError(".env not found, wrong path")
     load_dotenv(env_path)
 
@@ -34,22 +39,14 @@
             for name, value in kwargs.items():
                 setattr(self, name, value)
                 self._FIELDS[name] = value
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id}>"
 
-    class DoesNotExist(Exception):
-
-        def __init__(self, obj_id):
-            self.id = obj_id
-
-        def __str__(self):
-            return f'Element by id {self.id} does not exist'
-
     @classmethod
     def search_read(cls, query=[], **kwargs):
         records = cls._MODELS.execute_kw(
             cls._DATABASE,
             cls._UUID,
             cls._PASSWORD,
             cls._name,
@@ -63,22 +60,30 @@
     @classmethod
     def search_count(cls, query=[]):
         records = cls.search_read(query=query)
         return len(records)
 
     @classmethod
     def search_by_id(cls, obj_id=None):
-        if obj_id is None:
-            raise ValueError("id is required")
+        cls._validate_id_required(obj_id)
         record = cls.search_read(query=[["id", '=', obj_id]])
-        if len(record) == 0:
-            raise cls.DoesNotExist(obj_id)
+        cls._validate_object_not_exist(record, obj_id)
         return record[0]
 
     @classmethod
+    def _validate_id_required(cls, obj_id):
+        if obj_id is None:
+            raise IDRequiredException()
+
+    @classmethod
+    def _validate_object_not_exist(cls, record, obj_id):
+        if len(record) == 0:
+            raise ObjectDoesNotExist(obj_id)
+
+    @classmethod
     def _instances_from_list(cls, records):
         return [cls._create_instance_from_dict(record) for record in records]
 
     @classmethod
     def _create_instance_from_dict(cls, obj):
         return cls(**obj)
 
@@ -88,18 +93,21 @@
     def update(self):
         return self._MODELS.execute_kw(self._DATABASE, self._UUID, self._PASSWORD, self._name, 'write', [[self.id], self._FIELDS])
 
     def delete(self):
         return self._MODELS.execute_kw(self._DATABASE, self._UUID, self._PASSWORD, self._name, 'unlink', [[self.id]])
 
     def __init_subclass__(cls):
-        cls._set_config_envs()
-        cls._fill_fields()
-        cls._set_attributes_initialized_none()
-        super().__init_subclass__()
+        try:
+            cls._set_config_envs()
+            cls._fill_fields()
+            cls._set_attributes_initialized_none()
+            super().__init_subclass__()
+        except OSError:
+            raise EnvVariablesException()
 
     @classmethod
     def _set_attributes_initialized_none(cls):
         cls._set_models_attribute()
         cls._set_uuid_attribute()
 
     @classmethod
@@ -107,15 +115,16 @@
         cls._DATABASE = os.getenv('DATABASE')
         cls._USERNAME = os.getenv('USERNAME')
         cls._PASSWORD = os.getenv('PASSWORD')
         cls._URL = os.getenv('URL')
 
     @classmethod
     def _set_uuid_attribute(cls):
-        common = xmlrpc.client.ServerProxy('{}{}'.format(cls._URL, cls._COMMON))
+        common = xmlrpc.client.ServerProxy(
+            '{}{}'.format(cls._URL, cls._COMMON))
         cls._UUID = common.authenticate(
             cls._DATABASE, cls._USERNAME, cls._PASSWORD, {})
 
     @classmethod
     def _set_models_attribute(cls):
         cls._MODELS = xmlrpc.client.ServerProxy(
             '{}{}'.format(cls._URL, cls._OBJECTS))
```

### Comparing `odoo_models_connect-0.1.8/odoo_models_connect.egg-info/PKG-INFO` & `odoo_models_connect-0.1.9/odoo_models_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-models-connect
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.8/setup.py` & `odoo_models_connect-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.8'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.9'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 # Debe coincidir con el nombre de la carpeta
 PACKAGE_NAME = 'odoo_models_connect'
 AUTHOR = 'Deiver Jose Vazquez Moreno'  # Modificar con vuestros datos
 AUTHOR_EMAIL = 'estudiandovazmore@gmail.com'  # Modificar con vuestros datos
 # Modificar con vuestros datos
 URL = 'https://github.com/DeijoseDevelop/odoo_models_connect'
```

