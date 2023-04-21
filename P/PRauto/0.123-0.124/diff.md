# Comparing `tmp/PRauto-0.123.tar.gz` & `tmp/PRauto-0.124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.123.tar", last modified: Fri Apr 21 01:37:09 2023, max compression
+gzip compressed data, was "PRauto-0.124.tar", last modified: Fri Apr 21 01:42:33 2023, max compression
```

## Comparing `PRauto-0.123.tar` & `PRauto-0.124.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:37:09.261313 PRauto-0.123/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.123/LICENSE
--rw-rw-rw-   0        0        0      349 2023-04-21 01:37:09.260788 PRauto-0.123/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-21 01:37:09.246502 PRauto-0.123/PRauto.egg-info/
--rw-rw-rw-   0        0        0      349 2023-04-21 01:37:09.000000 PRauto-0.123/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-04-21 01:37:09.000000 PRauto-0.123/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:37:09.000000 PRauto-0.123/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-21 01:37:09.000000 PRauto-0.123/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-21 01:37:09.000000 PRauto-0.123/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-04-21 01:04:02.000000 PRauto-0.123/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 01:37:09.248532 PRauto-0.123/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.123/prauto/__init__.py
--rw-rw-rw-   0        0        0     2246 2023-04-20 08:16:28.000000 PRauto-0.123/prauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:37:09.251502 PRauto-0.123/prauto/prepauto/
--rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.123/prauto/prepauto/__init__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.123/prauto/prepauto/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:37:09.258787 PRauto-0.123/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.123/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     2246 2023-04-20 08:16:28.000000 PRauto-0.123/prauto/retriever/__main__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.123/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2685 2023-04-20 06:05:57.000000 PRauto-0.123/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.123/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-21 01:37:09.261313 PRauto-0.123/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-04-21 01:36:43.000000 PRauto-0.123/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.808723 PRauto-0.124/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.124/LICENSE
+-rw-rw-rw-   0        0        0      349 2023-04-21 01:42:33.808723 PRauto-0.124/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.793723 PRauto-0.124/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 01:42:33.000000 PRauto-0.124/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-04-21 01:04:02.000000 PRauto-0.124/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.796723 PRauto-0.124/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.124/prauto/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-04-21 01:41:27.000000 PRauto-0.124/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.799724 PRauto-0.124/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.124/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.124/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:42:33.806753 PRauto-0.124/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.124/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-04-21 01:40:55.000000 PRauto-0.124/prauto/retriever/__main__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.124/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     2685 2023-04-20 06:05:57.000000 PRauto-0.124/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.124/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 01:42:33.809723 PRauto-0.124/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-04-21 01:42:18.000000 PRauto-0.124/setup.py
```

### Comparing `PRauto-0.123/LICENSE` & `PRauto-0.124/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/README.md` & `PRauto-0.124/README.md`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/prauto/__main__.py` & `PRauto-0.124/prauto/retriever/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from get_fasta import *
-from get_pdb import *
-from get_ligand import *
+from .get_fasta import *
+from .get_pdb import *
+from .get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.123/prauto/prepauto/__main__.py` & `PRauto-0.124/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/prauto/retriever/__main__.py` & `PRauto-0.124/prauto/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
-from get_fasta import *
-from get_pdb import *
-from get_ligand import *
+from .retriever.get_fasta import *
+from .retriever.get_pdb import *
+from .retriever.get_ligand import *
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
```

### Comparing `PRauto-0.123/prauto/retriever/get_fasta.py` & `PRauto-0.124/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/prauto/retriever/get_ligand.py` & `PRauto-0.124/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/prauto/retriever/get_pdb.py` & `PRauto-0.124/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.123/setup.py` & `PRauto-0.124/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages, Extension
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.123',
+        version = '0.124',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

