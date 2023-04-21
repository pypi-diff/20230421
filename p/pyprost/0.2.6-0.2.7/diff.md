# Comparing `tmp/pyprost-0.2.6.tar.gz` & `tmp/pyprost-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprost-0.2.6.tar", last modified: Wed Dec  7 21:02:31 2022, max compression
+gzip compressed data, was "pyprost-0.2.7.tar", last modified: Fri Apr 21 00:42:24 2023, max compression
```

## Comparing `pyprost-0.2.6.tar` & `pyprost-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mesih    (420785) domain users   (101)        0 2022-12-07 21:02:31.357184 pyprost-0.2.6/
--rw-rw-r--   0 mesih    (420785) domain users   (101)     1069 2022-12-07 20:55:06.000000 pyprost-0.2.6/LICENSE
--rw-rw-r--   0 mesih    (420785) domain users   (101)     2663 2022-12-07 21:02:31.365184 pyprost-0.2.6/PKG-INFO
--rw-rw-r--   0 mesih    (420785) domain users   (101)     2181 2022-12-07 20:55:43.000000 pyprost-0.2.6/README.md
-drwxrwxr-x   0 mesih    (420785) domain users   (101)        0 2022-12-07 21:02:30.108191 pyprost-0.2.6/bin/
--rwxrwxr-x   0 mesih    (420785) domain users   (101)     5869 2022-12-07 20:55:06.000000 pyprost-0.2.6/bin/prost
--rw-rw-r--   0 mesih    (420785) domain users   (101)      185 2022-12-07 20:55:55.000000 pyprost-0.2.6/pyproject.toml
--rw-rw-r--   0 mesih    (420785) domain users   (101)      694 2022-12-07 21:02:31.422184 pyprost-0.2.6/setup.cfg
-drwxrwxr-x   0 mesih    (420785) domain users   (101)        0 2022-12-07 21:02:29.784192 pyprost-0.2.6/src/
-drwxrwxr-x   0 mesih    (420785) domain users   (101)        0 2022-12-07 21:02:30.578188 pyprost-0.2.6/src/pyprost/
--rw-rw-r--   0 mesih    (420785) domain users   (101)     1080 2022-12-07 20:55:06.000000 pyprost-0.2.6/src/pyprost/__init__.py
--rw-rw-r--   0 mesih    (420785) domain users   (101)     1869 2022-12-07 20:55:06.000000 pyprost-0.2.6/src/pyprost/esmts25_13.py
--rw-rw-r--   0 mesih    (420785) domain users   (101)      754 2022-12-07 20:55:06.000000 pyprost-0.2.6/src/pyprost/prosttools.py
-drwxrwxr-x   0 mesih    (420785) domain users   (101)        0 2022-12-07 21:02:31.280185 pyprost-0.2.6/src/pyprost.egg-info/
--rw-rw-r--   0 mesih    (420785) domain users   (101)     2663 2022-12-07 21:02:29.000000 pyprost-0.2.6/src/pyprost.egg-info/PKG-INFO
--rw-rw-r--   0 mesih    (420785) domain users   (101)      302 2022-12-07 21:02:29.000000 pyprost-0.2.6/src/pyprost.egg-info/SOURCES.txt
--rw-rw-r--   0 mesih    (420785) domain users   (101)        1 2022-12-07 21:02:29.000000 pyprost-0.2.6/src/pyprost.egg-info/dependency_links.txt
--rw-rw-r--   0 mesih    (420785) domain users   (101)       39 2022-12-07 21:02:29.000000 pyprost-0.2.6/src/pyprost.egg-info/requires.txt
--rw-rw-r--   0 mesih    (420785) domain users   (101)        8 2022-12-07 21:02:29.000000 pyprost-0.2.6/src/pyprost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 00:40:11.000000 pyprost-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 00:42:24.746184 pyprost-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-21 00:40:11.000000 pyprost-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15023 2023-04-21 00:40:11.000000 pyprost-0.2.7/bin/prost
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 00:40:11.000000 pyprost-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 00:42:24.746184 pyprost-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.738185 pyprost-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/src/pyprost/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/esmts25_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/prosttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/src/pyprost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/top_level.txt
```

### Comparing `pyprost-0.2.6/LICENSE` & `pyprost-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.6/PKG-INFO` & `pyprost-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyprost
-Version: 0.2.6
+Version: 0.2.7
 Summary: PRotein Ortholog Search Tool
 Home-page: https://github.com/mesihk/prost
 Author: Mesih Kilinc
 Author-email: mesih@iastate.edu
 Project-URL: Bug Tracker, https://github.com/mesihk/prost/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## PROST python package v0.2.6
+## PROST python package v0.2.7
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
@@ -28,15 +28,15 @@
 
 ### How to use
 
 Following commands can be used to create databases and perform homology search.
 
 * makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
 * search: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
-* searchsp: searches a query database agains a SwissProt January 2022 database. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold. 
+* searchsp: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis.
 
 ```
 prost makedb db/sp.fa db/sp.prdb
 prost makedb db/covid.fa db/covid.prdb
 prost search --thr 0.05 db/covid.prdb db/sp.prdb results.tsv
 prost searchsp --thr 0.05 db/covid.prdb results.tsv
 ```
@@ -62,7 +62,15 @@
 clc2embedding = pyprost.quantSeq(clc2)
 
 dist = pyprost.prostDistance(hpo30embedding,clc2embedding)
 print('HPO30-CLC2 prost distance:',dist)
 #Should print: HPO30-CLC2 prost distance: 3479.0
 #Distance smaller than 6875 may indicate homology
 ```
+
+### Resources
+
+* Yeast analysis: https://mesihk.github.io/prostyeast
+* Unannotated Human Proteins Analysis: https://mesihk.github.io/prosthuman
+* Webserver: https://mesihk.github.io/prost 
+* PROST Python package: https://github.com/MesihK/prost
+* PROST Research Data: https://github.com/MesihK/prost-data
```

### Comparing `pyprost-0.2.6/README.md` & `pyprost-0.2.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## PROST python package v0.2.6
+## PROST python package v0.2.7
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
@@ -13,15 +13,15 @@
 
 ### How to use
 
 Following commands can be used to create databases and perform homology search.
 
 * makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
 * search: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
-* searchsp: searches a query database agains a SwissProt January 2022 database. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold. 
+* searchsp: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis.
 
 ```
 prost makedb db/sp.fa db/sp.prdb
 prost makedb db/covid.fa db/covid.prdb
 prost search --thr 0.05 db/covid.prdb db/sp.prdb results.tsv
 prost searchsp --thr 0.05 db/covid.prdb results.tsv
 ```
@@ -47,7 +47,15 @@
 clc2embedding = pyprost.quantSeq(clc2)
 
 dist = pyprost.prostDistance(hpo30embedding,clc2embedding)
 print('HPO30-CLC2 prost distance:',dist)
 #Should print: HPO30-CLC2 prost distance: 3479.0
 #Distance smaller than 6875 may indicate homology
 ```
+
+### Resources
+
+* Yeast analysis: https://mesihk.github.io/prostyeast
+* Unannotated Human Proteins Analysis: https://mesihk.github.io/prosthuman
+* Webserver: https://mesihk.github.io/prost 
+* PROST Python package: https://github.com/MesihK/prost
+* PROST Research Data: https://github.com/MesihK/prost-data
```

### Comparing `pyprost-0.2.6/setup.cfg` & `pyprost-0.2.7/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyprost
-version = 0.2.6
+version = 0.2.7
 author = Mesih Kilinc
 author_email = mesih@iastate.edu
 description = PRotein Ortholog Search Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mesihk/prost
 project_urls = 
@@ -24,14 +24,15 @@
 install_requires = 
 	numpy
 	scipy
 	click
 	blosc
 	torch
 	fair-esm
+	statsmodels
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyprost-0.2.6/src/pyprost/esmts25_13.py` & `pyprost-0.2.7/src/pyprost/esmts25_13.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.6/src/pyprost/prosttools.py` & `pyprost-0.2.7/src/pyprost/prosttools.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.6/src/pyprost.egg-info/PKG-INFO` & `pyprost-0.2.7/src/pyprost.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyprost
-Version: 0.2.6
+Version: 0.2.7
 Summary: PRotein Ortholog Search Tool
 Home-page: https://github.com/mesihk/prost
 Author: Mesih Kilinc
 Author-email: mesih@iastate.edu
 Project-URL: Bug Tracker, https://github.com/mesihk/prost/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-## PROST python package v0.2.6
+## PROST python package v0.2.7
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
@@ -28,15 +28,15 @@
 
 ### How to use
 
 Following commands can be used to create databases and perform homology search.
 
 * makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
 * search: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
-* searchsp: searches a query database agains a SwissProt January 2022 database. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold. 
+* searchsp: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis.
 
 ```
 prost makedb db/sp.fa db/sp.prdb
 prost makedb db/covid.fa db/covid.prdb
 prost search --thr 0.05 db/covid.prdb db/sp.prdb results.tsv
 prost searchsp --thr 0.05 db/covid.prdb results.tsv
 ```
@@ -62,7 +62,15 @@
 clc2embedding = pyprost.quantSeq(clc2)
 
 dist = pyprost.prostDistance(hpo30embedding,clc2embedding)
 print('HPO30-CLC2 prost distance:',dist)
 #Should print: HPO30-CLC2 prost distance: 3479.0
 #Distance smaller than 6875 may indicate homology
 ```
+
+### Resources
+
+* Yeast analysis: https://mesihk.github.io/prostyeast
+* Unannotated Human Proteins Analysis: https://mesihk.github.io/prosthuman
+* Webserver: https://mesihk.github.io/prost 
+* PROST Python package: https://github.com/MesihK/prost
+* PROST Research Data: https://github.com/MesihK/prost-data
```

