# Comparing `tmp/discotoolkit-1.0.tar.gz` & `tmp/discotoolkit-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discotoolkit-1.0.tar", last modified: Fri Apr 21 05:44:58 2023, max compression
+gzip compressed data, was "discotoolkit-1.0.0.1.tar", last modified: Fri Apr 21 05:57:44 2023, max compression
```

## Comparing `discotoolkit-1.0.tar` & `discotoolkit-1.0.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:44:49.468897 discotoolkit-1.0/
--rw-rw-r--   0 rom       (1013) rom       (1027)      690 2023-04-21 05:44:49.468897 discotoolkit-1.0/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      812 2023-04-21 05:15:25.000000 discotoolkit-1.0/README.md
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:44:49.432898 discotoolkit-1.0/discotoolkit/
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:44.000000 discotoolkit-1.0/discotoolkit/CELLiD.py
--rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0/discotoolkit/CellMapper.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     1373 2023-04-17 05:08:54.000000 discotoolkit-1.0/discotoolkit/DiscoClass.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     4489 2023-04-21 05:15:25.000000 discotoolkit-1.0/discotoolkit/DownloadDiscoData.py
--rw-rw-r--   0 rom       (1013) rom       (1027)     8380 2023-04-21 05:15:25.000000 discotoolkit-1.0/discotoolkit/GetMetadata.py
--rw-rw-r--   0 rom       (1013) rom       (1027)      556 2023-04-21 05:15:25.000000 discotoolkit-1.0/discotoolkit/GlobalVariable.py
--rw-rw-r--   0 rom       (1013) rom       (1027)       85 2023-04-14 07:12:49.000000 discotoolkit-1.0/discotoolkit/__init__.py
-drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:44:49.460898 discotoolkit-1.0/discotoolkit.egg-info/
--rw-rw-r--   0 rom       (1013) rom       (1027)      690 2023-04-21 05:44:49.000000 discotoolkit-1.0/discotoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rom       (1013) rom       (1027)      392 2023-04-21 05:44:49.000000 discotoolkit-1.0/discotoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-04-21 05:44:49.000000 discotoolkit-1.0/discotoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:44:49.000000 discotoolkit-1.0/discotoolkit.egg-info/requires.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:44:49.000000 discotoolkit-1.0/discotoolkit.egg-info/top_level.txt
--rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-04-21 05:44:49.468897 discotoolkit-1.0/setup.cfg
--rw-rw-r--   0 rom       (1013) rom       (1027)      829 2023-04-21 05:44:33.000000 discotoolkit-1.0/setup.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.659289 discotoolkit-1.0.0.1/
+-rw-rw-r--   0 rom       (1013) rom       (1027)       17 2023-04-21 05:48:20.000000 discotoolkit-1.0.0.1/MANIFEST.in
+-rw-rw-r--   0 rom       (1013) rom       (1027)      911 2023-04-21 05:57:34.655289 discotoolkit-1.0.0.1/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      812 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/README.md
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.619289 discotoolkit-1.0.0.1/discotoolkit/
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:44.000000 discotoolkit-1.0.0.1/discotoolkit/CELLiD.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)        0 2023-04-13 08:19:05.000000 discotoolkit-1.0.0.1/discotoolkit/CellMapper.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1373 2023-04-17 05:08:54.000000 discotoolkit-1.0.0.1/discotoolkit/DiscoClass.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     4489 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/DownloadDiscoData.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)     8380 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/GetMetadata.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)      556 2023-04-21 05:15:25.000000 discotoolkit-1.0.0.1/discotoolkit/GlobalVariable.py
+-rw-rw-r--   0 rom       (1013) rom       (1027)       85 2023-04-14 07:12:49.000000 discotoolkit-1.0.0.1/discotoolkit/__init__.py
+drwxrwxr-x   0 rom       (1013) rom       (1027)        0 2023-04-21 05:57:34.651289 discotoolkit-1.0.0.1/discotoolkit.egg-info/
+-rw-rw-r--   0 rom       (1013) rom       (1027)      911 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rom       (1013) rom       (1027)      404 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)        1 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       13 2023-04-21 05:57:34.000000 discotoolkit-1.0.0.1/discotoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 rom       (1013) rom       (1027)       38 2023-04-21 05:57:34.659289 discotoolkit-1.0.0.1/setup.cfg
+-rw-rw-r--   0 rom       (1013) rom       (1027)     1061 2023-04-21 05:57:31.000000 discotoolkit-1.0.0.1/setup.py
```

### Comparing `discotoolkit-1.0/PKG-INFO` & `discotoolkit-1.0.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0
-Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
-                    Filter and download DISCO data based on sample metadata and cell type information
-                    CELLiD: cell type annotation
-                    scEnrichment: geneset enrichment using DISCO DEGs
-                    CellMapper: project data into DISCO atlas
-Home-page: UNKNOWN
+Version: 1.0.0.1
+Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
+Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
-Description: UNKNOWN
+Description: 
+            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
+            
+        
+            Filter and download DISCO data based on sample metadata and cell type information
+            
+        CELLiD: cell type annotation
+            
+        scEnrichment: geneset enrichment using DISCO DEGs
+            
+        CellMapper: project data into DISCO atlas
+            
 Platform: UNKNOWN
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `discotoolkit-1.0/README.md` & `discotoolkit-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0/discotoolkit/DiscoClass.py` & `discotoolkit-1.0.0.1/discotoolkit/DiscoClass.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0/discotoolkit/DownloadDiscoData.py` & `discotoolkit-1.0.0.1/discotoolkit/DownloadDiscoData.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0/discotoolkit/GetMetadata.py` & `discotoolkit-1.0.0.1/discotoolkit/GetMetadata.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0/discotoolkit/GlobalVariable.py` & `discotoolkit-1.0.0.1/discotoolkit/GlobalVariable.py`

 * *Files identical despite different names*

### Comparing `discotoolkit-1.0/discotoolkit.egg-info/PKG-INFO` & `discotoolkit-1.0.0.1/discotoolkit.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: discotoolkit
-Version: 1.0
-Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
-                    Filter and download DISCO data based on sample metadata and cell type information
-                    CELLiD: cell type annotation
-                    scEnrichment: geneset enrichment using DISCO DEGs
-                    CellMapper: project data into DISCO atlas
-Home-page: UNKNOWN
+Version: 1.0.0.1
+Summary: DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database.
+Home-page: http://www.immunesinglecell.org/
 Author: Li Mengwei, Rom Uddamvathanak
 Author-email: uddamvathanak_rom@immunol.a-star.edu.sg
 License: UNKNOWN
-Description: UNKNOWN
+Description: 
+            DISCOtoolkit is an python package that allows users to access data and use the tools provided by the DISCO database. It provides the following functions:
+            
+        
+            Filter and download DISCO data based on sample metadata and cell type information
+            
+        CELLiD: cell type annotation
+            
+        scEnrichment: geneset enrichment using DISCO DEGs
+            
+        CellMapper: project data into DISCO atlas
+            
 Platform: UNKNOWN
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

