# Comparing `tmp/crypt-dir-1.1.7.tar.gz` & `tmp/crypt-dir-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypt-dir-1.1.7.tar", last modified: Sat Apr  8 11:46:21 2023, max compression
+gzip compressed data, was "crypt-dir-1.1.8.tar", last modified: Fri Apr 21 09:10:19 2023, max compression
```

## Comparing `crypt-dir-1.1.7.tar` & `crypt-dir-1.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-08 11:46:21.423169 crypt-dir-1.1.7/
--rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-03-31 12:34:48.000000 crypt-dir-1.1.7/LICENSE
--rw-r--r--   0 khanh      (501) staff       (20)     3764 2023-04-08 11:46:21.423008 crypt-dir-1.1.7/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)     3506 2023-04-06 16:16:43.000000 crypt-dir-1.1.7/README.md
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-08 11:46:21.421984 crypt-dir-1.1.7/crypt_dir/
--rw-r--r--   0 khanh      (501) staff       (20)      181 2023-04-08 11:45:56.000000 crypt-dir-1.1.7/crypt_dir/__init__.py
--rw-r--r--   0 khanh      (501) staff       (20)     2751 2023-04-08 11:45:00.000000 crypt-dir-1.1.7/crypt_dir/crypt.py
--rw-r--r--   0 khanh      (501) staff       (20)     6101 2023-04-06 16:56:20.000000 crypt-dir-1.1.7/crypt_dir/crypt_dir.py
--rw-r--r--   0 khanh      (501) staff       (20)     4075 2023-04-07 17:36:26.000000 crypt-dir-1.1.7/crypt_dir/crypt_file.py
--rw-r--r--   0 khanh      (501) staff       (20)      257 2023-04-06 15:59:40.000000 crypt-dir-1.1.7/crypt_dir/serialize.py
--rw-r--r--   0 khanh      (501) staff       (20)      805 2023-04-06 16:03:15.000000 crypt-dir-1.1.7/crypt_dir/signature.py
-drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-08 11:46:21.422803 crypt-dir-1.1.7/crypt_dir.egg-info/
--rw-r--r--   0 khanh      (501) staff       (20)     3764 2023-04-08 11:46:21.000000 crypt-dir-1.1.7/crypt_dir.egg-info/PKG-INFO
--rw-r--r--   0 khanh      (501) staff       (20)      324 2023-04-08 11:46:21.000000 crypt-dir-1.1.7/crypt_dir.egg-info/SOURCES.txt
--rw-r--r--   0 khanh      (501) staff       (20)        1 2023-04-08 11:46:21.000000 crypt-dir-1.1.7/crypt_dir.egg-info/dependency_links.txt
--rw-r--r--   0 khanh      (501) staff       (20)       20 2023-04-08 11:46:21.000000 crypt-dir-1.1.7/crypt_dir.egg-info/requires.txt
--rw-r--r--   0 khanh      (501) staff       (20)       10 2023-04-08 11:46:21.000000 crypt-dir-1.1.7/crypt_dir.egg-info/top_level.txt
--rw-r--r--   0 khanh      (501) staff       (20)       38 2023-04-08 11:46:21.423220 crypt-dir-1.1.7/setup.cfg
--rw-r--r--   0 khanh      (501) staff       (20)      586 2023-04-08 11:46:16.000000 crypt-dir-1.1.7/setup.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.108338 crypt-dir-1.1.8/
+-rw-r--r--   0 khanh      (501) staff       (20)     1069 2023-03-31 12:34:48.000000 crypt-dir-1.1.8/LICENSE
+-rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-21 09:10:19.108204 crypt-dir-1.1.8/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)     4158 2023-04-09 16:58:00.000000 crypt-dir-1.1.8/README.md
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.107249 crypt-dir-1.1.8/crypt_dir/
+-rw-r--r--   0 khanh      (501) staff       (20)      181 2023-04-08 11:45:56.000000 crypt-dir-1.1.8/crypt_dir/__init__.py
+-rw-r--r--   0 khanh      (501) staff       (20)     2748 2023-04-09 15:05:50.000000 crypt-dir-1.1.8/crypt_dir/crypt.py
+-rw-r--r--   0 khanh      (501) staff       (20)     6101 2023-04-06 16:56:20.000000 crypt-dir-1.1.8/crypt_dir/crypt_dir.py
+-rw-r--r--   0 khanh      (501) staff       (20)     4075 2023-04-07 17:36:26.000000 crypt-dir-1.1.8/crypt_dir/crypt_file.py
+-rw-r--r--   0 khanh      (501) staff       (20)      257 2023-04-06 15:59:40.000000 crypt-dir-1.1.8/crypt_dir/serialize.py
+-rw-r--r--   0 khanh      (501) staff       (20)      805 2023-04-06 16:03:15.000000 crypt-dir-1.1.8/crypt_dir/signature.py
+drwxr-xr-x   0 khanh      (501) staff       (20)        0 2023-04-21 09:10:19.108011 crypt-dir-1.1.8/crypt_dir.egg-info/
+-rw-r--r--   0 khanh      (501) staff       (20)     4407 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/PKG-INFO
+-rw-r--r--   0 khanh      (501) staff       (20)      324 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh      (501) staff       (20)        1 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       20 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/requires.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       10 2023-04-21 09:10:19.000000 crypt-dir-1.1.8/crypt_dir.egg-info/top_level.txt
+-rw-r--r--   0 khanh      (501) staff       (20)       38 2023-04-21 09:10:19.108383 crypt-dir-1.1.8/setup.cfg
+-rw-r--r--   0 khanh      (501) staff       (20)      577 2023-04-21 09:09:52.000000 crypt-dir-1.1.8/setup.py
```

### Comparing `crypt-dir-1.1.7/LICENSE` & `crypt-dir-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.7/PKG-INFO` & `crypt-dir-1.1.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: crypt-dir
-Version: 1.1.7
-Home-page: https://github.com/khanh-nguyen-code/crypt-dir
-Author: Nguyen Ngoc Khanh
-Author-email: khanh.nguyen.contact@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CRYPT_DIR
 
 - Encrypt all your files and write into another directory if there is update
 - Clean the encrypted directory if files or directories have been deleted
 - Restore
 - Minimize writing to SSDs
 
@@ -60,14 +50,36 @@
     key=key,
     encrypted_dir=encrypted_dir,
     restored_dir=restored_dir,
     max_workers=12,
 )
 ```
 
+- certificate
+
+```python
+import crypt_dir
+
+correct_password = b"password123"
+
+cert = crypt_dir.make_certificate(correct_password)
+print("cert", cert)
+
+try:
+    wrong_password = b"password456"
+    _ = crypt_dir.verify_certificate(cert, wrong_password)
+except AssertionError as e:
+    print("expected assertion error: ", e)
+
+key = crypt_dir.verify_certificate(cert, correct_password)
+
+print("generated key from correct password", key)
+
+```
+
 # INSTALLATION
 
 ```shell
 pip install --upgrade crypt-dir
 ```
 
 # DECRYPT IT YOURSELF
@@ -92,17 +104,20 @@
         - `key_sig`: `SHA1` bytes of key
         - `file_size`: little-endian encoded file size in uint64
         - `init_vec`: `AES256` initialization vector
 
     - `file encrypted`: `AES256` file encrypted bytes with chunk size of `2^30`
 
 ```
-|                                      header                            |   encrypted_data  |
-|   file_sig         |   key_sig         |   file_size   |   init_vec    |   encrypted_data  |
-|   8 bytes          |   20 bytes        |   8 bytes     |   16 bytes    |   n bytes         |
+__________________________________________________________________________________
+|                          header                           |   encrypted_data   |
+|___________________________________________________________|____________________|
+|   file_sig   |   key_sig   |   file_size   |   init_vec   |   encrypted_data   |
+|   8 bytes    |   20 bytes  |   8 bytes     |   16 bytes   |   n bytes          |
+|___________________________________________________________|____________________|
 ```
 
 ## SPECIFICATION 0.*
 
 You don't need to know the specification. For some folks who want to know exactly what happened with their files, here
 is the specification for `key_file` and `.enc` files:
```

### Comparing `crypt-dir-1.1.7/README.md` & `crypt-dir-1.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: crypt-dir
+Version: 1.1.8
+Home-page: https://github.com/khanh101/crypt-dir
+Author: Nguyen Ngoc Khanh
+Author-email: khanh.nguyen.contact@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CRYPT_DIR
 
 - Encrypt all your files and write into another directory if there is update
 - Clean the encrypted directory if files or directories have been deleted
 - Restore
 - Minimize writing to SSDs
 
@@ -50,14 +60,36 @@
     key=key,
     encrypted_dir=encrypted_dir,
     restored_dir=restored_dir,
     max_workers=12,
 )
 ```
 
+- certificate
+
+```python
+import crypt_dir
+
+correct_password = b"password123"
+
+cert = crypt_dir.make_certificate(correct_password)
+print("cert", cert)
+
+try:
+    wrong_password = b"password456"
+    _ = crypt_dir.verify_certificate(cert, wrong_password)
+except AssertionError as e:
+    print("expected assertion error: ", e)
+
+key = crypt_dir.verify_certificate(cert, correct_password)
+
+print("generated key from correct password", key)
+
+```
+
 # INSTALLATION
 
 ```shell
 pip install --upgrade crypt-dir
 ```
 
 # DECRYPT IT YOURSELF
@@ -82,17 +114,20 @@
         - `key_sig`: `SHA1` bytes of key
         - `file_size`: little-endian encoded file size in uint64
         - `init_vec`: `AES256` initialization vector
 
     - `file encrypted`: `AES256` file encrypted bytes with chunk size of `2^30`
 
 ```
-|                                      header                            |   encrypted_data  |
-|   file_sig         |   key_sig         |   file_size   |   init_vec    |   encrypted_data  |
-|   8 bytes          |   20 bytes        |   8 bytes     |   16 bytes    |   n bytes         |
+__________________________________________________________________________________
+|                          header                           |   encrypted_data   |
+|___________________________________________________________|____________________|
+|   file_sig   |   key_sig   |   file_size   |   init_vec   |   encrypted_data   |
+|   8 bytes    |   20 bytes  |   8 bytes     |   16 bytes   |   n bytes          |
+|___________________________________________________________|____________________|
 ```
 
 ## SPECIFICATION 0.*
 
 You don't need to know the specification. For some folks who want to know exactly what happened with their files, here
 is the specification for `key_file` and `.enc` files:
```

### Comparing `crypt-dir-1.1.7/crypt_dir/crypt.py` & `crypt-dir-1.1.8/crypt_dir/crypt.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,24 +76,24 @@
     key = hash[:KEY_SIZE]
     return key
 
 
 @dataclass
 class Certificate:
     salt: bytes
-    key_hash: bytes
+    key_sig: bytes
 
 
 def verify_certificate(cert: Certificate, password: bytes) -> bytes:
     password_with_salt = cert.salt + password
     key = make_key_from_password(password_with_salt)
     key_hash = sha1_hash(io.BytesIO(key))
-    assert key_hash == cert.key_hash, "password_does_not_match"
+    assert key_hash == cert.key_sig, "password_does_not_match"
     return key
 
 
 def make_certificate(password: bytes) -> Certificate:
     salt = os.urandom(SALT_SIZE)
     password_with_salt = salt + password
     key = make_key_from_password(password_with_salt)
     key_hash = sha1_hash(io.BytesIO(key))
-    return Certificate(salt=salt, key_hash=key_hash)
+    return Certificate(salt=salt, key_sig=key_hash)
```

### Comparing `crypt-dir-1.1.7/crypt_dir/crypt_dir.py` & `crypt-dir-1.1.8/crypt_dir/crypt_dir.py`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.7/crypt_dir/crypt_file.py` & `crypt-dir-1.1.8/crypt_dir/crypt_file.py`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.7/crypt_dir/signature.py` & `crypt-dir-1.1.8/crypt_dir/signature.py`

 * *Files identical despite different names*

### Comparing `crypt-dir-1.1.7/crypt_dir.egg-info/PKG-INFO` & `crypt-dir-1.1.8/crypt_dir.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crypt-dir
-Version: 1.1.7
-Home-page: https://github.com/khanh-nguyen-code/crypt-dir
+Version: 1.1.8
+Home-page: https://github.com/khanh101/crypt-dir
 Author: Nguyen Ngoc Khanh
 Author-email: khanh.nguyen.contact@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CRYPT_DIR
@@ -60,14 +60,36 @@
     key=key,
     encrypted_dir=encrypted_dir,
     restored_dir=restored_dir,
     max_workers=12,
 )
 ```
 
+- certificate
+
+```python
+import crypt_dir
+
+correct_password = b"password123"
+
+cert = crypt_dir.make_certificate(correct_password)
+print("cert", cert)
+
+try:
+    wrong_password = b"password456"
+    _ = crypt_dir.verify_certificate(cert, wrong_password)
+except AssertionError as e:
+    print("expected assertion error: ", e)
+
+key = crypt_dir.verify_certificate(cert, correct_password)
+
+print("generated key from correct password", key)
+
+```
+
 # INSTALLATION
 
 ```shell
 pip install --upgrade crypt-dir
 ```
 
 # DECRYPT IT YOURSELF
@@ -92,17 +114,20 @@
         - `key_sig`: `SHA1` bytes of key
         - `file_size`: little-endian encoded file size in uint64
         - `init_vec`: `AES256` initialization vector
 
     - `file encrypted`: `AES256` file encrypted bytes with chunk size of `2^30`
 
 ```
-|                                      header                            |   encrypted_data  |
-|   file_sig         |   key_sig         |   file_size   |   init_vec    |   encrypted_data  |
-|   8 bytes          |   20 bytes        |   8 bytes     |   16 bytes    |   n bytes         |
+__________________________________________________________________________________
+|                          header                           |   encrypted_data   |
+|___________________________________________________________|____________________|
+|   file_sig   |   key_sig   |   file_size   |   init_vec   |   encrypted_data   |
+|   8 bytes    |   20 bytes  |   8 bytes     |   16 bytes   |   n bytes          |
+|___________________________________________________________|____________________|
 ```
 
 ## SPECIFICATION 0.*
 
 You don't need to know the specification. For some folks who want to know exactly what happened with their files, here
 is the specification for `key_file` and `.enc` files:
```

### Comparing `crypt-dir-1.1.7/setup.py` & `crypt-dir-1.1.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 if __name__ == "__main__":
     with open("README.md") as f:
         long_description = f.read()
     setuptools.setup(
         name="crypt-dir",
-        version="1.1.7",
+        version="1.1.8",
         author="Nguyen Ngoc Khanh",
         author_email="khanh.nguyen.contact@gmail.com",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        url="https://github.com/khanh-nguyen-code/crypt-dir",
+        url="https://github.com/khanh101/crypt-dir",
         packages=setuptools.find_packages(),
         license="MIT",
         install_requires=[
             "pycryptodomex==3.17",
         ],
     )
```

