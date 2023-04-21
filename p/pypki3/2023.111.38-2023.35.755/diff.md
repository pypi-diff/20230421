# Comparing `tmp/pypki3-2023.111.38.tar.gz` & `tmp/pypki3-2023.35.755.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypki3-2023.111.38.tar", max compression
+gzip compressed data, was "pypki3-2023.35.755.tar", max compression
```

## Comparing `pypki3-2023.111.38.tar` & `pypki3-2023.35.755.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1056 2023-04-21 00:38:37.460792 pypki3-2023.111.38/LICENSE
--rw-r--r--   0        0        0     4188 2023-04-21 00:38:37.460792 pypki3-2023.111.38/README.md
--rw-r--r--   0        0        0      110 2023-04-21 00:38:37.460792 pypki3-2023.111.38/pypki3/README.md
--rw-r--r--   0        0        0      343 2023-04-21 00:38:37.460792 pypki3-2023.111.38/pypki3/__init__.py
--rw-r--r--   0        0        0    13356 2023-04-21 00:38:37.460792 pypki3-2023.111.38/pypki3/config.py
--rw-r--r--   0        0        0       43 2023-04-21 00:38:37.460792 pypki3-2023.111.38/pypki3/exceptions.py
--rw-r--r--   0        0        0      428 2023-04-21 00:38:37.460792 pypki3-2023.111.38/pypki3/utils.py
--rw-r--r--   0        0        0      827 2023-04-21 00:38:58.004699 pypki3-2023.111.38/pyproject.toml
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 pypki3-2023.111.38/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-02-04 12:34:57.703791 pypki3-2023.35.755/LICENSE
+-rw-r--r--   0        0        0     4188 2023-02-04 12:34:57.703791 pypki3-2023.35.755/README.md
+-rw-r--r--   0        0        0      110 2023-02-04 12:34:57.703791 pypki3-2023.35.755/pypki3/README.md
+-rw-r--r--   0        0        0      343 2023-02-04 12:34:57.703791 pypki3-2023.35.755/pypki3/__init__.py
+-rw-r--r--   0        0        0    13324 2023-02-04 12:34:57.703791 pypki3-2023.35.755/pypki3/config.py
+-rw-r--r--   0        0        0       43 2023-02-04 12:34:57.703791 pypki3-2023.35.755/pypki3/exceptions.py
+-rw-r--r--   0        0        0      428 2023-02-04 12:34:57.703791 pypki3-2023.35.755/pypki3/utils.py
+-rw-r--r--   0        0        0      827 2023-02-04 12:35:15.123934 pypki3-2023.35.755/pyproject.toml
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 pypki3-2023.35.755/setup.py
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 pypki3-2023.35.755/PKG-INFO
```

### Comparing `pypki3-2023.111.38/LICENSE` & `pypki3-2023.35.755/LICENSE`

 * *Files identical despite different names*

### Comparing `pypki3-2023.111.38/README.md` & `pypki3-2023.35.755/README.md`

 * *Files identical despite different names*

### Comparing `pypki3-2023.111.38/pypki3/config.py` & `pypki3-2023.35.755/pypki3/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         a password if the certificate is encrypted.
         '''
         ContextManagerClass = CreateNamedTemporaryKeyCertPathsContextManager(self)
 
         with ContextManagerClass(password) as key_cert_paths:
             key_path = key_cert_paths[0]
             cert_path = key_cert_paths[1]
-            context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLS_CLIENT)
+            context = ssl.SSLContext()
             context.load_cert_chain(cert_path, key_path)
             context.verify_mode = ssl.CERT_REQUIRED
             context.load_verify_locations(cafile=self.ca_path())
             return context
 
     def pip(self, *args, **kwargs):
         new_args = []
```

### Comparing `pypki3-2023.111.38/pyproject.toml` & `pypki3-2023.35.755/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry]
 authors = ["Bill Allen <billallen256@gmail.com>"]
 description = "More user-friendly way to access PKI-enabled services."
 homepage = "http://github.com/nbgallery/pypki3"
 license = "MIT"
 name = "pypki3"
 readme = "README.md"
-version = "2023.111.38"
+version = "2023.35.755"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 cryptography = "*"
 pem = "*"
 temppath = "*"
```

### Comparing `pypki3-2023.111.38/PKG-INFO` & `pypki3-2023.35.755/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypki3
-Version: 2023.111.38
+Version: 2023.35.755
 Summary: More user-friendly way to access PKI-enabled services.
 Home-page: http://github.com/nbgallery/pypki3
 License: MIT
 Author: Bill Allen
 Author-email: billallen256@gmail.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
```

