# Comparing `tmp/otlmow_modelbuilder-0.6.tar.gz` & `tmp/otlmow_modelbuilder-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otlmow_modelbuilder-0.6.tar", last modified: Wed Jan 18 09:16:15 2023, max compression
+gzip compressed data, was "otlmow_modelbuilder-0.7.tar", last modified: Thu Feb 16 22:20:26 2023, max compression
```

## Comparing `otlmow_modelbuilder-0.6.tar` & `otlmow_modelbuilder-0.7.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:15.635617 otlmow_modelbuilder-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-01-18 09:16:03.000000 otlmow_modelbuilder-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44121 2023-01-18 09:16:15.635617 otlmow_modelbuilder-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-01-18 09:16:03.000000 otlmow_modelbuilder-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:15.631617 otlmow_modelbuilder-0.6/otlmow_modelbuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/AbstractDatatypeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/DatatypeBuilderFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/GenericBuilderFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieArtefactCollector.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieInMemoryCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieInheritanceProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/HelperFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/ModelBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/NewOTLBaseClassNotImplemented.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OSLOInMemoryCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLClassCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLComplexDatatypeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLEnumerationCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLModelCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLPrimitiveDatatypeCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLUnionDatatypeCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:15.635617 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/Inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOAttribuut.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOCollector.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeComplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeComplexAttribuut.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypePrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypePrimitiveAttribuut.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeUnion.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeUnionAttribuut.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOEnumeration.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLORelatie.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOTypeLink.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDbReader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 09:16:15.631617 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44121 2023-01-18 09:16:15.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-01-18 09:16:15.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 09:16:15.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-18 09:16:15.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-18 09:16:15.000000 otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-18 09:16:04.000000 otlmow_modelbuilder-0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 09:16:15.635617 otlmow_modelbuilder-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:26.692634 otlmow_modelbuilder-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44121 2023-02-16 22:20:26.692634 otlmow_modelbuilder-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:26.688634 otlmow_modelbuilder-0.7/otlmow_modelbuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/AbstractDatatypeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/DatatypeBuilderFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/GenericBuilderFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieArtefactCollector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieInMemoryCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieInheritanceProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/HelperFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/ModelBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/NewOTLBaseClassNotImplemented.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OSLOInMemoryCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLClassCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLComplexDatatypeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10411 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLEnumerationCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLModelCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLPrimitiveDatatypeCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLUnionDatatypeCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:26.692634 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/Inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOAttribuut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOCollector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeComplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeComplexAttribuut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypePrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypePrimitiveAttribuut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeUnion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLODatatypeUnionAttribuut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOEnumeration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLORelatie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOTypeLink.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDbReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/SettingsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 22:20:26.692634 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44121 2023-02-16 22:20:26.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-16 22:20:26.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 22:20:26.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-16 22:20:26.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-16 22:20:26.000000 otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-16 22:20:17.000000 otlmow_modelbuilder-0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 22:20:26.692634 otlmow_modelbuilder-0.7/setup.cfg
```

### Comparing `otlmow_modelbuilder-0.6/LICENSE` & `otlmow_modelbuilder-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/PKG-INFO` & `otlmow_modelbuilder-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow_modelbuilder
-Version: 0.6
+Version: 0.7
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_modelbuilder-0.6/README.md` & `otlmow_modelbuilder-0.7/README.md`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/AbstractDatatypeCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/AbstractDatatypeCreator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-import os
 from abc import ABC
-from typing import List
+from typing import Dict
 
 from otlmow_modelbuilder.DatatypeBuilderFunctions import get_attributen_by_type_field
 from otlmow_modelbuilder.GenericBuilderFunctions import add_attributen_to_data_block, \
     get_fields_to_import_from_list_of_attributes
 from otlmow_modelbuilder.HelperFunctions import wrap_in_quotes
 from otlmow_modelbuilder.SQLDataClasses.OSLOCollector import OSLOCollector
 
 
 class AbstractDatatypeCreator(ABC):
     def __init__(self, oslo_collector: OSLOCollector):
         self.oslo_collector = oslo_collector
 
     def create_block_to_write_from_complex_primitive_or_union_types(self, oslo_datatype, type_field='',
-                                                                    model_location=''):
+                                                                    model_location='', valid_uri_and_types: Dict = None):
+        if valid_uri_and_types is None:
+            valid_uri_and_types = {}
         attributen = get_attributen_by_type_field(self.oslo_collector, type_field, oslo_datatype)
 
         datablock = ['# coding=utf-8',
                      'from otlmow_model.BaseClasses.OTLAttribuut import OTLAttribuut']
 
         list_fields_to_start_with = [f'{type_field}Field']
         if type_field == 'UnionType':
             list_fields_to_start_with.append('UnionWaarden')
         elif type_field == 'Complex':
             datablock.append('from otlmow_model.BaseClasses.WaardenObject import WaardenObject')
         elif type_field == 'Primitive' or type_field == 'KwantWrd':
             datablock.append('from otlmow_model.BaseClasses.OTLField import OTLField')
             datablock.append('from otlmow_model.BaseClasses.WaardenObject import WaardenObject')
             list_fields_to_start_with = []
-        list_of_fields = get_fields_to_import_from_list_of_attributes(self.oslo_collector, attributen, list_fields_to_start_with)
+        list_of_fields = get_fields_to_import_from_list_of_attributes(self.oslo_collector, attributen,
+                                                                      valid_uri_and_types=valid_uri_and_types,
+                                                                      list_to_start_from=list_fields_to_start_with)
         base_fields = ['BooleanField', 'ComplexField', 'DateField', 'DateTimeField', 'FloatOrDecimalField',
                        'IntegerField',
                        'KeuzelijstField', 'UnionTypeField', 'URIField', 'LiteralField', 'NonNegIntegerField',
                        'TimeField',
                        'StringField', 'UnionWaarden']
         for module in list_of_fields:
             model_module = 'otlmow_model'
@@ -50,22 +53,21 @@
 
         datablock.append('')
         datablock.append('')
         datablock.append(f'# Generated with {self.__class__.__name__}. To modify: extend, do not edit')
         if type_field == 'UnionType':
             datablock.append(f'class {oslo_datatype.name}Waarden(UnionWaarden):')
             datablock.append('    def __init__(self):')
-#            datablock.append('        AttributeInfo.__init__(self, parent)')
             datablock.append('        UnionWaarden.__init__(self)')
         else:
             datablock.append(f'class {oslo_datatype.name}Waarden(WaardenObject):')
             datablock.append('    def __init__(self):')
             datablock.append('        WaardenObject.__init__(self)')
 
-        add_attributen_to_data_block(attributen=attributen, datablock=datablock, type_field=type_field)
+        add_attributen_to_data_block(attributen=attributen, datablock=datablock, type_field=type_field, valid_uri_and_types=valid_uri_and_types)
 
         if type_field == 'Primitive' or type_field == 'KwantWrd':
             type_field = 'OTL'
 
         datablock.append(''),
         datablock.append(f'# Generated with {self.__class__.__name__}. To modify: extend, do not edit')
         datablock.append(f'class {oslo_datatype.name}({type_field}Field):')
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/DatatypeBuilderFunctions.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/DatatypeBuilderFunctions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Dict
+
+
 def get_single_field_from_type_uri(field_type: str):
     if field_type.startswith('https://wegenenverkeer.data.vlaanderen.be/ns/') and '#' in field_type:
         return field_type.split('#')[1]
 
     if field_type is None:
         return ''
     elif field_type == 'http://www.w3.org/2001/XMLSchema#decimal':
@@ -28,24 +31,20 @@
         return 'DtcContactinfo'
     elif field_type == 'http://www.w3.org/2000/01/rdf-schema#Literal':
         return 'StringField'
     else:
         raise NotImplemented('not supported field_type in get_single_field_from_type_uri()')
 
 
-def get_non_single_field_from_type_uri(field_type: str):
+def get_non_single_field_from_type_uri(field_type: str, valid_uri_and_types: Dict):
     if '#Dtc' in field_type:
         type_name = field_type[field_type.find("#") + 1::]
         return ['ComplexField', type_name]
-    if field_type.startswith("https://schema.org/"):
-        if field_type == "https://schema.org/ContactPoint":
-            return ['ComplexField', "DtcContactinfo"]
-        if field_type == "https://schema.org/OpeningHoursSpecification":
-            return ['ComplexField', "DtcOpeningsurenSpecificatie"]
-        raise NotImplementedError(f"Field of type {field_type} is not implemented in DatatypeCreator")
+    if field_type in valid_uri_and_types.keys():
+        return ['ComplexField', valid_uri_and_types[field_type]]
     if '#Dte' in field_type or '#KwantWrd' in field_type:
         type_name = field_type[field_type.find("#") + 1::]
         return ['ComplexField', type_name]
     if '#Kl' in field_type or field_type in [
             'https://wegenenverkeer.data.vlaanderen.be/ns/onderdeel#AntiParkeerpaalType',
             'https://wegenenverkeer.data.vlaanderen.be/ns/onderdeel#KLLuidsprekerVormgeving']:
         type_name = field_type[field_type.find("#") + 1::]
@@ -53,70 +52,64 @@
     if '#Dtu' in field_type:
         type_name = field_type[field_type.find("#") + 1::]
         return ['UnionTypeField', type_name]
 
     raise NotImplementedError(f'not supported field_type {field_type} in get_non_single_field_from_type_uri()')
 
 
-def get_field_name_from_type_uri(attribuut_type):
+def get_field_name_from_type_uri(attribuut_type, valid_uri_and_types):
     if attribuut_type.startswith('http://www.w3.org/2001/XMLSchema#'):
         return get_single_field_from_type_uri(attribuut_type)
     if attribuut_type.startswith("https://schema.org/"):
-        return get_non_single_field_from_type_uri(attribuut_type)[1]
-    return get_non_single_field_from_type_uri(attribuut_type)[1]
+        return get_non_single_field_from_type_uri(attribuut_type, valid_uri_and_types)[1]
+    return get_non_single_field_from_type_uri(attribuut_type, valid_uri_and_types)[1]
 
 
 def get_attributen_by_type_field(oslo_collector, type_field, oslo_datatype):
     if type_field == 'Complex':
         return oslo_collector.find_complex_datatype_attributes_by_class_uri(oslo_datatype.objectUri)
     elif type_field == 'UnionType':
         return oslo_collector.find_union_datatype_attributes_by_class_uri(oslo_datatype.objectUri)
     else:
         return oslo_collector.find_primitive_datatype_attributes_by_class_uri(oslo_datatype.objectUri)
 
 
-def get_type_name_of_complex_attribuut(type_uri: str):
-    if type_uri.startswith("https://wegenenverkeer.data.vlaanderen.be/ns/") or type_uri.startswith(
-            "http://www.w3.org/2001/XMLSchema#"):
-        return type_uri[type_uri.find("#") + 1::]
-    elif type_uri.startswith("https://schema.org/"):
-        if type_uri == "https://schema.org/ContactPoint":
-            return "DtcContactinfo"
-        if type_uri == "https://schema.org/OpeningHoursSpecification":
-            return "DtcOpeningsurenSpecificatie"
-        raise NotImplementedError(
-            f"Field of type {type_uri} is not implemented in DatatypeCreator.get_type_name_of_complex_attribuut")
+def get_type_name_of_complex_attribuut(type_uri: str, valid_uri_and_types):
+    if '/ns/' in type_uri or type_uri.startswith('http://www.w3.org/2001/XMLSchema#'):
+        return type_uri[type_uri.find('#') + 1::]
+    if type_uri in valid_uri_and_types.keys():
+        return valid_uri_and_types[type_uri]
 
     raise NotImplementedError(f"get_type_name_of_complex_attribuut fails to get typename from {type_uri}")
 
 
 def get_type_link_from_attribuut(oslo_collector, attribuut):
     type_link = oslo_collector.find_type_link_by_uri(attribuut.type)
     if type_link is not None:
         return type_link
 
 
-def get_fields_and_names_from_list_of_attributes(attributen):
+def get_fields_and_names_from_list_of_attributes(attributen, valid_uri_and_types):
     if len(attributen) == 0:
         return []
 
     primitive_types_list = list(
         filter(lambda t: t.type.startswith('http://www.w3.org/2001/XMLSchema#'), attributen))
     other_types_list = list(
         filter(lambda t: not t.type.startswith('http://www.w3.org/2001/XMLSchema#'), attributen))
 
     select_types_list = list(
         map(lambda a: (get_single_field_from_type_uri(a.type), a.name), primitive_types_list))
 
     for nonPrimitiveType in other_types_list:
-        select_types_list.append((get_field_name_from_type_uri(nonPrimitiveType.type), nonPrimitiveType.name))
+        select_types_list.append((get_field_name_from_type_uri(nonPrimitiveType.type, valid_uri_and_types), nonPrimitiveType.name))
 
     distinct_types_list = list(set(select_types_list))
     sorted_list = sorted(distinct_types_list, key=lambda t: t)
     return sorted_list
 
 
 def get_type_name_of_union_attribuut(type_uri: str):
-    if type_uri.startswith("https://wegenenverkeer.data.vlaanderen.be/ns/"):
-        return type_uri[type_uri.find("#") + 1::]
+    if '/ns/' in type_uri and '#' in type_uri:
+        return type_uri[type_uri.find('#') + 1::]
 
-    raise NotImplementedError(f"get_type_name_of_complex_attribuut fails to get typename from {type_uri}")
+    raise NotImplementedError(f'get_type_name_of_complex_attribuut fails to get typename from {type_uri}')
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/GenericBuilderFunctions.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/GenericBuilderFunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import List
+from typing import List, Dict
 
 from otlmow_modelbuilder.DatatypeBuilderFunctions import get_single_field_from_type_uri, get_type_link_from_attribuut, \
     get_type_name_of_complex_attribuut, get_type_name_of_union_attribuut, get_field_name_from_type_uri, \
     get_non_single_field_from_type_uri
 from otlmow_modelbuilder.HelperFunctions import wrap_in_quotes
 
 
@@ -30,15 +30,15 @@
             if line == 'from typing import List':
                 break
         return f'List[{type_string}]'
     else:
         return type_string
 
 
-def get_type_hint_from_field(attribute, datablock):
+def get_type_hint_from_field(attribute, datablock, valid_uri_and_types):
     field_name = get_single_field_from_type_uri(attribute.type)
     if field_name == 'StringField' or field_name == 'URIField':
         return f' -> {cardinality_check(attribute, "str", datablock)}'
     elif field_name == 'FloatOrDecimalField':
         return f' -> {cardinality_check(attribute, "float", datablock)}'
     elif field_name == 'BooleanField':
         return f' -> {cardinality_check(attribute, "bool", datablock)}'
@@ -50,15 +50,15 @@
     elif field_name == 'DateTimeField':
         import_datetime(datablock, 'datetime')
         return f' -> {cardinality_check(attribute, "datetime", datablock)}'
     elif field_name == 'TimeField':
         import_datetime(datablock, 'time')
         return f' -> {cardinality_check(attribute, "time", datablock)}'
     else:
-        field_name = get_non_single_field_from_type_uri(attribute.type)
+        field_name = get_non_single_field_from_type_uri(attribute.type, valid_uri_and_types)
         if field_name[0] == 'KeuzelijstField':
             return f' -> {cardinality_check(attribute, "str", datablock)}'
         if field_name[0] == 'ComplexField' or field_name[0] == 'UnionTypeField':
             for index, line in enumerate(datablock):
                 if line[0] not in ['#', 'f']:  # only loop over the import part
                     break
                 if field_name[1] not in line:
@@ -69,15 +69,16 @@
                 break
             return f' -> {cardinality_check(attribute, field_name[1] + "Waarden", datablock)}'
         else:
             print('not complexe waarde')
     return ''
 
 
-def add_attributen_to_data_block(attributen, datablock: List[str], for_class_use=False, type_field=''):
+def add_attributen_to_data_block(attributen, datablock: List[str], valid_uri_and_types: Dict, for_class_use=False,
+                                 type_field=''):
     prop_datablock = []
     for attribuut in sorted(attributen, key=lambda a: a.name):
         if attribuut.overerving == 1:
             raise NotImplementedError(f"overerving 1 is not implemented, found in {attributen.objectUri}")
 
         whitespace = get_white_space_equivalent(f'        self._{attribuut.name} = OTLAttribuut(')
         field_name = get_single_field_from_type_uri(attribuut.type)
@@ -107,15 +108,15 @@
         datablock.append(f'{whitespace}owner=self)')
         datablock.append('')
 
         owner_self = ', owner=self'
         if not for_class_use:
             owner_self += '._parent'
 
-        type_hint = get_type_hint_from_field(attribuut, datablock)
+        type_hint = get_type_hint_from_field(attribuut, datablock, valid_uri_and_types)
 
         prop_datablock.append(f'    @property'),
         prop_datablock.append(f'    def {attribuut.name}(self){type_hint}:'),
         prop_datablock.append(f'        """{attribuut.definition}"""'),
         if type_field == 'KwantWrd' and attribuut.name == 'standaardEenheid':
             prop_datablock.append(f'        return self._{attribuut.name}.usagenote.split(\'"\')[1]'),
         else:
@@ -132,15 +133,16 @@
             prop_datablock.append(f'')
 
     datablock.extend(prop_datablock)
 
     return datablock
 
 
-def get_fields_to_import_from_list_of_attributes(oslo_collector, attributen, list_to_start_from=None):
+def get_fields_to_import_from_list_of_attributes(oslo_collector, attributen, valid_uri_and_types,
+                                                 list_to_start_from=None):
     if list_to_start_from is None:
         list_to_start_from = []
     if len(attributen) == 0:
         return list_to_start_from
 
     collected_list = []
     collected_list.extend(list_to_start_from)
@@ -148,15 +150,16 @@
     for attribuut in attributen:
         type_link = get_type_link_from_attribuut(oslo_collector, attribuut).item_tabel
         if type_link == "OSLOEnumeration":
             collected_list.append(attribuut.type.split('#')[1])
         elif type_link == "OSLODatatypePrimitive":
             collected_list.append(get_single_field_from_type_uri(attribuut.type))
         elif type_link == "OSLODatatypeComplex":
-            collected_list.append(get_type_name_of_complex_attribuut(attribuut.type))
+            collected_list.append(get_type_name_of_complex_attribuut(attribuut.type,
+                                                                     valid_uri_and_types=valid_uri_and_types))
         elif type_link == "OSLODatatypeUnion":
             collected_list.append(get_type_name_of_union_attribuut(attribuut.type))
         else:
             raise not NotImplementedError(f"{type_link} not implemented")
 
     distinct_types_list = list(set(collected_list))
     sorted_list = sorted(distinct_types_list, key=lambda t: t)
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieArtefactCollector.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieArtefactCollector.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieInMemoryCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieInMemoryCreator.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/GeometrieInheritanceProcessor.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/GeometrieInheritanceProcessor.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/HelperFunctions.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/HelperFunctions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 def get_ns_and_name_from_uri(objectUri):
-    if 'https://wegenenverkeer.data.vlaanderen.be/ns/' not in objectUri:
-        raise ValueError(f'{objectUri} is not a valid uri to extract a namespace from')
+    if '/ns/' not in objectUri:
+        raise ValueError(f"{objectUri} is not a valid uri because it does not define a namespace ('/ns' is missing)")
+
+    if '#' not in objectUri:
+        raise ValueError(f"{objectUri} is not a valid uri because can not be split into a ns and name ('#' is missing)")
 
     short_uri = objectUri.split('/ns/')[1]
     short_uri_array = short_uri.split('#')
     return short_uri_array[0], short_uri_array[1]
 
 
 def get_class_directory_from_ns(ns):
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/ModelBuilder.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/ModelBuilder.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 from otlmow_modelbuilder.GeometrieArtefactCollector import GeometrieArtefactCollector
 from otlmow_modelbuilder.GeometrieInMemoryCreator import GeometrieInMemoryCreator
 from otlmow_modelbuilder.OSLOInMemoryCreator import OSLOInMemoryCreator
 from otlmow_modelbuilder.OTLModelCreator import OTLModelCreator
 from otlmow_modelbuilder.SQLDataClasses.OSLOCollector import OSLOCollector
 from otlmow_modelbuilder.SQLDbReader import SQLDbReader
+from otlmow_modelbuilder.SettingsManager import load_settings
 
 
 class ModelBuilder:
     @staticmethod
     def build_otl_datamodel(otl_subset_location: Path,
                             directory: Path,
                             environment: str = 'prd',
-                            geometry_artefact_location: Path = None):
+                            geometry_artefact_location: Path = None,
+                            settings_path: Path = None):
         if directory is None:
             this_file_path = Path(__file__)
             directory = this_file_path.parent
 
         sql_reader = SQLDbReader(otl_subset_location)
         oslo_creator = OSLOInMemoryCreator(sql_reader)
         subset_collector = OSLOCollector(oslo_creator)
@@ -27,10 +29,12 @@
             geo_memory_creator = GeometrieInMemoryCreator(sql_reader_ga)
             geo_artefact_collector = GeometrieArtefactCollector(geo_memory_creator)
 
         subset_collector.collect()
         if geo_artefact_collector is not None:
             geo_artefact_collector.collect()
 
-        OTLModelCreator.create_full_model(directory=directory, environment=environment,
+        settings = load_settings(settings_path)
+
+        OTLModelCreator.create_full_model(directory=directory, environment=environment, settings=settings,
                                           oslo_collector=subset_collector,
                                           geo_artefact_collector=geo_artefact_collector)
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OSLOInMemoryCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OSLOInMemoryCreator.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLClassCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLClassCreator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import re
+from typing import Dict
 
 from otlmow_modelbuilder.GenericBuilderFunctions import add_attributen_to_data_block, \
     get_fields_to_import_from_list_of_attributes
 from otlmow_modelbuilder.GeometrieArtefactCollector import GeometrieArtefactCollector
 from otlmow_modelbuilder.GeometrieInheritanceProcessor import GeometrieInheritanceProcessor
 from otlmow_modelbuilder.GeometrieType import GeometrieType
 from otlmow_modelbuilder.HelperFunctions import get_ns_and_name_from_uri, get_class_directory_from_ns
@@ -22,30 +24,34 @@
 
         if geo_a_collector is not None:
             gip = GeometrieInheritanceProcessor(classes=oslo_collector.classes,
                                                 geometrie_types=self.geoACollector.geometrie_types,
                                                 inheritances=self.oslo_collector.inheritances)
             self.geometry_types = gip.process_inheritances()
 
-    def create_blocks_to_write_from_classes(self, oslo_class: OSLOClass, model_location='') -> [str]:
+    def create_blocks_to_write_from_classes(self, oslo_class: OSLOClass, model_location='', valid_uri_and_types: Dict = None) -> [str]:
         if not isinstance(oslo_class, OSLOClass):
             raise ValueError(f"Input is not a OSLOClass")
 
-        if oslo_class.objectUri == '' or not (
-                oslo_class.objectUri.startswith(
-                    'https://wegenenverkeer.data.vlaanderen.be/ns/') or oslo_class.objectUri.
-                        startswith('http://purl.org/dc/terms')):
+        if oslo_class.objectUri == '':
+            raise ValueError(f"OSLOClass.objectUri is invalid. Value = '{oslo_class.objectUri}'")
+
+        if oslo_class.objectUri == 'http://purl.org/dc/terms/Agent':
+            pass
+        elif not re.match(pattern="^.+/ns/.+#.+", string=oslo_class.objectUri):
             raise ValueError(f"OSLOClass.objectUri is invalid. Value = '{oslo_class.objectUri}'")
 
         if oslo_class.name == '':
             raise ValueError(f"OSLOClass.name is invalid. Value = '{oslo_class.name}'")
 
-        return self.create_block_from_class(oslo_class, model_location)
+        return self.create_block_from_class(oslo_class, model_location, valid_uri_and_types=valid_uri_and_types)
 
-    def create_block_from_class(self, oslo_class: OSLOClass, model_location: str = '') -> [str]:
+    def create_block_from_class(self, oslo_class: OSLOClass, model_location: str = '', valid_uri_and_types: Dict = None) -> [str]:
+        if valid_uri_and_types is None:
+            valid_uri_and_types = {}
         attributen = self.oslo_collector.find_attributes_by_class(oslo_class)
         inheritances = self.oslo_collector.find_inheritances_by_class(oslo_class)
         list_of_geometry_types = self.get_geometry_types_from_uri(oslo_class.objectUri)
 
         if oslo_class.objectUri in ['https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#AIMObject',
                                     'https://wegenenverkeer.data.vlaanderen.be/ns/implementatieelement#Derdenobject',
                                     'https://wegenenverkeer.data.vlaanderen.be/ns/abstracten#AbstracteAanvullendeGeometrie']:
@@ -102,15 +108,16 @@
                     datablock.append(f'from {model_module}.{class_directory}.{inheritance.base_name} '
                                      f'import {inheritance.base_name}')
 
         if any(atr.readonly == 1 for atr in attributen):
             raise NotImplementedError("readonly property is assumed to be 0 on value fields")
 
         list_of_fields = get_fields_to_import_from_list_of_attributes(oslo_collector=self.oslo_collector,
-                                                                      attributen=attributen)
+                                                                      attributen=attributen,
+                                                                      valid_uri_and_types=valid_uri_and_types)
         base_fields = ['BooleanField', 'ComplexField', 'DateField', 'DateTimeField', 'FloatOrDecimalField',
                        'IntegerField', 'KeuzelijstField', 'UnionTypeField', 'URIField', 'LiteralField',
                        'NonNegIntegerField', 'TimeField', 'StringField', 'UnionWaarden']
         for type_field in list_of_fields:
             model_module = 'otlmow_model'
             if model_location != '' and type_field not in base_fields:
                 if 'UnitTests' in model_location:
@@ -158,15 +165,15 @@
                 datablock.append(f'        {inheritance.base_name}.__init__(self)')
             for geo_type in sorted(list_of_geometry_types):
                 datablock.append(f'        {geo_type}.__init__(self)')
             datablock.append('')
 
         self.add_relations_to_datablock(datablock, oslo_class.objectUri)
 
-        add_attributen_to_data_block(attributen, datablock, for_class_use=True)
+        add_attributen_to_data_block(attributen, datablock, for_class_use=True, valid_uri_and_types=valid_uri_and_types)
         if len(inheritances) == 0 and len(attributen) == 0:
             datablock.append('        pass')
 
         if datablock[-1] == '':
             datablock.pop()
 
         return datablock
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLComplexDatatypeCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLComplexDatatypeCreator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import logging
+import re
+from typing import Dict
 
 from otlmow_modelbuilder.AbstractDatatypeCreator import AbstractDatatypeCreator
 from otlmow_modelbuilder.SQLDataClasses.OSLOCollector import OSLOCollector
 from otlmow_modelbuilder.SQLDataClasses.OSLODatatypeComplex import OSLODatatypeComplex
 
 
 class OTLComplexDatatypeCreator(AbstractDatatypeCreator):
     def __init__(self, oslo_collector: OSLOCollector):
         super().__init__(oslo_collector)
         logging.info("Created an instance of OTLComplexDatatypeCreator")
 
-    def create_block_to_write_from_complex_types(self, oslo_datatype_complex: OSLODatatypeComplex, model_location='') -> [str]:
+    def create_block_to_write_from_complex_types(self, oslo_datatype_complex: OSLODatatypeComplex,
+                                                 complex_datatype_validation_rules: Dict, model_location='') -> [str]:
         if not isinstance(oslo_datatype_complex, OSLODatatypeComplex):
             raise ValueError(f"Input is not a OSLODatatypeComplex")
 
-        if oslo_datatype_complex.objectUri == '' or not (oslo_datatype_complex.objectUri == 'https://schema.org/ContactPoint' or
-                                                         oslo_datatype_complex.objectUri == 'https://schema.org/OpeningHoursSpecification' or
-                                                         (oslo_datatype_complex.objectUri.startswith(
-                                                           'https://wegenenverkeer.data.vlaanderen.be/ns/') and 'Dtc' in oslo_datatype_complex.objectUri)):
+        if oslo_datatype_complex.objectUri == '':
             raise ValueError(f"OSLODatatypeComplex.objectUri is invalid. Value = '{oslo_datatype_complex.objectUri}'")
 
+        if oslo_datatype_complex.objectUri in complex_datatype_validation_rules['valid_uri_and_types'].keys():
+            pass
+        else:
+            match_re = False
+            for regex in complex_datatype_validation_rules["valid_regexes"]:
+                match_re = re.match(pattern=regex, string=oslo_datatype_complex.objectUri)
+                if match_re:
+                    break
+            if not match_re:
+                raise ValueError(
+                    f"OSLODatatypeComplex.objectUri is invalid. Value = '{oslo_datatype_complex.objectUri}'")
+
         if oslo_datatype_complex.name == '':
             raise ValueError(f"OSLODatatypeComplex.name is invalid. Value = '{oslo_datatype_complex.name}'")
 
-        if oslo_datatype_complex.objectUri.startswith(
-                'https://wegenenverkeer.data.vlaanderen.be/ns/') and 'Dtc' in oslo_datatype_complex.objectUri:
-            return self.create_block_to_write_from_complex_primitive_or_union_types(oslo_datatype_complex, type_field='Complex',
-                                                                                    model_location=model_location)
-        elif oslo_datatype_complex.objectUri.startswith('https://schema.org/'):
-            return self.create_block_to_write_from_complex_primitive_or_union_types(oslo_datatype_complex, type_field='Complex',
-                                                                                    model_location=model_location)
-        else:
-            raise NotImplementedError
+        return self.create_block_to_write_from_complex_primitive_or_union_types(
+            oslo_datatype_complex, type_field='Complex', model_location=model_location,
+            valid_uri_and_types=complex_datatype_validation_rules['valid_uri_and_types'])
 
     @staticmethod
     def get_unit_from_constraints(constraints: str) -> str:
         if constraints == '':
             raise ValueError
         split_text = constraints.split('"')
         return split_text[1]
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLEnumerationCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLEnumerationCreator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import re
 from os.path import abspath
 
 import rdflib
 from rdflib import URIRef, Graph
 
 from otlmow_modelbuilder.AbstractDatatypeCreator import AbstractDatatypeCreator
 from otlmow_modelbuilder.GenericBuilderFunctions import get_white_space_equivalent
@@ -32,26 +33,41 @@
     most_recent_graph = None
 
     def __init__(self, oslo_collector: OSLOCollector):
         super().__init__(oslo_collector)
         logging.info("Created an instance of OTLEnumerationCreator")
         self.osloCollector = oslo_collector
 
-    def create_block_to_write_from_enumerations(self, oslo_enumeration: OSLOEnumeration, environment: str = default_environment) -> [str]:
+    def create_block_to_write_from_enumerations(self, oslo_enumeration: OSLOEnumeration, enumeration_validation_rules,
+                                                environment: str = default_environment) -> [str]:
         if not isinstance(oslo_enumeration, OSLOEnumeration):
             raise ValueError(f"Input is not a OSLOEnumeration")
-        if oslo_enumeration.objectUri == '' or not oslo_enumeration.objectUri.startswith(
-                'https://wegenenverkeer.data.vlaanderen.be/ns/'):
+
+        if oslo_enumeration.objectUri == '':
             raise ValueError(f"OSLOEnumeration.objectUri is invalid. Value = '{oslo_enumeration.objectUri}'")
+
+        if oslo_enumeration.objectUri in enumeration_validation_rules['valid_uri_and_types'].keys():
+            pass
+        else:
+            match_re = False
+            for regex in enumeration_validation_rules["valid_regexes"]:
+                match_re = re.match(pattern=regex, string=oslo_enumeration.objectUri)
+                if match_re:
+                    break
+            if not match_re:
+                raise ValueError(
+                    f"OSLOEnumeration.objectUri is invalid. Value = '{oslo_enumeration.objectUri}'")
+
         if oslo_enumeration.name == '':
             raise ValueError(f"OSLOEnumeration.name is invalid. Value = '{oslo_enumeration.name}'")
 
         return self.create_block_to_write_from_enumeration(oslo_enumeration=oslo_enumeration, environment=environment)
 
-    def create_block_to_write_from_enumeration(self, oslo_enumeration: OSLOEnumeration, environment: str = default_environment) -> [str]:
+    def create_block_to_write_from_enumeration(self, oslo_enumeration: OSLOEnumeration,
+                                               environment: str = default_environment) -> [str]:
         keuzelijst_waardes = self.get_keuzelijstwaardes_by_name(oslo_enumeration.name, env=environment)
         adm_status = self.get_adm_status_by_name(oslo_enumeration.name, env=environment)
 
         datablock = ['# coding=utf-8', 'import random',
                      'from otlmow_model.BaseClasses.KeuzelijstField import KeuzelijstField']
         if len(keuzelijst_waardes) > 0:
             datablock.append('from otlmow_model.BaseClasses.KeuzelijstWaarde import KeuzelijstWaarde')
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLModelCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLModelCreator.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import shutil
 from concurrent.futures import FIRST_COMPLETED
 from datetime import datetime
 from os import path
 from pathlib import Path
+from typing import Dict
 
 from tqdm import tqdm
 
 from otlmow_modelbuilder.GenericBuilderFunctions import write_to_file
 from otlmow_modelbuilder.GeometrieArtefactCollector import GeometrieArtefactCollector
 from otlmow_modelbuilder.HelperFunctions import get_ns_and_name_from_uri, get_class_directory_from_ns
 from otlmow_modelbuilder.OTLClassCreator import OTLClassCreator
@@ -22,29 +23,39 @@
 
 class OTLModelCreator:
     def __init__(self, oslo_collector: OSLOCollector, geo_artefact_collector: GeometrieArtefactCollector = None):
         self.oslo_collector = oslo_collector
         self.geo_artefact_collector = geo_artefact_collector
 
     @staticmethod
-    def create_full_model(directory: Path, oslo_collector, geo_artefact_collector, environment: str = ''):
+    def create_full_model(directory: Path, oslo_collector, geo_artefact_collector, settings: Dict, environment: str = ''):
         logging.info('started creating model at ' + datetime.now().strftime("%d/%m/%Y %H:%M:%S"))
         OTLModelCreator.check_and_create_subdirectories(directory)
         oslo_collector.query_correct_base_classes()
-        OTLModelCreator.check_for_nested_attributes_in_classes(collector=oslo_collector)
-        OTLModelCreator.create_primitive_datatypes(directory=directory, oslo_collector=oslo_collector)
-        OTLModelCreator.create_complex_datatypes(directory=directory, oslo_collector=oslo_collector)
-        OTLModelCreator.create_union_datatypes(directory=directory, oslo_collector=oslo_collector)
-        OTLModelCreator.create_enumerations(directory=directory, environment=environment, oslo_collector=oslo_collector)
-        OTLModelCreator.create_classes(directory=directory, oslo_collector=oslo_collector,
-                                       geo_artefact_collector=geo_artefact_collector)
+        OTLModelCreator.check_for_nested_attributes_in_classes(collector=oslo_collector,
+                                                               known_classes_uris=settings['nested_list_class_uris'])
+        OTLModelCreator.create_primitive_datatypes(
+            directory=directory, oslo_collector=oslo_collector,
+            primitive_datatype_validation_rules=settings['primitive_datatype_validation_rules'])
+        OTLModelCreator.create_complex_datatypes(
+            directory=directory, oslo_collector=oslo_collector,
+            complex_datatype_validation_rules=settings['complex_datatype_validation_rules'])
+        OTLModelCreator.create_union_datatypes(
+            directory=directory, oslo_collector=oslo_collector,
+            union_datatype_validation_rules=settings['union_datatype_validation_rules'])
+        OTLModelCreator.create_enumerations(
+            directory=directory, environment=environment, oslo_collector=oslo_collector,
+            enumeration_validation_rules=settings['enumeration_validation_rules'])
+        OTLModelCreator.create_classes(
+            directory=directory, oslo_collector=oslo_collector, geo_artefact_collector=geo_artefact_collector,
+            valid_uri_and_types=settings['complex_datatype_validation_rules']['valid_uri_and_types'])
         logging.info(f'finished creating model in {directory} at ' + datetime.now().strftime("%d/%m/%Y %H:%M:%S"))
 
     @staticmethod
-    def create_primitive_datatypes(directory, oslo_collector):
+    def create_primitive_datatypes(directory, oslo_collector, primitive_datatype_validation_rules):
         creator = OTLPrimitiveDatatypeCreator(oslo_collector)
 
         for prim_datatype in tqdm(oslo_collector.primitive_datatypes):
             if prim_datatype.objectUri in ['http://www.w3.org/2000/01/rdf-schema#Literal',
                                            'http://www.w3.org/2001/XMLSchema#dateTime',
                                            'http://www.w3.org/2001/XMLSchema#integer',
                                            'http://www.w3.org/2001/XMLSchema#decimal',
@@ -55,16 +66,17 @@
                                            'http://www.w3.org/2001/XMLSchema#boolean',
                                            'http://www.w3.org/2001/XMLSchema#anyURI']:
                 logging.info(f"Skip creating class for {prim_datatype.name}")
                 continue
 
             try:
                 model_name = OTLModelCreator.get_model_name_from_directory_path(directory)
-                data_to_write = creator.create_block_to_write_from_primitive_types(prim_datatype,
-                                                                                   model_location=model_name)
+                data_to_write = creator.create_block_to_write_from_primitive_types(
+                    prim_datatype, model_location=model_name,
+                    primitive_datatype_validation_rules=primitive_datatype_validation_rules)
                 if data_to_write is None:
                     logging.info(f"Could not create a class for {prim_datatype.name}")
                     pass
                 if len(data_to_write) == 0:
                     logging.info(f"Could not create a class for {prim_datatype.name}")
                     pass
                 write_to_file(prim_datatype, 'Datatypes', data_to_write, relative_path=directory)
@@ -76,101 +88,109 @@
     def get_model_name_from_directory_path(directory):
         if directory.name == 'TestClasses':
             return directory.parent.name + '.' + directory.name
         else:
             return directory.name
 
     @staticmethod
-    def create_complex_datatypes(directory, oslo_collector):
+    def create_complex_datatypes(directory, oslo_collector, complex_datatype_validation_rules):
         creator = OTLComplexDatatypeCreator(oslo_collector)
 
         for complex_datatype in tqdm(oslo_collector.complex_datatypes):
             try:
                 model_name = OTLModelCreator.get_model_name_from_directory_path(directory)
-                data_to_write = creator.create_block_to_write_from_complex_types(complex_datatype,
-                                                                                 model_location=model_name)
+                data_to_write = creator.create_block_to_write_from_complex_types(
+                    complex_datatype, complex_datatype_validation_rules=complex_datatype_validation_rules,
+                    model_location=model_name)
                 if data_to_write is None:
                     logging.info(f"Could not create a class for {complex_datatype.name}")
                     pass
                 if len(data_to_write) == 0:
                     logging.info(f"Could not create a class for {complex_datatype.name}")
                     pass
                 write_to_file(complex_datatype, 'Datatypes', data_to_write, relative_path=directory)
             except BaseException as e:
                 logging.error(str(e))
                 logging.error(f"Could not create a class for {complex_datatype.name}")
 
     @staticmethod
-    def create_union_datatypes(directory, oslo_collector):
+    def create_union_datatypes(directory, oslo_collector, union_datatype_validation_rules):
         creator = OTLUnionDatatypeCreator(oslo_collector)
 
         for union_datatype in tqdm(oslo_collector.union_datatypes):
             try:
                 model_name = OTLModelCreator.get_model_name_from_directory_path(directory)
-                data_to_write = creator.create_block_to_write_from_union_types(union_datatype,
-                                                                               model_location=model_name)
+                data_to_write = creator.create_block_to_write_from_union_types(
+                    union_datatype, model_location=model_name,
+                    union_datatype_validation_rules=union_datatype_validation_rules)
                 if data_to_write is None:
                     logging.info(f"Could not create a class for {union_datatype.name}")
                     pass
                 if len(data_to_write) == 0:
                     logging.info(f"Could not create a class for {union_datatype.name}")
                     pass
                 write_to_file(union_datatype, 'Datatypes', data_to_write, relative_path=directory)
             except BaseException as e:
                 logging.error(str(e))
                 logging.error(f"Could not create a class for {union_datatype.name}")
 
     @staticmethod
-    def create_enumerations(directory, oslo_collector, environment: str = ''):
+    def create_enumerations(directory, oslo_collector, enumeration_validation_rules, environment: str = ''):
         creator = OTLEnumerationCreator(oslo_collector)
 
         with concurrent.futures.ThreadPoolExecutor() as executor:
             futures = {executor.submit(OTLModelCreator.create_enumeration, creator=creator, directory=directory,
-                                       enumeration=enumeration, environment=environment): enumeration for enumeration in oslo_collector.enumerations}
+                                       enumeration=enumeration, environment=environment,
+                                       enumeration_validation_rules=enumeration_validation_rules): enumeration for
+                       enumeration in oslo_collector.enumerations}
             with tqdm(total=len(futures)) as pbar:
                 while len(futures) > 0:
                     new_futures = {}
                     done, pending = concurrent.futures.wait(futures, return_when=FIRST_COMPLETED, timeout=60)
                     for fut in done:
                         if fut.exception():
                             enumeration = futures[fut]
-                            new_futures[executor.submit(OTLModelCreator.create_enumeration, creator=creator, directory=directory,
-                                           enumeration=enumeration, environment=environment)] = job
+                            new_futures[executor.submit(OTLModelCreator.create_enumeration, creator=creator,
+                                                        directory=directory, enumeration=enumeration,
+                                                        environment=environment,
+                                                        enumeration_validation_rules=enumeration_validation_rules)] = job
                         else:
                             pbar.update()
                     for fut in pending:
                         job = futures[fut]
                         new_futures[fut] = job
                     futures = new_futures
 
     @staticmethod
-    def create_enumeration(creator, directory, enumeration, environment):
+    def create_enumeration(creator, directory, enumeration, environment, enumeration_validation_rules):
         try:
             model_name = OTLModelCreator.get_model_name_from_directory_path(directory)
-            data_to_write = creator.create_block_to_write_from_enumerations(enumeration, environment=environment)
+            data_to_write = creator.create_block_to_write_from_enumerations(
+                enumeration, environment=environment, enumeration_validation_rules=enumeration_validation_rules)
             if data_to_write is None:
                 logging.error(f"Could not create a class for {enumeration.name}")
                 pass
             if len(data_to_write) == 0:
                 logging.error(f"Could not create a class for {enumeration.name}")
                 pass
             write_to_file(enumeration, 'Datatypes', data_to_write, relative_path=directory)
             # logging.info(f"Created a class for {enumeration.name}")
         except BaseException as e:
             logging.error(str(e))
             logging.error(f"Could not create a class for {enumeration.name}")
 
     @staticmethod
-    def create_classes(directory, oslo_collector, geo_artefact_collector):
+    def create_classes(directory, oslo_collector, geo_artefact_collector, valid_uri_and_types):
         creator = OTLClassCreator(oslo_collector, geo_artefact_collector)
 
         for oslo_class in tqdm(oslo_collector.classes):
             try:
                 model_name = OTLModelCreator.get_model_name_from_directory_path(directory)
-                data_to_write = creator.create_blocks_to_write_from_classes(oslo_class, model_location=model_name)
+                data_to_write = creator.create_blocks_to_write_from_classes(oslo_class, model_location=model_name,
+                                                                            valid_uri_and_types=valid_uri_and_types)
                 if data_to_write is None:
                     logging.info(f"Could not create a class for {oslo_class.name}")
                     pass
                 if len(data_to_write) == 0:
                     logging.info(f"Could not create a class for {oslo_class.name}")
                     pass
 
@@ -223,15 +243,18 @@
             dir_path = os.path.join(directory, subdir)
             try:
                 shutil.rmtree(dir_path)
             except Exception as e:
                 print(f'Failed to delete {subdir}. Reason: {e}')
 
     @staticmethod
-    def check_for_nested_attributes_in_classes(collector: OSLOCollector, exceptions=None):
+    def check_for_nested_attributes_in_classes(collector: OSLOCollector, exceptions=None,
+                                               known_classes_uris: [str] = None):
+        if known_classes_uris is None:
+            known_classes_uris = []
         if exceptions is None:
             exceptions = [
                 'https://wegenenverkeer.data.vlaanderen.be/ns/onderdeel#AllCasesTestClass.testComplexTypeMetKard']
         for cl in collector.classes:
             if cl.abstract:
                 continue
 
@@ -249,16 +272,15 @@
                 if len(nested_attrs) == 0:
                     nested_attrs = collector.find_union_datatype_attributes_by_class_uri(attr.type)
 
                 if len(nested_attrs) > 1:
                     try:
                         OTLModelCreator.check_for_nested_attributes_in_attributes(list_found, nested_attrs, collector)
                     except NotImplementedError as exc:
-                        if cl.objectUri not in ['http://purl.org/dc/terms/Agent',
-                                                'https://wegenenverkeer.data.vlaanderen.be/ns/onderdeel#HeeftBetrokkene']:
+                        if cl.objectUri not in known_classes_uris:
                             raise NotImplementedError(f'found in {cl.objectUri} {attr.objectUri}') from exc
 
     @staticmethod
     def check_for_nested_attributes_in_attributes(list_already_found, attributes, collector):
         for attr in attributes:
             list_found = False
             if attr.kardinaliteit_max != '1':
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/OTLUnionDatatypeCreator.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/OTLUnionDatatypeCreator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 import logging
+import re
+from typing import Dict
 
 from otlmow_modelbuilder.AbstractDatatypeCreator import AbstractDatatypeCreator
 from otlmow_modelbuilder.SQLDataClasses.OSLOCollector import OSLOCollector
 from otlmow_modelbuilder.SQLDataClasses.OSLODatatypeUnion import OSLODatatypeUnion
 
 
 class OTLUnionDatatypeCreator(AbstractDatatypeCreator):
     def __init__(self, oslo_collector: OSLOCollector):
         super().__init__(oslo_collector)
         logging.info("Created an instance of OTLUnionDatatypeCreator")
 
     def create_block_to_write_from_union_types(self, union_datatype: OSLODatatypeUnion,
-                                               model_location: str = '') -> [str]:
+                                               union_datatype_validation_rules: Dict, model_location: str = '') -> [str]:
         if not isinstance(union_datatype, OSLODatatypeUnion):
             raise ValueError(f"Input is not a OSLODatatypeUnion")
 
-        if union_datatype.objectUri == '' or not (union_datatype.objectUri.startswith(
-                'https://wegenenverkeer.data.vlaanderen.be/ns/') and 'Dtu' in union_datatype.objectUri):
+        if union_datatype.objectUri == '':
             raise ValueError(f"OSLODatatypeUnion.objectUri is invalid. Value = '{union_datatype.objectUri}'")
 
+        if union_datatype.objectUri in union_datatype_validation_rules['valid_uri_and_types'].keys():
+            pass
+        else:
+            match_re = False
+            for regex in union_datatype_validation_rules["valid_regexes"]:
+                match_re = re.match(pattern=regex, string=union_datatype.objectUri)
+                if match_re:
+                    break
+            if not match_re:
+                raise ValueError(
+                    f"OSLODatatypeUnion.objectUri is invalid. Value = '{union_datatype.objectUri}'")
+
         if union_datatype.name == '':
             raise ValueError(f"OSLODatatypeUnion.name is invalid. Value = '{union_datatype.name}'")
 
         return self.create_block_to_write_from_complex_primitive_or_union_types(oslo_datatype=union_datatype,
                                                                                 type_field='UnionType',
                                                                                 model_location=model_location)
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDataClasses/OSLOCollector.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDataClasses/OSLOCollector.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder/SQLDbReader.py` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder/SQLDbReader.py`

 * *Files identical despite different names*

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/PKG-INFO` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otlmow-modelbuilder
-Version: 0.6
+Version: 0.7
 Author-email: David Vlaminck <david.vlaminck@mow.vlaanderen.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `otlmow_modelbuilder-0.6/otlmow_modelbuilder.egg-info/SOURCES.txt` & `otlmow_modelbuilder-0.7/otlmow_modelbuilder.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 otlmow_modelbuilder/OTLClassCreator.py
 otlmow_modelbuilder/OTLComplexDatatypeCreator.py
 otlmow_modelbuilder/OTLEnumerationCreator.py
 otlmow_modelbuilder/OTLModelCreator.py
 otlmow_modelbuilder/OTLPrimitiveDatatypeCreator.py
 otlmow_modelbuilder/OTLUnionDatatypeCreator.py
 otlmow_modelbuilder/SQLDbReader.py
+otlmow_modelbuilder/SettingsManager.py
 otlmow_modelbuilder/__init__.py
 otlmow_modelbuilder/main.py
 otlmow_modelbuilder.egg-info/PKG-INFO
 otlmow_modelbuilder.egg-info/SOURCES.txt
 otlmow_modelbuilder.egg-info/dependency_links.txt
 otlmow_modelbuilder.egg-info/requires.txt
 otlmow_modelbuilder.egg-info/top_level.txt
```

### Comparing `otlmow_modelbuilder-0.6/pyproject.toml` & `otlmow_modelbuilder-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otlmow_modelbuilder"
-version = "0.6"
+version = "0.7"
 authors = [{name = "David Vlaminck", email = "david.vlaminck@mow.vlaanderen.be"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

