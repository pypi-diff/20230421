# Comparing `tmp/PRauto-0.121.tar.gz` & `tmp/PRauto-0.122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.121.tar", last modified: Wed Apr 19 11:36:51 2023, max compression
+gzip compressed data, was "PRauto-0.122.tar", last modified: Fri Apr 21 01:05:54 2023, max compression
```

## Comparing `PRauto-0.121.tar` & `PRauto-0.122.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.862825 PRauto-0.121/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.121/LICENSE
--rw-rw-rw-   0        0        0      349 2023-04-19 11:36:51.861824 PRauto-0.121/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.848852 PRauto-0.121/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 11:36:51.000000 PRauto-0.121/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-04-19 11:33:52.000000 PRauto-0.121/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.851856 PRauto-0.121/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.121/prauto/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-04-19 01:41:22.000000 PRauto-0.121/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.853824 PRauto-0.121/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.121/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:36:51.859829 PRauto-0.121/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.121/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.121/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.121/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-19 11:36:51.862825 PRauto-0.121/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-04-19 11:36:20.000000 PRauto-0.121/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:05:54.811526 PRauto-0.122/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.122/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-04-21 01:05:54.810551 PRauto-0.122/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:05:54.784603 PRauto-0.122/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-04-21 01:05:54.000000 PRauto-0.122/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-04-21 01:05:54.000000 PRauto-0.122/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:05:54.000000 PRauto-0.122/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-21 01:05:54.000000 PRauto-0.122/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 01:05:54.000000 PRauto-0.122/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-04-21 01:04:02.000000 PRauto-0.122/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:05:54.787521 PRauto-0.122/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.122/prauto/__init__.py
+-rw-rw-rw-   0        0        0     1758 2023-04-21 00:56:05.000000 PRauto-0.122/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:05:54.794521 PRauto-0.122/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.122/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.122/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:05:54.809551 PRauto-0.122/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.122/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     2246 2023-04-20 08:16:28.000000 PRauto-0.122/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.122/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     2685 2023-04-20 06:05:57.000000 PRauto-0.122/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.122/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:05:54.811526 PRauto-0.122/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-04-21 00:54:58.000000 PRauto-0.122/setup.py
```

### Comparing `PRauto-0.121/LICENSE` & `PRauto-0.122/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.121/README.md` & `PRauto-0.122/README.md`

 * *Files identical despite different names*

### Comparing `PRauto-0.121/prauto/__main__.py` & `PRauto-0.122/prauto/retriever/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from .retriever.get_fasta import *
-from .retriever.get_pdb import *
-from .retriever.get_ligand import *
+from get_fasta import *
+from get_pdb import *
+from get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.121/prauto/prepauto/__main__.py` & `PRauto-0.122/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.121/prauto/retriever/get_fasta.py` & `PRauto-0.122/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.121/prauto/retriever/get_ligand.py` & `PRauto-0.122/prauto/retriever/get_ligand.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 bioactivities = bioactivities_api.filter(target_chembl_id=target, standard_type="IC50",
                                                       assay_type__in=["B","F"],relation__in=['=', '<', '<='],
                                                       **{f"activity_IC50__isnull": False}).only(
                     *target_columns_list)
 
                 compound_columns_list = ["molecule_chembl_id", 'molecule_structures']
                 compounds = compounds_api.filter(
-                    molecule_properties__num_ro5_violations=0,
                     molecule_chembl_id__in=[x['molecule_chembl_id'] for x in bioactivities],
                     molecule_properties__mw_freebase__lte=700).only(*compound_columns_list)
 
                 compounds_list = [record for record in compounds]
 
                 if len(compounds_list) != 0:
                     # Iterate through the list and save each molecule as a .pdb file
```

### Comparing `PRauto-0.121/prauto/retriever/get_pdb.py` & `PRauto-0.122/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.121/setup.py` & `PRauto-0.122/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.121',
+        version = '0.122',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

