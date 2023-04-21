# Comparing `tmp/mobio-location-sdk-test-1.0.6.tar.gz` & `tmp/mobio-location-sdk-test-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-location-sdk-test-1.0.6.tar", last modified: Tue Feb 21 04:57:31 2023, max compression
+gzip compressed data, was "mobio-location-sdk-test-1.0.7.tar", last modified: Fri Apr 21 09:21:25 2023, max compression
```

## Comparing `mobio-location-sdk-test-1.0.6.tar` & `mobio-location-sdk-test-1.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.777619 mobio-location-sdk-test-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-21 04:57:31.776619 mobio-location-sdk-test-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       30 2023-02-14 03:27:38.000000 mobio-location-sdk-test-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.762618 mobio-location-sdk-test-1.0.6/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.766618 mobio-location-sdk-test-1.0.6/mobio/sdks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-14 03:27:38.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.766618 mobio-location-sdk-test-1.0.6/mobio/sdks/location/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-14 03:27:38.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.768618 mobio-location-sdk-test-1.0.6/mobio/sdks/location/helpers/
--rw-r--r--   0 root         (0) root         (0)      204 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3765 2023-02-19 15:41:58.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/helpers/function.py
--rw-r--r--   0 root         (0) root         (0)     2126 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/helpers/redis_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.772618 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-14 03:27:38.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-02-21 04:28:33.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/address_mapping.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/base_model.py
--rw-r--r--   0 root         (0) root         (0)      987 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/country_configs.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/db_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 04:57:31.775618 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)      887 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      715 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-21 04:57:31.000000 mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-02-15 10:02:32.000000 mobio-location-sdk-test-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-21 04:57:31.777619 mobio-location-sdk-test-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8885 2023-02-21 04:57:30.000000 mobio-location-sdk-test-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.955853 mobio-location-sdk-test-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-21 09:21:25.954853 mobio-location-sdk-test-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.941853 mobio-location-sdk-test-1.0.7/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.944853 mobio-location-sdk-test-1.0.7/mobio/sdks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.945853 mobio-location-sdk-test-1.0.7/mobio/sdks/location/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.947853 mobio-location-sdk-test-1.0.7/mobio/sdks/location/helpers/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/helpers/function.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/helpers/redis_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.950853 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/address_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/country_configs.py
+-rw-r--r--   0 root         (0) root         (0)      882 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/db_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:21:25.953853 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      715 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-21 09:19:51.000000 mobio-location-sdk-test-1.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:21:25.955853 mobio-location-sdk-test-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8885 2023-04-21 09:21:25.000000 mobio-location-sdk-test-1.0.7/setup.py
```

### Comparing `mobio-location-sdk-test-1.0.6/mobio/sdks/location/helpers/redis_helper.py` & `mobio-location-sdk-test-1.0.7/mobio/sdks/location/helpers/redis_helper.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/address_mapping.py` & `mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/address_mapping.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/base_model.py` & `mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/base_model.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/country_configs.py` & `mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/country_configs.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/mobio/sdks/location/models/db_manager.py` & `mobio-location-sdk-test-1.0.7/mobio/sdks/location/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/mobio_location_sdk_test.egg-info/SOURCES.txt` & `mobio-location-sdk-test-1.0.7/mobio_location_sdk_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-location-sdk-test-1.0.6/setup.py` & `mobio-location-sdk-test-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         :param filename:
         :return:
         """
         requirements = ["m-singleton", "redis", "pymongo"]
         return requirements
 
 
-version_dev='1.0.6'
-version_prod='1.0.0'
+version_dev='1.0.7'
+version_prod='1.0.1'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="mobio-location-sdk" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.6',  # Required, Phần này cũng không được format file.
+    version='1.0.7',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Location SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

