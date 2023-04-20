# Comparing `tmp/polymers-0.3.1-cp39-none-win_amd64.whl.zip` & `tmp/polymers-0.3.2-cp38-cp38-macosx_10_7_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1172636 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4213 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     1569 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      115 b- defN 23-Apr-18 19:35 polymers/__init__.py
--rwxr-xr-x  4.6 unx  4857344 b- defN 23-Apr-18 19:35 polymers/polymers.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      484 b- defN 23-Apr-18 19:35 polymers-0.3.1.dist-info/RECORD
-6 files, 4863821 bytes uncompressed, 1171766 bytes compressed:  75.9%
+Zip file size: 1301818 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4133 b- defN 23-Apr-20 23:23 polymers-0.3.2.dist-info/METADATA
+-rw-r--r--  4.6 unx      105 b- defN 23-Apr-20 23:23 polymers-0.3.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1541 b- defN 23-Apr-20 23:23 polymers-0.3.2.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      115 b- defN 23-Apr-20 23:23 polymers/__init__.py
+-rwxr-xr-x  4.6 unx  5815728 b- defN 23-Apr-20 23:23 polymers/polymers.cpython-38-darwin.so
+-rw-r--r--  4.6 unx      487 b- defN 23-Apr-20 23:23 polymers-0.3.2.dist-info/RECORD
+6 files, 5822109 bytes uncompressed, 1300944 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polymers-0.3.1.dist-info/METADATA
+Filename: polymers-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: polymers-0.3.1.dist-info/WHEEL
+Filename: polymers-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: polymers-0.3.1.dist-info/license_files/LICENSE
+Filename: polymers-0.3.2.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: polymers/__init__.py
 Comment: 
 
-Filename: polymers/polymers.cp39-win_amd64.pyd
+Filename: polymers/polymers.cpython-38-darwin.so
 Comment: 
 
-Filename: polymers-0.3.1.dist-info/RECORD
+Filename: polymers-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `polymers-0.3.1.dist-info/METADATA` & `polymers-0.3.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymers
-Version: 0.3.1
+Version: 0.3.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: cffi
@@ -18,88 +18,88 @@
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/sandialabs/polymers
 Project-URL: Documentation, https://polymers.readthedocs.io
 Project-URL: Homepage, https://sandialabs.github.io/Polymers
 
-# Polymers Modeling Library
-
-[![website](https://img.shields.io/badge/GitHub-website-6e5494?logo=github)](https://sandialabs.github.io/Polymers)
-[![examples](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/binder.svg)](https://mybinder.org/v2/gh/sandialabs/Polymers/main)
-
-The library is implemented entirely in Rust, including the Python API. The Julia API calls the Rust library.
-
-## Python
-
-[![docs (stable)](https://img.shields.io/badge/Docs-stable-8CA1AF?logo=readthedocs)](https://polymers.readthedocs.io/en/stable)
-[![docs (latest)](https://img.shields.io/badge/Docs-latest-8CA1AF?logo=readthedocs)](https://polymers.readthedocs.io/en/latest)
-[![pypi](https://img.shields.io/pypi/v/polymers?logo=pypi&logoColor=FBE072&label=PyPI&color=4B8BBE)](https://pypi.org/project/polymers)
-
-The library can be installed as a Python package:
-
-```shell
-pip install polymers
-```
-
-If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
-
-```shell
-git clone git@github.com:sandialabs/Polymers.git
-cd Polymers/
-pip install maturin
-maturin build --features python
-pip install target/wheels/*.whl
-```
-
-## Julia
-
-[![docs (stable)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-stable.svg)](https://sandialabs.github.io/Polymers/julia/docs/stable)
-[![docs (latest)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-latest.svg)](https://sandialabs.github.io/Polymers/julia/docs/latest)
-[![Pkg](https://img.shields.io/github/v/release/sandialabs/Polymers?color=cb3c33&label=Pkg&logo=Julia&logoColor=cb3c33)](#)
-
-The library can be installed as a Julia package:
-
-```julia
-using Pkg
-Pkg.add("Polymers")
-```
-
-If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
-
-```julia
-using Pkg
-Pkg.add(url="https://github.com/sandialabs/Polymers")
-```
-
-## Rust
-
-[![docs (stable)](https://img.shields.io/badge/Docs-stable-e57300?logo=rust&logoColor=000000)](https://docs.rs/crate/polymers)
-[![docs (latest)](https://img.shields.io/badge/Docs-latest-e57300?logo=rust&logoColor=000000)](https://sandialabs.github.io/Polymers/rust/docs/latest)
-[![crates](https://img.shields.io/crates/v/polymers?logo=rust&logoColor=000000&label=Crates&color=32592f)](https://crates.io/crates/polymers)
-
-The library can be used in an existing Rust project by adding the `polymers` crate to Cargo.toml:
-
-```toml
-[dependencies]
-polymers = "*"
-```
-To use the latest edition of the library, add the GitHub repository to Cargo.toml:
-
-```toml
-[dependencies]
-regex = { git = "https://github.com/sandialabs/polymers" }
-```
-
-## Citation
-
-[![doi](https://img.shields.io/badge/Zenodo-10.5281%2Fzenodo.7041983-blue)](https://doi.org/10.5281/zenodo.7041983)
-
-Michael R. Buche. Polymers Modeling Library. [Zenodo (2023)](https://doi.org/10.5281/zenodo.7041983).
-
-## Copyright
-
-[![license](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/bsd3c.svg)](https://github.com/sandialabs/polymers/blob/main/LICENSE)
-
-Copyright 2022 National Technology & Engineering Solutions of Sandia, LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
-
+# Polymers Modeling Library
+
+[![website](https://img.shields.io/badge/GitHub-website-6e5494?logo=github)](https://sandialabs.github.io/Polymers)
+[![examples](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/binder.svg)](https://mybinder.org/v2/gh/sandialabs/Polymers/main)
+
+The library is implemented entirely in Rust, including the Python API. The Julia API calls the Rust library.
+
+## Python
+
+[![docs (stable)](https://img.shields.io/badge/Docs-stable-8CA1AF?logo=readthedocs)](https://polymers.readthedocs.io/en/stable)
+[![docs (latest)](https://img.shields.io/badge/Docs-latest-8CA1AF?logo=readthedocs)](https://polymers.readthedocs.io/en/latest)
+[![pypi](https://img.shields.io/pypi/v/polymers?logo=pypi&logoColor=FBE072&label=PyPI&color=4B8BBE)](https://pypi.org/project/polymers)
+
+The library can be installed as a Python package:
+
+```shell
+pip install polymers
+```
+
+If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
+
+```shell
+git clone git@github.com:sandialabs/Polymers.git
+cd Polymers/
+pip install maturin
+maturin build --features python
+pip install target/wheels/*.whl
+```
+
+## Julia
+
+[![docs (stable)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-stable.svg)](https://sandialabs.github.io/Polymers/julia/docs/stable)
+[![docs (latest)](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/julia-docs-latest.svg)](https://sandialabs.github.io/Polymers/julia/docs/latest)
+[![Pkg](https://img.shields.io/github/v/release/sandialabs/Polymers?color=cb3c33&label=Pkg&logo=Julia&logoColor=cb3c33)](#)
+
+The library can be installed as a Julia package:
+
+```julia
+using Pkg
+Pkg.add("Polymers")
+```
+
+If Rust is installed, the latest edition of the library can be installed from the GitHub repository:
+
+```julia
+using Pkg
+Pkg.add(url="https://github.com/sandialabs/Polymers")
+```
+
+## Rust
+
+[![docs (stable)](https://img.shields.io/badge/Docs-stable-e57300?logo=rust&logoColor=000000)](https://docs.rs/crate/polymers)
+[![docs (latest)](https://img.shields.io/badge/Docs-latest-e57300?logo=rust&logoColor=000000)](https://sandialabs.github.io/Polymers/rust/docs/latest)
+[![crates](https://img.shields.io/crates/v/polymers?logo=rust&logoColor=000000&label=Crates&color=32592f)](https://crates.io/crates/polymers)
+
+The library can be used in an existing Rust project by adding the `polymers` crate to Cargo.toml:
+
+```toml
+[dependencies]
+polymers = "*"
+```
+To use the latest edition of the library, add the GitHub repository to Cargo.toml:
+
+```toml
+[dependencies]
+regex = { git = "https://github.com/sandialabs/polymers" }
+```
+
+## Citation
+
+[![doi](https://img.shields.io/badge/Zenodo-10.5281%2Fzenodo.7041983-blue)](https://doi.org/10.5281/zenodo.7041983)
+
+Michael R. Buche. Polymers Modeling Library. [Zenodo (2023)](https://doi.org/10.5281/zenodo.7041983).
+
+## Copyright
+
+[![license](https://raw.githubusercontent.com/sandialabs/Polymers/main/pages/assets/images/bsd3c.svg)](https://github.com/sandialabs/polymers/blob/main/LICENSE)
+
+Copyright 2022 National Technology & Engineering Solutions of Sandia, LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
```

## Comparing `polymers-0.3.1.dist-info/license_files/LICENSE` & `polymers-0.3.2.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright 2022 National Technology & Engineering Solutions of Sandia, LLC.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright 2022 National Technology & Engineering Solutions of Sandia, LLC.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

