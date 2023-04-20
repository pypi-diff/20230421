# Comparing `tmp/ak_file-0.0.3.tar.gz` & `tmp/ak_file-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_file-0.0.3.tar", last modified: Wed Feb  8 00:16:14 2023, max compression
+gzip compressed data, was "ak_file-0.0.4.tar", last modified: Thu Apr 20 22:17:28 2023, max compression
```

## Comparing `ak_file-0.0.3.tar` & `ak_file-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      654 2023-02-07 22:49:09.380147 ak_file-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1988 2023-02-07 21:16:19.260745 ak_file-0.0.3/.gitignore
--rw-r--r--   0        0        0     1100 2023-02-07 21:19:07.471488 ak_file-0.0.3/LICENSE
--rw-r--r--   0        0        0     2946 2023-02-07 23:52:32.686917 ak_file-0.0.3/README.md
--rw-r--r--   0        0        0      153 2023-02-08 00:16:00.613571 ak_file-0.0.3/ak_file/__init__.py
--rw-r--r--   0        0        0     2460 2023-02-07 23:05:17.332039 ak_file-0.0.3/ak_file/main.py
--rw-r--r--   0        0        0     1895 2023-02-07 23:05:23.278177 ak_file-0.0.3/ak_file/sanitize.py
--rw-r--r--   0        0        0      832 2023-02-08 00:10:58.879553 ak_file-0.0.3/ak_file/search.py
--rw-r--r--   0        0        0      474 2023-02-07 21:20:51.851021 ak_file-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1330 2023-02-07 22:34:45.079468 ak_file-0.0.3/tests/test_main.py
--rw-r--r--   0        0        0      386 2023-02-07 21:37:50.345021 ak_file-0.0.3/tests/test_sanitize.py
--rw-r--r--   0        0        0      415 2023-02-08 00:14:55.664744 ak_file-0.0.3/tests/test_search.py
--rw-r--r--   0        0        0     3186 1970-01-01 00:00:00.000000 ak_file-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      684 2023-04-20 22:07:55.202574 ak_file-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1988 2023-04-20 22:07:55.203575 ak_file-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1100 2023-04-20 22:07:55.204574 ak_file-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2946 2023-04-20 22:07:55.205572 ak_file-0.0.4/README.md
+-rw-r--r--   0        0        0      153 2023-04-20 22:17:01.683828 ak_file-0.0.4/ak_file/__init__.py
+-rw-r--r--   0        0        0     2460 2023-04-20 22:07:55.207572 ak_file-0.0.4/ak_file/main.py
+-rw-r--r--   0        0        0     1895 2023-04-20 22:07:55.208571 ak_file-0.0.4/ak_file/sanitize.py
+-rw-r--r--   0        0        0      832 2023-04-20 22:07:55.209570 ak_file-0.0.4/ak_file/search.py
+-rw-r--r--   0        0        0      446 2023-04-20 22:07:55.210570 ak_file-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1330 2023-04-20 22:15:07.659848 ak_file-0.0.4/tests/test_main.py
+-rw-r--r--   0        0        0      386 2023-04-20 22:07:55.213569 ak_file-0.0.4/tests/test_sanitize.py
+-rw-r--r--   0        0        0      415 2023-04-20 22:15:13.399405 ak_file-0.0.4/tests/test_search.py
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 ak_file-0.0.4/PKG-INFO
```

### Comparing `ak_file-0.0.3/.github/workflows/test.yml` & `ak_file-0.0.4/.github/workflows/test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -20,8 +20,8 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flit
           flit install
       - name: Test with pytest
         run: |
-          pytest .
+          pytest . -W ignore::DeprecationWarning
```

### Comparing `ak_file-0.0.3/.gitignore` & `ak_file-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/LICENSE` & `ak_file-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/README.md` & `ak_file-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/ak_file/main.py` & `ak_file-0.0.4/ak_file/main.py`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/ak_file/sanitize.py` & `ak_file-0.0.4/ak_file/sanitize.py`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/ak_file/search.py` & `ak_file-0.0.4/ak_file/search.py`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/tests/test_main.py` & `ak_file-0.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ak_file-0.0.3/PKG-INFO` & `ak_file-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ak_file
-Version: 0.0.3
+Version: 0.0.4
 Summary: File Parsing function
 Author-email: Arun Kishore <pypi@rpakishore.co.in>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pytest>=7.2.1
-Requires-Dist: python-docx>=0.8.11
 Project-URL: Home, https://github.com/rpakishore/ak-file
 
 <!--- Heading --->
 <div align="center">
   <img src="assets/banner.png" alt="banner" width="auto" height="auto" />
   <h1>ak-file</h1>
   <p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: ak_file Version: 0.0.3 Summary: File Parsing
+Metadata-Version: 2.1 Name: ak_file Version: 0.0.4 Summary: File Parsing
 function Author-email: Arun Kishore
 rpakishore.co.in> Description-Content-Type: text/markdown Classifier: License
-:: OSI Approved :: MIT License Requires-Dist: pytest>=7.2.1 Requires-Dist:
-python-docx>=0.8.11 Project-URL: Home, https://github.com/rpakishore/ak-file
+:: OSI Approved :: MIT License Requires-Dist: pytest>=7.2.1 Project-URL: Home,
+https://github.com/rpakishore/ak-file
                                    [banner]
                              ****** ak-file ******
                  A base module to manipulate files and folders
    *** View_Demo  Â·  Documentation  Â·  Report_Bug  Â·  Request_Feature ***
 
 [![tests](https://github.com/rpakishore/ak-file/actions/workflows/test.yml/
 badge.svg)](https://github.com/rpakishore/ak-file/actions/workflows/test.yml) !
```

