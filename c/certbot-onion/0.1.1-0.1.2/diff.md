# Comparing `tmp/certbot-onion-0.1.1.tar.gz` & `tmp/certbot-onion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.1.tar", last modified: Thu Apr 20 23:05:25 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.2.tar", last modified: Fri Apr 21 11:38:08 2023, max compression
```

## Comparing `certbot-onion-0.1.1.tar` & `certbot-onion-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,24 @@
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.031373 certbot-onion-0.1.1/
--rw-r--r--   0 q          (501) staff       (20)     1075 2023-04-20 20:46:39.000000 certbot-onion-0.1.1/LICENSE.md
--rw-r--r--   0 q          (501) staff       (20)      199 2023-04-20 21:02:59.000000 certbot-onion-0.1.1/MANIFEST.in
--rw-r--r--   0 q          (501) staff       (20)     1522 2023-04-20 23:05:25.031258 certbot-onion-0.1.1/PKG-INFO
--rw-r--r--   0 q          (501) staff       (20)     1159 2023-04-20 23:03:27.000000 certbot-onion-0.1.1/README.md
--rw-r--r--   0 q          (501) staff       (20)      729 2023-04-20 23:05:07.000000 certbot-onion-0.1.1/pyproject.toml
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.024973 certbot-onion-0.1.1/rust/
--rw-r--r--   0 q          (501) staff       (20)    17302 2023-04-20 17:54:56.000000 certbot-onion-0.1.1/rust/Cargo.lock
--rw-r--r--   0 q          (501) staff       (20)      381 2023-04-20 17:43:25.000000 certbot-onion-0.1.1/rust/Cargo.toml
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.025231 certbot-onion-0.1.1/rust/src/
--rw-r--r--   0 q          (501) staff       (20)     2829 2023-04-20 18:18:12.000000 certbot-onion-0.1.1/rust/src/lib.rs
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.022820 certbot-onion-0.1.1/rust/target/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.022884 certbot-onion-0.1.1/rust/target/debug/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023100 certbot-onion-0.1.1/rust/target/debug/build/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023008 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.025514 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/
--rw-r--r--   0 q          (501) staff       (20)     1844 2023-04-20 17:02:25.000000 certbot-onion-0.1.1/rust/target/debug/build/target-lexicon-6729fb3681a2ca35/out/host.rs
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023163 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.027470 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/
--rw-r--r--   0 q          (501) staff       (20)   217663 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/consts.rs
--rw-r--r--   0 q          (501) staff       (20)    45992 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/op.rs
--rw-r--r--   0 q          (501) staff       (20)   622662 2023-04-20 17:02:26.000000 certbot-onion-0.1.1/rust/target/debug/build/typenum-84ff2b94b30974f3/out/tests.rs
--rw-r--r--   0 q          (501) staff       (20)       38 2023-04-20 23:05:25.031413 certbot-onion-0.1.1/setup.cfg
--rw-r--r--   0 q          (501) staff       (20)      286 2023-04-20 17:02:11.000000 certbot-onion-0.1.1/setup.py
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.023386 certbot-onion-0.1.1/src/
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.029953 certbot-onion-0.1.1/src/certbot_onion/
--rw-r--r--   0 q          (501) staff       (20)     3861 2023-04-20 18:26:40.000000 certbot-onion-0.1.1/src/certbot_onion/__init__.py
-drwxr-xr-x   0 q          (501) staff       (20)        0 2023-04-20 23:05:25.031082 certbot-onion-0.1.1/src/certbot_onion.egg-info/
--rw-r--r--   0 q          (501) staff       (20)     1522 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 q          (501) staff       (20)      674 2023-04-20 23:05:25.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 q          (501) staff       (20)       58 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 q          (501) staff       (20)        1 2023-04-20 17:01:57.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 q          (501) staff       (20)        8 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 q          (501) staff       (20)       14 2023-04-20 23:05:24.000000 certbot-onion-0.1.1/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)    17302 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.054533 certbot-onion-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.058534 certbot-onion-0.1.2/src/certbot_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-21 11:37:57.000000 certbot-onion-0.1.2/src/certbot_onion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:38:08.062534 certbot-onion-0.1.2/src/certbot_onion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:38:07.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 11:38:08.000000 certbot-onion-0.1.2/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.1/LICENSE.md` & `certbot-onion-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.1/PKG-INFO` & `certbot-onion-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `certbot-onion-0.1.1/README.md` & `certbot-onion-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.1/pyproject.toml` & `certbot-onion-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "certbot-onion"
-version = "0.1.1"
+version = "0.1.2"
 description = "Certbot authenticator plugin for the onion-csr-01 challenge"
 authors = [
     {name = "Q Misell", email = "q@as207960.net"}
 ]
 license = {text = "MIT"}
 dependencies = [
     "certbot"
@@ -12,20 +12,23 @@
 readme = "README.md"
 
 [project.urls]
 "Homepage" = "https://acmeforonions.org"
 "Bug Tracker" = "https://github.com/AS207960/certbot-onion"
 
 [build-system]
-requires = ["setuptools>=61.0.0", "wheel", "setuptools-rust"]
+requires = ["setuptools", "wheel", "setuptools-rust"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["certbot_onion*"]
 
 [tool.setuptools]
 zip-safe = false
 package-dir = {"" = "src"}
 
 [project.entry-points."certbot.plugins"]
-onion-csr = "certbot_onion:Authenticator"
+onion-csr = "certbot_onion:Authenticator"
+
+[tool.cibuildwheel]
+before-all = "curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y"
```

### Comparing `certbot-onion-0.1.1/rust/Cargo.lock` & `certbot-onion-0.1.2/rust/Cargo.lock`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.1/rust/src/lib.rs` & `certbot-onion-0.1.2/rust/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -63,18 +63,14 @@
             Ok(())
         }))
     }).unwrap();
 
     Ok(req)
 }
 
-fn encode_asn1_bit_string(data: &[u8]) -> Vec<u8> {
-    asn1::write_single(&asn1::BitString::new(data, 0)).unwrap()
-}
-
 extern "C" {
     fn i2d_re_X509_REQ_tbs(req: *const openssl_sys::X509_REQ, buf: *mut *mut u8) -> libc::c_int;
     fn X509_REQ_add1_attr_by_txt(
         req: *const openssl_sys::X509_REQ, attr_name: *const u8, attr_type: libc::c_int,
         bytes: *const u8, len: libc::c_int
     ) -> libc::c_int;
 }
```

### Comparing `certbot-onion-0.1.1/src/certbot_onion/__init__.py` & `certbot-onion-0.1.2/src/certbot_onion/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.1/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.2/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

