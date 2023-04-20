# Comparing `tmp/ak_cache-0.0.1.tar.gz` & `tmp/ak_cache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_cache-0.0.1.tar", last modified: Thu Apr 20 22:20:44 2023, max compression
+gzip compressed data, was "ak_cache-0.0.2.tar", last modified: Thu Apr 20 23:07:07 2023, max compression
```

## Comparing `ak_cache-0.0.1.tar` & `ak_cache-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
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
+-rw-r--r--   0        0        0      653 2023-04-20 22:08:13.913017 ak_cache-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1994 2023-04-20 23:03:21.343856 ak_cache-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1100 2023-04-20 21:26:58.094393 ak_cache-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2974 2023-04-20 23:06:34.285317 ak_cache-0.0.2/README.md
+-rw-r--r--   0        0        0      434 2023-04-20 21:29:05.433062 ak_cache-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      904 2023-03-03 01:17:18.748006 ak_cache-0.0.2/run.bat
+-rw-r--r--   0        0        0      109 2023-04-20 23:04:55.319811 ak_cache-0.0.2/src/ak_cache/__init__.py
+-rw-r--r--   0        0        0     2428 2023-04-20 23:03:37.053784 ak_cache-0.0.2/src/ak_cache/main.py
+-rw-r--r--   0        0        0     3193 1970-01-01 00:00:00.000000 ak_cache-0.0.2/PKG-INFO
```

### Comparing `ak_cache-0.0.1/.github/workflows/test.yml` & `ak_cache-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ak_cache-0.0.1/.gitignore` & `ak_cache-0.0.2/.gitignore`

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

### Comparing `ak_cache-0.0.1/LICENSE` & `ak_cache-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_cache-0.0.1/README.md` & `ak_cache-0.0.2/README.md`

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

### Comparing `ak_cache-0.0.1/run.bat` & `ak_cache-0.0.2/run.bat`

 * *Files identical despite different names*

### Comparing `ak_cache-0.0.1/PKG-INFO` & `ak_cache-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak_cache
-Version: 0.0.1
+Version: 0.0.2
 Summary: General Cache File to cache anything you like
 Author-email: Arun Kishore <pypi@rpakishore.co.in>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: ak_file
 Project-URL: Home, https://github.com/rpakishore/ak_cache
 
@@ -55,15 +55,15 @@
 
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
@@ -82,18 +82,28 @@
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ak_cache Version: 0.0.1 Summary: General Cache File
+Metadata-Version: 2.1 Name: ak_cache Version: 0.0.2 Summary: General Cache File
 to cache anything you like Author-email: Arun Kishore
 rpakishore.co.in> Description-Content-Type: text/markdown Classifier: License
 :: OSI Approved :: MIT License Requires-Dist: ak_file Project-URL: Home, https:
 //github.com/rpakishore/ak_cache
                             ****** ak_cache ******
                     Cache any data for your python projects
    *** View_Demo  Â·  Documentation  Â·  Report_Bug  Â·  Request_Feature ***
@@ -13,22 +13,25 @@
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

