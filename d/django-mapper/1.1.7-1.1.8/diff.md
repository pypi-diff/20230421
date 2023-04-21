# Comparing `tmp/django-mapper-1.1.7.tar.gz` & `tmp/django-mapper-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mapper-1.1.7.tar", last modified: Thu Apr 20 07:15:56 2023, max compression
+gzip compressed data, was "django-mapper-1.1.8.tar", last modified: Fri Apr 21 06:24:22 2023, max compression
```

## Comparing `django-mapper-1.1.7.tar` & `django-mapper-1.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 07:15:56.633073 django-mapper-1.1.7/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.7/README.md
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/django_mapper/
--rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.7/django_mapper/__init__.py
--rw-r--r--   0 shubham   (1000) shubham   (1000)     4788 2023-04-20 07:08:54.000000 django-mapper-1.1.7/django_mapper/mapper.py
-drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-20 07:15:56.633073 django-mapper-1.1.7/django_mapper.egg-info/
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/PKG-INFO
--rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/SOURCES.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/dependency_links.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/requires.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-20 07:15:56.000000 django-mapper-1.1.7/django_mapper.egg-info/top_level.txt
--rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-20 07:15:56.633073 django-mapper-1.1.7/setup.cfg
--rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-20 07:13:01.000000 django-mapper-1.1.7/setup.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 06:24:22.155055 django-mapper-1.1.8/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       15 2023-04-13 21:24:22.000000 django-mapper-1.1.8/README.md
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/django_mapper/
+-rw-r--r--   0 shubham   (1000) shubham   (1000)       30 2023-04-18 05:43:41.000000 django-mapper-1.1.8/django_mapper/__init__.py
+-rw-r--r--   0 shubham   (1000) shubham   (1000)     5026 2023-04-21 06:20:41.000000 django-mapper-1.1.8/django_mapper/mapper.py
+drwxrwxr-x   0 shubham   (1000) shubham   (1000)        0 2023-04-21 06:24:22.155055 django-mapper-1.1.8/django_mapper.egg-info/
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      676 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/PKG-INFO
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)      252 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)        1 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       12 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/requires.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       14 2023-04-21 06:24:22.000000 django-mapper-1.1.8/django_mapper.egg-info/top_level.txt
+-rw-rw-r--   0 shubham   (1000) shubham   (1000)       38 2023-04-21 06:24:22.155055 django-mapper-1.1.8/setup.cfg
+-rw-r--r--   0 shubham   (1000) shubham   (1000)      787 2023-04-21 06:21:15.000000 django-mapper-1.1.8/setup.py
```

### Comparing `django-mapper-1.1.7/PKG-INFO` & `django-mapper-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.7
+Version: 1.1.8
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.7/django_mapper/mapper.py` & `django-mapper-1.1.8/django_mapper/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class DataMapper:
     def __init__(self, config, target_model=None, enable_logging=False):
         self.config = config
         self.target_model = target_model
         self.enable_logging = enable_logging
         self.logger = logging.getLogger(__name__)
     
-    def map_data(self, data, default_values={}):
+    def map_data(self, data, default_values={}, dont_save=False):
         mapped_data = {}
         for mapping in self.config:
             to_field = mapping.get('to_field')
             
             from_field = mapping.get('from_field')
             default_value = mapping.get('default_value')
 
@@ -38,15 +38,15 @@
             else:
                 raise ValueError("from_field or compute_method should be provided")
 
         if default_values:
             mapped_data.update(default_values)
 
         if self.target_model:
-            instance = self.create_instance(self.target_model, mapped_data, default_values=default_values)
+            instance = self.create_instance(self.target_model, mapped_data, default_values=default_values, dont_save=dont_save)
             self.logger.info(f"Created instance of {self.target_model.__name__}")
             return instance
         else:
             return mapped_data
     
     def get_value(self, data, field, mapper=None):
         current_data = data
@@ -77,15 +77,15 @@
         for f in fields[:-1]:
             if f not in data:
                 data[f] = {}
             data = data[f]
         data[fields[-1]] = value
         return data
     
-    def create_instance(self, model, data, default_values={}):
+    def create_instance(self, model, data, default_values={}, dont_save=False):
         instance_kwargs = {}
         m2m_fields = {}
         for key, value in data.items():
             if value is None:
                 continue
 
             if isinstance(value, dict):
@@ -97,29 +97,35 @@
             elif isinstance(value, list) or isinstance(value, QuerySet):
                 field = model._meta.get_field(key)
                 related_model = field.related_model
 
                 for single_value in value:
                     related_model_instance = single_value
                     if not isinstance(single_value, related_model):
-                        related_model_instance = self.create_instance(related_model, single_value)
+                        related_model_instance = self.create_instance(related_model, single_value, dont_save=dont_save)
                     
                     if key in m2m_fields:
                         m2m_fields[key].append(related_model_instance)
                     else:
                         m2m_fields[key] = [related_model_instance]
 
             else:
                 instance_kwargs[key] = value
         
         instance_kwargs.update(default_values)
-        instance = model.objects.create(**instance_kwargs)
 
-        save_again =  False
-        for m2m_field in m2m_fields:
-            getattr(instance, m2m_field).add(*m2m_fields[m2m_field])
-            save_again = True
+        if not dont_save:
+            instance = model.objects.create(**instance_kwargs)
 
-        if save_again:
-            instance.save()
+            save_again =  False
+            for m2m_field in m2m_fields:
+                getattr(instance, m2m_field).add(*m2m_fields[m2m_field])
+                save_again = True
 
-        return instance
+            if save_again:
+                instance.save()
+
+            return instance
+        else:
+            instance = model(**instance_kwargs)
+
+            return instance, m2m_fields
```

### Comparing `django-mapper-1.1.7/django_mapper.egg-info/PKG-INFO` & `django-mapper-1.1.8/django_mapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-mapper
-Version: 1.1.7
+Version: 1.1.8
 Summary: A utility class for mapping data between Django models
 Home-page: https://github.com/shubh95/django-mapper
 Author: Shubham Vashisht
 Author-email: shubhvas95@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-mapper-1.1.7/setup.py` & `django-mapper-1.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django-mapper',
-    version='1.1.7',
+    version='1.1.8',
     description='A utility class for mapping data between Django models',
     author='Shubham Vashisht',
     author_email='shubhvas95@gmail.com',
     url='https://github.com/shubh95/django-mapper',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

