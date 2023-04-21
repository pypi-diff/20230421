# Comparing `tmp/nh3-0.2.8.tar.gz` & `tmp/nh3-0.2.9.tar.gz`

## Comparing `nh3-0.2.8.tar` & `nh3-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 nh3-0.2.8/Cargo.toml
--rw-r--r--   0      501       20       17 2023-02-08 08:49:58.000000 nh3-0.2.8/.github/FUNDING.yml
--rw-r--r--   0      501       20      504 2023-02-08 08:49:58.000000 nh3-0.2.8/.github/dependabot.yml
--rw-r--r--   0      501       20     6383 2023-02-08 08:49:58.000000 nh3-0.2.8/.github/workflows/CI.yml
--rw-r--r--   0      501       20      652 2023-02-08 08:49:58.000000 nh3-0.2.8/.gitignore
--rw-r--r--   0      501       20      334 2023-02-08 08:49:58.000000 nh3-0.2.8/.readthedocs.yml
--rw-r--r--   0      501       20     1086 2023-02-08 08:49:58.000000 nh3-0.2.8/LICENSE
--rw-r--r--   0      501       20     1255 2023-02-08 08:49:58.000000 nh3-0.2.8/README.md
--rw-r--r--   0      501       20      634 2023-02-08 08:49:58.000000 nh3-0.2.8/docs/Makefile
--rw-r--r--   0      501       20     1961 2023-02-08 08:49:58.000000 nh3-0.2.8/docs/conf.py
--rw-r--r--   0      501       20      473 2023-02-08 08:49:58.000000 nh3-0.2.8/docs/index.rst
--rw-r--r--   0      501       20      800 2023-02-08 08:49:58.000000 nh3-0.2.8/docs/make.bat
--rw-r--r--   0      501       20      557 2023-02-08 08:49:58.000000 nh3-0.2.8/docs/requirements.txt
--rw-r--r--   0      501       20      526 2023-02-08 08:49:58.000000 nh3-0.2.8/nh3.pyi
--rw-r--r--   0      501       20       76 2023-02-08 08:49:58.000000 nh3-0.2.8/pyproject.toml
--rw-r--r--   0      501       20     7315 2023-02-08 08:49:58.000000 nh3-0.2.8/src/lib.rs
--rw-r--r--   0      501       20     1889 2023-02-08 08:49:58.000000 nh3-0.2.8/tests/test_nh3.py
--rw-r--r--   0      501       20    15267 2023-02-08 08:49:58.000000 nh3-0.2.8/Cargo.lock
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 nh3-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 nh3-0.2.9/Cargo.toml
+-rw-r--r--   0      501       20       17 2023-03-25 01:27:35.000000 nh3-0.2.9/.github/FUNDING.yml
+-rw-r--r--   0      501       20      504 2023-03-25 01:27:35.000000 nh3-0.2.9/.github/dependabot.yml
+-rw-r--r--   0      501       20     6383 2023-03-25 01:27:35.000000 nh3-0.2.9/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      652 2023-03-25 01:27:35.000000 nh3-0.2.9/.gitignore
+-rw-r--r--   0      501       20      334 2023-03-25 01:27:35.000000 nh3-0.2.9/.readthedocs.yml
+-rw-r--r--   0      501       20     1086 2023-03-25 01:27:35.000000 nh3-0.2.9/LICENSE
+-rw-r--r--   0      501       20     1255 2023-03-25 01:27:35.000000 nh3-0.2.9/README.md
+-rw-r--r--   0      501       20      634 2023-03-25 01:27:35.000000 nh3-0.2.9/docs/Makefile
+-rw-r--r--   0      501       20     1964 2023-03-25 01:27:35.000000 nh3-0.2.9/docs/conf.py
+-rw-r--r--   0      501       20      473 2023-03-25 01:27:35.000000 nh3-0.2.9/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-03-25 01:27:35.000000 nh3-0.2.9/docs/make.bat
+-rw-r--r--   0      501       20      560 2023-03-25 01:27:35.000000 nh3-0.2.9/docs/requirements.txt
+-rw-r--r--   0      501       20      526 2023-03-25 01:27:35.000000 nh3-0.2.9/nh3.pyi
+-rw-r--r--   0      501       20       76 2023-03-25 01:27:35.000000 nh3-0.2.9/pyproject.toml
+-rw-r--r--   0      501       20     7315 2023-03-25 01:27:35.000000 nh3-0.2.9/src/lib.rs
+-rw-r--r--   0      501       20     1889 2023-03-25 01:27:35.000000 nh3-0.2.9/tests/test_nh3.py
+-rw-r--r--   0      501       20    15267 2023-03-25 01:27:35.000000 nh3-0.2.9/Cargo.lock
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 nh3-0.2.9/PKG-INFO
```

### Comparing `nh3-0.2.8/.github/workflows/CI.yml` & `nh3-0.2.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/.gitignore` & `nh3-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/LICENSE` & `nh3-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/README.md` & `nh3-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/docs/Makefile` & `nh3-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/docs/conf.py` & `nh3-0.2.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'furo'
+html_theme = 'shibuya'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 pygments_style = "xcode"
```

### Comparing `nh3-0.2.8/docs/make.bat` & `nh3-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/docs/requirements.txt` & `nh3-0.2.9/docs/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 alabaster==0.7.13
 Babel==2.11.0
 beautifulsoup4==4.11.1
 certifi==2022.12.7
 charset-normalizer==3.0.1
 docutils==0.19
-furo==2022.12.7
 idna==3.4
 imagesize==1.4.1
 Jinja2==3.1.2
 MarkupSafe==2.1.2
 maturin==0.14.10
 packaging==23.0
 Pygments==2.14.0
 pytz==2022.7.1
 requests==2.28.2
+shibuya==2023.3.19
 snowballstemmer==2.2.0
 soupsieve==2.3.2.post1
 Sphinx==6.1.3
 sphinx-basic-ng==1.0.0b1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
```

### Comparing `nh3-0.2.8/nh3.pyi` & `nh3-0.2.9/nh3.pyi`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/src/lib.rs` & `nh3-0.2.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/tests/test_nh3.py` & `nh3-0.2.9/tests/test_nh3.py`

 * *Files identical despite different names*

### Comparing `nh3-0.2.8/Cargo.lock` & `nh3-0.2.9/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.140"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -157,25 +157,25 @@
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
 name = "nh3"
-version = "0.2.8"
+version = "0.2.9"
 dependencies = [
  "ammonia",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -250,86 +250,86 @@
 name = "precomputed-hash"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "925383efa346730478fb4838dbe9137d2a47675ad789c546d150a6e1dd4ab31c"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "ba466839c78239c09faf015484e5cc04860f88242cff4d03eb038f04b4699b73"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -373,17 +373,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.158"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
 
 [[package]]
 name = "siphasher"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
 
@@ -391,17 +391,17 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "string_cache"
-version = "0.8.4"
+version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213494b7a2b503146286049378ce02b482200519accc31872ee8be91fa820a08"
+checksum = "f91138e76242f575eb1d3b38b4f1362f10d3a43f47d182a5b359af488a02293b"
 dependencies = [
  "new_debug_unreachable",
  "once_cell",
  "parking_lot",
  "phf_shared",
  "precomputed-hash",
  "serde",
@@ -417,28 +417,28 @@
  "phf_shared",
  "proc-macro2",
  "quote",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tendril"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d24a120c5fc464a3458240ee02c299ebcb9d67b5249c8848b09d639dca8d7bb0"
 dependencies = [
@@ -460,23 +460,23 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.10"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54675592c1dbefd78cbd98db9bacd89886e1ca50692a0692baefffdeb92dd58"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -519,61 +519,61 @@
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `nh3-0.2.8/PKG-INFO` & `nh3-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nh3
-Version: 0.2.8
+Version: 0.2.9
 Summary: Ammonia HTML sanitizer Python binding
 Author: messense <messense@icloud.com>
 Author-email: messense <messense@icloud.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/messense/nh3
```

