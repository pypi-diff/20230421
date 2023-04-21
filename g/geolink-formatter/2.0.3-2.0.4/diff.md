# Comparing `tmp/geolink_formatter-2.0.3.tar.gz` & `tmp/geolink_formatter-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolink_formatter-2.0.3.tar", last modified: Mon Jan 16 14:52:28 2023, max compression
+gzip compressed data, was "geolink_formatter-2.0.4.tar", last modified: Fri Apr 21 11:39:13 2023, max compression
```

## Comparing `geolink_formatter-2.0.3.tar` & `geolink_formatter-2.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7235 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/geolink_formatter/
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/format.py
--rw-r--r--   0 runner    (1001) docker     (122)     8105 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/geolink_formatter/schema/
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.0.0.xsd
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.1.1.xsd
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.0.xsd
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.1.xsd
--rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/geolink_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7235 2023-01-16 14:52:28.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-01-16 14:52:28.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-16 14:52:28.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-16 14:52:17.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-01-16 14:52:28.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-01-16 14:52:28.000000 geolink_formatter-2.0.3/geolink_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-01-16 14:52:28.089260 geolink_formatter-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1554 2023-01-16 14:52:15.000000 geolink_formatter-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:39:13.444683 geolink_formatter-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7384 2023-04-21 11:39:13.444683 geolink_formatter-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:39:13.440683 geolink_formatter-2.0.4/geolink_formatter/
+-rw-r--r--   0 runner    (1001) docker     (122)     2243 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8426 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8171 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:39:13.444683 geolink_formatter-2.0.4/geolink_formatter/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.0.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.1.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.1.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.2.xsd
+-rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.3.xsd
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 11:39:13.440683 geolink_formatter-2.0.4/geolink_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7384 2023-04-21 11:39:13.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-04-21 11:39:13.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 11:39:13.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 11:39:02.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-21 11:39:13.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 11:39:13.000000 geolink_formatter-2.0.4/geolink_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-21 11:39:13.444683 geolink_formatter-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-21 11:39:00.000000 geolink_formatter-2.0.4/setup.py
```

### Comparing `geolink_formatter-2.0.3/CHANGELOG` & `geolink_formatter-2.0.4/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0.4
+-----
+
+Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default), v1.2.3
+
+- Drop support for Python 3.7
+
 2.0.3
 -----
 
 Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default)
 
 - Remove tox
 - Remove versioning for documentation (sphinxcontrib-versioning)
```

### Comparing `geolink_formatter-2.0.3/PKG-INFO` & `geolink_formatter-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: geolink_formatter
-Version: 2.0.3
+Version: 2.0.4
 Summary: OEREBlex geoLink Formatter
 Home-page: https://gitlab.com/gf-bl/python-geolink-formatter
 Author: Karsten Deininger
 Author-email: karsten.deininger@bl.ch
 License: BSD
 Description: OEREBlex geoLink Formatter
         ==========================
@@ -36,14 +36,21 @@
         .. |code quality| image:: https://api.codacy.com/project/badge/Grade/d2bb03f17bf3438cb295c0b5ea131ac8
            :target: https://www.codacy.com/app/openoereb/geolink_formatter?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=openoereb/geolink_formatter&amp;utm_campaign=Badge_Grade
         
         
         Changelog
         =========
         
+        2.0.4
+        -----
+        
+        Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default), v1.2.3
+        
+        - Drop support for Python 3.7
+        
         2.0.3
         -----
         
         Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default)
         
         - Remove tox
         - Remove versioning for documentation (sphinxcontrib-versioning)
@@ -196,14 +203,13 @@
 Keywords: oereb lex geolink formatter html
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `geolink_formatter-2.0.3/README.rst` & `geolink_formatter-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/__init__.py` & `geolink_formatter-2.0.4/geolink_formatter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import unicode_literals
 
 from geolink_formatter.entity import Msg
 from geolink_formatter.format import HTML
 from geolink_formatter.parser import XML
 
 
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 
 class GeoLinkFormatter(object):
     def __init__(self, host_url=None, version='1.2.0', dtd_validation=False):
         """Creates a new GeoLinkFormatter instance.
 
         Args:
```

### Comparing `geolink_formatter-2.0.3/geolink_formatter/entity.py` & `geolink_formatter-2.0.4/geolink_formatter/entity.py`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/format.py` & `geolink_formatter-2.0.4/geolink_formatter/format.py`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/parser.py` & `geolink_formatter-2.0.4/geolink_formatter/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
     V1_2_1 = '1.2.1'
     """str: geoLink schema version 1.2.1"""
 
     V1_2_2 = '1.2.2'
     """str: geoLink schema version 1.2.2"""
 
+    V1_2_3 = '1.2.3'
+    """str: geoLink schema version 1.2.3"""
+
 
 class XML(object):
 
     _date_format = '%Y-%m-%d'
     """str: Format of date values in XML."""
 
     def __init__(self, host_url=None, version='1.2.2', dtd_validation=False, xsd_validation=True):
```

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.0.0.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.0.0.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.1.0.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.1.1.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.1.1.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.0.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.0.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.1.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.1.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter/schema/v1.2.2.xsd` & `geolink_formatter-2.0.4/geolink_formatter/schema/v1.2.2.xsd`

 * *Files identical despite different names*

### Comparing `geolink_formatter-2.0.3/geolink_formatter.egg-info/PKG-INFO` & `geolink_formatter-2.0.4/geolink_formatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: geolink-formatter
-Version: 2.0.3
+Version: 2.0.4
 Summary: OEREBlex geoLink Formatter
 Home-page: https://gitlab.com/gf-bl/python-geolink-formatter
 Author: Karsten Deininger
 Author-email: karsten.deininger@bl.ch
 License: BSD
 Description: OEREBlex geoLink Formatter
         ==========================
@@ -36,14 +36,21 @@
         .. |code quality| image:: https://api.codacy.com/project/badge/Grade/d2bb03f17bf3438cb295c0b5ea131ac8
            :target: https://www.codacy.com/app/openoereb/geolink_formatter?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=openoereb/geolink_formatter&amp;utm_campaign=Badge_Grade
         
         
         Changelog
         =========
         
+        2.0.4
+        -----
+        
+        Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default), v1.2.3
+        
+        - Drop support for Python 3.7
+        
         2.0.3
         -----
         
         Supported GEO-Link API versions: v1.0.0, v1.1.0, v1.1.1, v1.2.0, v1.2.1, v1.2.2 (default)
         
         - Remove tox
         - Remove versioning for documentation (sphinxcontrib-versioning)
@@ -196,14 +203,13 @@
 Keywords: oereb lex geolink formatter html
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `geolink_formatter-2.0.3/geolink_formatter.egg-info/SOURCES.txt` & `geolink_formatter-2.0.4/geolink_formatter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 geolink_formatter.egg-info/requires.txt
 geolink_formatter.egg-info/top_level.txt
 geolink_formatter/schema/v1.0.0.xsd
 geolink_formatter/schema/v1.1.0.xsd
 geolink_formatter/schema/v1.1.1.xsd
 geolink_formatter/schema/v1.2.0.xsd
 geolink_formatter/schema/v1.2.1.xsd
-geolink_formatter/schema/v1.2.2.xsd
+geolink_formatter/schema/v1.2.2.xsd
+geolink_formatter/schema/v1.2.3.xsd
```

### Comparing `geolink_formatter-2.0.3/setup.py` & `geolink_formatter-2.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,24 @@
     'lxml>=3.7.0',
     'defusedxml',
     'requests',
     'xmlschema'
 ]
 
 setup(name='geolink_formatter',
-      version='2.0.3',
+      version='2.0.4',
       description='OEREBlex geoLink Formatter',
       license='BSD',
       long_description='{readme}\n\n{changelog}'.format(readme=readme, changelog=changelog),
       classifiers=[
           "Development Status :: 5 - Production/Stable",
           "Intended Audience :: Developers",
           "License :: OSI Approved :: BSD License",
           "Natural Language :: English",
           "Operating System :: OS Independent",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
           "Topic :: Scientific/Engineering :: GIS",
           "Topic :: Software Development :: Libraries :: Python Modules"
       ],
```

