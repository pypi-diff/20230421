# Comparing `tmp/gemcall-0.9.1.tar.gz` & `tmp/gemcall-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemcall-0.9.1.tar", last modified: Wed Mar 29 19:34:24 2023, max compression
+gzip compressed data, was "gemcall-0.9.2.tar", last modified: Fri Apr 21 14:16:35 2023, max compression
```

## Comparing `gemcall-0.9.1.tar` & `gemcall-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-03-29 19:34:24.556469 gemcall-0.9.1/
--rw-r--r--   0 cyber     (1000) users      (100)     1077 2021-12-05 14:28:46.000000 gemcall-0.9.1/LICENSE
--rw-r--r--   0 cyber     (1000) users      (100)     3324 2023-03-29 19:34:24.556469 gemcall-0.9.1/PKG-INFO
--rw-r--r--   0 cyber     (1000) users      (100)     2609 2022-06-03 07:16:15.000000 gemcall-0.9.1/README.md
-drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-03-29 19:34:24.554469 gemcall-0.9.1/gemcall/
--rw-r--r--   0 cyber     (1000) users      (100)       39 2021-12-05 14:28:46.000000 gemcall-0.9.1/gemcall/__init__.py
--rwxr-xr-x   0 cyber     (1000) users      (100)     2084 2021-12-05 14:28:46.000000 gemcall-0.9.1/gemcall/__main__.py
--rwxr-xr-x   0 cyber     (1000) users      (100)     2166 2022-07-29 03:42:23.000000 gemcall-0.9.1/gemcall/gemcall.py
-drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-03-29 19:34:24.555469 gemcall-0.9.1/gemcall.egg-info/
--rw-r--r--   0 cyber     (1000) users      (100)     3324 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/PKG-INFO
--rw-r--r--   0 cyber     (1000) users      (100)      283 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/SOURCES.txt
--rw-r--r--   0 cyber     (1000) users      (100)        1 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/dependency_links.txt
--rw-r--r--   0 cyber     (1000) users      (100)       50 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/entry_points.txt
--rw-r--r--   0 cyber     (1000) users      (100)       13 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/requires.txt
--rw-r--r--   0 cyber     (1000) users      (100)        8 2023-03-29 19:34:24.000000 gemcall-0.9.1/gemcall.egg-info/top_level.txt
--rw-r--r--   0 cyber     (1000) users      (100)      870 2023-03-29 19:34:24.557469 gemcall-0.9.1/setup.cfg
--rw-r--r--   0 cyber     (1000) users      (100)       38 2021-12-05 14:28:46.000000 gemcall-0.9.1/setup.py
+drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-04-21 14:16:35.291218 gemcall-0.9.2/
+-rw-r--r--   0 cyber     (1000) users      (100)     1077 2021-12-05 14:28:46.000000 gemcall-0.9.2/LICENSE
+-rw-r--r--   0 cyber     (1000) users      (100)     3324 2023-04-21 14:16:35.291218 gemcall-0.9.2/PKG-INFO
+-rw-r--r--   0 cyber     (1000) users      (100)     2609 2022-06-03 07:16:15.000000 gemcall-0.9.2/README.md
+drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-04-21 14:16:35.271219 gemcall-0.9.2/gemcall/
+-rw-r--r--   0 cyber     (1000) users      (100)       39 2021-12-05 14:28:46.000000 gemcall-0.9.2/gemcall/__init__.py
+-rwxr-xr-x   0 cyber     (1000) users      (100)     2084 2021-12-05 14:28:46.000000 gemcall-0.9.2/gemcall/__main__.py
+-rwxr-xr-x   0 cyber     (1000) users      (100)     2301 2023-04-21 14:14:11.000000 gemcall-0.9.2/gemcall/gemcall.py
+drwxr-xr-x   0 cyber     (1000) users      (100)        0 2023-04-21 14:16:35.289218 gemcall-0.9.2/gemcall.egg-info/
+-rw-r--r--   0 cyber     (1000) users      (100)     3324 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/PKG-INFO
+-rw-r--r--   0 cyber     (1000) users      (100)      283 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber     (1000) users      (100)        1 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber     (1000) users      (100)       50 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/entry_points.txt
+-rw-r--r--   0 cyber     (1000) users      (100)       13 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/requires.txt
+-rw-r--r--   0 cyber     (1000) users      (100)        8 2023-04-21 14:16:35.000000 gemcall-0.9.2/gemcall.egg-info/top_level.txt
+-rw-r--r--   0 cyber     (1000) users      (100)      870 2023-04-21 14:16:35.304217 gemcall-0.9.2/setup.cfg
+-rw-r--r--   0 cyber     (1000) users      (100)       38 2021-12-05 14:28:46.000000 gemcall-0.9.2/setup.py
```

### Comparing `gemcall-0.9.1/LICENSE` & `gemcall-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gemcall-0.9.1/PKG-INFO` & `gemcall-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemcall
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library and CLI tool for making gemini requests
 Home-page: https://notabug.org/tinyrabbit/gemcall
 Author: Björn Wärmedal
 Author-email: bjorn.warmedal@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `gemcall-0.9.1/README.md` & `gemcall-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `gemcall-0.9.1/gemcall/__main__.py` & `gemcall-0.9.2/gemcall/__main__.py`

 * *Files identical despite different names*

### Comparing `gemcall-0.9.1/gemcall/gemcall.py` & `gemcall-0.9.2/gemcall/gemcall.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 
         cert: bytes = self._socket.getpeercert(binary_form=True)
         try:
             certobj: RSA.RsaKey = RSA.import_key(cert)
         except ValueError:
             certobj: ECC.EccKey = ECC.import_key(cert)
         # "\n" is added for API compatibility
-        pubkey: str = certobj.public_key().export_key(format="PEM").decode() + "\n"
+        expkey = certobj.public_key().export_key(format="PEM")
+        if type(expkey) == str:
+            pubkey: str = expkey + "\n"
+        if type(expkey) == bytes:
+            pubkey: str = expkey.decode() + "\n"
+
 
         self.serverpubkey: bytes = pubkey.encode()
         self._filehandle = self._socket.makefile(mode = "rb")
 
         # Two code digits, one space and a maximum of 1024 bytes of meta info.
         try:
             self.responsecode, self.meta = self._filehandle.readline(1027).split(maxsplit=1)
```

### Comparing `gemcall-0.9.1/gemcall.egg-info/PKG-INFO` & `gemcall-0.9.2/gemcall.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemcall
-Version: 0.9.1
+Version: 0.9.2
 Summary: A library and CLI tool for making gemini requests
 Home-page: https://notabug.org/tinyrabbit/gemcall
 Author: Björn Wärmedal
 Author-email: bjorn.warmedal@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `gemcall-0.9.1/setup.cfg` & `gemcall-0.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gemcall
-version = 0.9.1
+version = 0.9.2
 description = A library and CLI tool for making gemini requests
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://notabug.org/tinyrabbit/gemcall
 author = Björn Wärmedal
 author_email = bjorn.warmedal@gmail.com
 license = MIT License
```

