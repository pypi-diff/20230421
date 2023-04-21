# Comparing `tmp/ak_cache-0.0.1.tar.gz` & `tmp/ak_cache-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_cache-0.0.1.tar", last modified: Thu Apr 20 22:20:44 2023, max compression
+gzip compressed data, was "ak_cache-0.0.3.tar", last modified: Fri Apr 21 00:10:42 2023, max compression
```

## Comparing `ak_cache-0.0.1.tar` & `ak_cache-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      653 2023-04-20 22:08:13.913017 ak_cache-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1988 2023-04-20 21:25:06.070062 ak_cache-0.0.1/.gitignore
--rw-r--r--   0        0        0       29 2023-04-20 21:52:12.406278 ak_cache-0.0.1/Cache.pkl
--rw-r--r--   0        0        0     1100 2023-04-20 21:26:58.094393 ak_cache-0.0.1/LICENSE
--rw-r--r--   0        0        0     2735 2023-04-20 22:07:15.805997 ak_cache-0.0.1/README.md
--rw-r--r--   0        0        0      434 2023-04-20 21:29:05.433062 ak_cache-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      904 2023-03-03 01:17:18.748006 ak_cache-0.0.1/run.bat
--rw-r--r--   0        0        0      109 2023-04-20 21:46:10.987824 ak_cache-0.0.1/src/ak_cache/__init__.py
--rw-r--r--   0        0        0     1047 2023-04-20 21:44:56.019843 ak_cache-0.0.1/src/ak_cache/main.py
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 ak_cache-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      653 2023-04-20 22:08:13.913017 ak_cache-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1994 2023-04-20 23:03:21.343856 ak_cache-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1100 2023-04-20 21:26:58.094393 ak_cache-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2974 2023-04-20 23:06:34.285317 ak_cache-0.0.3/README.md
+-rw-r--r--   0        0        0      460 2023-04-21 00:05:39.465309 ak_cache-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-04-21 00:10:20.944735 ak_cache-0.0.3/src/ak_cache/__init__.py
+-rw-r--r--   0        0        0     2428 2023-04-20 23:03:37.053784 ak_cache-0.0.3/src/ak_cache/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 23:20:25.604241 ak_cache-0.0.3/src/tests/__init__.py
+-rw-r--r--   0        0        0     1282 2023-04-20 23:32:30.268139 ak_cache-0.0.3/src/tests/test_main.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 ak_cache-0.0.3/PKG-INFO
```

### Comparing `ak_cache-0.0.1/.github/workflows/test.yml` & `ak_cache-0.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ak_cache-0.0.1/.gitignore` & `ak_cache-0.0.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -126,7 +126,8 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 .vscode/settings.json
 WebDriver/chromedriver.exe
 nosync*
+*.pkl
```

### Comparing `ak_cache-0.0.1/LICENSE` & `ak_cache-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_cache-0.0.1/README.md` & `ak_cache-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 <!-- Prerequisites -->
 ### 2.1. Prerequisites
 
 <!-- Installation -->
 ### 2.2. Installation
 
-Install my-project with npm
+Install my-project with flit
 
 ```bash
 git clone https://github.com/rpakishore/ak_cache.git
 cd ak_cache
 pip install flit
 flit install
 ```
@@ -72,18 +72,28 @@
 ```python
 $ from ak_cache import Cache
 $ cache_file = Cache(r'Path\to\Cache\file.pkl')
 $ cache_file.write('This is a text')
 $ cache_file.read()
 'This is a text'
 ```
+
+Encrypt your pickle file as below
+
+```python
+$ cache_file = Cache(r'Path\to\Cache\encr_file.pkl', password="Strong_Password")
+
+$ cache_file.write('This is an encrypted text')
+$ cache_file.read()
+'This is an encrypted text'
+```
 <!-- Roadmap -->
 ## 4. Roadmap
 
-- [ ] Add encryption option to the cache file
+- [x] Add encryption option to the cache file
 
 <!-- License -->
 ## 5. License
 
 See LICENSE.txt for more information.
 
 <!-- Contact -->
```

#### html2text {}

```diff
@@ -8,22 +8,25 @@
 ***** Table of Contents *****
 - [1. About the Project](#1-about-the-project) - [1.1. Features](#11-features)
 - [2. Getting Started](#2-getting-started) - [2.1. Prerequisites](#21-
 prerequisites) - [2.2. Installation](#22-installation) - [3. Usage](#3-usage) -
 [4. Roadmap](#4-roadmap) - [5. License](#5-license) - [6. Contact](#6-contact)
 - [7. Acknowledgements](#7-acknowledgements)  ## 1. About the Project  ### 1.1.
 Features - Read and write data to a Cached Pickle File  ## 2. Getting Started
-### 2.1. Prerequisites  ### 2.2. Installation Install my-project with npm
+### 2.1. Prerequisites  ### 2.2. Installation Install my-project with flit
 ```bash git clone https://github.com/rpakishore/ak_cache.git cd ak_cache pip
 install flit flit install ``` Alternatively, you can use pip ```bash pip
 install ak_cache ```  ## 3. Usage Use this space to tell a little more about
 your project and how it can be used. Show additional screenshots, code samples,
 demos or link to other resources. ```python $ from ak_cache import Cache $
 cache_file = Cache(r'Path\to\Cache\file.pkl') $ cache_file.write('This is a
-text') $ cache_file.read() 'This is a text' ```  ## 4. Roadmap - [ ] Add
+text') $ cache_file.read() 'This is a text' ``` Encrypt your pickle file as
+below ```python $ cache_file = Cache(r'Path\to\Cache\encr_file.pkl',
+password="Strong_Password") $ cache_file.write('This is an encrypted text') $
+cache_file.read() 'This is an encrypted text' ```  ## 4. Roadmap - [x] Add
 encryption option to the cache file  ## 5. License See LICENSE.txt for more
 information.  ## 6. Contact Arun Kishore - [@rpakishore](mailto:
 rpakishore@gmail.com) Project Link: [https://github.com/rpakishore/](https://
 github.com/rpakishore/ak_cache)  ## 7. Acknowledgements Use this section to
 mention useful resources and libraries that you have used in your projects. -
 [Awesome README Template](https://github.com/Louis3797/awesome-readme-template/
 blob/main/README-WITHOUT-EMOJI.md) - [Banner Maker](https://banner.godori.dev/
```

### Comparing `ak_cache-0.0.1/PKG-INFO` & `ak_cache-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: ak_cache
-Version: 0.0.1
+Version: 0.0.3
 Summary: General Cache File to cache anything you like
 Author-email: Arun Kishore <pypi@rpakishore.co.in>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ak_file
+Requires-Dist: pytest
+Requires-Dist: cryptography
 Project-URL: Home, https://github.com/rpakishore/ak_cache
 
 <!--- Heading --->
 <div align="center">
   <h1>ak_cache</h1>
   <p>
     Cache any data for your python projects
@@ -55,15 +57,15 @@
 
 <!-- Prerequisites -->
 ### 2.1. Prerequisites
 
 <!-- Installation -->
 ### 2.2. Installation
 
-Install my-project with npm
+Install my-project with flit
 
 ```bash
 git clone https://github.com/rpakishore/ak_cache.git
 cd ak_cache
 pip install flit
 flit install
 ```
@@ -82,18 +84,28 @@
 ```python
 $ from ak_cache import Cache
 $ cache_file = Cache(r'Path\to\Cache\file.pkl')
 $ cache_file.write('This is a text')
 $ cache_file.read()
 'This is a text'
 ```
+
+Encrypt your pickle file as below
+
+```python
+$ cache_file = Cache(r'Path\to\Cache\encr_file.pkl', password="Strong_Password")
+
+$ cache_file.write('This is an encrypted text')
+$ cache_file.read()
+'This is an encrypted text'
+```
 <!-- Roadmap -->
 ## 4. Roadmap
 
-- [ ] Add encryption option to the cache file
+- [x] Add encryption option to the cache file
 
 <!-- License -->
 ## 5. License
 
 See LICENSE.txt for more information.
 
 <!-- Contact -->
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1 Name: ak_cache Version: 0.0.1 Summary: General Cache File
+Metadata-Version: 2.1 Name: ak_cache Version: 0.0.3 Summary: General Cache File
 to cache anything you like Author-email: Arun Kishore
 rpakishore.co.in> Description-Content-Type: text/markdown Classifier: License
-:: OSI Approved :: MIT License Requires-Dist: ak_file Project-URL: Home, https:
-//github.com/rpakishore/ak_cache
+:: OSI Approved :: MIT License Requires-Dist: ak_file Requires-Dist: pytest
+Requires-Dist: cryptography Project-URL: Home, https://github.com/rpakishore/
+ak_cache
                             ****** ak_cache ******
                     Cache any data for your python projects
    *** View_Demo  Â·  Documentation  Â·  Report_Bug  Â·  Request_Feature ***
 
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/
 rpakishore/ak_cache) ![GitHub last commit](https://img.shields.io/github/last-
 commit/rpakishore/ak_cache)
 ***** Table of Contents *****
 - [1. About the Project](#1-about-the-project) - [1.1. Features](#11-features)
 - [2. Getting Started](#2-getting-started) - [2.1. Prerequisites](#21-
 prerequisites) - [2.2. Installation](#22-installation) - [3. Usage](#3-usage) -
 [4. Roadmap](#4-roadmap) - [5. License](#5-license) - [6. Contact](#6-contact)
 - [7. Acknowledgements](#7-acknowledgements)  ## 1. About the Project  ### 1.1.
 Features - Read and write data to a Cached Pickle File  ## 2. Getting Started
-### 2.1. Prerequisites  ### 2.2. Installation Install my-project with npm
+### 2.1. Prerequisites  ### 2.2. Installation Install my-project with flit
 ```bash git clone https://github.com/rpakishore/ak_cache.git cd ak_cache pip
 install flit flit install ``` Alternatively, you can use pip ```bash pip
 install ak_cache ```  ## 3. Usage Use this space to tell a little more about
 your project and how it can be used. Show additional screenshots, code samples,
 demos or link to other resources. ```python $ from ak_cache import Cache $
 cache_file = Cache(r'Path\to\Cache\file.pkl') $ cache_file.write('This is a
-text') $ cache_file.read() 'This is a text' ```  ## 4. Roadmap - [ ] Add
+text') $ cache_file.read() 'This is a text' ``` Encrypt your pickle file as
+below ```python $ cache_file = Cache(r'Path\to\Cache\encr_file.pkl',
+password="Strong_Password") $ cache_file.write('This is an encrypted text') $
+cache_file.read() 'This is an encrypted text' ```  ## 4. Roadmap - [x] Add
 encryption option to the cache file  ## 5. License See LICENSE.txt for more
 information.  ## 6. Contact Arun Kishore - [@rpakishore](mailto:
 rpakishore@gmail.com) Project Link: [https://github.com/rpakishore/](https://
 github.com/rpakishore/ak_cache)  ## 7. Acknowledgements Use this section to
 mention useful resources and libraries that you have used in your projects. -
 [Awesome README Template](https://github.com/Louis3797/awesome-readme-template/
 blob/main/README-WITHOUT-EMOJI.md) - [Banner Maker](https://banner.godori.dev/
```

