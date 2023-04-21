# Comparing `tmp/directory_ch_client-3.0.2-py3-none-any.whl.zip` & `tmp/directory_ch_client-3.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4515 bytes, number of entries: 8
--rw-r--r--  2.0 unx       96 b- defN 23-Feb-17 09:03 directory_ch_client/__init__.py
--rw-r--r--  2.0 unx      845 b- defN 23-Feb-17 09:03 directory_ch_client/client.py
--rw-r--r--  2.0 unx     1157 b- defN 23-Feb-17 09:03 directory_ch_client/company.py
--rw-r--r--  2.0 unx     1091 b- defN 23-Feb-17 09:03 directory_ch_client-3.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3628 b- defN 23-Feb-17 09:03 directory_ch_client-3.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-17 09:03 directory_ch_client-3.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Feb-17 09:03 directory_ch_client-3.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      704 b- defN 23-Feb-17 09:03 directory_ch_client-3.0.2.dist-info/RECORD
-8 files, 7633 bytes uncompressed, 3267 bytes compressed:  57.2%
+Zip file size: 4514 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       96 b- defN 23-Apr-21 09:55 directory_ch_client/__init__.py
+-rw-r--r--  2.0 unx      845 b- defN 23-Apr-21 09:55 directory_ch_client/client.py
+-rw-r--r--  2.0 unx     1157 b- defN 23-Apr-21 09:55 directory_ch_client/company.py
+-rw-r--r--  2.0 unx     1091 b- defN 23-Apr-21 09:55 directory_ch_client-3.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3657 b- defN 23-Apr-21 09:55 directory_ch_client-3.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 09:55 directory_ch_client-3.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-21 09:55 directory_ch_client-3.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      704 b- defN 23-Apr-21 09:55 directory_ch_client-3.0.3.dist-info/RECORD
+8 files, 7662 bytes uncompressed, 3266 bytes compressed:  57.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: directory_ch_client/client.py
 Comment: 
 
 Filename: directory_ch_client/company.py
 Comment: 
 
-Filename: directory_ch_client-3.0.2.dist-info/LICENSE
+Filename: directory_ch_client-3.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: directory_ch_client-3.0.2.dist-info/METADATA
+Filename: directory_ch_client-3.0.3.dist-info/METADATA
 Comment: 
 
-Filename: directory_ch_client-3.0.2.dist-info/WHEEL
+Filename: directory_ch_client-3.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: directory_ch_client-3.0.2.dist-info/top_level.txt
+Filename: directory_ch_client-3.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_ch_client-3.0.2.dist-info/RECORD
+Filename: directory_ch_client-3.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_ch_client-3.0.2.dist-info/LICENSE` & `directory_ch_client-3.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_ch_client-3.0.2.dist-info/METADATA` & `directory_ch_client-3.0.3.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-ch-client
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python API client for Export Directory Companies House.
 Home-page: https://github.com/uktrade/directory-companies-house-search-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -26,18 +26,19 @@
 Description-Content-Type: text/markdown
 Requires-Dist: django (<4.0.0,>=3.2.18)
 Requires-Dist: requests (<3.0.0,>=2.18.4)
 Requires-Dist: monotonic (<3.0,>=1.2)
 Requires-Dist: directory-client-core (<8.0.0,>=6.1.0)
 Provides-Extra: test
 Requires-Dist: pytest (==7.1.3) ; extra == 'test'
-Requires-Dist: pytest-cov (==3.0.0) ; extra == 'test'
+Requires-Dist: pytest-cov ; extra == 'test'
+Requires-Dist: pytest-codecov ; extra == 'test'
+Requires-Dist: GitPython ; extra == 'test'
 Requires-Dist: flake8 (==5.0.4) ; extra == 'test'
 Requires-Dist: requests-mock (==1.1.0) ; extra == 'test'
-Requires-Dist: codecov (>=2.0.16) ; extra == 'test'
 Requires-Dist: twine (<2.0.0,>=1.11.0) ; extra == 'test'
 Requires-Dist: wheel (<1.0.0,>=0.31.0) ; extra == 'test'
 Requires-Dist: setuptools (<39.0.0,>=38.6.0) ; extra == 'test'
 
 # directory-companies-house-search-client
 
 [![code-climate-image]][code-climate]
```

## Comparing `directory_ch_client-3.0.2.dist-info/RECORD` & `directory_ch_client-3.0.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 directory_ch_client/__init__.py,sha256=6WyxPF0ZPu3BO-7kSqvOsC7TW05RrTHO_A0igTBN5N8,96
 directory_ch_client/client.py,sha256=P6wnuf2PLS2YWlCdbuBE1QmJXluOn1718NMtoiiEnTE,845
 directory_ch_client/company.py,sha256=xalUJIxKjPVFVdRBfhv7QrD0EIgByztmant9oPfaxco,1157
-directory_ch_client-3.0.2.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
-directory_ch_client-3.0.2.dist-info/METADATA,sha256=S9BQNH_b5RTsVLKA1frga9EyB6ak8-5hqoQWK_sz7qk,3628
-directory_ch_client-3.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-directory_ch_client-3.0.2.dist-info/top_level.txt,sha256=eOG6Euz-yfVpcEFgzfJMpSfDICdhfJww1TqTZQO-Mg0,20
-directory_ch_client-3.0.2.dist-info/RECORD,,
+directory_ch_client-3.0.3.dist-info/LICENSE,sha256=y-ArErAQz98OorLek2xntwEp9bo3ZcqfQMtAIcjBdvQ,1091
+directory_ch_client-3.0.3.dist-info/METADATA,sha256=jd3vwOWe9rlW6z6mx9XEd7_pNCZsvTKYWhrgk4Mtiog,3657
+directory_ch_client-3.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_ch_client-3.0.3.dist-info/top_level.txt,sha256=eOG6Euz-yfVpcEFgzfJMpSfDICdhfJww1TqTZQO-Mg0,20
+directory_ch_client-3.0.3.dist-info/RECORD,,
```

