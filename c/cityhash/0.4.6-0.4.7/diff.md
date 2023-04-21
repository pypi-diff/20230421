# Comparing `tmp/cityhash-0.4.6.tar.gz` & `tmp/cityhash-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cityhash-0.4.6.tar", last modified: Sat Dec 17 04:34:09 2022, max compression
+gzip compressed data, was "cityhash-0.4.7.tar", last modified: Fri Apr 21 04:28:37 2023, max compression
```

## Comparing `cityhash-0.4.6.tar` & `cityhash-0.4.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-17 04:34:09.135079 cityhash-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2022-12-17 04:34:00.000000 cityhash-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-12-17 04:34:00.000000 cityhash-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2022-12-17 04:34:09.135079 cityhash-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2022-12-17 04:34:00.000000 cityhash-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      287 2022-12-17 04:34:00.000000 cityhash-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-17 04:34:09.135079 cityhash-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2022-12-17 04:34:00.000000 cityhash-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-17 04:34:09.135079 cityhash-0.4.6/src/
--rw-r--r--   0 runner    (1001) docker     (122)    19320 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/city.cc
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/city.h
--rw-r--r--   0 runner    (1001) docker     (122)     1862 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/citycrc.h
--rw-r--r--   0 runner    (1001) docker     (122)   237363 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/cityhash.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-17 04:34:09.135079 cityhash-0.4.6/src/cityhash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2022-12-17 04:34:09.000000 cityhash-0.4.6/src/cityhash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      400 2022-12-17 04:34:09.000000 cityhash-0.4.6/src/cityhash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-17 04:34:09.000000 cityhash-0.4.6/src/cityhash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-17 04:34:09.000000 cityhash-0.4.6/src/cityhash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-17 04:34:09.000000 cityhash-0.4.6/src/cityhash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9512 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/cityhash.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   199788 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/cityhashcrc.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5907 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/cityhashcrc.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   283275 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/farm.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10293 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/farm.h
--rw-r--r--   0 runner    (1001) docker     (122)   293421 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/farmhash.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14476 2022-12-17 04:34:00.000000 cityhash-0.4.6/src/farmhash.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 04:28:37.004794 cityhash-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-21 04:28:27.000000 cityhash-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-21 04:28:27.000000 cityhash-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6569 2023-04-21 04:28:37.004794 cityhash-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5273 2023-04-21 04:28:27.000000 cityhash-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-21 04:28:27.000000 cityhash-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 04:28:37.004794 cityhash-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-04-21 04:28:27.000000 cityhash-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 04:28:37.004794 cityhash-0.4.7/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    19320 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/city.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/city.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1862 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/citycrc.h
+-rw-r--r--   0 runner    (1001) docker     (122)   238422 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/cityhash.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 04:28:37.004794 cityhash-0.4.7/src/cityhash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6569 2023-04-21 04:28:36.000000 cityhash-0.4.7/src/cityhash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-21 04:28:36.000000 cityhash-0.4.7/src/cityhash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 04:28:36.000000 cityhash-0.4.7/src/cityhash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 04:28:36.000000 cityhash-0.4.7/src/cityhash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-21 04:28:36.000000 cityhash-0.4.7/src/cityhash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9512 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/cityhash.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   200847 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/cityhashcrc.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5907 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/cityhashcrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   283275 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/farm.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10293 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/farm.h
+-rw-r--r--   0 runner    (1001) docker     (122)   294480 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/farmhash.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14476 2023-04-21 04:28:27.000000 cityhash-0.4.7/src/farmhash.pyx
```

### Comparing `cityhash-0.4.6/LICENSE` & `cityhash-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/PKG-INFO` & `cityhash-0.4.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cityhash
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python bindings for CityHash and FarmHash
 Home-page: https://github.com/escherba/python-cityhash
 Author: Eugene Scherba
 Author-email: escherba+cityhash@gmail.com
 License: MIT
-Download-URL: https://github.com/escherba/python-cityhash/tarball/master/0.4.6
+Download-URL: https://github.com/escherba/python-cityhash/tarball/master/0.4.7
 Keywords: google,hash,hashing,cityhash,farmhash,murmurhash,cython
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,32 +31,36 @@
 
 # CityHash/FarmHash
 
 Python wrapper for [FarmHash](https://github.com/google/farmhash) and
 [CityHash](https://github.com/google/cityhash), a family of fast
 non-cryptographic hash functions.
 
-[![Build
-Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
-[![Latest
-Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Conda-Forge Version](https://anaconda.org/conda-forge/python-cityhash/badges/version.svg)](https://anaconda.org/conda-forge/python-cityhash)
 [![Downloads](https://img.shields.io/pypi/dm/cityhash.svg)](https://pypistats.org/packages/cityhash)
 [![License](https://img.shields.io/pypi/l/cityhash.svg)](https://opensource.org/licenses/mit-license)
-[![Supported Python
-versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
 
 ## Getting Started
 
-This simplest way to use this package is to install it from PyPI:
+To install from PyPI:
 
 ``` bash
 pip install cityhash
 ```
 
-This package exposes Python APIs for CityHash and FarmHash under `cityhash` and
+To install in a Conda environment:
+
+``` bash
+conda install -c conda-forge python-cityhash
+```
+
+The package exposes Python APIs for CityHash and FarmHash under `cityhash` and
 `farmhash` namespaces, respectively. Each provides 32-, 64- and 128-bit
 implementations.
 
 ## Usage Examples
 
 ### Stateless hashing
 
@@ -71,111 +75,111 @@
 >>> FarmHash128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Hardware-independent fingerprints
 
-Fingerprints are seedless hashes which are guaranteed to be hardware- and
+Fingerprints are seedless hashes that are guaranteed to be hardware- and
 platform-independent. This can be useful for networking applications which
 require persisting hashed values.
 
 ``` python
 >>> from farmhash import Fingerprint128
 >>> Fingerprint128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Incremental hashing
 
 CityHash and FarmHash do not support incremental hashing and thus are not ideal
-for hashing of streams. If you require incremental hashing feature, use
+for hashing of character streams. If you require incremental hashing, consider
+another hashing library, such as
 [MetroHash](https://github.com/escherba/python-metrohash) or
-[xxHash](https://github.com/ifduyue/python-xxhash) instead, which do support
-it.
+[xxHash](https://github.com/ifduyue/python-xxhash).
 
 ### Fast hashing of NumPy arrays
 
-The Python [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html)
-allows Python objects to expose their data as raw byte arrays to other objects,
-for fast access without copying to a separate location in memory. Among others,
-NumPy is a major framework that supports this protocol.
-
-All hashing functions in this packege will read byte arrays from objects that
-expose them via the buffer protocol. Here is an example showing hashing of a 4D
-NumPy array:
+The [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html) allows
+Python objects to expose their data as raw byte arrays for fast access without
+having to copy to a separate location in memory. NumPy is one well-known
+library that extensively uses this protocol.
+
+All hashing functions in this package will read byte arrays from objects that
+expose them via the buffer protocol. Here is an example showing hashing of a
+four-dimensional NumPy array:
 
 ``` python
 >>> import numpy as np
 >>> from farmhash import FarmHash64
 >>> arr = np.zeros((256, 256, 4))
 >>> FarmHash64(arr)
 1550282412043536862
 
 ```
 
-The arrays need to be contiguous for this to work. To convert a non-contiguous
-array, use NumPy's `ascontiguousarray()` function.
+The NumPy arrays need to be contiguous for this to work. To convert a
+non-contiguous array, use NumPy's `ascontiguousarray()` function.
 
 ## SSE4.2 support
 
-For x86-64 platforms, the PyPi repository for this package includes wheels
-compiled with SSE4.2 support.  The 32- and 64-bit FarmHash variants
-significantly benefit from SSE4.2 instructions. The 128-bit version,
-unfortunately, does not exhibit speed up after compiling with SSE4.2 support.
-
-The vanilla CityHash fucntions (under `cityhash` module) do not take advantage
-of SSE4.2. Instead, the `cityhashcrc` module provided with this package exposes
-128- and 256-bit CRC functions which do harness SSE4.2. These functions are
-very fast, and beat `FarmHash128` on speed (FarmHash does not include a 256-bit
-function). Since FarmHash is the intended successor of CityHash, I would be
-careful before using the CityHash-CRC functions, however, and would verify
-whether they provide sufficient randomness for your intended application.
+For x86-64 platforms, the PyPI repository for this package includes wheels
+compiled with SSE4.2 support.  The 32- and 64-bit (but not the 128-bit)
+variants of FarmHash significantly benefit from SSE4.2 instructions.
+
+The vanilla CityHash functions (under `cityhash` module) do not take advantage
+of SSE4.2. Instead, one can use the `cityhashcrc` module provided with this
+package which exposes 128- and 256-bit CRC functions that do harness SSE4.2.
+These functions are very fast, and beat `FarmHash128` on speed (FarmHash does
+not include a 256-bit function). Since FarmHash is the intended successor of
+CityHash, I would be careful before using the CityHash-CRC functions, however,
+and would verify whether they provide sufficient randomness for your intended
+application.
 
 ## Development
 
 ### Local workflow
 
-For those who want to contribute, here is a quick start using some makefile
-commands:
+For those wanting to contribute, here is a quick start using Make commands:
 
 ``` bash
 git clone https://github.com/escherba/python-cityhash.git
 cd python-cityhash
 make env           # create a virtual environment
 make test          # run Python tests
 make cpp-test      # run C++ tests
 make shell         # enter IPython shell
 ```
 
-To find out which Make targets are available, type:
+To find out which Make targets are available, enter:
 
 ``` bash
 make help
 ```
 
 ### Distribution
 
-The wheels are built using [cibuildwheel](https://cibuildwheel.readthedocs.io/)
-and are distributed to PyPI using GitHub actions. The wheels contain compiled
-binaries and are available for the following platforms: windows-amd64,
-ubuntu-x86, linux-x86\_64, linux-aarch64, and macosx-x86\_64.
+The package wheels are built using
+[cibuildwheel](https://cibuildwheel.readthedocs.io/) and are distributed to
+PyPI using GitHub actions. The wheels contain compiled binaries and are
+available for the following platforms: windows-amd64, ubuntu-x86,
+linux-x86\_64, linux-aarch64, and macosx-x86\_64.
 
 ## See Also
 
 For other fast non-cryptographic hash functions available as Python extensions,
 see [MetroHash](https://github.com/escherba/python-metrohash),
 [MurmurHash](https://github.com/hajimes/mmh3), and
 [xxHash](https://github.com/ifduyue/python-xxhash).
 
 ## Authors
 
 The original CityHash Python bindings are due to Alexander \[Amper\] Marshalov.
-These were rewritten in Cython by Eugene Scherba, who also added the FarmHash
+They were rewritten in Cython by Eugene Scherba, who also added the FarmHash
 bindings. The CityHash and FarmHash algorithms and their C++ implementation are
 by Google.
 
 ## License
 
 This software is licensed under the [MIT
 License](http://www.opensource.org/licenses/mit-license). See the included
```

### Comparing `cityhash-0.4.6/README.md` & `cityhash-0.4.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # CityHash/FarmHash
 
 Python wrapper for [FarmHash](https://github.com/google/farmhash) and
 [CityHash](https://github.com/google/cityhash), a family of fast
 non-cryptographic hash functions.
 
-[![Build
-Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
-[![Latest
-Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Conda-Forge Version](https://anaconda.org/conda-forge/python-cityhash/badges/version.svg)](https://anaconda.org/conda-forge/python-cityhash)
 [![Downloads](https://img.shields.io/pypi/dm/cityhash.svg)](https://pypistats.org/packages/cityhash)
 [![License](https://img.shields.io/pypi/l/cityhash.svg)](https://opensource.org/licenses/mit-license)
-[![Supported Python
-versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
 
 ## Getting Started
 
-This simplest way to use this package is to install it from PyPI:
+To install from PyPI:
 
 ``` bash
 pip install cityhash
 ```
 
-This package exposes Python APIs for CityHash and FarmHash under `cityhash` and
+To install in a Conda environment:
+
+``` bash
+conda install -c conda-forge python-cityhash
+```
+
+The package exposes Python APIs for CityHash and FarmHash under `cityhash` and
 `farmhash` namespaces, respectively. Each provides 32-, 64- and 128-bit
 implementations.
 
 ## Usage Examples
 
 ### Stateless hashing
 
@@ -40,111 +44,111 @@
 >>> FarmHash128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Hardware-independent fingerprints
 
-Fingerprints are seedless hashes which are guaranteed to be hardware- and
+Fingerprints are seedless hashes that are guaranteed to be hardware- and
 platform-independent. This can be useful for networking applications which
 require persisting hashed values.
 
 ``` python
 >>> from farmhash import Fingerprint128
 >>> Fingerprint128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Incremental hashing
 
 CityHash and FarmHash do not support incremental hashing and thus are not ideal
-for hashing of streams. If you require incremental hashing feature, use
+for hashing of character streams. If you require incremental hashing, consider
+another hashing library, such as
 [MetroHash](https://github.com/escherba/python-metrohash) or
-[xxHash](https://github.com/ifduyue/python-xxhash) instead, which do support
-it.
+[xxHash](https://github.com/ifduyue/python-xxhash).
 
 ### Fast hashing of NumPy arrays
 
-The Python [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html)
-allows Python objects to expose their data as raw byte arrays to other objects,
-for fast access without copying to a separate location in memory. Among others,
-NumPy is a major framework that supports this protocol.
-
-All hashing functions in this packege will read byte arrays from objects that
-expose them via the buffer protocol. Here is an example showing hashing of a 4D
-NumPy array:
+The [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html) allows
+Python objects to expose their data as raw byte arrays for fast access without
+having to copy to a separate location in memory. NumPy is one well-known
+library that extensively uses this protocol.
+
+All hashing functions in this package will read byte arrays from objects that
+expose them via the buffer protocol. Here is an example showing hashing of a
+four-dimensional NumPy array:
 
 ``` python
 >>> import numpy as np
 >>> from farmhash import FarmHash64
 >>> arr = np.zeros((256, 256, 4))
 >>> FarmHash64(arr)
 1550282412043536862
 
 ```
 
-The arrays need to be contiguous for this to work. To convert a non-contiguous
-array, use NumPy's `ascontiguousarray()` function.
+The NumPy arrays need to be contiguous for this to work. To convert a
+non-contiguous array, use NumPy's `ascontiguousarray()` function.
 
 ## SSE4.2 support
 
-For x86-64 platforms, the PyPi repository for this package includes wheels
-compiled with SSE4.2 support.  The 32- and 64-bit FarmHash variants
-significantly benefit from SSE4.2 instructions. The 128-bit version,
-unfortunately, does not exhibit speed up after compiling with SSE4.2 support.
-
-The vanilla CityHash fucntions (under `cityhash` module) do not take advantage
-of SSE4.2. Instead, the `cityhashcrc` module provided with this package exposes
-128- and 256-bit CRC functions which do harness SSE4.2. These functions are
-very fast, and beat `FarmHash128` on speed (FarmHash does not include a 256-bit
-function). Since FarmHash is the intended successor of CityHash, I would be
-careful before using the CityHash-CRC functions, however, and would verify
-whether they provide sufficient randomness for your intended application.
+For x86-64 platforms, the PyPI repository for this package includes wheels
+compiled with SSE4.2 support.  The 32- and 64-bit (but not the 128-bit)
+variants of FarmHash significantly benefit from SSE4.2 instructions.
+
+The vanilla CityHash functions (under `cityhash` module) do not take advantage
+of SSE4.2. Instead, one can use the `cityhashcrc` module provided with this
+package which exposes 128- and 256-bit CRC functions that do harness SSE4.2.
+These functions are very fast, and beat `FarmHash128` on speed (FarmHash does
+not include a 256-bit function). Since FarmHash is the intended successor of
+CityHash, I would be careful before using the CityHash-CRC functions, however,
+and would verify whether they provide sufficient randomness for your intended
+application.
 
 ## Development
 
 ### Local workflow
 
-For those who want to contribute, here is a quick start using some makefile
-commands:
+For those wanting to contribute, here is a quick start using Make commands:
 
 ``` bash
 git clone https://github.com/escherba/python-cityhash.git
 cd python-cityhash
 make env           # create a virtual environment
 make test          # run Python tests
 make cpp-test      # run C++ tests
 make shell         # enter IPython shell
 ```
 
-To find out which Make targets are available, type:
+To find out which Make targets are available, enter:
 
 ``` bash
 make help
 ```
 
 ### Distribution
 
-The wheels are built using [cibuildwheel](https://cibuildwheel.readthedocs.io/)
-and are distributed to PyPI using GitHub actions. The wheels contain compiled
-binaries and are available for the following platforms: windows-amd64,
-ubuntu-x86, linux-x86\_64, linux-aarch64, and macosx-x86\_64.
+The package wheels are built using
+[cibuildwheel](https://cibuildwheel.readthedocs.io/) and are distributed to
+PyPI using GitHub actions. The wheels contain compiled binaries and are
+available for the following platforms: windows-amd64, ubuntu-x86,
+linux-x86\_64, linux-aarch64, and macosx-x86\_64.
 
 ## See Also
 
 For other fast non-cryptographic hash functions available as Python extensions,
 see [MetroHash](https://github.com/escherba/python-metrohash),
 [MurmurHash](https://github.com/hajimes/mmh3), and
 [xxHash](https://github.com/ifduyue/python-xxhash).
 
 ## Authors
 
 The original CityHash Python bindings are due to Alexander \[Amper\] Marshalov.
-These were rewritten in Cython by Eugene Scherba, who also added the FarmHash
+They were rewritten in Cython by Eugene Scherba, who also added the FarmHash
 bindings. The CityHash and FarmHash algorithms and their C++ implementation are
 by Google.
 
 ## License
 
 This software is licensed under the [MIT
 License](http://www.opensource.org/licenses/mit-license). See the included
```

### Comparing `cityhash-0.4.6/setup.py` & `cityhash-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             language="c++",
             extra_compile_args=CXXFLAGS,
             include_dirs=["src"],
         )
     )
 
 
-VERSION = "0.4.6"
+VERSION = "0.4.7"
 URL = "https://github.com/escherba/python-cityhash"
 
 
 def get_long_description(relpath, encoding="utf-8"):
     _long_desc = """
 
     """
```

### Comparing `cityhash-0.4.6/src/city.cc` & `cityhash-0.4.7/src/city.cc`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/src/city.h` & `cityhash-0.4.7/src/city.h`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/src/citycrc.h` & `cityhash-0.4.7/src/citycrc.h`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/src/cityhash.cpp` & `cityhash-0.4.7/src/cityhash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -562,35 +562,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1168,20 +1168,28 @@
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
@@ -1371,15 +1379,15 @@
 static const char __pyx_k_got[] = ", got '";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_0_4_6[] = "0.4.6";
+static const char __pyx_k_0_4_7[] = "0.4.7";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_seed0[] = "seed0";
 static const char __pyx_k_seed1[] = "seed1";
 static const char __pyx_k_tseed[] = "tseed";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_result[] = "result";
@@ -1399,15 +1407,15 @@
 static const char __pyx_k_CityHash64WithSeed[] = "CityHash64WithSeed";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_CityHash128WithSeed[] = "CityHash128WithSeed";
 static const char __pyx_k_CityHash64WithSeeds[] = "CityHash64WithSeeds";
 static const char __pyx_k_Python_wrapper_for_CityHash[] = "\nPython wrapper for CityHash\n";
 static const char __pyx_k_escherba_cityhash_gmail_com[] = "escherba+cityhash@gmail.com";
 static const char __pyx_k_has_incorrect_type_expected[] = "' has incorrect type: expected ";
-static PyObject *__pyx_kp_u_0_4_6;
+static PyObject *__pyx_kp_u_0_4_7;
 static PyObject *__pyx_kp_u_Argument;
 static PyObject *__pyx_n_s_CityHash128;
 static PyObject *__pyx_n_u_CityHash128;
 static PyObject *__pyx_n_s_CityHash128WithSeed;
 static PyObject *__pyx_n_u_CityHash128WithSeed;
 static PyObject *__pyx_n_s_CityHash32;
 static PyObject *__pyx_n_u_CityHash32;
@@ -3231,15 +3239,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_4_6, __pyx_k_0_4_6, sizeof(__pyx_k_0_4_6), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_4_7, __pyx_k_0_4_7, sizeof(__pyx_k_0_4_7), 0, 1, 0, 0},
   {&__pyx_kp_u_Argument, __pyx_k_Argument, sizeof(__pyx_k_Argument), 0, 1, 0, 0},
   {&__pyx_n_s_CityHash128, __pyx_k_CityHash128, sizeof(__pyx_k_CityHash128), 0, 0, 1, 1},
   {&__pyx_n_u_CityHash128, __pyx_k_CityHash128, sizeof(__pyx_k_CityHash128), 0, 1, 0, 1},
   {&__pyx_n_s_CityHash128WithSeed, __pyx_k_CityHash128WithSeed, sizeof(__pyx_k_CityHash128WithSeed), 0, 0, 1, 1},
   {&__pyx_n_u_CityHash128WithSeed, __pyx_k_CityHash128WithSeed, sizeof(__pyx_k_CityHash128WithSeed), 0, 1, 0, 1},
   {&__pyx_n_s_CityHash32, __pyx_k_CityHash32, sizeof(__pyx_k_CityHash32), 0, 0, 1, 1},
   {&__pyx_n_u_CityHash32, __pyx_k_CityHash32, sizeof(__pyx_k_CityHash32), 0, 1, 0, 1},
@@ -3366,15 +3374,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0L = PyLong_FromString((char *)"0", 0, 0); if (unlikely(!__pyx_int_0L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64L = PyLong_FromString((char *)"64", 0, 0); if (unlikely(!__pyx_int_64L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_18446744073709551615L = PyLong_FromString((char *)"18446744073709551615", 0, 0); if (unlikely(!__pyx_int_18446744073709551615L)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -3427,29 +3435,31 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -3634,15 +3644,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_cityhash) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3673,39 +3683,39 @@
   #endif
 
   /* "cityhash.pyx":11
  * """
  * 
  * __author__      = "Eugene Scherba"             # <<<<<<<<<<<<<<
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Eugene_Scherba) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
   /* "cityhash.pyx":12
  * 
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"             # <<<<<<<<<<<<<<
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_email, __pyx_kp_u_escherba_cityhash_gmail_com) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
   /* "cityhash.pyx":13
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'             # <<<<<<<<<<<<<<
+ * __version__     = '0.4.7'             # <<<<<<<<<<<<<<
  * __all__         = [
  *     "CityHash32",
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_6) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_7) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
 
   /* "cityhash.pyx":14
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [             # <<<<<<<<<<<<<<
  *     "CityHash32",
  *     "CityHash64",
  */
   __pyx_t_1 = PyList_New(6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_CityHash32);
@@ -4348,28 +4358,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -4516,44 +4526,62 @@
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -4601,15 +4629,15 @@
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `cityhash-0.4.6/src/cityhash.egg-info/PKG-INFO` & `cityhash-0.4.7/src/cityhash.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cityhash
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python bindings for CityHash and FarmHash
 Home-page: https://github.com/escherba/python-cityhash
 Author: Eugene Scherba
 Author-email: escherba+cityhash@gmail.com
 License: MIT
-Download-URL: https://github.com/escherba/python-cityhash/tarball/master/0.4.6
+Download-URL: https://github.com/escherba/python-cityhash/tarball/master/0.4.7
 Keywords: google,hash,hashing,cityhash,farmhash,murmurhash,cython
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,32 +31,36 @@
 
 # CityHash/FarmHash
 
 Python wrapper for [FarmHash](https://github.com/google/farmhash) and
 [CityHash](https://github.com/google/cityhash), a family of fast
 non-cryptographic hash functions.
 
-[![Build
-Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
-[![Latest
-Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/escherba/python-cityhash/build.yml?branch=master)](https://github.com/escherba/python-cityhash/actions/workflows/build.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Conda-Forge Version](https://anaconda.org/conda-forge/python-cityhash/badges/version.svg)](https://anaconda.org/conda-forge/python-cityhash)
 [![Downloads](https://img.shields.io/pypi/dm/cityhash.svg)](https://pypistats.org/packages/cityhash)
 [![License](https://img.shields.io/pypi/l/cityhash.svg)](https://opensource.org/licenses/mit-license)
-[![Supported Python
-versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/cityhash.svg)](https://pypi.python.org/pypi/cityhash)
 
 ## Getting Started
 
-This simplest way to use this package is to install it from PyPI:
+To install from PyPI:
 
 ``` bash
 pip install cityhash
 ```
 
-This package exposes Python APIs for CityHash and FarmHash under `cityhash` and
+To install in a Conda environment:
+
+``` bash
+conda install -c conda-forge python-cityhash
+```
+
+The package exposes Python APIs for CityHash and FarmHash under `cityhash` and
 `farmhash` namespaces, respectively. Each provides 32-, 64- and 128-bit
 implementations.
 
 ## Usage Examples
 
 ### Stateless hashing
 
@@ -71,111 +75,111 @@
 >>> FarmHash128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Hardware-independent fingerprints
 
-Fingerprints are seedless hashes which are guaranteed to be hardware- and
+Fingerprints are seedless hashes that are guaranteed to be hardware- and
 platform-independent. This can be useful for networking applications which
 require persisting hashed values.
 
 ``` python
 >>> from farmhash import Fingerprint128
 >>> Fingerprint128("abc")
 76434233956484675513733017140465933893
 
 ```
 
 ### Incremental hashing
 
 CityHash and FarmHash do not support incremental hashing and thus are not ideal
-for hashing of streams. If you require incremental hashing feature, use
+for hashing of character streams. If you require incremental hashing, consider
+another hashing library, such as
 [MetroHash](https://github.com/escherba/python-metrohash) or
-[xxHash](https://github.com/ifduyue/python-xxhash) instead, which do support
-it.
+[xxHash](https://github.com/ifduyue/python-xxhash).
 
 ### Fast hashing of NumPy arrays
 
-The Python [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html)
-allows Python objects to expose their data as raw byte arrays to other objects,
-for fast access without copying to a separate location in memory. Among others,
-NumPy is a major framework that supports this protocol.
-
-All hashing functions in this packege will read byte arrays from objects that
-expose them via the buffer protocol. Here is an example showing hashing of a 4D
-NumPy array:
+The [Buffer Protocol](https://docs.python.org/3/c-api/buffer.html) allows
+Python objects to expose their data as raw byte arrays for fast access without
+having to copy to a separate location in memory. NumPy is one well-known
+library that extensively uses this protocol.
+
+All hashing functions in this package will read byte arrays from objects that
+expose them via the buffer protocol. Here is an example showing hashing of a
+four-dimensional NumPy array:
 
 ``` python
 >>> import numpy as np
 >>> from farmhash import FarmHash64
 >>> arr = np.zeros((256, 256, 4))
 >>> FarmHash64(arr)
 1550282412043536862
 
 ```
 
-The arrays need to be contiguous for this to work. To convert a non-contiguous
-array, use NumPy's `ascontiguousarray()` function.
+The NumPy arrays need to be contiguous for this to work. To convert a
+non-contiguous array, use NumPy's `ascontiguousarray()` function.
 
 ## SSE4.2 support
 
-For x86-64 platforms, the PyPi repository for this package includes wheels
-compiled with SSE4.2 support.  The 32- and 64-bit FarmHash variants
-significantly benefit from SSE4.2 instructions. The 128-bit version,
-unfortunately, does not exhibit speed up after compiling with SSE4.2 support.
-
-The vanilla CityHash fucntions (under `cityhash` module) do not take advantage
-of SSE4.2. Instead, the `cityhashcrc` module provided with this package exposes
-128- and 256-bit CRC functions which do harness SSE4.2. These functions are
-very fast, and beat `FarmHash128` on speed (FarmHash does not include a 256-bit
-function). Since FarmHash is the intended successor of CityHash, I would be
-careful before using the CityHash-CRC functions, however, and would verify
-whether they provide sufficient randomness for your intended application.
+For x86-64 platforms, the PyPI repository for this package includes wheels
+compiled with SSE4.2 support.  The 32- and 64-bit (but not the 128-bit)
+variants of FarmHash significantly benefit from SSE4.2 instructions.
+
+The vanilla CityHash functions (under `cityhash` module) do not take advantage
+of SSE4.2. Instead, one can use the `cityhashcrc` module provided with this
+package which exposes 128- and 256-bit CRC functions that do harness SSE4.2.
+These functions are very fast, and beat `FarmHash128` on speed (FarmHash does
+not include a 256-bit function). Since FarmHash is the intended successor of
+CityHash, I would be careful before using the CityHash-CRC functions, however,
+and would verify whether they provide sufficient randomness for your intended
+application.
 
 ## Development
 
 ### Local workflow
 
-For those who want to contribute, here is a quick start using some makefile
-commands:
+For those wanting to contribute, here is a quick start using Make commands:
 
 ``` bash
 git clone https://github.com/escherba/python-cityhash.git
 cd python-cityhash
 make env           # create a virtual environment
 make test          # run Python tests
 make cpp-test      # run C++ tests
 make shell         # enter IPython shell
 ```
 
-To find out which Make targets are available, type:
+To find out which Make targets are available, enter:
 
 ``` bash
 make help
 ```
 
 ### Distribution
 
-The wheels are built using [cibuildwheel](https://cibuildwheel.readthedocs.io/)
-and are distributed to PyPI using GitHub actions. The wheels contain compiled
-binaries and are available for the following platforms: windows-amd64,
-ubuntu-x86, linux-x86\_64, linux-aarch64, and macosx-x86\_64.
+The package wheels are built using
+[cibuildwheel](https://cibuildwheel.readthedocs.io/) and are distributed to
+PyPI using GitHub actions. The wheels contain compiled binaries and are
+available for the following platforms: windows-amd64, ubuntu-x86,
+linux-x86\_64, linux-aarch64, and macosx-x86\_64.
 
 ## See Also
 
 For other fast non-cryptographic hash functions available as Python extensions,
 see [MetroHash](https://github.com/escherba/python-metrohash),
 [MurmurHash](https://github.com/hajimes/mmh3), and
 [xxHash](https://github.com/ifduyue/python-xxhash).
 
 ## Authors
 
 The original CityHash Python bindings are due to Alexander \[Amper\] Marshalov.
-These were rewritten in Cython by Eugene Scherba, who also added the FarmHash
+They were rewritten in Cython by Eugene Scherba, who also added the FarmHash
 bindings. The CityHash and FarmHash algorithms and their C++ implementation are
 by Google.
 
 ## License
 
 This software is licensed under the [MIT
 License](http://www.opensource.org/licenses/mit-license). See the included
```

### Comparing `cityhash-0.4.6/src/cityhash.pyx` & `cityhash-0.4.7/src/cityhash.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 Python wrapper for CityHash
 """
 
 __author__      = "Eugene Scherba"
 __email__       = "escherba+cityhash@gmail.com"
-__version__     = '0.4.6'
+__version__     = '0.4.7'
 __all__         = [
     "CityHash32",
     "CityHash64",
     "CityHash64WithSeed",
     "CityHash64WithSeeds",
     "CityHash128",
     "CityHash128WithSeed",
```

### Comparing `cityhash-0.4.6/src/cityhashcrc.cpp` & `cityhash-0.4.7/src/cityhashcrc.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -562,35 +562,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1169,20 +1169,28 @@
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
@@ -1370,15 +1378,15 @@
 static const char __pyx_k_out[] = "out";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_0_4_6[] = "0.4.6";
+static const char __pyx_k_0_4_7[] = "0.4.7";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_tseed[] = "tseed";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_instead[] = "' instead";
 static const char __pyx_k_version[] = "__version__";
@@ -1393,15 +1401,15 @@
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_CityHashCrc256Bytes[] = "CityHashCrc256Bytes";
 static const char __pyx_k_src_cityhashcrc_pyx[] = "src/cityhashcrc.pyx";
 static const char __pyx_k_CityHashCrc128WithSeed[] = "CityHashCrc128WithSeed";
 static const char __pyx_k_escherba_cityhash_gmail_com[] = "escherba+cityhash@gmail.com";
 static const char __pyx_k_has_incorrect_type_expected[] = "' has incorrect type: expected ";
 static const char __pyx_k_Python_wrapper_for_CityHash_CRC[] = "\nPython wrapper for CityHash-CRC\n";
-static PyObject *__pyx_kp_u_0_4_6;
+static PyObject *__pyx_kp_u_0_4_7;
 static PyObject *__pyx_kp_u_Argument;
 static PyObject *__pyx_n_s_CityHashCrc128;
 static PyObject *__pyx_n_u_CityHashCrc128;
 static PyObject *__pyx_n_s_CityHashCrc128WithSeed;
 static PyObject *__pyx_n_u_CityHashCrc128WithSeed;
 static PyObject *__pyx_n_s_CityHashCrc256Bytes;
 static PyObject *__pyx_n_u_CityHashCrc256Bytes;
@@ -2408,15 +2416,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_4_6, __pyx_k_0_4_6, sizeof(__pyx_k_0_4_6), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_4_7, __pyx_k_0_4_7, sizeof(__pyx_k_0_4_7), 0, 1, 0, 0},
   {&__pyx_kp_u_Argument, __pyx_k_Argument, sizeof(__pyx_k_Argument), 0, 1, 0, 0},
   {&__pyx_n_s_CityHashCrc128, __pyx_k_CityHashCrc128, sizeof(__pyx_k_CityHashCrc128), 0, 0, 1, 1},
   {&__pyx_n_u_CityHashCrc128, __pyx_k_CityHashCrc128, sizeof(__pyx_k_CityHashCrc128), 0, 1, 0, 1},
   {&__pyx_n_s_CityHashCrc128WithSeed, __pyx_k_CityHashCrc128WithSeed, sizeof(__pyx_k_CityHashCrc128WithSeed), 0, 0, 1, 1},
   {&__pyx_n_u_CityHashCrc128WithSeed, __pyx_k_CityHashCrc128WithSeed, sizeof(__pyx_k_CityHashCrc128WithSeed), 0, 1, 0, 1},
   {&__pyx_n_s_CityHashCrc256Bytes, __pyx_k_CityHashCrc256Bytes, sizeof(__pyx_k_CityHashCrc256Bytes), 0, 0, 1, 1},
   {&__pyx_n_u_CityHashCrc256Bytes, __pyx_k_CityHashCrc256Bytes, sizeof(__pyx_k_CityHashCrc256Bytes), 0, 1, 0, 1},
@@ -2500,15 +2508,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0L = PyLong_FromString((char *)"0", 0, 0); if (unlikely(!__pyx_int_0L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64L = PyLong_FromString((char *)"64", 0, 0); if (unlikely(!__pyx_int_64L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_18446744073709551615L = PyLong_FromString((char *)"18446744073709551615", 0, 0); if (unlikely(!__pyx_int_18446744073709551615L)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -2561,29 +2569,31 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -2768,15 +2778,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_cityhashcrc) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2807,39 +2817,39 @@
   #endif
 
   /* "cityhashcrc.pyx":11
  * """
  * 
  * __author__      = "Eugene Scherba"             # <<<<<<<<<<<<<<
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Eugene_Scherba) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
   /* "cityhashcrc.pyx":12
  * 
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"             # <<<<<<<<<<<<<<
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_email, __pyx_kp_u_escherba_cityhash_gmail_com) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
   /* "cityhashcrc.pyx":13
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'             # <<<<<<<<<<<<<<
+ * __version__     = '0.4.7'             # <<<<<<<<<<<<<<
  * __all__         = [
  *     "CityHashCrc128",
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_6) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_7) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
 
   /* "cityhashcrc.pyx":14
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [             # <<<<<<<<<<<<<<
  *     "CityHashCrc128",
  *     "CityHashCrc128WithSeed",
  */
   __pyx_t_1 = PyList_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_CityHashCrc128);
@@ -3437,28 +3447,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -3605,44 +3615,62 @@
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -3690,15 +3718,15 @@
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `cityhash-0.4.6/src/cityhashcrc.pyx` & `cityhash-0.4.7/src/cityhashcrc.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 Python wrapper for CityHash-CRC
 """
 
 __author__      = "Eugene Scherba"
 __email__       = "escherba+cityhash@gmail.com"
-__version__     = '0.4.6'
+__version__     = '0.4.7'
 __all__         = [
     "CityHashCrc128",
     "CityHashCrc128WithSeed",
     "CityHashCrc256Bytes",
 ]
```

### Comparing `cityhash-0.4.6/src/farm.cc` & `cityhash-0.4.7/src/farm.cc`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/src/farm.h` & `cityhash-0.4.7/src/farm.h`

 * *Files identical despite different names*

### Comparing `cityhash-0.4.6/src/farmhash.cpp` & `cityhash-0.4.7/src/farmhash.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -83,15 +83,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -562,35 +562,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1168,20 +1168,28 @@
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
@@ -1374,15 +1382,15 @@
 static const char __pyx_k_got[] = ", got '";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_test[] = "__test__";
-static const char __pyx_k_0_4_6[] = "0.4.6";
+static const char __pyx_k_0_4_7[] = "0.4.7";
 static const char __pyx_k_email[] = "__email__";
 static const char __pyx_k_seed0[] = "seed0";
 static const char __pyx_k_seed1[] = "seed1";
 static const char __pyx_k_tseed[] = "tseed";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_buffer[] = "buffer";
 static const char __pyx_k_result[] = "result";
@@ -1406,15 +1414,15 @@
 static const char __pyx_k_FarmHash64WithSeed[] = "FarmHash64WithSeed";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_FarmHash128WithSeed[] = "FarmHash128WithSeed";
 static const char __pyx_k_FarmHash64WithSeeds[] = "FarmHash64WithSeeds";
 static const char __pyx_k_Python_wrapper_for_FarmHash[] = "\nPython wrapper for FarmHash\n";
 static const char __pyx_k_escherba_cityhash_gmail_com[] = "escherba+cityhash@gmail.com";
 static const char __pyx_k_has_incorrect_type_expected[] = "' has incorrect type: expected ";
-static PyObject *__pyx_kp_u_0_4_6;
+static PyObject *__pyx_kp_u_0_4_7;
 static PyObject *__pyx_kp_u_Argument;
 static PyObject *__pyx_kp_u_Eugene_Scherba;
 static PyObject *__pyx_n_s_FarmHash128;
 static PyObject *__pyx_n_u_FarmHash128;
 static PyObject *__pyx_n_s_FarmHash128WithSeed;
 static PyObject *__pyx_n_u_FarmHash128WithSeed;
 static PyObject *__pyx_n_s_FarmHash32;
@@ -4225,15 +4233,15 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_0_4_6, __pyx_k_0_4_6, sizeof(__pyx_k_0_4_6), 0, 1, 0, 0},
+  {&__pyx_kp_u_0_4_7, __pyx_k_0_4_7, sizeof(__pyx_k_0_4_7), 0, 1, 0, 0},
   {&__pyx_kp_u_Argument, __pyx_k_Argument, sizeof(__pyx_k_Argument), 0, 1, 0, 0},
   {&__pyx_kp_u_Eugene_Scherba, __pyx_k_Eugene_Scherba, sizeof(__pyx_k_Eugene_Scherba), 0, 1, 0, 0},
   {&__pyx_n_s_FarmHash128, __pyx_k_FarmHash128, sizeof(__pyx_k_FarmHash128), 0, 0, 1, 1},
   {&__pyx_n_u_FarmHash128, __pyx_k_FarmHash128, sizeof(__pyx_k_FarmHash128), 0, 1, 0, 1},
   {&__pyx_n_s_FarmHash128WithSeed, __pyx_k_FarmHash128WithSeed, sizeof(__pyx_k_FarmHash128WithSeed), 0, 0, 1, 1},
   {&__pyx_n_u_FarmHash128WithSeed, __pyx_k_FarmHash128WithSeed, sizeof(__pyx_k_FarmHash128WithSeed), 0, 1, 0, 1},
   {&__pyx_n_s_FarmHash32, __pyx_k_FarmHash32, sizeof(__pyx_k_FarmHash32), 0, 0, 1, 1},
@@ -4416,15 +4424,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0L = PyLong_FromString((char *)"0", 0, 0); if (unlikely(!__pyx_int_0L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64L = PyLong_FromString((char *)"64", 0, 0); if (unlikely(!__pyx_int_64L)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_18446744073709551615L = PyLong_FromString((char *)"18446744073709551615", 0, 0); if (unlikely(!__pyx_int_18446744073709551615L)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -4477,29 +4485,31 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(2, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4684,15 +4694,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_farmhash) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4723,39 +4733,39 @@
   #endif
 
   /* "farmhash.pyx":11
  * """
  * 
  * __author__      = "Eugene Scherba"             # <<<<<<<<<<<<<<
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_author, __pyx_kp_u_Eugene_Scherba) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
 
   /* "farmhash.pyx":12
  * 
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"             # <<<<<<<<<<<<<<
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_email, __pyx_kp_u_escherba_cityhash_gmail_com) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
 
   /* "farmhash.pyx":13
  * __author__      = "Eugene Scherba"
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'             # <<<<<<<<<<<<<<
+ * __version__     = '0.4.7'             # <<<<<<<<<<<<<<
  * __all__         = [
  *     "FarmHash32",
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_6) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_0_4_7) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
 
   /* "farmhash.pyx":14
  * __email__       = "escherba+cityhash@gmail.com"
- * __version__     = '0.4.6'
+ * __version__     = '0.4.7'
  * __all__         = [             # <<<<<<<<<<<<<<
  *     "FarmHash32",
  *     "FarmHash32WithSeed",
  */
   __pyx_t_1 = PyList_New(10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_u_FarmHash32);
@@ -5458,28 +5468,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -5626,44 +5636,62 @@
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -5711,15 +5739,15 @@
         return 0;
     return obj_dict_version == __Pyx_get_object_dict_version(obj);
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `cityhash-0.4.6/src/farmhash.pyx` & `cityhash-0.4.7/src/farmhash.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """
 Python wrapper for FarmHash
 """
 
 __author__      = "Eugene Scherba"
 __email__       = "escherba+cityhash@gmail.com"
-__version__     = '0.4.6'
+__version__     = '0.4.7'
 __all__         = [
     "FarmHash32",
     "FarmHash32WithSeed",
     "Fingerprint32",
     "FarmHash64",
     "FarmHash64WithSeed",
     "FarmHash64WithSeeds",
```

