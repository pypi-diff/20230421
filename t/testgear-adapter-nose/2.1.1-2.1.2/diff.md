# Comparing `tmp/testgear-adapter-nose-2.1.1.tar.gz` & `tmp/testgear-adapter-nose-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-nose-2.1.1.tar", last modified: Fri Mar 31 06:32:00 2023, max compression
+gzip compressed data, was "testgear-adapter-nose-2.1.2.tar", last modified: Fri Apr 21 14:56:40 2023, max compression
```

## Comparing `testgear-adapter-nose-2.1.1.tar` & `testgear-adapter-nose-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:00.623490 testgear-adapter-nose-2.1.1/
--rw-rw-rw-   0        0        0     9662 2023-03-31 06:32:00.623490 testgear-adapter-nose-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7280 2023-03-31 06:28:55.000000 testgear-adapter-nose-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 06:32:00.623490 testgear-adapter-nose-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1061 2023-03-31 06:28:55.000000 testgear-adapter-nose-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:00.607855 testgear-adapter-nose-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:00.607855 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/
--rw-rw-rw-   0        0        0        0 2023-03-27 12:00:18.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/__init__.py
--rw-rw-rw-   0        0        0     1263 2023-03-27 12:00:18.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/listener.py
--rw-rw-rw-   0        0        0      986 2023-03-27 12:00:18.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/plugin.py
--rw-rw-rw-   0        0        0     8373 2023-03-27 12:00:18.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:32:00.623490 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/
--rw-rw-rw-   0        0        0     9662 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-31 06:32:00.000000 testgear-adapter-nose-2.1.1/src/testgear_adapter_nose.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/
+-rw-rw-rw-   0        0        0     7830 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7280 2023-03-31 06:28:55.000000 testgear-adapter-nose-2.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2023-04-21 14:02:44.000000 testgear-adapter-nose-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.172878 testgear-adapter-nose-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.172878 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/__init__.py
+-rw-rw-rw-   0        0        0     1263 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/listener.py
+-rw-rw-rw-   0        0        0      986 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/plugin.py
+-rw-rw-rw-   0        0        0     8373 2023-04-21 13:59:17.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:40.198191 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/
+-rw-rw-rw-   0        0        0     7830 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-04-21 14:56:40.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-21 14:56:39.000000 testgear-adapter-nose-2.1.2/src/testgear_adapter_nose.egg-info/top_level.txt
```

### Comparing `testgear-adapter-nose-2.1.1/README.md` & `testgear-adapter-nose-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `testgear-adapter-nose-2.1.1/setup.py` & `testgear-adapter-nose-2.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testgear-adapter-nose',
-    version='2.1.1',
+    version='2.1.2',
     description='Nose adapter for Test Gear',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testgear-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@test-gear.io',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testgear_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testgear-python-commons==2.1.1'],
+    install_requires=['attrs', 'nose2', 'testgear-python-commons==2.1.2'],
     entry_points={
             'nose.plugins.0.10': [
                 'testgear_adapter_nose = testgear_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/listener.py` & `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/listener.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/plugin.py` & `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-nose-2.1.1/src/testgear_adapter_nose/utils.py` & `testgear-adapter-nose-2.1.2/src/testgear_adapter_nose/utils.py`

 * *Files identical despite different names*

