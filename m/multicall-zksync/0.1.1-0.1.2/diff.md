# Comparing `tmp/multicall_zksync-0.1.1.tar.gz` & `tmp/multicall_zksync-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall_zksync-0.1.1.tar", max compression
+gzip compressed data, was "multicall_zksync-0.1.2.tar", max compression
```

## Comparing `multicall_zksync-0.1.1.tar` & `multicall_zksync-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      116 2023-04-21 16:37:49.256165 multicall_zksync-0.1.1/multicall_zksync/__init__.py
--rw-r--r--   0        0        0     4884 2023-04-21 16:37:49.258896 multicall_zksync-0.1.1/multicall_zksync/call.py
--rw-r--r--   0        0        0    34908 2023-04-21 16:37:49.260856 multicall_zksync-0.1.1/multicall_zksync/constants.py
--rw-r--r--   0        0        0       54 2023-04-21 16:37:49.262625 multicall_zksync-0.1.1/multicall_zksync/exceptions.py
--rw-r--r--   0        0        0      267 2023-04-21 16:37:49.264845 multicall_zksync-0.1.1/multicall_zksync/loggers.py
--rw-r--r--   0        0        0     8331 2023-04-21 16:37:49.268861 multicall_zksync-0.1.1/multicall_zksync/multicall.py
--rw-r--r--   0        0        0     2490 2023-04-21 16:37:49.270751 multicall_zksync-0.1.1/multicall_zksync/signature.py
--rw-r--r--   0        0        0     3116 2023-04-21 16:37:49.272632 multicall_zksync-0.1.1/multicall_zksync/utils.py
--rw-r--r--   0        0        0      594 2023-04-21 16:51:14.104138 multicall_zksync-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      623 2023-04-21 16:52:08.070335 multicall_zksync-0.1.1/setup.py
--rw-r--r--   0        0        0      428 2023-04-21 16:52:08.070546 multicall_zksync-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-04-21 16:37:49.256165 multicall_zksync-0.1.2/multicall_zksync/__init__.py
+-rw-r--r--   0        0        0     4884 2023-04-21 16:37:49.258896 multicall_zksync-0.1.2/multicall_zksync/call.py
+-rw-r--r--   0        0        0    34908 2023-04-21 16:37:49.260856 multicall_zksync-0.1.2/multicall_zksync/constants.py
+-rw-r--r--   0        0        0       54 2023-04-21 16:37:49.262625 multicall_zksync-0.1.2/multicall_zksync/exceptions.py
+-rw-r--r--   0        0        0      267 2023-04-21 16:37:49.264845 multicall_zksync-0.1.2/multicall_zksync/loggers.py
+-rw-r--r--   0        0        0     8331 2023-04-21 16:37:49.268861 multicall_zksync-0.1.2/multicall_zksync/multicall.py
+-rw-r--r--   0        0        0     2490 2023-04-21 16:37:49.270751 multicall_zksync-0.1.2/multicall_zksync/signature.py
+-rw-r--r--   0        0        0     3116 2023-04-21 16:37:49.272632 multicall_zksync-0.1.2/multicall_zksync/utils.py
+-rw-r--r--   0        0        0      594 2023-04-21 16:56:25.378101 multicall_zksync-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      623 2023-04-21 16:56:38.952298 multicall_zksync-0.1.2/setup.py
+-rw-r--r--   0        0        0      428 2023-04-21 16:56:38.952506 multicall_zksync-0.1.2/PKG-INFO
```

### Comparing `multicall_zksync-0.1.1/multicall_zksync/call.py` & `multicall_zksync-0.1.2/multicall_zksync/call.py`

 * *Files identical despite different names*

### Comparing `multicall_zksync-0.1.1/multicall_zksync/constants.py` & `multicall_zksync-0.1.2/multicall_zksync/constants.py`

 * *Files identical despite different names*

### Comparing `multicall_zksync-0.1.1/multicall_zksync/multicall.py` & `multicall_zksync-0.1.2/multicall_zksync/multicall.py`

 * *Files identical despite different names*

### Comparing `multicall_zksync-0.1.1/multicall_zksync/signature.py` & `multicall_zksync-0.1.2/multicall_zksync/signature.py`

 * *Files identical despite different names*

### Comparing `multicall_zksync-0.1.1/multicall_zksync/utils.py` & `multicall_zksync-0.1.2/multicall_zksync/utils.py`

 * *Files identical despite different names*

### Comparing `multicall_zksync-0.1.1/pyproject.toml` & `multicall_zksync-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "multicall_zksync"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["JIVIN0902 <jivinvaidya@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 # These web3.py versions have a busted async provider and cannot be used in any multithreaded applications
 # web3 = "^5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
-web3 = "^5.28"
+web3 = "^5.27"
 eth_retry = "^0.1.8"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 flake8 = "^5.0"
 black = "^22.8"
```

### Comparing `multicall_zksync-0.1.1/setup.py` & `multicall_zksync-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['multicall_zksync']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['eth_retry>=0.1.8,<0.2.0', 'web3>=5.28,<6.0']
+['eth_retry>=0.1.8,<0.2.0', 'web3>=5.27,<6.0']
 
 setup_kwargs = {
     'name': 'multicall-zksync',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': None,
     'author': 'JIVIN0902',
     'author_email': 'jivinvaidya@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

