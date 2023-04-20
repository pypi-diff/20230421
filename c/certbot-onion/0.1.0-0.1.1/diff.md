# Comparing `tmp/certbot-onion-0.1.0.tar.gz` & `tmp/certbot-onion-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.0.tar", last modified: Thu Apr 20 21:03:05 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.1.tar", last modified: Thu Apr 20 23:05:25 2023, max compression
```

## Comparing `certbot-onion-0.1.0.tar` & `certbot-onion-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.036007 certbot-onion-0.1.0/
--rw-r--r--   0 q          (501) staff       (20)     1075 2023-04-20 20:46:39.000000 certbot-onion-0.1.0/LICENSE.md
--rw-r--r--   0 q          (501) staff       (20)      199 2023-04-20 21:02:59.000000 certbot-onion-0.1.0/MANIFEST.in
--rw-r--r--   0 q          (501) staff       (20)     1531 2023-04-20 21:03:05.035866 certbot-onion-0.1.0/PKG-INFO
--rw-r--r--   0 q          (501) staff       (20)     1168 2023-04-20 20:58:56.000000 certbot-onion-0.1.0/README.md
--rw-r--r--   0 q          (501) staff       (20)      729 2023-04-20 20:46:06.000000 certbot-onion-0.1.0/pyproject.toml
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.023994 certbot-onion-0.1.0/rust/
--rw-r--r--   0 q          (501) staff       (20)    17302 2023-04-20 17:54:56.000000 certbot-onion-0.1.0/rust/Cargo.lock
--rw-r--r--   0 q          (501) staff       (20)      381 2023-04-20 17:43:25.000000 certbot-onion-0.1.0/rust/Cargo.toml
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.024358 certbot-onion-0.1.0/rust/src/
--rw-r--r--   0 q          (501) staff       (20)     2829 2023-04-20 18:18:12.000000 certbot-onion-0.1.0/rust/src/lib.rs
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.020931 certbot-onion-0.1.0/rust/target/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.021044 certbot-onion-0.1.0/rust/target/debug/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.021530 certbot-onion-0.1.0/rust/target/debug/build/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.021278 certbot-onion-0.1.0/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.024652 certbot-onion-0.1.0/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/
--rw-r--r--   0 q          (501) staff       (20)     1844 2023-04-20 17:02:25.000000 certbot-onion-0.1.0/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/host.rs
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.021674 certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.027521 certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/
--rw-r--r--   0 q          (501) staff       (20)   217663 2023-04-20 17:02:26.000000 certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/consts.rs
--rw-r--r--   0 q          (501) staff       (20)    45992 2023-04-20 17:02:26.000000 certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/op.rs
--rw-r--r--   0 q          (501) staff       (20)   622662 2023-04-20 17:02:26.000000 certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/tests.rs
--rw-r--r--   0 q          (501) staff       (20)       38 2023-04-20 21:03:05.036053 certbot-onion-0.1.0/setup.cfg
--rw-r--r--   0 q          (501) staff       (20)      286 2023-04-20 17:02:11.000000 certbot-onion-0.1.0/setup.py
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.022019 certbot-onion-0.1.0/src/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.034353 certbot-onion-0.1.0/src/certbot_onion/
--rw-r--r--   0 q          (501) staff       (20)     3861 2023-04-20 18:26:40.000000 certbot-onion-0.1.0/src/certbot_onion/__init__.py
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 21:03:05.035678 certbot-onion-0.1.0/src/certbot_onion.egg-info/
--rw-r--r--   0 q          (501) staff       (20)     1531 2023-04-20 21:03:04.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 q          (501) staff       (20)      674 2023-04-20 21:03:05.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 21:03:04.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 q          (501) staff       (20)       58 2023-04-20 21:03:04.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 17:01:57.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 q          (501) staff       (20)        8 2023-04-20 21:03:04.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 q          (501) staff       (20)       14 2023-04-20 21:03:04.000000 certbot-onion-0.1.0/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.031373 certbot-onion-0.1.1/
+-rw-r--r--   0 q          (501) staff       (20)     1075 2023-04-20 20:46:39.000000 certbot-onion-0.1.1/LICENSE.md
+-rw-r--r--   0 q          (501) staff       (20)      199 2023-04-20 21:02:59.000000 certbot-onion-0.1.1/MANIFEST.in
+-rw-r--r--   0 q          (501) staff       (20)     1522 2023-04-20 23:05:25.031258 certbot-onion-0.1.1/PKG-INFO
+-rw-r--r--   0 q          (501) staff       (20)     1159 2023-04-20 23:03:27.000000 certbot-onion-0.1.1/README.md
+-rw-r--r--   0 q          (501) staff       (20)      729 2023-04-20 23:05:07.000000 certbot-onion-0.1.1/pyproject.toml
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.024973 certbot-onion-0.1.1/rust/
+-rw-r--r--   0 q          (501) staff       (20)    17302 2023-04-20 17:54:56.000000 certbot-onion-0.1.1/rust/Cargo.lock
+-rw-r--r--   0 q          (501) staff       (20)      381 2023-04-20 17:43:25.000000 certbot-onion-0.1.1/rust/Cargo.toml
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.025231 certbot-onion-0.1.1/rust/src/
+-rw-r--r--   0 q          (501) staff       (20)     2829 2023-04-20 18:18:12.000000 certbot-onion-0.1.1/rust/src/lib.rs
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.022820 certbot-onion-0.1.1/rust/target/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.022884 certbot-onion-0.1.1/rust/target/debug/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023100 certbot-onion-0.1.1/rust/target/debug/build/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023008 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.025514 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/
+-rw-r--r--   0 q          (501) staff       (20)     1844 2023-04-20 17:02:25.000000 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/host.rs
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023163 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.027470 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/
+-rw-r--r--   0 q          (501) staff       (20)   217663 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/consts.rs
+-rw-r--r--   0 q          (501) staff       (20)    45992 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/op.rs
+-rw-r--r--   0 q          (501) staff       (20)   622662 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/tests.rs
+-rw-r--r--   0 q          (501) staff       (20)       38 2023-04-20 23:05:25.031413 certbot-onion-0.1.1/setup.cfg
+-rw-r--r--   0 q          (501) staff       (20)      286 2023-04-20 17:02:11.000000 certbot-onion-0.1.1/setup.py
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023386 certbot-onion-0.1.1/src/
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.029953 certbot-onion-0.1.1/src/certbot_onion/
+-rw-r--r--   0 q          (501) staff       (20)     3861 2023-04-20 18:26:40.000000 certbot-onion-0.1.1/src/certbot_onion/__init__.py
+drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.031082 certbot-onion-0.1.1/src/certbot_onion.egg-info/
+-rw-r--r--   0 q          (501) staff       (20)     1522 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 q          (501) staff       (20)      674 2023-04-20 23:05:25.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 q          (501) staff       (20)       58 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 17:01:57.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 q          (501) staff       (20)        8 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 q          (501) staff       (20)       14 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.0/LICENSE.md` & `certbot-onion-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/PKG-INFO` & `certbot-onion-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.0
+Version: 0.1.1
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# certbot-dns-ispconfig
+# certbot-onion
 
 `onion-csr-01` Authenticator plugin for Certbot
 
-This process allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
+This plugin allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
 signing the request with the key of the hidden service.
 
 ## Installation
 
 ```shell
 pip install certbot-onion
 ```
```

### Comparing `certbot-onion-0.1.0/README.md` & `certbot-onion-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# certbot-dns-ispconfig
+# certbot-onion
 
 `onion-csr-01` Authenticator plugin for Certbot
 
-This process allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
+This plugin allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
 signing the request with the key of the hidden service.
 
 ## Installation
 
 ```shell
 pip install certbot-onion
 ```
```

### Comparing `certbot-onion-0.1.0/pyproject.toml` & `certbot-onion-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "certbot-onion"
-version = "0.1.0"
+version = "0.1.1"
 description = "Certbot authenticator plugin for the onion-csr-01 challenge"
 authors = [
     {name = "Q Misell", email = "q@as207960.net"}
 ]
 license = {text = "MIT"}
 dependencies = [
     "certbot"
```

### Comparing `certbot-onion-0.1.0/rust/Cargo.lock` & `certbot-onion-0.1.1/rust/Cargo.lock`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/rust/src/lib.rs` & `certbot-onion-0.1.1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/host.rs` & `certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/host.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/consts.rs` & `certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/consts.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/op.rs` & `certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/op.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/rust/target/debug/build/typenum-84ff2b94b30974f3/out/tests.rs` & `certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/tests.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/src/certbot_onion/__init__.py` & `certbot-onion-0.1.1/src/certbot_onion/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.0/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.1/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.0
+Version: 0.1.1
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# certbot-dns-ispconfig
+# certbot-onion
 
 `onion-csr-01` Authenticator plugin for Certbot
 
-This process allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
+This plugin allows certbot to request certificates for `.onion` domains using the `onion-csr-01` challenge type,
 signing the request with the key of the hidden service.
 
 ## Installation
 
 ```shell
 pip install certbot-onion
 ```
```

### Comparing `certbot-onion-0.1.0/src/certbot_onion.egg-info/SOURCES.txt` & `certbot-onion-0.1.1/src/certbot_onion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

