# Comparing `tmp/rormula-0.1.1.tar.gz` & `tmp/rormula-0.1.2.tar.gz`

## Comparing `rormula-0.1.1.tar` & `rormula-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 rormula-0.1.1/local_dependencies/rormula-rs/Cargo.toml
--rw-r--r--   0     1001      123        6 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/.gitignore
--rw-r--r--   0     1001      123     4474 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/array.rs
--rw-r--r--   0     1001      123     4235 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs
--rw-r--r--   0     1001      123    10877 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs
--rw-r--r--   0     1001      123      211 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/expression/mod.rs
--rw-r--r--   0     1001      123     3092 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/expression/ops_common.rs
--rw-r--r--   0     1001      123     1552 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/expression/value.rs
--rw-r--r--   0     1001      123       66 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/lib.rs
--rw-r--r--   0     1001      123     1232 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/src/result.rs
--rw-r--r--   0     1001      123     2090 2023-04-21 17:09:51.000000 rormula-0.1.1/local_dependencies/rormula-rs/tests/test_rormula.rs
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 rormula-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123        6 2023-04-21 17:09:51.000000 rormula-0.1.1/.gitignore
--rw-r--r--   0     1001      123     3523 2023-04-21 17:09:51.000000 rormula-0.1.1/benches/benchmark.rs
--rw-r--r--   0     1001      123      330 2023-04-21 17:09:51.000000 rormula-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     2592 2023-04-21 17:09:51.000000 rormula-0.1.1/rormula/__init__.py
--rw-r--r--   0     1001      123      806 2023-04-21 17:09:51.000000 rormula-0.1.1/rormula/_rormula.pyi
--rw-r--r--   0     1001      123     7887 2023-04-21 17:09:51.000000 rormula-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-04-21 17:09:51.000000 rormula-0.1.1/test/__init__.py
--rw-r--r--   0     1001      123      999 2023-04-21 17:09:51.000000 rormula-0.1.1/test/test_arithmetic.py
--rw-r--r--   0     1001      123     5637 2023-04-21 17:09:51.000000 rormula-0.1.1/test/test_wilkinson.py
--rw-r--r--   0     1001      123    25081 2023-04-21 17:09:51.000000 rormula-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      209 1970-01-01 00:00:00.000000 rormula-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      227 1970-01-01 00:00:00.000000 rormula-0.1.2/local_dependencies/rormula-rs/Cargo.toml
+-rw-r--r--   0     1001      123        6 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/.gitignore
+-rw-r--r--   0     1001      123     4474 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/array.rs
+-rw-r--r--   0     1001      123     4235 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs
+-rw-r--r--   0     1001      123    10877 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs
+-rw-r--r--   0     1001      123      211 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      123     3092 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/expression/ops_common.rs
+-rw-r--r--   0     1001      123     1552 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/expression/value.rs
+-rw-r--r--   0     1001      123       66 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/lib.rs
+-rw-r--r--   0     1001      123     1232 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/src/result.rs
+-rw-r--r--   0     1001      123     2090 2023-04-21 18:28:08.000000 rormula-0.1.2/local_dependencies/rormula-rs/tests/test_rormula.rs
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 rormula-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123        6 2023-04-21 18:28:08.000000 rormula-0.1.2/.gitignore
+-rw-r--r--   0     1001      123     3523 2023-04-21 18:28:08.000000 rormula-0.1.2/benches/benchmark.rs
+-rw-r--r--   0     1001      123      739 2023-04-21 18:28:08.000000 rormula-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     2570 2023-04-21 18:28:08.000000 rormula-0.1.2/rormula/__init__.py
+-rw-r--r--   0     1001      123      806 2023-04-21 18:28:08.000000 rormula-0.1.2/rormula/_rormula.pyi
+-rw-r--r--   0     1001      123     7887 2023-04-21 18:28:08.000000 rormula-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-21 18:28:08.000000 rormula-0.1.2/test/__init__.py
+-rw-r--r--   0     1001      123      999 2023-04-21 18:28:08.000000 rormula-0.1.2/test/test_arithmetic.py
+-rw-r--r--   0     1001      123     5635 2023-04-21 18:28:08.000000 rormula-0.1.2/test/test_wilkinson.py
+-rw-r--r--   0     1001      123    25081 2023-04-21 18:28:08.000000 rormula-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 rormula-0.1.2/PKG-INFO
```

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/array.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/array.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/expression/expr_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/expression/expr_wilkinson.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/expression/ops_common.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/expression/ops_common.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/expression/value.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/expression/value.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/src/result.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/src/result.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/local_dependencies/rormula-rs/tests/test_rormula.rs` & `rormula-0.1.2/local_dependencies/rormula-rs/tests/test_rormula.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/benches/benchmark.rs` & `rormula-0.1.2/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/rormula/__init__.py` & `rormula-0.1.2/rormula/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from typing import List, NamedTuple, Tuple, Union
 import numpy as np
 import pandas as pd
-
-import pandas as pd
-
 from rormula import _rormula as ror
 
 
 class SeparatedData(NamedTuple):
     numerical_cols: List[str]
     numerical_data: np.ndarray
     categorical_cols: List[str]
```

### Comparing `rormula-0.1.1/rormula/_rormula.pyi` & `rormula-0.1.2/rormula/_rormula.pyi`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/src/lib.rs` & `rormula-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/test/test_arithmetic.py` & `rormula-0.1.2/test/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `rormula-0.1.1/test/test_wilkinson.py` & `rormula-0.1.2/test/test_wilkinson.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,8 +168,8 @@
     rormula = RormulaWilkinson("alpha + beta + alpha:gamma")
     names, mm = rormula.eval(separated_data)
     assert names == ["Intercept", "alpha", "beta", "alpha:gamma"]
     assert mm.shape == (100, 4)
 
 
 if __name__ == "__main__":
-    test_separated()
+    test_num_cat()
```

### Comparing `rormula-0.1.1/Cargo.lock` & `rormula-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -657,15 +657,15 @@
 name = "regex-syntax"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rormula"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "criterion",
  "numpy",
  "pyo3",
  "rormula-rs",
  "which",
 ]
```

