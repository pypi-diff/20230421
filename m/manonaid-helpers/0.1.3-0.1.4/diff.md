# Comparing `tmp/manonaid_helpers-0.1.3.tar.gz` & `tmp/manonaid_helpers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Self Learning\Python\manonaid_helpers\dist\.tmp-2z6uufyk\manonaid_helpers-0.1.3.tar", last modified: Wed Mar  8 14:46:11 2023, max compression
+gzip compressed data, was "D:\Self Learning\Python\manonaid_helpers\dist\.tmp-hcbmob4_\manonaid_helpers-0.1.4.tar", last modified: Fri Apr 21 07:03:27 2023, max compression
```

## Comparing `manonaid_helpers-0.1.3.tar` & `manonaid_helpers-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/
--rw-rw-rw-   0        0        0        0 2023-03-04 08:36:46.000000 manonaid_helpers-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2959 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2664 2023-03-08 14:45:24.000000 manonaid_helpers-0.1.3/README.md
--rw-rw-rw-   0        0        0      108 2023-03-04 08:40:06.000000 manonaid_helpers-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      506 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/
--rw-rw-rw-   0        0        0        0 2023-03-04 08:31:17.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/__init__.py
--rw-rw-rw-   0        0        0     2355 2023-03-05 07:10:44.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/checks.py
--rw-rw-rw-   0        0        0     2007 2023-03-05 07:06:44.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/core.py
--rw-rw-rw-   0        0        0     2764 2023-03-08 14:08:51.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/download.py
--rw-rw-rw-   0        0        0      379 2023-03-08 14:15:39.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/script.py
--rw-rw-rw-   0        0        0     1384 2023-03-08 14:15:10.000000 manonaid_helpers-0.1.3/src/manonaid_helpers/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/
--rw-rw-rw-   0        0        0     2959 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-08 14:46:11.000000 manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/
+-rw-rw-rw-   0        0        0        0 2023-03-04 08:36:46.000000 manonaid_helpers-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2584 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2287 2023-04-21 07:03:15.000000 manonaid_helpers-0.1.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-03-04 08:40:06.000000 manonaid_helpers-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      506 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/
+-rw-rw-rw-   0        0        0        0 2023-03-04 08:31:17.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/__init__.py
+-rw-rw-rw-   0        0        0     2355 2023-03-05 07:10:44.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/checks.py
+-rw-rw-rw-   0        0        0     2007 2023-03-05 07:06:44.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/core.py
+-rw-rw-rw-   0        0        0     2764 2023-03-08 14:08:51.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/download.py
+-rw-rw-rw-   0        0        0     1384 2023-03-08 14:15:10.000000 manonaid_helpers-0.1.4/src/manonaid_helpers/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/
+-rw-rw-rw-   0        0        0     2584 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-21 07:03:27.000000 manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/top_level.txt
```

### Comparing `manonaid_helpers-0.1.3/PKG-INFO` & `manonaid_helpers-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manonaid_helpers
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Author: manonaid
 Author-email: manoharan.naidu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -87,24 +87,7 @@
 
 ## List blobs
 
 With the `Utils.list_blobs` method we can do advanced listing of blobs in a container or specific folder in a container.
 We have several argument we can use to define our scope of information:
 
 - `name_starts_with`: This can be used to filter files with certain prefix, or to select certain folders: `name_starts_with=folder1/subfolder/lastfolder/`
-
-### 1. List a whole container with just the filenames as a list.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(container='containername').list_blobs()
-```
-
-### 2. List a folder in a container.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(
-   container='containername',
-   name_starts_with="foldername/"
-).list_blobs()
-```
```

### Comparing `manonaid_helpers-0.1.3/README.md` & `manonaid_helpers-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -75,25 +75,8 @@
 ```
 
 ## List blobs
 
 With the `Utils.list_blobs` method we can do advanced listing of blobs in a container or specific folder in a container.
 We have several argument we can use to define our scope of information:
 
-- `name_starts_with`: This can be used to filter files with certain prefix, or to select certain folders: `name_starts_with=folder1/subfolder/lastfolder/`
-
-### 1. List a whole container with just the filenames as a list.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(container='containername').list_blobs()
-```
-
-### 2. List a folder in a container.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(
-   container='containername',
-   name_starts_with="foldername/"
-).list_blobs()
-```
+- `name_starts_with`: This can be used to filter files with certain prefix, or to select certain folders: `name_starts_with=folder1/subfolder/lastfolder/`
```

### Comparing `manonaid_helpers-0.1.3/src/manonaid_helpers/checks.py` & `manonaid_helpers-0.1.4/src/manonaid_helpers/checks.py`

 * *Files identical despite different names*

### Comparing `manonaid_helpers-0.1.3/src/manonaid_helpers/core.py` & `manonaid_helpers-0.1.4/src/manonaid_helpers/core.py`

 * *Files identical despite different names*

### Comparing `manonaid_helpers-0.1.3/src/manonaid_helpers/download.py` & `manonaid_helpers-0.1.4/src/manonaid_helpers/download.py`

 * *Files identical despite different names*

### Comparing `manonaid_helpers-0.1.3/src/manonaid_helpers/utils.py` & `manonaid_helpers-0.1.4/src/manonaid_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `manonaid_helpers-0.1.3/src/manonaid_helpers.egg-info/PKG-INFO` & `manonaid_helpers-0.1.4/src/manonaid_helpers.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manonaid-helpers
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small example package
 Author: manonaid
 Author-email: manoharan.naidu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -87,24 +87,7 @@
 
 ## List blobs
 
 With the `Utils.list_blobs` method we can do advanced listing of blobs in a container or specific folder in a container.
 We have several argument we can use to define our scope of information:
 
 - `name_starts_with`: This can be used to filter files with certain prefix, or to select certain folders: `name_starts_with=folder1/subfolder/lastfolder/`
-
-### 1. List a whole container with just the filenames as a list.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(container='containername').list_blobs()
-```
-
-### 2. List a folder in a container.
-```python
-from azurebatchload import Utils
-
-list_blobs = Utils(
-   container='containername',
-   name_starts_with="foldername/"
-).list_blobs()
-```
```

