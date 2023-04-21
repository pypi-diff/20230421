# Comparing `tmp/uniprot-id-mapper-1.0.1.tar.gz` & `tmp/uniprot-id-mapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniprot-id-mapper-1.0.1.tar", last modified: Thu Apr 20 12:36:41 2023, max compression
+gzip compressed data, was "uniprot-id-mapper-1.0.2.tar", last modified: Fri Apr 21 10:08:19 2023, max compression
```

## Comparing `uniprot-id-mapper-1.0.1.tar` & `uniprot-id-mapper-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.1/LICENSE
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.1/MANIFEST.in
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9378 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     7183 2023-04-20 12:29:44.000000 uniprot-id-mapper-1.0.1/README.md
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1650 2023-04-20 12:29:14.000000 uniprot-id-mapper-1.0.1/pyproject.toml
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/setup.cfg
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/src/
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/src/UniProtMapper/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      315 2023-03-17 13:30:05.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/__init__.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9119 2023-04-19 17:20:39.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10830 2023-04-19 17:20:48.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/interface.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_mapping_dbs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_return_fields.csv
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9330 2023-03-15 16:24:01.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/swiss_parser.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4269 2023-03-15 15:09:21.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/utils.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       93 2023-04-20 12:28:29.000000 uniprot-id-mapper-1.0.1/src/UniProtMapper/version.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9378 2023-04-20 12:36:41.000000 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      744 2023-04-20 12:36:41.000000 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-04-20 12:36:41.000000 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-04-20 12:36:41.000000 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/requires.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-04-20 12:36:41.000000 uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-20 12:36:41.606382 uniprot-id-mapper-1.0.1/tests/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.1/tests/test_field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.1/tests/test_id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.2/LICENSE
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.2/MANIFEST.in
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9418 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     7223 2023-04-21 10:05:22.000000 uniprot-id-mapper-1.0.2/README.md
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1650 2023-04-21 10:04:50.000000 uniprot-id-mapper-1.0.2/pyproject.toml
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/setup.cfg
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/UniProtMapper/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      315 2023-03-17 13:30:05.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/__init__.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9230 2023-04-21 10:00:21.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10830 2023-04-19 17:20:48.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/interface.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_mapping_dbs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_return_fields.csv
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9328 2023-04-21 10:01:31.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/swiss_parser.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4258 2023-04-21 10:03:15.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/utils.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       92 2023-04-21 10:04:41.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/version.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9418 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      744 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/requires.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/tests/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.2/tests/test_field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.2/tests/test_id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.2/tests/test_utils.py
```

### Comparing `uniprot-id-mapper-1.0.1/LICENSE` & `uniprot-id-mapper-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/PKG-INFO` & `uniprot-id-mapper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -46,15 +46,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
 
 # UniProtMapper
 
-An (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
+A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
@@ -76,15 +76,15 @@
 ## UniProtIDMapper
 
 </summary>
 <details>
 
 Supported databases and their respective type are stored under the attribute `self.supported_dbs_with_types`. These are also found as a list under `self._supported_fields`.
 ``` Python
-from UniProtIDMapper import UniProtIDMapper
+from UniProtMapper import UniProtIDMapper
 
 mapper = UniProtIDMapper()
 print(mapper.supported_dbs_with_types)
 ```
 
 To map a list of UniProt IDs to Ensembl IDs, the user can either call the object directly or use the `mapID` method.
 ``` Python
@@ -180,14 +180,16 @@
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
 ```
 
 SwissProt responses from `UniProtIDMapper` can be parsed using the `SwissProtParser` class, where the fields to extract from UniProt (:param: = toquery) are stored under `self._supported_fields` and the cross-referenced datasets are stored under `self._crossref_dbs` (:param: = crossrefs).
 
 ``` Python
+from UniProtMapper import SwissProtParser
+
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
 parser(result[0]['to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
```

### Comparing `uniprot-id-mapper-1.0.1/README.md` & `uniprot-id-mapper-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
 
 # UniProtMapper
 
-An (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
+A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
@@ -32,15 +32,15 @@
 ## UniProtIDMapper
 
 </summary>
 <details>
 
 Supported databases and their respective type are stored under the attribute `self.supported_dbs_with_types`. These are also found as a list under `self._supported_fields`.
 ``` Python
-from UniProtIDMapper import UniProtIDMapper
+from UniProtMapper import UniProtIDMapper
 
 mapper = UniProtIDMapper()
 print(mapper.supported_dbs_with_types)
 ```
 
 To map a list of UniProt IDs to Ensembl IDs, the user can either call the object directly or use the `mapID` method.
 ``` Python
@@ -136,14 +136,16 @@
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
 ```
 
 SwissProt responses from `UniProtIDMapper` can be parsed using the `SwissProtParser` class, where the fields to extract from UniProt (:param: = toquery) are stored under `self._supported_fields` and the cross-referenced datasets are stored under `self._crossref_dbs` (:param: = crossrefs).
 
 ``` Python
+from UniProtMapper import SwissProtParser
+
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
 parser(result[0]['to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
```

### Comparing `uniprot-id-mapper-1.0.1/pyproject.toml` & `uniprot-id-mapper-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniprot-id-mapper"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Python wrapper for the UniProt Mapping RESTful API."
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["uniprot", "database", "protein ID", "gene ID", "parser"]
 authors = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
 maintainers = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
```

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/field_retriever_api.py` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/field_retriever_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 import requests
 
 from UniProtMapper.interface import abc_UniProtAPI
 from UniProtMapper.utils import decode_results, divide_batches, print_progress_batches
 
 
 class UniProtRetriever(abc_UniProtAPI):
-    """Class for retrieving specific UniProt fields.
+    """Class for retrieving specific UniProt return fields. For the available fields,
+    check `self.fields_table` or https://www.uniprot.org/help/return_fields.
 
     Returns:
-        Tuple[pd.DataFrame, list]: A tuple containing a dataframe with the results
+        Tuple[pd.DataFrame, list]: A tuple containing a data frame with the results
         and a list of IDs that were not found.
 
     Example:
     >>> uni_retriever = UniProtRetriever()
     >>> result_df, failed = uni_retriever(["P30542", "Q16678", "Q02880"],
     >>>                                   fields=["accession", "id", "go_id",
     >>>                                           "go_p", "go_c", "go_f"])
```

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/id_mapping_api.py` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/id_mapping_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/interface.py` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/interface.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_mapping_dbs.json` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_mapping_dbs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/resources/uniprot_return_fields.csv` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_return_fields.csv`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/swiss_parser.py` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/swiss_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
+"""Module for parsing UniProtKB-Swiss-Prot json responses."""
+
 import json
 from collections import defaultdict
 
 import numpy as np
 import pkg_resources
 
 from .utils import (
     flatten_list_getunique,
     search_comments,
     search_keys_inlist,
     search_uniprot_crossrefs,
 )
 
-"""
-Module for parsing UniProtKB-Swiss-Prot json responses.
-"""
-
 
 class SwissProtParser:
     """Retrieve specified information UniProtKB-Swiss-Prot json response."""
 
     def __init__(self, toquery: list = None, crossrefs: list = None) -> None:
         """Initialize the class with the information to be retrieved
         and the crossreferences to be searched.
```

### Comparing `uniprot-id-mapper-1.0.1/src/UniProtMapper/utils.py` & `uniprot-id-mapper-1.0.2/src/UniProtMapper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # -*- coding: utf-8 -*-
+"""Module with utility functions for UniProtMapper and SwissProtParser."""
 import json
 import re
 import zlib
 from typing import List
 from xml.etree import ElementTree
 
 import numpy as np
 
-"""
-Module with utility functions for UniProtMapper and SwissProtParser.
-"""
-
 
 def search_keys_inlist(list_of_dicts: List[dict], desiredkey: str):
     for diction in list_of_dicts:
         if desiredkey in diction:
             return diction[desiredkey]
     return ""
 
@@ -115,12 +112,12 @@
     return ElementTree.tostring(merged_root, encoding="utf-8", xml_declaration=True)
 
 
 def print_progress_batches(batch_index, size, retrieved, failed):
     """Prints the progress of a batch process."""
     n_fetched = min((batch_index + 1) * size, retrieved)
     print(f"Fetched: {n_fetched} / {retrieved + failed}")
-    
-    
+
+
 def divide_batches(ids):
     """Divides a list of UniProtIDs into batches of 500"""
     return [ids[i : i + 500] for i in range(0, len(ids), 500)]
```

### Comparing `uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/PKG-INFO` & `uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -46,15 +46,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
 
 # UniProtMapper
 
-An (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
+A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
 - Parse json UniProt-SwissProt responses (handled by [SwissProtParser](#swissprotparser)).
 
 ## Installation
 
@@ -76,15 +76,15 @@
 ## UniProtIDMapper
 
 </summary>
 <details>
 
 Supported databases and their respective type are stored under the attribute `self.supported_dbs_with_types`. These are also found as a list under `self._supported_fields`.
 ``` Python
-from UniProtIDMapper import UniProtIDMapper
+from UniProtMapper import UniProtIDMapper
 
 mapper = UniProtIDMapper()
 print(mapper.supported_dbs_with_types)
 ```
 
 To map a list of UniProt IDs to Ensembl IDs, the user can either call the object directly or use the `mapID` method.
 ``` Python
@@ -180,14 +180,16 @@
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
 ```
 
 SwissProt responses from `UniProtIDMapper` can be parsed using the `SwissProtParser` class, where the fields to extract from UniProt (:param: = toquery) are stored under `self._supported_fields` and the cross-referenced datasets are stored under `self._crossref_dbs` (:param: = crossrefs).
 
 ``` Python
+from UniProtMapper import SwissProtParser
+
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
 parser(result[0]['to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
```

### Comparing `uniprot-id-mapper-1.0.1/src/uniprot_id_mapper.egg-info/SOURCES.txt` & `uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/tests/test_field_retriever_api.py` & `uniprot-id-mapper-1.0.2/tests/test_field_retriever_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/tests/test_id_mapping_api.py` & `uniprot-id-mapper-1.0.2/tests/test_id_mapping_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.1/tests/test_utils.py` & `uniprot-id-mapper-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

