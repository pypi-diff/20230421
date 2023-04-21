# Comparing `tmp/uniprot-id-mapper-1.0.2.tar.gz` & `tmp/uniprot-id-mapper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniprot-id-mapper-1.0.2.tar", last modified: Fri Apr 21 10:08:19 2023, max compression
+gzip compressed data, was "uniprot-id-mapper-1.0.3.tar", last modified: Fri Apr 21 11:10:50 2023, max compression
```

## Comparing `uniprot-id-mapper-1.0.2.tar` & `uniprot-id-mapper-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.2/LICENSE
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.2/MANIFEST.in
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9418 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     7223 2023-04-21 10:05:22.000000 uniprot-id-mapper-1.0.2/README.md
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1650 2023-04-21 10:04:50.000000 uniprot-id-mapper-1.0.2/pyproject.toml
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/setup.cfg
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/UniProtMapper/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      315 2023-03-17 13:30:05.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/__init__.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9230 2023-04-21 10:00:21.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10830 2023-04-19 17:20:48.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/interface.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_mapping_dbs.json
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_return_fields.csv
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9328 2023-04-21 10:01:31.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/swiss_parser.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4258 2023-04-21 10:03:15.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/utils.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       92 2023-04-21 10:04:41.000000 uniprot-id-mapper-1.0.2/src/UniProtMapper/version.py
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9418 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/PKG-INFO
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      744 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/requires.txt
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-04-21 10:08:19.000000 uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 10:08:19.737983 uniprot-id-mapper-1.0.2/tests/
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.2/tests/test_field_retriever_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.2/tests/test_id_mapping_api.py
--rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1070 2023-02-28 11:23:59.000000 uniprot-id-mapper-1.0.3/LICENSE
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       86 2023-03-17 12:50:04.000000 uniprot-id-mapper-1.0.3/MANIFEST.in
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10089 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     7893 2023-04-21 11:09:52.000000 uniprot-id-mapper-1.0.3/README.md
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1650 2023-04-21 11:07:13.000000 uniprot-id-mapper-1.0.3/pyproject.toml
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       38 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/setup.cfg
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.517283 uniprot-id-mapper-1.0.3/src/
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/UniProtMapper/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      315 2023-03-17 13:30:05.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/__init__.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9230 2023-04-21 10:00:21.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10510 2023-04-21 11:02:17.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     5134 2023-04-19 17:23:14.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/interface.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)   105497 2023-03-01 13:45:43.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2752 2023-03-14 14:33:07.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_mapping_dbs.json
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    18362 2023-04-19 15:52:45.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_return_fields.csv
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     9328 2023-04-21 10:01:31.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/swiss_parser.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     4258 2023-04-21 10:03:15.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/utils.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       92 2023-04-21 11:06:59.000000 uniprot-id-mapper-1.0.3/src/UniProtMapper/version.py
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)    10089 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)      744 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)        1 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       50 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/requires.txt
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)       14 2023-04-21 11:10:50.000000 uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 davidararipe  (1000) davidararipe  (1000)        0 2023-04-21 11:10:50.527283 uniprot-id-mapper-1.0.3/tests/
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2256 2023-04-19 17:44:47.000000 uniprot-id-mapper-1.0.3/tests/test_field_retriever_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     2955 2023-04-19 18:49:12.000000 uniprot-id-mapper-1.0.3/tests/test_id_mapping_api.py
+-rw-r--r--   0 davidararipe  (1000) davidararipe  (1000)     1862 2023-04-19 17:45:00.000000 uniprot-id-mapper-1.0.3/tests/test_utils.py
```

### Comparing `uniprot-id-mapper-1.0.2/LICENSE` & `uniprot-id-mapper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/PKG-INFO` & `uniprot-id-mapper-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -43,14 +43,15 @@
 License-File: LICENSE
 
 [![Linting Ruff](https://img.shields.io/badge/Linting%20-Ruff-red?style=flat-square)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
+[![Downloads:PyPI](https://img.shields.io/pypi/dm/uniprot-id-mapper?style=flat-square)](https://pypi.org/project/uniprot-id-mapper/)
 
 # UniProtMapper
 
 A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
@@ -116,15 +117,14 @@
 
 </summary>
 <details>
 
 This class supports retrieving any of the UniProt [return fields](https://www.uniprot.org/help/return_fields). The user can access these directly from the object, under the attribute `self.fields_table`, e.g.:
 
 ```Python
-import pandas as pd
 from UniProtMapper import UniProtRetriever
 
 field_retriever = UniProtRetriever()
 df = field_retriever.fields_table
 df.head()
 ```
 |    | Label                | Legacy Returned Field   | Returned Field   | Field Type       |
@@ -167,15 +167,15 @@
 Retrieving json UniProt-SwissProt (reviewed) responses is also possible, such as the following:
 
 ``` Python
 result, failed = mapper(
     ids=["P30542", "Q16678", "Q02880"], from_db="UniProtKB_AC-ID", to_db="UniProtKB-Swiss-Prot"
 )
 
-print(result[0])
+print(result.loc[0, 'to'])
 >>> {'from': 'P30542',
 >>>  'to': {'entryType': 'UniProtKB reviewed (Swiss-Prot)',
 >>>   'primaryAccession': 'P30542',
 >>> ...
 >>>     'Beta strand': 2,
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
@@ -185,15 +185,15 @@
 
 ``` Python
 from UniProtMapper import SwissProtParser
 
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
-parser(result[0]['to'])
+parser(result.loc[0, 'to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
 >>>  'cellLocation': 'Cell membrane',
 >>>  'GO_crossref': ['GO:0030673~GoTerm~C:axolemma',
 >>>   'GO:0030673~GoEvidenceType~IEA:Ensembl',
 >>> ...
@@ -211,28 +211,54 @@
     ids=["P30542", "Q16678", "Q02880"],
     from_db="UniProtKB_AC-ID",
     to_db="UniProtKB-Swiss-Prot",
     parser=parser,
 )
 ```
 </details>
-<!-- 
-This functionality needs to be improved
 
-### Mapping identifiers to orthologs
+<summary>
+
+## Mapping identifiers to orthologs
 
-This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt.
+</summary>
+<details>
 
-The user can also specify which information fields to retrieve with the parameters `uniprot_info` and `crossref_dbs`. Leaving those as default will retrieve all supported UniProt information and no cross-references.
+This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt. Desired fields to retrieve using `SwissProtParser` can be specified with the parameters `uniprot_info` and `crossref_dbs`.
 
 Queried objects are in the column `original_id` and their OrthoDB identifier is found on `orthodb_id`.
 ``` Python
+from UniProtMapper import UniProtIDMapper
+
 mapper = UniProtIDMapper()
-result, failed = mapper.uniprot_ids_to_orthologs(
+result, failed = mapper.uniprotIDsToOrthologs(
     ids=["P30542", "Q16678", "Q02880"], organism="Mus musculus"
 )
 
 # Fetched results contain all retrieved species.
 # Filtering by organism is done on the full response.
 >>> Fetched: 3 / 3
->>> Fetched: 349 / 349
+>>> Fetched: 246 / 246
 ```
+
+Alternatively, OrthoDB IDs can be obtained using UniProtIDMapper, and used to retrieve any of the desired UniProt return fields using UniProtRetriever.
+
+``` Python
+from UniProtMapper import UniProtIDMapper, UniProtRetriever
+
+mapper = UniProtIDMapper()
+result, failed = mapper(
+    ids=["P30542", "Q16678", "Q02880"],
+    from_db="UniProtKB_AC-ID",
+    to_db="OrthoDB",
+)
+field_retriever = UniProtRetriever()
+ortho_results, failed = field_retriever.retrieveFields(
+    ids=result["to"].tolist(), from_db="OrthoDB"
+)
+
+>>> Retrying in 3s
+>>> Fetched: 3 / 3
+>>> Retrying in 3s
+>>> Fetched: 246 / 246
+```
+</details>
```

### Comparing `uniprot-id-mapper-1.0.2/README.md` & `uniprot-id-mapper-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![Linting Ruff](https://img.shields.io/badge/Linting%20-Ruff-red?style=flat-square)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
+[![Downloads:PyPI](https://img.shields.io/pypi/dm/uniprot-id-mapper?style=flat-square)](https://pypi.org/project/uniprot-id-mapper/)
 
 # UniProtMapper
 
 A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
@@ -72,15 +73,14 @@
 
 </summary>
 <details>
 
 This class supports retrieving any of the UniProt [return fields](https://www.uniprot.org/help/return_fields). The user can access these directly from the object, under the attribute `self.fields_table`, e.g.:
 
 ```Python
-import pandas as pd
 from UniProtMapper import UniProtRetriever
 
 field_retriever = UniProtRetriever()
 df = field_retriever.fields_table
 df.head()
 ```
 |    | Label                | Legacy Returned Field   | Returned Field   | Field Type       |
@@ -123,15 +123,15 @@
 Retrieving json UniProt-SwissProt (reviewed) responses is also possible, such as the following:
 
 ``` Python
 result, failed = mapper(
     ids=["P30542", "Q16678", "Q02880"], from_db="UniProtKB_AC-ID", to_db="UniProtKB-Swiss-Prot"
 )
 
-print(result[0])
+print(result.loc[0, 'to'])
 >>> {'from': 'P30542',
 >>>  'to': {'entryType': 'UniProtKB reviewed (Swiss-Prot)',
 >>>   'primaryAccession': 'P30542',
 >>> ...
 >>>     'Beta strand': 2,
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
@@ -141,15 +141,15 @@
 
 ``` Python
 from UniProtMapper import SwissProtParser
 
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
-parser(result[0]['to'])
+parser(result.loc[0, 'to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
 >>>  'cellLocation': 'Cell membrane',
 >>>  'GO_crossref': ['GO:0030673~GoTerm~C:axolemma',
 >>>   'GO:0030673~GoEvidenceType~IEA:Ensembl',
 >>> ...
@@ -167,28 +167,54 @@
     ids=["P30542", "Q16678", "Q02880"],
     from_db="UniProtKB_AC-ID",
     to_db="UniProtKB-Swiss-Prot",
     parser=parser,
 )
 ```
 </details>
-<!-- 
-This functionality needs to be improved
 
-### Mapping identifiers to orthologs
+<summary>
+
+## Mapping identifiers to orthologs
 
-This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt.
+</summary>
+<details>
 
-The user can also specify which information fields to retrieve with the parameters `uniprot_info` and `crossref_dbs`. Leaving those as default will retrieve all supported UniProt information and no cross-references.
+This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt. Desired fields to retrieve using `SwissProtParser` can be specified with the parameters `uniprot_info` and `crossref_dbs`.
 
 Queried objects are in the column `original_id` and their OrthoDB identifier is found on `orthodb_id`.
 ``` Python
+from UniProtMapper import UniProtIDMapper
+
 mapper = UniProtIDMapper()
-result, failed = mapper.uniprot_ids_to_orthologs(
+result, failed = mapper.uniprotIDsToOrthologs(
     ids=["P30542", "Q16678", "Q02880"], organism="Mus musculus"
 )
 
 # Fetched results contain all retrieved species.
 # Filtering by organism is done on the full response.
 >>> Fetched: 3 / 3
->>> Fetched: 349 / 349
+>>> Fetched: 246 / 246
+```
+
+Alternatively, OrthoDB IDs can be obtained using UniProtIDMapper, and used to retrieve any of the desired UniProt return fields using UniProtRetriever.
+
+``` Python
+from UniProtMapper import UniProtIDMapper, UniProtRetriever
+
+mapper = UniProtIDMapper()
+result, failed = mapper(
+    ids=["P30542", "Q16678", "Q02880"],
+    from_db="UniProtKB_AC-ID",
+    to_db="OrthoDB",
+)
+field_retriever = UniProtRetriever()
+ortho_results, failed = field_retriever.retrieveFields(
+    ids=result["to"].tolist(), from_db="OrthoDB"
+)
+
+>>> Retrying in 3s
+>>> Fetched: 3 / 3
+>>> Retrying in 3s
+>>> Fetched: 246 / 246
 ```
+</details>
```

### Comparing `uniprot-id-mapper-1.0.2/pyproject.toml` & `uniprot-id-mapper-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uniprot-id-mapper"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Python wrapper for the UniProt Mapping RESTful API."
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["uniprot", "database", "protein ID", "gene ID", "parser"]
 authors = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
 maintainers = [{ name = "David Araripe", email = "david.araripe17@gmail.com" }]
```

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/field_retriever_api.py` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/field_retriever_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/id_mapping_api.py` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/id_mapping_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -206,15 +206,15 @@
                 all_dfs.append(df)
                 failed_ids = failed_ids + failed
             df = pd.concat(all_dfs, ignore_index=True) if all_dfs else pd.DataFrame()
             return df, failed_ids
         else:
             return _get_results(ids)
 
-    def uniprot_ids_to_orthologs(
+    def uniprotIDsToOrthologs(
         self,
         ids: Union[List[str], str],
         organism: Optional[List[str]] = None,
         uniprot_info: Optional[list] = None,
         crossref_dbs: Optional[list] = None,
         case: bool = False,
     ) -> Tuple[pd.DataFrame, dict]:
@@ -243,33 +243,26 @@
                 pass
             elif isinstance(organism, list):
                 organism = "|".join(organism)
             else:
                 raise ValueError("organism must be a string or a list of strings.")
 
         case = case
-        to_ortho_r, failed_r = self.uniprot_id_mapping(ids, to_db="OrthoDB")
+        to_ortho_r, failed_r = self.mapIDs(ids, to_db="OrthoDB")
 
-        ortho_mapping = {
-            to_ortho_r[idx]["to"]: to_ortho_r[idx]["from"]
-            for idx in range(len(to_ortho_r))
-        }
+        ortho_mapping = dict(zip(to_ortho_r["to"], to_ortho_r["from"]))
 
-        ortho_ids = [to_ortho_r[k]["to"] for k in to_ortho_r]
         parser = SwissProtParser(toquery=uniprot_info, crossrefs=crossref_dbs)
-        ortho_r, failed_r = self.uniprot_id_mapping(
-            ortho_ids, from_db="OrthoDB", parser=parser
+        ortho_df, failed_r = self.mapIDs(
+            to_ortho_r["to"].tolist(), from_db="OrthoDB", parser=parser
         )
-        for idx in ortho_r.keys():
-            ortho_r[idx].update({"orthodb_id": ortho_r[idx]["from"]})
-            ortho_r[idx].update({"original_id": ortho_mapping[ortho_r[idx]["from"]]})
-        parsed_df = pd.DataFrame.from_dict(ortho_r, orient="index")
+        ortho_df = ortho_df.assign(original_id=ortho_df["from"].map(ortho_mapping))
 
         if organism is not None:
-            parsed_df = parsed_df.query(
+            ortho_df = ortho_df.query(
                 "organism.str.contains(@organism, regex=True, case=@case)"
             ).reset_index(drop=True)
 
         queried_arr = np.array(ids)
-        retrieved = parsed_df["original_id"].unique()
+        retrieved = ortho_df["original_id"].unique()
         failed = np.compress(~np.isin(queried_arr, retrieved), queried_arr).tolist()
-        return parsed_df, failed
+        return ortho_df, failed
```

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/interface.py` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/interface.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_abbrev_crossrefs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_mapping_dbs.json` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_mapping_dbs.json`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/resources/uniprot_return_fields.csv` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/resources/uniprot_return_fields.csv`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/swiss_parser.py` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/swiss_parser.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/UniProtMapper/utils.py` & `uniprot-id-mapper-1.0.3/src/UniProtMapper/utils.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/PKG-INFO` & `uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniprot-id-mapper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the UniProt Mapping RESTful API.
 Author-email: David Araripe <david.araripe17@gmail.com>
 Maintainer-email: David Araripe <david.araripe17@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 David Araripe
         
@@ -43,14 +43,15 @@
 License-File: LICENSE
 
 [![Linting Ruff](https://img.shields.io/badge/Linting%20-Ruff-red?style=flat-square)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](https://opensource.org/licenses/MIT)
 [![GitHub Actions](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDavid-Araripe%2FUniProtMapper%2Fbadge%3Fref%3Dmaster&style=flat-square)](https://actions-badge.atrox.dev/David-Araripe/UniProtMapper/goto?ref=master)
+[![Downloads:PyPI](https://img.shields.io/pypi/dm/uniprot-id-mapper?style=flat-square)](https://pypi.org/project/uniprot-id-mapper/)
 
 # UniProtMapper
 
 A (unofficial) Python wrapper for the [UniProt Retrieve/ID Mapping](https://www.uniprot.org/id-mapping) RESTful API. This package supports the following functionalities:
 
 - Map UniProt IDs other identifiers (handled by [UniProtIDMapper](#uniprotidmapper));
 - Retrieve any of the supported [return fields](https://www.uniprot.org/help/return_fields) (handled by [UniprotRetriever](#uniprotretriever))
@@ -116,15 +117,14 @@
 
 </summary>
 <details>
 
 This class supports retrieving any of the UniProt [return fields](https://www.uniprot.org/help/return_fields). The user can access these directly from the object, under the attribute `self.fields_table`, e.g.:
 
 ```Python
-import pandas as pd
 from UniProtMapper import UniProtRetriever
 
 field_retriever = UniProtRetriever()
 df = field_retriever.fields_table
 df.head()
 ```
 |    | Label                | Legacy Returned Field   | Returned Field   | Field Type       |
@@ -167,15 +167,15 @@
 Retrieving json UniProt-SwissProt (reviewed) responses is also possible, such as the following:
 
 ``` Python
 result, failed = mapper(
     ids=["P30542", "Q16678", "Q02880"], from_db="UniProtKB_AC-ID", to_db="UniProtKB-Swiss-Prot"
 )
 
-print(result[0])
+print(result.loc[0, 'to'])
 >>> {'from': 'P30542',
 >>>  'to': {'entryType': 'UniProtKB reviewed (Swiss-Prot)',
 >>>   'primaryAccession': 'P30542',
 >>> ...
 >>>     'Beta strand': 2,
 >>>     'Turn': 1},
 >>>    'uniParcId': 'UPI00000503E1'}}}
@@ -185,15 +185,15 @@
 
 ``` Python
 from UniProtMapper import SwissProtParser
 
 parser = SwissProtParser(
     toquery=["organism", "tissueExpression", "cellLocation"], crossrefs=["GO"]
 )
-parser(result[0]['to'])
+parser(result.loc[0, 'to'])
 
 >>> {'organism': 'Homo sapiens',
 >>>  'tissueExpression': '',
 >>>  'cellLocation': 'Cell membrane',
 >>>  'GO_crossref': ['GO:0030673~GoTerm~C:axolemma',
 >>>   'GO:0030673~GoEvidenceType~IEA:Ensembl',
 >>> ...
@@ -211,28 +211,54 @@
     ids=["P30542", "Q16678", "Q02880"],
     from_db="UniProtKB_AC-ID",
     to_db="UniProtKB-Swiss-Prot",
     parser=parser,
 )
 ```
 </details>
-<!-- 
-This functionality needs to be improved
 
-### Mapping identifiers to orthologs
+<summary>
+
+## Mapping identifiers to orthologs
 
-This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt.
+</summary>
+<details>
 
-The user can also specify which information fields to retrieve with the parameters `uniprot_info` and `crossref_dbs`. Leaving those as default will retrieve all supported UniProt information and no cross-references.
+This package also allows mapping UniProt IDs to orthologs. The function `uniprot_ids_to_orthologs` does that by mapping UniProt IDs to OrthoDB and then re-mapping these results to UniProt-SwissProt. Desired fields to retrieve using `SwissProtParser` can be specified with the parameters `uniprot_info` and `crossref_dbs`.
 
 Queried objects are in the column `original_id` and their OrthoDB identifier is found on `orthodb_id`.
 ``` Python
+from UniProtMapper import UniProtIDMapper
+
 mapper = UniProtIDMapper()
-result, failed = mapper.uniprot_ids_to_orthologs(
+result, failed = mapper.uniprotIDsToOrthologs(
     ids=["P30542", "Q16678", "Q02880"], organism="Mus musculus"
 )
 
 # Fetched results contain all retrieved species.
 # Filtering by organism is done on the full response.
 >>> Fetched: 3 / 3
->>> Fetched: 349 / 349
+>>> Fetched: 246 / 246
 ```
+
+Alternatively, OrthoDB IDs can be obtained using UniProtIDMapper, and used to retrieve any of the desired UniProt return fields using UniProtRetriever.
+
+``` Python
+from UniProtMapper import UniProtIDMapper, UniProtRetriever
+
+mapper = UniProtIDMapper()
+result, failed = mapper(
+    ids=["P30542", "Q16678", "Q02880"],
+    from_db="UniProtKB_AC-ID",
+    to_db="OrthoDB",
+)
+field_retriever = UniProtRetriever()
+ortho_results, failed = field_retriever.retrieveFields(
+    ids=result["to"].tolist(), from_db="OrthoDB"
+)
+
+>>> Retrying in 3s
+>>> Fetched: 3 / 3
+>>> Retrying in 3s
+>>> Fetched: 246 / 246
+```
+</details>
```

### Comparing `uniprot-id-mapper-1.0.2/src/uniprot_id_mapper.egg-info/SOURCES.txt` & `uniprot-id-mapper-1.0.3/src/uniprot_id_mapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/tests/test_field_retriever_api.py` & `uniprot-id-mapper-1.0.3/tests/test_field_retriever_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/tests/test_id_mapping_api.py` & `uniprot-id-mapper-1.0.3/tests/test_id_mapping_api.py`

 * *Files identical despite different names*

### Comparing `uniprot-id-mapper-1.0.2/tests/test_utils.py` & `uniprot-id-mapper-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

