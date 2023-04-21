# Comparing `tmp/pyprost-0.2.7.tar.gz` & `tmp/pyprost-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprost-0.2.7.tar", last modified: Fri Apr 21 00:42:24 2023, max compression
+gzip compressed data, was "pyprost-0.2.8.tar", last modified: Fri Apr 21 01:00:50 2023, max compression
```

## Comparing `pyprost-0.2.7.tar` & `pyprost-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 00:40:11.000000 pyprost-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 00:42:24.746184 pyprost-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-21 00:40:11.000000 pyprost-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15023 2023-04-21 00:40:11.000000 pyprost-0.2.7/bin/prost
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 00:40:11.000000 pyprost-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 00:42:24.746184 pyprost-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.738185 pyprost-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/src/pyprost/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/esmts25_13.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 00:40:11.000000 pyprost-0.2.7/src/pyprost/prosttools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:42:24.742184 pyprost-0.2.7/src/pyprost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 00:42:24.000000 pyprost-0.2.7/src/pyprost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 00:58:38.000000 pyprost-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 01:00:50.828802 pyprost-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-21 00:58:38.000000 pyprost-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15023 2023-04-21 00:58:38.000000 pyprost-0.2.8/bin/prost
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 00:58:38.000000 pyprost-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 01:00:50.832803 pyprost-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/pyprost/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/esmts25_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/prosttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/pyprost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/top_level.txt
```

### Comparing `pyprost-0.2.7/LICENSE` & `pyprost-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.7/PKG-INFO` & `pyprost-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyprost
-Version: 0.2.7
+Version: 0.2.8
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
 
-## PROST python package v0.2.7
+## PROST python package v0.2.8
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
```

### Comparing `pyprost-0.2.7/README.md` & `pyprost-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## PROST python package v0.2.7
+## PROST python package v0.2.8
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
```

### Comparing `pyprost-0.2.7/bin/prost` & `pyprost-0.2.8/bin/prost`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.7/setup.cfg` & `pyprost-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyprost
-version = 0.2.7
+version = 0.2.8
 author = Mesih Kilinc
 author_email = mesih@iastate.edu
 description = PRotein Ortholog Search Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mesihk/prost
 project_urls =
```

### Comparing `pyprost-0.2.7/src/pyprost/__init__.py` & `pyprost-0.2.8/src/pyprost/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if not os.path.exists(prostdir+'/'+name):
             print(info)
             link=f'https://github.com/MesihK/prost/releases/download/{v}/{name}'
             urllib.request.urlretrieve(link, prostdir+'/'+name)
             if md5(prostdir+'/'+name) == md5sum:
                 print("Done.")
             else:
-            print("Download error, MD5 missmatch!")
+                print("Download error, MD5 missmatch!")
 
     if not os.path.exists(prostdir+'/traced_esm1b_25_13.pt'):
         download_file('traced_esm1b_25_13.part1','Downloading ESM1b weights part1','c18e325af45d02724400c656a3f0a229')
         download_file('traced_esm1b_25_13.part2','Downloading ESM1b weights part2','4c3939d9454503548af127858cfa8deb')
 
         print("Merge ESM1b weights")
         with open(prostdir+"/traced_esm1b_25_13.part1", "rb") as output_file1:
```

### Comparing `pyprost-0.2.7/src/pyprost/esmts25_13.py` & `pyprost-0.2.8/src/pyprost/esmts25_13.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.7/src/pyprost/prosttools.py` & `pyprost-0.2.8/src/pyprost/prosttools.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.7/src/pyprost.egg-info/PKG-INFO` & `pyprost-0.2.8/src/pyprost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyprost
-Version: 0.2.7
+Version: 0.2.8
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
 
-## PROST python package v0.2.7
+## PROST python package v0.2.8
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
 The package can be installed with:
```

