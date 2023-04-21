# Comparing `tmp/tf2jax-0.3.3.tar.gz` & `tmp/tf2jax-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2jax-0.3.3.tar", last modified: Fri Feb 10 20:21:27 2023, max compression
+gzip compressed data, was "tf2jax-0.3.4.tar", last modified: Fri Apr 21 09:07:46 2023, max compression
```

## Comparing `tf2jax-0.3.3.tar` & `tf2jax-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:27.774671 tf2jax-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-10 20:21:17.000000 tf2jax-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-10 20:21:17.000000 tf2jax-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-02-10 20:21:27.770671 tf2jax-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-02-10 20:21:17.000000 tf2jax-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-10 20:21:17.000000 tf2jax-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-10 20:21:17.000000 tf2jax-0.3.3/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:21:27.774671 tf2jax-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-02-10 20:21:17.000000 tf2jax-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:27.770671 tf2jax-0.3.3/tf2jax/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:27.770671 tf2jax-0.3.3/tf2jax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:27.770671 tf2jax-0.3.3/tf2jax/_src/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/experimental/mhlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/experimental/mhlo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/experimental/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/linalg_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/numpy_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/numpy_compat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79180 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    70036 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33127 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/roundtrip_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    44340 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/tf2jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/tf2jax_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/_src/xla_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-10 20:21:17.000000 tf2jax-0.3.3/tf2jax/tf2jax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:21:27.770671 tf2jax-0.3.3/tf2jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-10 20:21:27.000000 tf2jax-0.3.3/tf2jax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 09:07:33.000000 tf2jax-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 09:07:33.000000 tf2jax-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-21 09:07:46.049760 tf2jax-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-21 09:07:33.000000 tf2jax-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 09:07:33.000000 tf2jax-0.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 09:07:33.000000 tf2jax-0.3.4/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 09:07:46.049760 tf2jax-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-21 09:07:33.000000 tf2jax-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/linalg_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/numpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/numpy_compat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86540 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76011 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36772 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/roundtrip_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46673 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/tf2jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/tf2jax_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/_src/xla_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/mhlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/mhlo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/experimental/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-21 09:07:33.000000 tf2jax-0.3.4/tf2jax/tf2jax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 09:07:46.049760 tf2jax-0.3.4/tf2jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 09:07:46.000000 tf2jax-0.3.4/tf2jax.egg-info/top_level.txt
```

### Comparing `tf2jax-0.3.3/LICENSE` & `tf2jax-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/PKG-INFO` & `tf2jax-0.3.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: tf2jax
-Version: 0.3.3
-Summary: TF2JAX: Convert TensorFlow to JAX
-Home-page: https://github.com/deepmind/tf2jax
-Author: DeepMind
-Author-email: tf2jax-dev@google.com
-License: Apache 2.0
-Keywords: jax tensorflow conversion translate
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TF2JAX
 
 ![CI status](https://github.com/deepmind/tf2jax/workflows/ci/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/tf2jax)
 
 TF2JAX is an experimental library for converting [TensorFlow] functions/graphs
 to [JAX] functions.
@@ -203,15 +177,15 @@
 import tensorflow_hub as hub
 
 hub_model = hub.load("/tmp/blah")
 jax_func, jax_params = tf2jax.convert(tf.function(hub_model), tf.zeros_like(x))
 jax_outputs, updated_jax_params = jax_func(jax_params, x)
 ```
 
-## JAX to TensorFlow and Back Again.
+## JAX to TensorFlow and back again.
 
 `tf2jax.convert_functional` can convert the outputs of `jax2tf.convert` back
 into JAX code.
 
 ```python
 # Some JAX function.
 def forward(*inputs):
@@ -322,14 +296,57 @@
 operations from `reduce_window` operations generated by JAX2TF. This provides
 better performance because `reduce_window` implementation of these ops have
 O(N^2) complexity on CPU and GPU backends, and can suffer from long compilation
 times due to aggressive constant folding.
 
 See [jax2tf_cumulative_reduction] for more context.
 
+## JAX2TF Native Serialization and XlaCallModule.
+
+From JAX v0.4.7 and onward, `jax2tf.convert` preferred mode of operation (soon
+to be default) is **native serialization** in which the target function is
+lowered to [StableHLO] and wrapped in a single TensorFlow op, `XlaCallModule`.
+
+The new native serialization format will more faithfully reproduce the semantics
+of the target function, at the cost of some reduced flexibility for downstream
+processing as the computation graph is no longer exposed as a tf.Graph.
+
+`XlaCallModule` is supported by TF2JAX from v0.3.4 and onward.
+
+However as this makes use of a custom JAX primitive that aims to encapsulate
+[StableHLO] payload found in `XlaCallModule`, it does not possess JAX rules for
+transformations such as (but not limited to) batching and differentiation.
+
+* **Differentiation**: first order derivative of serialized function is
+still supported through custom gradients requested at serialization time with
+`jax2tf.convert(..., with_gradient=True)`. This is the default behaviour.
+* **Batching**: `jax.vmap` will fail, though users may be able to naively
+replicate the desired behavior with `jax.lax.map`, albeit with poorer
+performance.
+
+### Platform Specificity
+
+Natively serialized JAX programs are platform specific ([link](https://github.com/google/jax/blob/main/jax/experimental/jax2tf/README.md#natively-serialized-jax-modules-are-platform-specific)). Executing a natively
+serialized program on platforms other than the one for which it was lowered,
+would raise a ValueError, e.g.:
+
+```python
+ValueError: Unsupported backend: `cpu` not in `('tpu',)`.
+```
+
+This matches the behaviour of `XlaCallModule`.
+
+Users can disable this check via a config flag, but the resulting program may
+be slower or fail to execute completely.
+
+```python
+with tf2jax.override_config("xlacallmodule_strict_checks", False):
+  jax_func(np.zeros((20, 5), np.float32))
+```
+
 ## Limitations
 
 Currently, only a subset of TensorFlow ops are supported, and not necessarily
 all functionalities are supported for some ops. The code will fail fast. Support
 for additional TensorFlow ops are added on a as-needed basis. Please submit your
 requests via Github issues or send in your pull requests.
 
@@ -382,7 +399,8 @@
 
 [DeepMind JAX Ecosystem]: https://deepmind.com/blog/article/using-jax-to-accelerate-our-research "DeepMind JAX Ecosystem"
 [DeepMind JAX Ecosystem citation]: https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt "Citation"
 [JAX]: https://github.com/google/jax "JAX on GitHub"
 [TensorFlow]: https://github.com/tensorflow/tensorflow "TensorFlow on GitHub"
 [jax2tf documentation]: https://github.com/google/jax/blob/master/jax/experimental/jax2tf/README.md#calling-tensorflow-functions-from-jax "jax2tf documentation"
 [jax2tf_cumulative_reduction]: https://github.com/google/jax/blob/main/jax/experimental/jax2tf/jax2tf.py#L2172
+[StableHLO]: https://github.com/openxla/stablehlo
```

### Comparing `tf2jax-0.3.3/README.md` & `tf2jax-0.3.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: tf2jax
+Version: 0.3.4
+Summary: TF2JAX: Convert TensorFlow to JAX
+Home-page: https://github.com/deepmind/tf2jax
+Author: DeepMind
+Author-email: tf2jax-dev@google.com
+License: Apache 2.0
+Keywords: jax tensorflow conversion translate
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # TF2JAX
 
 ![CI status](https://github.com/deepmind/tf2jax/workflows/ci/badge.svg)
 ![pypi](https://img.shields.io/pypi/v/tf2jax)
 
 TF2JAX is an experimental library for converting [TensorFlow] functions/graphs
 to [JAX] functions.
@@ -177,15 +203,15 @@
 import tensorflow_hub as hub
 
 hub_model = hub.load("/tmp/blah")
 jax_func, jax_params = tf2jax.convert(tf.function(hub_model), tf.zeros_like(x))
 jax_outputs, updated_jax_params = jax_func(jax_params, x)
 ```
 
-## JAX to TensorFlow and Back Again.
+## JAX to TensorFlow and back again.
 
 `tf2jax.convert_functional` can convert the outputs of `jax2tf.convert` back
 into JAX code.
 
 ```python
 # Some JAX function.
 def forward(*inputs):
@@ -296,14 +322,57 @@
 operations from `reduce_window` operations generated by JAX2TF. This provides
 better performance because `reduce_window` implementation of these ops have
 O(N^2) complexity on CPU and GPU backends, and can suffer from long compilation
 times due to aggressive constant folding.
 
 See [jax2tf_cumulative_reduction] for more context.
 
+## JAX2TF Native Serialization and XlaCallModule.
+
+From JAX v0.4.7 and onward, `jax2tf.convert` preferred mode of operation (soon
+to be default) is **native serialization** in which the target function is
+lowered to [StableHLO] and wrapped in a single TensorFlow op, `XlaCallModule`.
+
+The new native serialization format will more faithfully reproduce the semantics
+of the target function, at the cost of some reduced flexibility for downstream
+processing as the computation graph is no longer exposed as a tf.Graph.
+
+`XlaCallModule` is supported by TF2JAX from v0.3.4 and onward.
+
+However as this makes use of a custom JAX primitive that aims to encapsulate
+[StableHLO] payload found in `XlaCallModule`, it does not possess JAX rules for
+transformations such as (but not limited to) batching and differentiation.
+
+* **Differentiation**: first order derivative of serialized function is
+still supported through custom gradients requested at serialization time with
+`jax2tf.convert(..., with_gradient=True)`. This is the default behaviour.
+* **Batching**: `jax.vmap` will fail, though users may be able to naively
+replicate the desired behavior with `jax.lax.map`, albeit with poorer
+performance.
+
+### Platform Specificity
+
+Natively serialized JAX programs are platform specific ([link](https://github.com/google/jax/blob/main/jax/experimental/jax2tf/README.md#natively-serialized-jax-modules-are-platform-specific)). Executing a natively
+serialized program on platforms other than the one for which it was lowered,
+would raise a ValueError, e.g.:
+
+```python
+ValueError: Unsupported backend: `cpu` not in `('tpu',)`.
+```
+
+This matches the behaviour of `XlaCallModule`.
+
+Users can disable this check via a config flag, but the resulting program may
+be slower or fail to execute completely.
+
+```python
+with tf2jax.override_config("xlacallmodule_strict_checks", False):
+  jax_func(np.zeros((20, 5), np.float32))
+```
+
 ## Limitations
 
 Currently, only a subset of TensorFlow ops are supported, and not necessarily
 all functionalities are supported for some ops. The code will fail fast. Support
 for additional TensorFlow ops are added on a as-needed basis. Please submit your
 requests via Github issues or send in your pull requests.
 
@@ -356,7 +425,8 @@
 
 [DeepMind JAX Ecosystem]: https://deepmind.com/blog/article/using-jax-to-accelerate-our-research "DeepMind JAX Ecosystem"
 [DeepMind JAX Ecosystem citation]: https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt "Citation"
 [JAX]: https://github.com/google/jax "JAX on GitHub"
 [TensorFlow]: https://github.com/tensorflow/tensorflow "TensorFlow on GitHub"
 [jax2tf documentation]: https://github.com/google/jax/blob/master/jax/experimental/jax2tf/README.md#calling-tensorflow-functions-from-jax "jax2tf documentation"
 [jax2tf_cumulative_reduction]: https://github.com/google/jax/blob/main/jax/experimental/jax2tf/jax2tf.py#L2172
+[StableHLO]: https://github.com/openxla/stablehlo
```

### Comparing `tf2jax-0.3.3/setup.py` & `tf2jax-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/__init__.py` & `tf2jax-0.3.4/tf2jax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from tf2jax._src.tf2jax import AnnotatedFunction
 
 from tf2jax._src.tf2jax import convert
 from tf2jax._src.tf2jax import convert_from_restored
 from tf2jax._src.tf2jax import convert_functional
 from tf2jax._src.tf2jax import convert_functional_from_restored
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 #  _________________________________________
 # / Please don't use symbols in `_src` they \
 # \ are not part of the tf2jax public API.    /
 #  -----------------------------------------
 #         \   ^__^
 #          \  (oo)\_______
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/__init__.py` & `tf2jax-0.3.4/tf2jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/_src/config.py` & `tf2jax-0.3.4/tf2jax/_src/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     infer_relu_from_jax2tf=True,
     infer_cumulative_reduction_from_jax2tf=True,
     raise_on_prevent_gradient=True,
     # TensorFlow uses high/highest precision on TPU.
     resize_bilinear_precision="highest",
     # This is temporary until checkify supports debug mode.
     enable_checkify_for_asserts=False,
+    # Enable checks that each natively serialized computation is executed on a
+    # platform for which it was lowered.
+    xlacallmodule_strict_checks=True,
 )
 
 
 def get_config(name: str) -> Union[bool, str]:
   return _config[name]
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/experimental/__init__.py` & `tf2jax-0.3.4/tf2jax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/_src/experimental/mhlo.py` & `tf2jax-0.3.4/tf2jax/experimental/mhlo.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,33 @@
 
 import functools
 import threading
 from typing import Any, Dict, Tuple
 
 import jax
 from jax import core
-from jax._src.lib import xla_client as xc
-import jax._src.util as util  # pylint: disable=consider-using-from-import
 from jax.interpreters import mlir
+from jax.lib import xla_client as xc
 
 from jaxlib.mlir import ir
 from jaxlib.mlir.dialects import mhlo
 
 import numpy as np
 
-_program_cache: Dict[str, Tuple[str, xc._xla.XlaComputation]] = {}
+from tf2jax.experimental import util
+
+
+_program_cache: Dict[str, Tuple[str, xc.XlaComputation]] = {}
 _program_lock = threading.Lock()
 
 mhlo_apply_p = core.Primitive("mhlo_apply")
 mhlo_apply_p.multiple_results = True
 
 
-def _get_program(mhlo_text: str) -> Tuple[str, xc._xla.XlaComputation]:
+def _get_program(mhlo_text: str) -> Tuple[str, xc.XlaComputation]:
   """Thread-safe cache of MHLO string to XlaComputation."""
   try:
     return _program_cache[mhlo_text]
   except KeyError:
     pass
 
   with _program_lock:
@@ -81,15 +83,15 @@
 
 def mhlo_apply_abstract_eval(*args, mhlo_text: str):
   del args
   _, program = _get_program(mhlo_text)
   result_spec = program.program_shape().result_shape()
   assert result_spec.is_tuple()
   return tuple([
-      jax.ShapedArray(spec.dimensions(), spec.element_type())
+      core.ShapedArray(spec.dimensions(), spec.element_type())
       for spec in result_spec.tuple_shapes()
   ])
 
 mhlo_apply_p.def_abstract_eval(mhlo_apply_abstract_eval)
 
 
 def mhlo_apply_lowering(ctx: mlir.LoweringRuleContext, *args, mhlo_text: str):
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/experimental/mhlo_test.py` & `tf2jax-0.3.4/tf2jax/experimental/mhlo_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from absl.testing import absltest
 from absl.testing import parameterized
 
 import chex
 import jax
 import numpy as np
 
-from tf2jax._src.experimental import mhlo
+from tf2jax.experimental import mhlo
 
 
 def _convert_to_mhlo(jax_fn, inputs, *, dialect):
   lowered_forward = jax_fn.lower(*inputs)
   mhlo_text = lowered_forward.as_text(dialect=dialect)
   return mhlo_text
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/linalg_ops_test.py` & `tf2jax-0.3.4/tf2jax/_src/linalg_ops_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,17 @@
     jax_func = self.variant(jax_func)
 
     rng = jax.random.PRNGKey(42)
     jax_results, new_jax_params = jax_func(jax_params, *inputs, rng=rng)
     tf_results = tf_func(*inputs)
 
     # Check outputs
-    for tf_res, jax_res in zip(
-        tree.flatten(tf_results), tree.flatten(jax_results)):
+    for tf_res, jax_res in jax.util.safe_zip(
+        tree.flatten(tf_results), tree.flatten(jax_results)
+    ):
       self.assertEqual(tf_res.shape, jax_res.shape)
       if not check_shape_only:
         self.assertAllClose(np.asarray(tf_res), jax_res, atol=1e-5)
 
     return jax_results, new_jax_params
 
   @chex.variants(with_jit=True, without_jit=True)
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/numpy_compat.py` & `tf2jax-0.3.4/tf2jax/_src/numpy_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     tf.float32: jnp.float32,
     tf.float64: jnp.float64,
     tf.complex64: jnp.complex64,
     tf.complex128: jnp.complex128,
 }
 
 
-_NP_LIKES = (np.ndarray, np.number, np.bool_, bool, int, float)
+_NP_LIKES = (np.ndarray, np.number, np.bool_, bool, int, float, complex)
 
 
 # We avoids importing jax2tf.shape_poly.is_poly_dim as jax2tf often depends
 # on the most recent tensorflow version.
 # This should reflect is_poly_dim() at
 # https://github.com/google/jax/blob/main/jax/experimental/jax2tf/shape_poly.py#L676
 def is_poly_dim(x):
@@ -163,14 +163,25 @@
     axis = axis if axis < 0 else -(params.ndim - axis)
     take_fn = lambda p, i: jnp.take(p, i, axis=axis)
     for _ in range(batch_dims):
       take_fn = jax.vmap(take_fn)
     return take_fn(params, indices)
 
 
+def scatter_nd(indices, updates, shape):
+  np_ = _get_np(indices, updates)
+  res = np_.zeros(shape, updates.dtype)
+  key = tuple(np_.moveaxis(indices, -1, 0))
+  if np_ is np:
+    res[key] = updates
+  else:
+    res = res.at[key].set(updates)
+  return res
+
+
 # Reduction ops.
 def all_(arr, axis: Union[int, Sequence[int]], keepdims: bool):
   axis = tuple(axis) if isinstance(axis, (list, tuple)) else (axis,)
   return _get_np(arr).all(arr, axis=axis, keepdims=keepdims)
 
 
 def any_(arr, axis: Union[int, Sequence[int]], keepdims: bool):
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/numpy_compat_test.py` & `tf2jax-0.3.4/tf2jax/_src/numpy_compat_test.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/_src/ops.py` & `tf2jax-0.3.4/tf2jax/_src/ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,37 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Experimental functions for converting TF graphs to Jax functions."""
 
 import dataclasses
 import functools
-from typing import Any, Callable, List, Optional, Mapping, Sequence, Set, Tuple, Union
+from typing import Any, Callable, List, Optional, Mapping, Protocol, Sequence, Set, Tuple, Union
 
 from absl import logging
 
 import jax
 from jax._src.lax import control_flow as lax_control_flow
 from jax.experimental import checkify
 import jax.numpy as jnp
 import numpy as np
 import tensorflow as tf
 from tf2jax._src import config
 from tf2jax._src import numpy_compat as anp
 from tf2jax._src import xla_utils
 
 
+ArrayLike = Union[np.ndarray, jnp.ndarray]
+
 # NoOp inserted to trigger side effects in function with no return values.
 _EMPTY_RETURN_OP_NAME = "__NO_RETURN__"
 _EMPTY_RETURN_VALUE = object()
 
+safe_zip = jax.util.safe_zip
+
 
 def _check_attrs(proto, expected: Set[str]):
   unexpected = []
   for k, v in proto.attr.items():
     # Ignore attributes with "_" prefix, as they appear to be undocumented.
     if k not in expected and not k.startswith("_"):
       unexpected.append("  `" + f"{k}={v}".strip() + "`")
@@ -67,17 +71,20 @@
     "AddN": _get_jax_op(
         lambda *args: anp.sum_(anp.stack(args, axis=0), axis=0, keepdims=False),
         {"T", "N"}),
     "AddV2": _get_jax_op(anp.add, {"T"}),
     "ArgMax": _get_jax_op(jnp.argmax, {"T", "Tidx", "output_type"}),
     "ArgMin": _get_jax_op(jnp.argmin, {"T", "Tidx", "output_type"}),
     "Acosh": _get_jax_op(jnp.arccosh, {"T"}),
+    "Angle": _get_jax_op(jnp.angle, {"T", "Tout"}),
     "Asinh": _get_jax_op(jnp.arcsinh, {"T"}),
     "Atanh": _get_jax_op(jnp.arctanh, {"T"}),
     "Atan2": _get_jax_op(jnp.arctan2, {"T"}),
+    "BesselI0e": _get_jax_op(jax.lax.bessel_i0e, {"T"}),
+    "BesselI1e": _get_jax_op(jax.lax.bessel_i1e, {"T"}),
     "BitwiseAnd": _get_jax_op(jnp.bitwise_and, {"T"}),
     "BitwiseOr": _get_jax_op(jnp.bitwise_or, {"T"}),
     "BitwiseXor": _get_jax_op(jnp.bitwise_xor, {"T"}),
     "BroadcastTo": _get_jax_op(anp.broadcast_to, {"T", "Tidx"}),
     "Ceil": _get_jax_op(jnp.ceil, {"T"}),
     "Cholesky": _get_jax_op(jnp.linalg.cholesky, {"T"}),
     "Complex": _get_jax_op(jax.lax.complex, {"T", "Tout"}),
@@ -90,20 +97,40 @@
     "Elu": _get_jax_op(jax.nn.elu, {"T"}),
     "Equal": _get_jax_op(anp.equal, {"T", "incompatible_shape_error"}),
     "Erf": _get_jax_op(jax.lax.erf, {"T"}),
     "Erfc": _get_jax_op(jax.lax.erfc, {"T"}),
     "Erfinv": _get_jax_op(jax.lax.erf_inv, {"T"}),
     "Exp": _get_jax_op(jnp.exp, {"T"}),
     "Expm1": _get_jax_op(jnp.expm1, {"T"}),
+    "FFT": _get_jax_op(
+        functools.partial(jnp.fft.fftn, axes=(-1,)), {"Tcomplex"}),
+    "FFT2D": _get_jax_op(
+        functools.partial(jnp.fft.fftn, axes=(-2, -1,)), {"Tcomplex"}),
+    "FFT3D": _get_jax_op(
+        functools.partial(jnp.fft.fftn, axes=(-3, -2, -1,)), {"Tcomplex"}),
     "Floor": _get_jax_op(jnp.floor, {"T"}),
     "FloorMod": _get_jax_op(anp.mod, {"T"}),
     "FloorDiv": _get_jax_op(anp.floor_divide, {"T"}),
     "Greater": _get_jax_op(anp.greater, {"T"}),
     "GreaterEqual": _get_jax_op(anp.greater_equal, {"T"}),
     "Identity": _get_jax_op(lambda x: x, {"T"}),
+    "IFFT": _get_jax_op(
+        functools.partial(jnp.fft.ifftn, axes=(-1,)), {"Tcomplex"}),
+    "IFFT2D": _get_jax_op(
+        functools.partial(jnp.fft.ifftn, axes=(-2, -1,)), {"Tcomplex"}),
+    "IFFT3D": _get_jax_op(
+        functools.partial(jnp.fft.ifftn, axes=(-3, -2, -1,)), {"Tcomplex"}),
+    "IRFFT": _get_jax_op(
+        functools.partial(jnp.fft.irfftn, axes=(-1,)), {"Tcomplex", "Treal"}),
+    "IRFFT2D": _get_jax_op(
+        functools.partial(
+            jnp.fft.irfftn, axes=(-2, -1,)), {"Tcomplex", "Treal"}),
+    "IRFFT3D": _get_jax_op(
+        functools.partial(
+            jnp.fft.irfftn, axes=(-3, -2, -1,)), {"Tcomplex", "Treal"}),
     "Igamma": _get_jax_op(jax.lax.igamma, {"T"}),
     "Igammac": _get_jax_op(jax.lax.igammac, {"T"}),
     "Imag": _get_jax_op(jax.lax.imag, {"T", "Tout"}),
     "IsFinite": _get_jax_op(jnp.isfinite, {"T"}),
     "Invert": _get_jax_op(jnp.bitwise_not, {"T"}),
     "InvertPermutation": _get_jax_op(anp.invert_permutation, {"T"}),
     "L2Loss": _get_jax_op(lambda x: 0.5 * jnp.sum(jnp.square(x)), {"T"}),
@@ -119,23 +146,32 @@
     "Minimum": _get_jax_op(anp.minimum, {"T"}),
     "Maximum": _get_jax_op(anp.maximum, {"T"}),
     "Mul": _get_jax_op(anp.multiply, {"T"}),
     "Neg": _get_jax_op(anp.negative, {"T"}),
     "NoOp": _get_jax_op(lambda: _EMPTY_RETURN_VALUE, set({})),
     "NotEqual": _get_jax_op(anp.not_equal, {"T", "incompatible_shape_error"}),
     "OnesLike": _get_jax_op(jnp.ones_like, {"T"}),
+    "PopulationCount": _get_jax_op(jax.lax.population_count, {"T"}),
     "Pow": _get_jax_op(anp.power, {"T"}),
     "Rank": _get_jax_op(lambda x: np.array(jnp.ndim(x)), {"T"}),
     "Real": _get_jax_op(jax.lax.real, {"T", "Tout"}),
     "ReadVariableOp": _get_jax_op(lambda x: x, {"dtype"}),
     "RealDiv": _get_jax_op(anp.true_divide, {"T"}),
     "Reciprocal": _get_jax_op(anp.reciprocal, {"T"}),
     "Relu": _get_jax_op(jax.nn.relu, {"T"}),
     "Relu6": _get_jax_op(jax.nn.relu6, {"T"}),
     "ReverseV2": _get_jax_op(anp.flip, {"T", "Tidx"}),
+    "RFFT": _get_jax_op(
+        functools.partial(jnp.fft.rfftn, axes=(-1,)), {"Tcomplex", "Treal"}),
+    "RFFT2D": _get_jax_op(
+        functools.partial(
+            jnp.fft.rfftn, axes=(-2, -1,)), {"Tcomplex", "Treal"}),
+    "RFFT3D": _get_jax_op(
+        functools.partial(
+            jnp.fft.rfftn, axes=(-3, -2, -1,)), {"Tcomplex", "Treal"}),
     "RightShift": _get_jax_op(jnp.right_shift, {"T"}),
     "Round": _get_jax_op(jnp.round, {"T"}),
     "Rsqrt": _get_jax_op(jax.lax.rsqrt, {"T"}),
     "Shape": _get_jax_op(lambda x: np.array(jnp.shape(x)), {"T", "out_type"}),
     "Sigmoid": _get_jax_op(jax.nn.sigmoid, {"T"}),
     "Sign": _get_jax_op(jnp.sign, {"T"}),
     "Sin": _get_jax_op(jnp.sin, {"T"}),
@@ -167,20 +203,14 @@
     "Where": _get_jax_op(jnp.argwhere, {"T"}),
     "ZerosLike": _get_jax_op(jnp.zeros_like, {"T"}),
     # The assignment logic is handled in _OpNode and convert().
     "AssignAddVariableOp": _get_jax_op(jnp.add, {"dtype"}),
     "AssignSubVariableOp": _get_jax_op(jnp.subtract, {"dtype"}),
     "AssignVariableOp": _get_jax_op(
         lambda var, x: x, {"dtype", "validate_shape"}),
-    "RFFT":
-        _get_jax_op(lambda x, a: jnp.fft.rfft(x, a[0]), {"Tcomplex", "Treal"}),
-    "IRFFT":
-        _get_jax_op(lambda x, a: jnp.fft.irfft(x, a[0]), {"Tcomplex", "Treal"}),
-    "Angle":
-        _get_jax_op(jnp.angle, {"T", "Tout"}),
 }
 
 
 def get_parser(op_name: str) -> Callable[..., Callable[..., Any]]:
   return _jax_ops[op_name]
 
 
@@ -200,24 +230,36 @@
   return func
 
 
 def register_operation(op_name):
   return functools.partial(_register, op_name=op_name)
 
 
+class _LibraryFunction(Protocol):
+  # Inputs corresponding to VarHandleOp
+  variable_input_specs: Optional[Tuple[tf.TensorSpec, ...]] = None
+
+
 @dataclasses.dataclass
 class _HigherOrderFunction:
   """Base class for higher order ops."""
   inner_fn_names: Mapping[str, str]
 
   def get_inner_functions(
       self, library_functions: Mapping[str, Callable[..., Any]]
   ) -> Mapping[str, Callable[..., Any]]:
     return {k: library_functions[v] for k, v in self.inner_fn_names.items()}
 
+  def get_additional_inputs(
+      self, **inner_functions: _LibraryFunction
+  ) -> Tuple[str, ...]:
+    """Get additional input names required by the op."""
+    del inner_functions
+    return ()
+
 
 @register_operation("All")
 def _all(proto):
   _check_attrs(proto, {"Tidx", "keep_dims"})
   keep_dims = proto.attr["keep_dims"].b
   return lambda x, axis: anp.all_(x, axis=axis.tolist(), keepdims=keep_dims)
 
@@ -271,14 +313,108 @@
       window_counts = jax.lax.reduce_window(
           jnp.ones_like(x), **reduce_window_args)
     return pooled / window_counts
 
   return _func
 
 
+@register_operation("BatchToSpaceND")
+def _batch_to_space_nd(proto):
+  """Parse a BatchToSpaceND Op."""
+  _check_attrs(proto, {"T", "Tblock_shape", "Tcrops"})
+
+  def _func(
+      operand: jnp.ndarray, block_shape: jnp.ndarray, crops: jnp.ndarray
+  ) -> jnp.ndarray:
+    batch, *other_shape = list(operand.shape)
+    block_shape = block_shape.tolist()
+    num_spatial = len(block_shape)
+    crops = crops.tolist()
+    spatial_shape = other_shape[:num_spatial]
+    remaining_shape = other_shape[num_spatial:]
+
+    new_shape = (
+        block_shape
+        + [batch // np.prod(block_shape)]
+        + spatial_shape
+        + remaining_shape
+    )
+    reshaped = operand.reshape(new_shape)
+
+    permuted_axes = [num_spatial]
+    for idx in range(num_spatial):
+      permuted_axes.extend([idx + 1 + num_spatial, idx])
+    permuted_axes.extend(list(range(num_spatial * 2 + 1, len(new_shape))))
+    permuted = jnp.transpose(reshaped, axes=permuted_axes)
+
+    uncropped_shape = [new_shape[num_spatial]]
+    for idx in range(num_spatial):
+      uncropped_shape.append(block_shape[idx] * spatial_shape[idx])
+    uncropped_shape.extend(remaining_shape)
+    uncropped = permuted.reshape(uncropped_shape)
+
+    cropped_slice = [slice(None)]
+    for idx in range(num_spatial):
+      cropped_slice.append(
+          slice(crops[idx][0], uncropped_shape[1 + idx] - crops[idx][1])
+      )
+    cropped_slice += [slice(None)] * len(remaining_shape)
+    cropped = uncropped[tuple(cropped_slice)]
+
+    return cropped
+
+  return _func
+
+
+@register_operation("SpaceToBatchND")
+def _space_to_batch_nd(proto):
+  """Parse a SpaceToBatchND Op."""
+  _check_attrs(proto, {"T", "Tblock_shape", "Tpaddings"})
+
+  def _func(
+      operand: jnp.ndarray, block_shape: jnp.ndarray, paddings: jnp.ndarray
+  ) -> jnp.ndarray:
+    batch, *other_shape = list(operand.shape)
+    block_shape = block_shape.tolist()
+    num_spatial = len(block_shape)
+    paddings = paddings.tolist()
+    remaining_shape = other_shape[num_spatial:]
+
+    paddings = [[0, 0]] + paddings + [[0, 0]] * len(remaining_shape)
+    padded = jnp.pad(operand, paddings)
+    padded_shape = padded.shape
+
+    new_shape = [batch]
+    for idx in range(num_spatial):
+      new_shape.extend(
+          [padded_shape[idx + 1] // block_shape[idx], block_shape[idx]]
+      )
+    new_shape.extend(remaining_shape)
+    reshaped = padded.reshape(new_shape)
+
+    permuted_axes = []
+    for idx in range(num_spatial):
+      permuted_axes.append(idx * 2 + 2)
+    permuted_axes += [0]
+    for idx in range(num_spatial):
+      permuted_axes.append(idx * 2 + 1)
+    permuted_axes.extend(list(range(num_spatial * 2 + 1, len(new_shape))))
+    permuted = jnp.transpose(reshaped, axes=permuted_axes)
+
+    flatten_shape = [batch * np.prod(block_shape)]
+    for idx in range(num_spatial):
+      flatten_shape.append(padded_shape[idx + 1] // block_shape[idx])
+    flatten_shape.extend(remaining_shape)
+    flattened = permuted.reshape(flatten_shape)
+
+    return flattened
+
+  return _func
+
+
 @register_operation("BiasAdd")
 def _bias_add(proto):
   """Parse a BiasAdd Op."""
   _check_attrs(proto, {"T", "data_format"})
 
   data_format = str(proto.attr["data_format"].s, "utf-8")
   if data_format == "NHWC":
@@ -521,15 +657,15 @@
   """Parse a Cumsum Op."""
   _check_attrs(proto, {"T", "Tidx", "exclusive", "reverse"})
 
   exclusive = proto.attr["exclusive"].b
   reverse = proto.attr["reverse"].b
 
   def _func(x: jnp.ndarray, axis: jnp.ndarray) -> jnp.ndarray:
-    axis: int = axis.tolist()
+    axis = axis.item()
     if reverse:
       x = anp.flip(x, axis=axis)
     if exclusive:
       pad_shape = list(x.shape)
       pad_shape[axis] = 1
       x = anp.concatenate([np.zeros(pad_shape, dtype=x.dtype), x], axis=axis)
       x = x[(slice(None),) * axis + (slice(0, -1), Ellipsis)]
@@ -597,17 +733,21 @@
 
 @register_operation("DivNoNan")
 def _div_no_nan(proto):
   """Parse a DivNoNan op."""
   _check_attrs(proto, {"T"})
 
   @jax.custom_gradient
-  def _func(x: jnp.ndarray, y: jnp.ndarray) -> jnp.ndarray:
-
-    def _grad(g: jnp.ndarray) -> jnp.ndarray:
+  def _func(
+      x: jnp.ndarray, y: jnp.ndarray
+  ) -> Tuple[
+      jnp.ndarray,
+      Callable[[jnp.ndarray], Tuple[jnp.ndarray, jnp.ndarray]],
+  ]:
+    def _grad(g: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
       """Given upstream grad G and a Div op: Z = X/Y, the gradients are.
 
         dX = G / Y
         dY = -G*X / Y^2 = (X/Y) * -G / Y = -G*Z / Y
 
       Following tensorflow/tensorflow/c/experimental/gradients/math_grad.cc
       for handling NaNs.
@@ -632,15 +772,15 @@
 @register_operation("Eig")
 def _eig(proto):
   """Parse an Eig Op."""
   _check_attrs(proto, {"T", "Tout", "compute_v"})
 
   compute_v = proto.attr["compute_v"].b
 
-  def _func(x: jnp.ndarray) -> jnp.ndarray:
+  def _func(x: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
     if compute_v:
       evals, evecs = jnp.linalg.eig(x)
     else:
       evals = jnp.linalg.eigvals(x)
       evecs = jnp.zeros(shape=(), dtype=evals.dtype)
 
     # Sorting by eigenvalues to match tf.raw_ops.Eig better.
@@ -664,15 +804,15 @@
   _check_attrs(proto, {"T", "compute_v"})
 
   compute_v = proto.attr["compute_v"].b
 
   def symmetrize(x):
     return jnp.tril(x) + jnp.swapaxes(jnp.tril(x, -1), -2, -1)
 
-  def _func(x: jnp.ndarray) -> jnp.ndarray:
+  def _func(x: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray]:
     if compute_v:
       evals, evecs = jnp.linalg.eigh(x, symmetrize_input=False)
     else:
       # symmetrize_input does not exist for eigvalsh.
       # See https://github.com/google/jax/issues/9473
       evals, evecs = jnp.linalg.eigvalsh(symmetrize(x)), None
 
@@ -680,19 +820,18 @@
     sort_fn = lambda vals, inds: vals[..., inds]
     for _ in range(len(x.shape) - 2):
       sort_fn = jax.vmap(sort_fn, in_axes=(0, 0))
     einds = jnp.argsort(evals, axis=-1)
     evals = sort_fn(evals, einds)
     if compute_v:
       evecs = sort_fn(evecs, einds)
-
-    if compute_v:
-      return evals, evecs
     else:
-      return evals, jnp.zeros(shape=(), dtype=evals.dtype)
+      evecs = jnp.zeros(shape=(), dtype=evals.dtype)
+
+    return evals, evecs
 
   return _func
 
 
 @register_operation("Einsum")
 def _einsum(proto):
   """Parse an Einsum Op."""
@@ -731,16 +870,17 @@
 
   shape = [dim.size for dim in proto.attr["shape"].shape.dim]
 
   def is_compatible(x, s):
     return x == -1 or s == -1 or x == s
 
   def _func(x: jnp.ndarray) -> jnp.ndarray:
-    if (len(x.shape) != len(shape) or
-        not all(is_compatible(x, s) for x, s in zip(x.shape, shape))):
+    if len(x.shape) != len(shape) or not all(
+        is_compatible(x, s) for x, s in safe_zip(x.shape, shape)
+    ):
       raise ValueError(f"Expected shape={shape}, found {x.shape}.")
     return x
 
   return _func
 
 
 @register_operation("ExpandDims")
@@ -856,18 +996,18 @@
     raise ValueError(f"batch_dims={batch_dims} must be non-negative.")
 
   # TODO(b/249826984) Add test for ResourceGather, dtype and validate_indices.
 
   def _func(
       params: jnp.ndarray,
       indices: jnp.ndarray,
-      axis: jnp.ndarray = np.array(0, dtype=np.int32),
+      axis: ArrayLike = np.array(0, dtype=np.int32),
   ) -> jnp.ndarray:
     return anp.gather(
-        params, indices, axis=axis.tolist(), batch_dims=batch_dims)
+        params, indices, axis=axis.item(), batch_dims=batch_dims)
 
   return _func
 
 
 @dataclasses.dataclass
 class _IdentityN(_HigherOrderFunction):
   """Represents a IdentityN Op."""
@@ -944,14 +1084,27 @@
       updates: jnp.ndarray,
   ) -> jnp.ndarray:
     return jnp.asarray(inputs).at[indices].set(updates)
 
   return _func
 
 
+@register_operation("LeakyRelu")
+def _leaky_relu(proto):
+  """Parse a LeakyRelu Op."""
+  _check_attrs(proto, {"T", "alpha"})
+
+  alpha = proto.attr["alpha"].f
+
+  def _func(features: jnp.ndarray) -> jnp.ndarray:
+    return jax.nn.leaky_relu(features, alpha)
+
+  return _func
+
+
 @register_operation("LogSoftmax")
 def _log_softmax(proto):
   _check_attrs(proto, {"T"})
   return lambda x: jax.nn.log_softmax(x, axis=-1)
 
 
 @register_operation("MatMul")
@@ -1020,31 +1173,68 @@
     outputs = diag_fn(diagonals)
     mask = diag_fn(jnp.ones_like(diagonals, dtype=jnp.bool_))
     return jnp.where(mask, outputs, padding_value)
 
   return _func
 
 
+@register_operation("MatrixSetDiagV3")
+def _matrix_set_diag(proto):
+  """Parse a MatrixSetDiagV3 op."""
+  _check_attrs(proto, {"T", "align"})
+
+  align = str(proto.attr["align"].s, "utf-8")
+  if align != "RIGHT_LEFT":
+    raise ValueError(f"MatrixSetDiagV3 does not support `align={align}` yet.")
+
+  def _func(
+      inputs: jnp.ndarray,
+      diagonals: jnp.ndarray,
+      k: jnp.ndarray,
+  ) -> jnp.ndarray:
+    k = k.item()
+
+    def diag_fn(inps: jnp.ndarray, diag: jnp.ndarray) -> jnp.ndarray:
+      assert len(inps.shape) == 2, inps.shape
+      assert len(diag.shape) == 1, diag.shape
+      if ((diag.shape[0] + k > inps.shape[1]) or
+          (diag.shape[0] - k > inps.shape[0])):
+        raise ValueError(
+            f"Incompatible inputs shape ({inputs.shape}) and diagonals shape "
+            f"({diagonals.shape}).")
+
+      return jnp.diagflat(diag, k=k)[:inps.shape[0], :inps.shape[1]]
+
+    for _ in range(len(diagonals.shape) - 1):
+      diag_fn = jax.vmap(diag_fn)
+
+    outputs = diag_fn(inputs, diagonals)
+    mask = diag_fn(inputs, jnp.ones_like(diagonals, dtype=jnp.bool_))
+    return jnp.where(mask, outputs, inputs)
+
+  return _func
+
+
 @register_operation("MatrixBandPart")
 def _matrix_band_part(proto):
   """Parse a MatrixBandPart op."""
   _check_attrs(proto, {"T", "Tindex"})
 
   def _func(
       x: jnp.ndarray,
       lower: jnp.ndarray,
       upper: jnp.ndarray,
   ) -> jnp.ndarray:
     if len(x.shape) < 2:
       raise ValueError(
           f"Expected input of at least rank 2, found {len(x.shape)}")
     mask_shape = x.shape[-2:]
-    lower = lower.tolist() + 1 if lower.tolist() >= 0 else max(mask_shape)
+    lower = lower.item() + 1 if lower.item() >= 0 else max(mask_shape)
     mask_lower = jnp.tril(jnp.ones(mask_shape, jnp.int32), -lower)
-    upper = upper.tolist() + 1 if upper.tolist() >= 0 else max(mask_shape)
+    upper = upper.item() + 1 if upper.item() >= 0 else max(mask_shape)
     mask_upper = jnp.triu(jnp.ones(mask_shape, jnp.int32), upper)
     return jnp.where((mask_lower + mask_upper) == 0, x, 0)
 
   return _func
 
 
 @register_operation("MatrixTriangularSolve")
@@ -1146,15 +1336,15 @@
       on_value: jnp.ndarray,
       off_value: jnp.ndarray,
   ) -> jnp.ndarray:
     if axis != -1 and axis != len(indices.shape):
       raise ValueError(f"OneHot does not support axis={axis} yet, "
                        f"indices.shape={indices.shape}.")
 
-    mask = jax.nn.one_hot(indices, num_classes=depth, dtype=jnp.int32)
+    mask = jax.nn.one_hot(indices, num_classes=depth.item(), dtype=jnp.int32)
     return mask * on_value + (1 - mask) * off_value
 
   return _func
 
 
 @register_operation("Pack")
 def _pack(proto):
@@ -1196,14 +1386,25 @@
 
 class _PartitionedCall(_HigherOrderFunction):
   """Represents a PartitionedCall Op."""
 
   def __call__(self, *args, inner_fn, rng=None):
     return inner_fn(*args, rng=rng)
 
+  def get_additional_inputs(
+      self, **inner_functions: _LibraryFunction
+  ) -> Tuple[str, ...]:
+    """Get additional input names required by the op."""
+    return self._get_additional_inputs(**inner_functions)
+
+  def _get_additional_inputs(
+      self, inner_fn: _LibraryFunction
+  ) -> Tuple[str, ...]:
+    return tuple(spec.name for spec in inner_fn.variable_input_specs)
+
 
 @register_operation("StatefulPartitionedCall")
 @register_operation("PartitionedCall")
 def _partitioned_call(proto):
   """Parse a PartitionedCall op."""
   _check_attrs(proto,
                {"f", "Tin", "Tout", "config", "config_proto", "executor_type"})
@@ -1233,15 +1434,17 @@
 def _prevent_gradient(proto):
   """Parse a PreventGradient op."""
   _check_attrs(proto, {"T", "message"})
 
   message = str(proto.attr["message"].s, "utf-8")
 
   @jax.custom_gradient
-  def _raise_func(operand: jnp.ndarray) -> jnp.ndarray:
+  def _raise_func(
+      operand: jnp.ndarray,
+  ) -> Tuple[jnp.ndarray, Callable[..., Any]]:
     def grad_fn(_):
       raise LookupError(f"Gradient explicitly prevented on node {proto.name}. "
                         f"Original reason: {message}")
     return operand, grad_fn
 
   def _warn_func(operand: jnp.ndarray) -> jnp.ndarray:
     logging.warning("PreventGradient ignored on node %s. Original reason: %s",
@@ -1461,17 +1664,15 @@
   _check_attrs(proto, {"T", "Tindices"})
 
   def _func(
       indices: jnp.ndarray,
       updates: jnp.ndarray,
       shape: jnp.ndarray,
   ) -> jnp.ndarray:
-    zeros = jnp.zeros(shape, updates.dtype)
-    key = tuple(jnp.moveaxis(indices, -1, 0))
-    return zeros.at[key].set(updates)
+    return anp.scatter_nd(indices, updates, shape)
 
   return _func
 
 
 @register_operation("SelectV2")
 @register_operation("Select")
 def _select(proto):
@@ -1496,15 +1697,15 @@
 
   def _func(
       x: jnp.ndarray,
       begins: jnp.ndarray,
       sizes: jnp.ndarray,
   ) -> jnp.ndarray:
     """`begins` and `sizes` must be concrete arrays."""
-    slices = [slice(b, b + s) for b, s in zip(begins, sizes)]
+    slices = [slice(b, b + s) for b, s in safe_zip(begins, sizes)]
     return x[tuple(slices)]
 
   return _func
 
 
 @register_operation("Softmax")
 def _softmax(proto):
@@ -1549,15 +1750,15 @@
   def _func(
       value: jnp.ndarray,
       size_splits: jnp.ndarray,
       axis: jnp.ndarray,
   ) -> jnp.ndarray:
     assert size_splits.shape[0] == num_split, (size_splits.shape[0], num_split)
     splits = size_splits.tolist()
-    axis = axis.tolist()
+    axis = axis.item()
     defined_size = sum([x for x in splits if x >= 0])
     splits = [x if x >= 0 else value.shape[axis] - defined_size for x in splits]
     indices = np.cumsum(np.array(splits), axis=0)
     assert indices[-1] == value.shape[axis]
     return anp.split(value, indices[:-1], axis=axis)
 
   return _func
@@ -1609,15 +1810,15 @@
   def _func(
       logits: jnp.ndarray,
       num_samples: jnp.ndarray,
       seed: jnp.ndarray,
   ) -> jnp.ndarray:
     assert seed.shape == (2,), seed.shape
     seed = seed.astype(jnp.uint32)
-    shape = (num_samples, logits.shape[0])
+    shape = (num_samples.item(), logits.shape[0])
     samples = jax.random.categorical(seed, logits, shape=shape)
     return samples.astype(jax_dtype).transpose([1, 0])
 
   return _func
 
 
 @register_operation("StatelessRandomNormalV2")
@@ -1625,15 +1826,15 @@
   """Parse a StatelessRandomNormalV2 op."""
   _check_attrs(proto, {"T", "Tshape", "dtype"})
 
   dtype = tf.as_dtype(proto.attr["dtype"].type)
   jax_dtype = anp.get_jax_dtype(dtype)
 
   def _func(
-      shape: jnp.ndarray,
+      shape: Sequence[int],
       key: jnp.ndarray,
       counter: jnp.ndarray,
       alg: jnp.ndarray,
   ) -> jnp.ndarray:
     del counter, alg  # TODO(b/266553394) combine key and counter?
     return jax.random.normal(key=key, shape=shape, dtype=jax_dtype)
 
@@ -1645,15 +1846,15 @@
   """Parse a StatelessRandomNormalV2 op."""
   _check_attrs(proto, {"T", "Tshape", "dtype"})
 
   dtype = tf.as_dtype(proto.attr["dtype"].type)
   jax_dtype = anp.get_jax_dtype(dtype)
 
   def _func(
-      shape: jnp.ndarray,
+      shape: Sequence[int],
       key: jnp.ndarray,
       counter: jnp.ndarray,
       alg: jnp.ndarray,
   ) -> jnp.ndarray:
     del counter, alg  # TODO(b/266553394) combine key and counter?
     return jax.random.uniform(key=key, shape=shape, dtype=jax_dtype)
 
@@ -1675,28 +1876,33 @@
       counter: jnp.ndarray,
       alg: jnp.ndarray,
       minval: jnp.ndarray = jnp.iinfo(jax_dtype).min,
       maxval: jnp.ndarray = jnp.iinfo(jax_dtype).max,
   ) -> jnp.ndarray:
     del counter, alg  # TODO(b/266553394) combine key and counter?
     return jax.random.randint(
-        key=key, shape=shape, minval=minval, maxval=maxval, dtype=jax_dtype,)
+        key=key,
+        shape=shape.tolist(),
+        minval=minval,
+        maxval=maxval,
+        dtype=jax_dtype,
+    )
 
   return _func
 
 
 def _split_args(
     args: Sequence[Any],
     preds: Sequence[bool],
 ) -> Tuple[Tuple[Tuple[int, Any]], ...]:
   """Split args into two lists based on some predicates."""
   assert len(args) == len(preds), (len(args), len(preds))
   true_args = []
   false_args = []
-  for idx, (arg, pred) in enumerate(zip(args, preds)):
+  for idx, (arg, pred) in enumerate(safe_zip(args, preds)):
     if pred:
       true_args.append((idx, arg))
     else:
       false_args.append((idx, arg))
   return tuple(true_args), tuple(false_args)
 
 
@@ -1714,30 +1920,30 @@
 class _StatelessWhile(_HigherOrderFunction):
   """Represents a StatelessWhile Op."""
 
   def __call__(self, *all_args, cond_fun, body_fun, rng=None):
     # Pull captured arguments out of inputs to cond and body.
     const_idxs_args, trace_idxs_args = _split_args(
         all_args, body_fun.output_is_input)
-    trace_idxs, trace_args = zip(*trace_idxs_args)
+    trace_idxs, trace_args = safe_zip(*trace_idxs_args)
 
     def real_cond(args):
       *cond_args, rng = args
-      cond_idxs_args = tuple(zip(trace_idxs, cond_args))
+      cond_idxs_args = tuple(safe_zip(trace_idxs, cond_args))
       cond_args = _merge_args(const_idxs_args, cond_idxs_args)
       _, cond_key, _ = [None] * 3 if rng is None else jax.random.split(rng, 3)
       outputs = cond_fun(*cond_args, rng=cond_key)
       if len(outputs) != 1:
         raise ValueError(
             f"Expected cond_fun to return a single value, found {outputs}")
       return outputs[0]
 
     def real_body(args):
       *body_args, rng = args
-      body_idxs_args = tuple(zip(trace_idxs, body_args))
+      body_idxs_args = tuple(safe_zip(trace_idxs, body_args))
       body_args = _merge_args(const_idxs_args, body_idxs_args)
       key, _, body_key = [None] * 3 if rng is None else jax.random.split(rng, 3)
       outputs = body_fun(*body_args, rng=body_key)
       outputs = tuple([outputs[idx] for idx in trace_idxs])
       return outputs + (key,)
 
     def maybe_initialise(arg, spec):
@@ -1746,19 +1952,21 @@
         return jnp.zeros(shape=spec.shape, dtype=spec.dtype)
       else:
         return arg
 
     output_specs = jax.eval_shape(real_body, trace_args + (rng,))
     trace_args = tuple(
         maybe_initialise(arg, spec)
-        for arg, spec in zip(trace_args, output_specs))
+        for arg, spec in safe_zip(trace_args, output_specs[:-1]))
 
     outputs = jax.lax.while_loop(real_cond, real_body, trace_args + (rng,))
     *outputs, _ = outputs  # Drop rng.
-    outputs = _merge_args(const_idxs_args, tuple(zip(trace_idxs, outputs)))
+    outputs = _merge_args(
+        const_idxs_args, tuple(safe_zip(trace_idxs, outputs))
+    )
     assert len(outputs) == len(all_args), (len(outputs), len(all_args))
     return outputs
 
 
 @register_operation("StatelessWhile")
 @register_operation("While")
 def _stateless_while(proto):
@@ -1854,15 +2062,17 @@
 def _svd(proto):
   """Parse an Svd Op."""
   _check_attrs(proto, {"T", "compute_uv", "full_matrices"})
 
   compute_uv = proto.attr["compute_uv"].b
   full_matrices = proto.attr["full_matrices"].b
 
-  def _func(x: jnp.ndarray) -> Tuple[jnp.ndarray, jnp.ndarray, jnp.ndarray]:
+  def _func(
+      x: jnp.ndarray,
+  ) -> Tuple[jnp.ndarray, Optional[jnp.ndarray], Optional[jnp.ndarray]]:
     res = jnp.linalg.svd(
         x, compute_uv=compute_uv, full_matrices=full_matrices)
     if compute_uv:
       u, s, vh = res
       v = jnp.conjugate(jnp.swapaxes(vh, -1, -2))
     else:
       u, s, v = None, res, None
@@ -1912,17 +2122,17 @@
 def _tensor_list_reserve(proto):
   """Parse an TensorListReserve Op."""
   _check_attrs(proto, {"element_dtype", "shape_type"})
 
   dtype = tf.as_dtype(proto.attr["element_dtype"].type)
   dtype = anp.get_jax_dtype(dtype)
 
-  def _func(shape: jnp.ndarray, num_elements: jnp.ndarray) -> jnp.ndarray:
+  def _func(shape: jnp.ndarray, num_elements: jnp.ndarray) -> ArrayLike:
     return _create_tensor_list(
-        num_elements.tolist(), shape.tolist(), dtype=dtype)
+        num_elements.item(), shape.tolist(), dtype=dtype)
 
   return _func
 
 
 @register_operation("TensorListSetItem")
 def _tensor_list_set_item(proto):
   """Parse an TensorListSetItem Op."""
@@ -1956,15 +2166,15 @@
 def _tensor_list_stack(proto):
   """Parse an TensorListStack Op."""
   _check_attrs(proto, {"element_dtype", "num_elements"})
 
   dtype = tf.as_dtype(proto.attr["element_dtype"].type)
   dtype = anp.get_jax_dtype(dtype)
 
-  def _func(xs: jnp.ndarray, shape: jnp.ndarray) -> jnp.ndarray:
+  def _func(xs: jnp.ndarray, shape: jnp.ndarray) -> ArrayLike:
     if xs.size == 0:
       xs = _create_tensor_list(xs.shape[0], shape.tolist(), dtype=dtype)
     return xs
 
   return _func
 
 
@@ -1985,15 +2195,15 @@
         operand, indices, updates, dimension_numbers=dimension_numbers)
 
   return _func
 
 
 @register_operation("TopKV2")
 def _top_k(proto):
-  _check_attrs(proto, {"T", "sorted"})
+  _check_attrs(proto, {"T", "sorted", "Tk", "index_type"})
   sorted_arg = proto.attr["sorted"].b
   if not sorted_arg:
     raise ValueError("sorted=False in TopKV2 is not yet supported.")
 
   return jax.lax.top_k
 
 
@@ -2007,23 +2217,35 @@
 def _unpack(proto):
   """Parse a Unpack op."""
   _check_attrs(proto, {"T", "axis", "num"})
 
   axis = proto.attr["axis"].i
   num = proto.attr["num"].i
 
-  def _func(x: jnp.ndarray) -> jnp.ndarray:
+  def _func(x: jnp.ndarray) -> List[jnp.ndarray]:
     if x.shape[axis] != num:
       raise ValueError("Unpack expects dimension of {num} for axis={axis}, "
                        "found {x.shape[axis]}, shape={x.shape}")
     return [anp.squeeze(v, axis=axis) for v in anp.split(x, num, axis=axis)]
 
   return _func
 
 
+# TODO(b271811043) Add unit test.
+@register_operation("VarHandleOp")
+def _var_handle(proto):
+  _check_attrs(
+      proto, {"shared_name", "container", "allowed_devices", "shape", "dtype"})
+
+  def _func():
+    raise ValueError(f"VarHandleOp `{proto.name}` cannot be evaluated.")
+
+  return _func
+
+
 @register_operation("VariableV2")
 def _variable_v2(proto):
   _check_attrs(proto, {"container", "dtype", "shared_name", "shape"})
 
   name = proto.name
 
   def _func():
@@ -2066,15 +2288,15 @@
         lhs,
         rhs,
         window_strides=strides.tolist(),
         padding=[tuple(v) for v in padding],
         lhs_dilation=lhs_dilation.tolist(),
         rhs_dilation=rhs_dilation.tolist(),
         dimension_numbers=dimension_numbers,
-        feature_group_count=feature_group_count.tolist(),  # Should be int.
+        feature_group_count=feature_group_count.item(),
         batch_group_count=batch_group_count or 1,
         precision=precision_config,
         preferred_element_type=dst_dtype)
 
   return _func
 
 
@@ -2188,14 +2410,28 @@
 
   def _func(operand: jnp.ndarray) -> jnp.ndarray:
     return jax.lax.reduce_precision(operand, exponent, mantissa)
 
   return _func
 
 
+@register_operation("XlaSharding")
+def _xla_sharding(proto):
+  """Parse a XlaSharding op."""
+  _check_attrs(proto, {"T", "sharding", "unspecified_dims"})
+
+  sharding = proto.attr["sharding"].s
+  if sharding:
+    raise ValueError(
+        f"Sharding is not yet supported (except identity), found {proto}."
+    )
+
+  return lambda x: x
+
+
 def _maybe_get_jaxpreqn(
     jaxpr: jax.core.ClosedJaxpr) -> Optional[jax.core.JaxprEqn]:
   def is_all_vars(vs):
     return all([isinstance(v, jax.core.Var) for v in vs])
 
   if (len(jaxpr.eqns) == 1 and
       is_all_vars(jaxpr.jaxpr.invars) and is_all_vars(jaxpr.jaxpr.outvars) and
@@ -2261,15 +2497,15 @@
       else:
         break
 
     return num_keys
 
   def __call__(self, *args: jnp.ndarray, comparator: Callable[..., Any]):
     operands = args[:-1]
-    dimension = args[-1].tolist()
+    dimension = args[-1].item()
 
     with jax.ensure_compile_time_eval():
       dtypes = [x.dtype for x in operands]
       num_keys = self._compute_num_keys(dtypes, comparator)
 
     return jax.lax.sort(
         operands,
@@ -2430,15 +2666,15 @@
       shape: jnp.ndarray,
   ) -> Tuple[jnp.ndarray, jnp.ndarray]:
     return jax.lax.rng_bit_generator(
         key=key.reshape(-1),
         shape=shape,
         dtype=jax_dtype,
         # See tensorflow/compiler/tf2xla/ops/xla_ops.cc#L812
-        algorithm=xla_utils.get_random_algorithm_from_tf(algorithm.tolist()),
+        algorithm=xla_utils.get_random_algorithm_from_tf(algorithm.item()),
     )
 
   return _func
 
 
 @dataclasses.dataclass
 class _XlaScatter(_HigherOrderFunction):
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/ops_test.py` & `tf2jax-0.3.4/tf2jax/_src/ops_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,25 +67,26 @@
     jax_func = self.variant(jax_func)
 
     rng = jax.random.PRNGKey(42)
     jax_results, new_jax_params = jax_func(jax_params, *inputs, rng=rng)
     tf_results = tf_func(*inputs)
 
     # Check outputs
-    for tf_res, jax_res in zip(
-        tree.flatten(tf_results), tree.flatten(jax_results)):
+    for tf_res, jax_res in jax.util.safe_zip(
+        tree.flatten(tf_results), tree.flatten(jax_results)
+    ):
       self.assertEqual(tf_res.shape, jax_res.shape)
       if not check_shape_only:
         self.assertAllClose(np.asarray(tf_res), jax_res, atol=atol)
 
     return jax_results, new_jax_params
 
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.parameters("log_softmax", "sigmoid", "softmax", "softplus",
-                            "tanh", "relu", "relu6", "elu")
+                            "tanh", "relu", "relu6", "elu", "leaky_relu")
   def test_activations(self, op_name):
     np.random.seed(42)
     inputs = [np.random.normal(size=(10, 5)).astype(np.float32)]
 
     if jax.default_backend().lower() == "tpu" and op_name in ("softplus",):
       tols = dict(atol=1e-4)
     else:
@@ -99,19 +100,45 @@
     def assert_fn(cond, data):
       tf.Assert(condition=cond, data=data)
       return data
 
     self._test_convert(assert_fn, [np.array(5) > 0, [np.array(6)]])
 
   @chex.variants(with_jit=True, without_jit=True)
-  @parameterized.parameters("Abs", "Acosh", "Asinh", "Atanh", "Ceil", "Cos",
-                            "Cosh", "Digamma", "Erf", "Erfc", "Erfinv", "Exp",
-                            "Expm1", "Floor", "Lgamma", "Log", "Log1p", "Neg",
-                            "Reciprocal", "Round", "Rsqrt", "Sign", "Sin",
-                            "Sinh", "Sqrt", "Square", "Tan")
+  @parameterized.parameters(
+      "Abs",
+      "Acosh",
+      "Asinh",
+      "Atanh",
+      "BesselI0e",
+      "BesselI1e",
+      "Ceil",
+      "Cos",
+      "Cosh",
+      "Digamma",
+      "Erf",
+      "Erfc",
+      "Erfinv",
+      "Exp",
+      "Expm1",
+      "Floor",
+      "Lgamma",
+      "Log",
+      "Log1p",
+      "Neg",
+      "Reciprocal",
+      "Round",
+      "Rsqrt",
+      "Sign",
+      "Sin",
+      "Sinh",
+      "Sqrt",
+      "Square",
+      "Tan",
+  )
   def test_unary_numerics(self, op_name):
     np.random.seed(42)
     if op_name == "Erfinv":
       inputs = np.random.uniform(size=(10, 5)).astype(np.float32)
     else:
       inputs = np.random.normal(size=(10, 5)).astype(np.float32)
 
@@ -305,14 +332,128 @@
           strides=strides,
           padding=padding,
           data_format=data_format)
     self._test_convert(pool, [inputs])
 
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.named_parameters(
+      (
+          "case0",
+          [
+              [[[1]]],
+              [[[2]]],
+              [[[3]]],
+              [[[4]]],
+          ],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case1",
+          [
+              [[[1, 2, 3]]],
+              [[[4, 5, 6]]],
+              [[[7, 8, 9]]],
+              [[[10, 11, 12]]],
+          ],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case2",
+          [
+              [[[1], [3]], [[9], [11]]],
+              [[[2], [4]], [[10], [12]]],
+              [[[5], [7]], [[13], [15]]],
+              [[[6], [8]], [[14], [16]]],
+          ],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case3",
+          [
+              [[[0], [1], [3]]],
+              [[[0], [9], [11]]],
+              [[[0], [2], [4]]],
+              [[[0], [10], [12]]],
+              [[[0], [5], [7]]],
+              [[[0], [13], [15]]],
+              [[[0], [6], [8]]],
+              [[[0], [14], [16]]],
+          ],
+          (2, 2),
+          [[0, 0], [2, 0]],
+      ),
+  )
+  def test_batch_to_space_nd(self, inputs, block_shape, crops):
+    inputs = np.array(inputs)
+    block_shape = np.array(block_shape)
+    crops = np.array(crops)
+
+    def batch_to_space(x):
+      return tf.raw_ops.BatchToSpaceND(
+          input=x, block_shape=block_shape, crops=crops
+      )
+
+    self._test_convert(batch_to_space, [inputs])
+
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
+      (
+          "case0",
+          [
+              [[[1], [2]], [[3], [4]]],
+          ],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case1",
+          [
+              [[[1, 2, 3], [4, 5, 6]], [[7, 8, 9], [10, 11, 12]]],
+          ],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case2",
+          [[
+              [[1], [2], [3], [4]],
+              [[5], [6], [7], [8]],
+              [[9], [10], [11], [12]],
+              [[13], [14], [15], [16]],
+          ]],
+          (2, 2),
+          [[0, 0], [0, 0]],
+      ),
+      (
+          "case3",
+          [
+              [[[1], [2], [3], [4]], [[5], [6], [7], [8]]],
+              [[[9], [10], [11], [12]], [[13], [14], [15], [16]]],
+          ],
+          (2, 2),
+          [[0, 0], [2, 0]],
+      ),
+  )
+  def test_space_to_batch_nd(self, inputs, block_shape, paddings):
+    inputs = np.array(inputs)
+    block_shape = np.array(block_shape)
+    paddings = np.array(paddings)
+
+    def space_to_batch(x):
+      return tf.raw_ops.SpaceToBatchND(
+          input=x, block_shape=block_shape, paddings=paddings
+      )
+
+    self._test_convert(space_to_batch, [inputs])
+
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
       chex.params_product(
           (("NHWC", "NHWC"), ("NCHW", "NCHW")),
           (
               ("three_dims", (32, 16, 8)),
               ("four_dims", (3, 32, 16, 8)),
               ("five_dims", (2, 3, 32, 16, 8)),
           ),
@@ -681,14 +822,45 @@
         outputs = jax_fn(actual_inputs)
         self.assertAllClose(outputs, actual_inputs)
       else:
         with self.assertRaisesRegex(ValueError, "Expected shape="):
           jax_fn(actual_inputs)
 
   @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
+      ("FFT", tf.raw_ops.FFT, (10,)),
+      ("FFT2D", tf.raw_ops.FFT2D, (10, 8)),
+      ("FFT3D", tf.raw_ops.FFT3D, (10, 8, 6)),
+      ("IFFT", tf.raw_ops.IFFT, (10,)),
+      ("IFFT2D", tf.raw_ops.IFFT2D, (10, 8)),
+      ("IFFT3D", tf.raw_ops.IFFT3D, (10, 8, 6)),
+  )
+  def test_fft_ifft(self, fft_op, shape):
+    np.random.seed(42)
+    inputs = np.random.normal(size=(5,) + shape).astype(np.complex64)
+    tols = dict(atol=1e-4) if jax.default_backend().lower() == "cpu" else {}
+    self._test_convert(lambda x: fft_op(input=x), inputs, **tols)
+
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
+      ("RFFT", tf.raw_ops.RFFT, (10,), np.float32),
+      ("RFFT2D", tf.raw_ops.RFFT2D, (10, 8), np.float32),
+      ("RFFT3D", tf.raw_ops.RFFT3D, (10, 8, 6), np.float32),
+      ("IRFFT", tf.raw_ops.IRFFT, (10,), np.complex64),
+      ("IRFFT2D", tf.raw_ops.IRFFT2D, (10, 8), np.complex64),
+      ("IRFFT3D", tf.raw_ops.IRFFT3D, (10, 8, 6), np.complex64),
+  )
+  def test_rfft_irfft(self, fft_op, shape, dtype):
+    np.random.seed(42)
+    inputs = np.random.normal(size=(5,) + shape).astype(dtype)
+    self._test_convert(
+        lambda x: fft_op(input=x, fft_length=[6] * len(shape)), inputs
+    )
+
+  @chex.variants(with_jit=True, without_jit=True)
   def test_fill(self):
     dims, value = (np.int32(2),), np.int32(3)
 
     def fill(x):
       return tf.raw_ops.Fill(dims=dims, value=x)
     self._test_convert(fill, value)
 
@@ -981,14 +1153,39 @@
     self._test_convert(raw_func, inputs)
 
     def tf_func(x):
       return tf.linalg.diag(x, k=-2, padding_value=padding)
     self._test_convert(tf_func, inputs)
 
   @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.parameters(np.float32, np.int32, np.bool_)
+  def test_matrix_set_diag(self, dtype):
+    np.random.seed(42)
+
+    diagonal = np.array([[1, 2, 3], [4, 5, 6]]).astype(dtype)
+
+    if dtype == np.float32:
+      inputs = np.random.normal(size=[2, 3, 4]).astype(dtype)
+    elif dtype == np.int32:
+      inputs = np.random.randint(low=0, high=10, size=[2, 3, 4], dtype=dtype)
+    elif dtype == np.bool_:
+      inputs = np.random.normal(size=[2, 3, 4]) > 0.0
+      diagonal = diagonal > 3
+    else:
+      raise ValueError(f"Unsupported dtype={dtype}")
+
+    def raw_func(x, y):
+      return tf.raw_ops.MatrixSetDiagV3(input=x, diagonal=y, k=1)
+    self._test_convert(raw_func, [inputs, diagonal])
+
+    def tf_func(x, y):
+      return tf.linalg.set_diag(x, y, k=1)
+    self._test_convert(tf_func, [inputs, diagonal])
+
+  @chex.variants(with_jit=True, without_jit=True)
   def test_max(self):
     inputs = np.array(np.reshape(range(24), (4, 3, 2)), dtype=np.int32)
 
     def max_fn(xs):
       return tf.raw_ops.Max(input=xs, axis=[0, 2, 1])
     self._test_convert(max_fn, inputs)
 
@@ -1087,14 +1284,32 @@
 
     # Check static inputs result in static outputs.
     def pack_static():
       return tf.zeros(pack([10, 10]))
     self._test_convert(pack_static, [])
 
   @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.parameters(
+      np.int8,
+      np.int16,
+      np.int32,
+      np.int64,
+      np.uint8,
+      np.uint16,
+      np.uint32,
+      np.uint64,
+  )
+  def test_population_count(self, dtype):
+    def population_count(x):
+      return tf.raw_ops.PopulationCount(x=x)
+
+    inputs = np.arange(1000, dtype=dtype)
+    self._test_convert(population_count, inputs)
+
+  @chex.variants(with_jit=True, without_jit=True)
   def test_pow(self):
     def power(x, y):
       return tf.raw_ops.Pow(x=x, y=y)
     self._test_convert(power, [2, 3])
 
     # Check static inputs result in static outputs.
     def power_static():
@@ -1422,17 +1637,20 @@
   def test_scatter_nd(self):
     idxs = np.array([[2, 3], [5, 1]], dtype=np.int32)
     vals = np.array([[1, 2], [3, 4]], dtype=np.int32)
     shape = np.array([10, 5, 2], dtype=np.int32)
 
     def scatter_nd(idx, val):
       return tf.raw_ops.ScatterNd(indices=idx, updates=val, shape=shape)
-
     self._test_convert(scatter_nd, [idxs, vals])
 
+    def scatter_nd_static():
+      return tf.zeros((tf.reduce_sum(scatter_nd(idxs, vals),)))
+    self._test_convert(scatter_nd_static, ())
+
   @chex.variants(with_jit=True, without_jit=True)
   def test_select(self):
     inputs = [
         np.array([True, False]),
         np.array([[1, 2], [3, 4]]),
         np.array([[5, 6], [7, 8]]),
     ]
@@ -2037,10 +2255,20 @@
   def test_irfft(self):
     inputs = np.array([-2.25 + 4.75j, 3.25 + 5.75j] * 2, dtype=np.csingle)
 
     def irfft(x):
       return tf.raw_ops.IRFFT(input=x, fft_length=[len(x)])
     self._test_convert(irfft, inputs)
 
+  @chex.variants(with_jit=True, without_jit=True)
+  def test_var_handle(self):
+    def var_handle():
+      return tf.raw_ops.VarHandleOp(dtype=tf.float32, shape=(3, 5), name="blah")
+
+    with self.assertRaisesRegex(
+        ValueError, "VarHandleOp `blah` cannot be evaluated"
+    ):
+      self._test_convert(var_handle, [])
+
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/roundtrip_test.py` & `tf2jax-0.3.4/tf2jax/_src/roundtrip_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,76 +10,105 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for JAX -> TF -> JAX."""
 
+import os
+
+from absl import flags
 from absl.testing import absltest
 from absl.testing import parameterized
 
 import chex
 import haiku as hk
 import jax
 from jax.experimental import jax2tf
 import jax.numpy as jnp
 
 import numpy as np
 import tensorflow as tf
 from tf2jax._src import config
 from tf2jax._src import test_util
 from tf2jax._src import tf2jax
-from tf2jax._src.experimental import ops as experimental_ops  # pylint: disable=unused-import
 import tree
 
 from tensorflow.compiler.xla import xla_data_pb2  # pytype: disable=import-error
 
 # Parse absl flags test_srcdir and test_tmpdir.
 jax.config.parse_flags_with_absl()
 
 
+def _bool_env(varname: str, value: bool) -> bool:
+  val = os.getenv(varname, str(value))
+  return {"1": True, "0": False, "True": True, "False": False}[val]
+
+
+_NATIVE_SERIALIZATION = flags.DEFINE_bool(
+    "use_jax2tf_native_serialization_in_roundtrip_test",
+    _bool_env("USE_JAX2TF_NATIVE_SERIALIZATION_IN_ROUNDTRIP_TEST", False),
+    "Whether to call jax2tf.convert with native serialization enabled.",
+)
+
+
+def _parse_version(version: str):
+  return tuple(int(x.split("-")[0]) for x in version.split("."))
+
+
 def _compute_gradients(func, *inputs):
   def fn(*args):
-    return jax.tree_leaves(func(*args))[0]
+    return jax.tree_util.tree_leaves(func(*args))[0]
   return jax.grad(lambda *args: jnp.sum(fn(*args)))(*inputs)
 
 
+def _jax2tf_convert(func, **kwargs):
+  return jax2tf.convert(
+      func, native_serialization=_NATIVE_SERIALIZATION.value, **kwargs
+  )
+
+
+def uses_native_serialization():
+  return _NATIVE_SERIALIZATION.value
+
+
 class Jax2TfTest(test_util.TestCase):
 
   def _test_convert(
       self,
       jax_func,
       inputs,
       *,
       with_grad,
       enable_xla,
       with_custom_grad=False,
       grad_tols=None,
   ):
-    if jax.config.jax2tf_default_experimental_native_lowering:
+    if uses_native_serialization():
       if not enable_xla:
-        self.skipTest("native_lowering does not support enable_xla=False.")
+        self.skipTest("native_serialization does not support enable_xla=False.")
       if with_grad and not with_custom_grad:
         self.skipTest(
-            "native_lowering does not support differentiation without custom "
-            "gradient.")
+            "native_serialization does not support differentiation without "
+            "custom gradient.")
 
     grad_tols = grad_tols or {}
     def assert_grad_all_close(*args):
       return self.assertAllClose(*args, **grad_tols)
 
     # Jax
     jax_func = self.variant(jax_func)
     jax_outputs = jax_func(*inputs)
     if with_grad:
       jax_grads = _compute_gradients(jax_func, *inputs)
 
     # Jax -> TF
-    tf_func = jax2tf.convert(jax_func, with_gradient=with_grad,
-                             enable_xla=enable_xla)
+    tf_func = _jax2tf_convert(
+        jax_func, with_gradient=with_grad, enable_xla=enable_xla
+    )
     tf_func = tf.function(tf_func, jit_compile=True, autograph=False)
     tf_outputs = tf_func(*inputs)
     jax.tree_map(self.assertAllClose, jax_outputs, tf_outputs)
 
     # Jax -> TF -> Jax
     with config.override_config("convert_custom_gradient", with_custom_grad):
       rejax_func = tf2jax.convert_functional(
@@ -479,18 +508,18 @@
       return reducer(x, axis=axis, reverse=reverse)
 
     inputs = np.random.normal(size=(4, 3))
 
     with config.override_config("infer_cumulative_reduction_from_jax2tf",
                                 use_heuristic):
       roundtrip_forward = tf2jax.convert_functional(
-          tf.function(jax2tf.convert(forward), autograph=False), inputs)
+          tf.function(_jax2tf_convert(forward), autograph=False), inputs)
       roundtrip_jaxpr = jax.make_jaxpr(roundtrip_forward)(inputs)
       if (use_heuristic and
-          not jax.config.jax2tf_default_experimental_native_lowering):
+          not uses_native_serialization()):
         self.assertNotIn("reduce_window", roundtrip_jaxpr.pretty_print())
 
       if (with_grad and enable_xla and reducer is jax.lax.cumprod and
           not use_heuristic):
         self.skipTest("No differentiation rule for `reduce_window` with "
                       "`jax.lax.cumprod`.")
 
@@ -625,20 +654,17 @@
       chex.params_product(
           (("without_gradient", False), ("with_gradient", True)),
           (("disable_xla", False), ("enable_xla", True)),
           named=True,
       )
   )
   def test_polymorphic_shape(self, with_grad, enable_xla):
-    if jax.config.jax2tf_default_experimental_native_lowering:
+    if uses_native_serialization():
       if not enable_xla:
-        self.skipTest("native_lowering does not support enable_xla=False.")
-      if enable_xla:
-        # TODO(b/267480040): Clean this up accordingly.
-        self.skipTest("re-enable after shape refinement is finished.")
+        self.skipTest("native_serialization does not support enable_xla=False.")
 
     inputs = np.array(range(36), dtype=np.float32).reshape(9, 4)
 
     # TF
     @tf.function(autograph=False)
     def forward(x):
       shape = tf.shape(x)
@@ -653,15 +679,15 @@
     # TF -> JAX
     jax_func = tf2jax.convert_functional(forward, tf.TensorSpec((None, 4)))
     jax_func = self.variant(jax_func)
     jax_outputs = jax_func(inputs)
     self.assertAllClose(tf_outputs, jax_outputs)
 
     # TF -> JAX -> TF
-    new_tf_forward = jax2tf.convert(
+    new_tf_forward = _jax2tf_convert(
         jax_func,
         polymorphic_shapes=["(b, _)"],
         with_gradient=with_grad,
         enable_xla=enable_xla)
     new_tf_forward = tf.function(new_tf_forward, autograph=False)
     concrete_new_tf_forward = new_tf_forward.get_concrete_function(
         tf.TensorSpec(shape=(None, 4)))
@@ -674,17 +700,17 @@
   @parameterized.named_parameters(
       chex.params_product(
           (("with_gradient", True),),
           (("disable_xla", False), ("enable_xla", True)),
           named=True,
       ))
   def test_custom_gradient(self, with_grad, enable_xla):
-    if jax.config.jax2tf_default_experimental_native_lowering:
+    if uses_native_serialization():
       if not enable_xla:
-        self.skipTest("native_lowering does not support enable_xla=False.")
+        self.skipTest("native_serialization does not support enable_xla=False.")
 
     inputs = np.array(range(6), dtype=np.float32).reshape(3, 2)
 
     # JAX
     @jax.custom_gradient
     def forward(x):
       e = jnp.exp(x)
@@ -693,15 +719,15 @@
         return dy * (1 - 1 / (1 + e)) * jnp.sin(x) + 0.42
       return jnp.sum(jnp.log(1 + e)), grad
     forward = self.variant(forward)
     expected_outputs = forward(inputs)
     expected_grads = jax.grad(forward)(inputs)
 
     # JAX -> TF
-    tf_forward = jax2tf.convert(
+    tf_forward = _jax2tf_convert(
         forward, with_gradient=with_grad, enable_xla=enable_xla)
     tf_forward = tf.function(tf_forward, autograph=False)
 
     # JAX -> TF -> JAX
     with config.override_config("convert_custom_gradient", True):
       jax_forward = tf2jax.convert_functional(tf_forward,
                                               tf.zeros_like(inputs))
@@ -733,17 +759,17 @@
   @parameterized.named_parameters(
       chex.params_product(
           (("with_gradient", True),),
           (("disable_xla", False), ("enable_xla", True)),
           named=True,
       ))
   def test_custom_gradient_nested(self, with_grad, enable_xla):
-    if jax.config.jax2tf_default_experimental_native_lowering:
+    if uses_native_serialization():
       if not enable_xla:
-        self.skipTest("native_lowering does not support enable_xla=False.")
+        self.skipTest("native_serialization does not support enable_xla=False.")
 
     inputs = np.array(range(6), dtype=np.float32).reshape(3, 2)
 
     # JAX
     @jax.custom_gradient
     def forward(x):
       e = jnp.exp(x)
@@ -753,22 +779,22 @@
       return jnp.sum(jnp.log(1 + e)), grad
 
     forward = self.variant(forward)
     expected_outputs = forward(inputs)
     expected_grads = jax.grad(forward)(inputs)
 
     # JAX -> TF
-    tf_fn = jax2tf.convert(
+    tf_fn = _jax2tf_convert(
         forward, with_gradient=with_grad, enable_xla=enable_xla)
     tf_fn = tf.function(tf_fn, autograph=False)
 
     # JAX -> TF -> CALL_TF -> TF.
     # This creates dependencies between custom gradients.
     call_tf_fn = jax2tf.call_tf(tf_fn)
-    tf_fn_too = jax2tf.convert(call_tf_fn, with_gradient=with_grad)
+    tf_fn_too = _jax2tf_convert(call_tf_fn, with_gradient=with_grad)
     tf_fn_too = tf.function(tf_fn_too, autograph=False)
 
     # JAX -> TF -> CALL_TF -> TF -> JAX
     with config.override_config("convert_custom_gradient", True):
       jax_fn_too = tf2jax.convert_functional(tf_fn_too, np.zeros_like(inputs))
 
     jax_outputs = jax_fn_too(inputs)
@@ -795,17 +821,17 @@
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.named_parameters(
       chex.params_product(
           (("disable_xla", False), ("enable_xla", True)),
           named=True,
       ))
   def test_empty_return(self, enable_xla):
-    if jax.config.jax2tf_default_experimental_native_lowering:
+    if uses_native_serialization():
       if not enable_xla:
-        self.skipTest("native_lowering does not support enable_xla=False.")
+        self.skipTest("native_serialization does not support enable_xla=False.")
 
     np.random.seed(42)
 
     def forward(x):
       unused_y = jnp.cos(x)
       return ()
 
@@ -814,15 +840,15 @@
     inputs = np.random.normal((3, 2))
     with self.assertRaisesRegex(
         TypeError,
         "Gradient only defined for scalar-output functions. Output was ()."):
       jax.grad(forward)(inputs)
 
     # JAX -> TF
-    tf_forward = jax2tf.convert(
+    tf_forward = _jax2tf_convert(
         forward, with_gradient=True, enable_xla=enable_xla)
     tf_forward = tf.function(tf_forward, autograph=False)
 
     # JAX -> TF -> JAX
     with config.override_config("convert_custom_gradient", True):
       jax_forward = tf2jax.convert_functional(tf_forward,
                                               tf.zeros_like(inputs))
@@ -858,15 +884,15 @@
     def tf_fn(x):
       return tf.cos(x)
 
     def tf2jax_fn(x):
       jax_fn = tf2jax.convert_functional(tf_fn, x)
       return jnp.sin(self.variant(jax_fn)(x))
 
-    tf2jax2tf_fn = jax2tf.convert(tf2jax_fn)
+    tf2jax2tf_fn = _jax2tf_convert(tf2jax_fn)
     tf2jax2tf_fn = tf.function(tf2jax2tf_fn, autograph=False)
 
     inputs = np.linspace(-1., 1., 6, dtype=np.float32).reshape((2, 3))
     self.assertAllClose(tf.sin(tf_fn(inputs)), tf2jax2tf_fn(inputs))
 
   @chex.variants(with_jit=True, without_jit=True)
   @parameterized.named_parameters(
@@ -885,20 +911,20 @@
     self._test_convert(
         remat_fn,
         inputs,
         with_grad=with_gradient,
         enable_xla=True,
         with_custom_grad=True)
 
-    if jax.config.jax2tf_default_experimental_native_lowering:
-      self.skipTest("Skip remat jaxpr test with native_lowering.")
+    if uses_native_serialization():
+      self.skipTest("Skip remat jaxpr test with native_serialization.")
 
     # Check jaxpr.
     tf_fn = tf.function(
-        jax2tf.convert(remat_fn, with_gradient=True, enable_xla=True),
+        _jax2tf_convert(remat_fn, with_gradient=True, enable_xla=True),
         autograph=False)
     jax_fn = tf2jax.convert_functional(tf_fn, tf.TensorSpec((10, 5),
                                                             tf.float32))
     jax_fn = self.variant(jax_fn)
     out_jaxpr = jax.make_jaxpr(jax_fn)(*inputs)
     self.assertNotRegex(str(out_jaxpr), "remat")
     grad_jaxpr = jax.make_jaxpr(jax.grad(lambda x: jnp.sum(jax_fn(x))))(*inputs)
@@ -926,10 +952,109 @@
     inputs = np.random.normal((3, 2)).astype(np.float32)
     self._test_convert(
         forward, [inputs],
         with_grad=with_grad,
         enable_xla=enable_xla,
         with_custom_grad=with_custom_grad)
 
+  @chex.variants(with_jit=True, without_jit=True)
+  @parameterized.named_parameters(
+      chex.params_product(
+          (("without_gradient", True),),
+          (("enable_xla", True), ("disable_xla", False)),
+          (("with_custom_gradient", True),),
+          (
+              ("lower", True),
+              ("upper", False),
+          ),
+          (
+              ("unit_diagonal", True),
+              ("not_unit_diagonal", False),
+          ),
+          (
+              ("unbatched", ((5, 5), (5, 5))),
+              ("batched", ((3, 5, 5), (3, 5, 4))),
+              ("more_batched", ((2, 3, 5, 5), (2, 3, 5, 6))),
+          ),
+          named=True,
+      ))
+  def test_triangular_solve(
+      self,
+      with_grad,
+      enable_xla,
+      with_custom_grad,
+      lower,
+      unit_diagonal,
+      shapes,
+  ):
+    if uses_native_serialization():
+      self.skipTest(
+          "native_serialization: Cannot serialize code with custom calls whose "
+          "targets have no compatibility guarantees.")
+
+    np.random.seed(42)
+
+    lhs_shape, rhs_shape = shapes
+    inputs = (
+        np.random.normal(size=lhs_shape).astype(np.float32),
+        np.random.normal(size=rhs_shape).astype(np.float32),
+    )
+
+    def forward(a, b):
+      return jax.lax.linalg.triangular_solve(
+          a, b, left_side=True, lower=lower, unit_diagonal=unit_diagonal
+      )
+
+    tols = dict(atol=1e-5) if jax.default_backend().lower() == "tpu" else {}
+
+    self._test_convert(
+        forward, inputs,
+        with_grad=with_grad,
+        enable_xla=enable_xla,
+        with_custom_grad=with_custom_grad,
+        grad_tols=tols)
+
+  def test_explicit_native_serialization(self):
+    if _parse_version(tf.version.VERSION) < _parse_version("2.12.0"):
+      self.skipTest(f"Requires tf 2.12.0 or later, found {tf.version.VERSION}.")
+
+    def forward(x):
+      return x + 3.14
+
+    tf_fn = jax2tf.convert(forward, native_serialization=True)
+    tf_fn = tf.function(tf_fn, autograph=False)
+
+    try:
+      jax_fn = tf2jax.convert_functional(
+          tf_fn, tf.TensorSpec((2, 3), tf.float32)
+      )
+      jax_fn = jax.jit(jax_fn)
+      inputs = np.linspace(-1., 1., 6, dtype=np.float32).reshape((2, 3))
+      self.assertAllClose(jax_fn(inputs), tf_fn(inputs))
+    except ValueError as e:
+      if uses_native_serialization():
+        raise ValueError("Native lowering support failed.") from e
+      elif r"Unsupported operations in graph: ['XlaCallModule']" not in str(e):
+        raise ValueError("Unexpected unsupported operations found.") from e
+      elif r"check for import error if you see this message" not in str(e):
+        raise ValueError("Import/dependency error message not found.") from e
+      else:  # Expected failure.
+        return
+
+    if not uses_native_serialization():
+      raise ValueError(
+          "Unexpected success with native serialization. Test may be "
+          "misconfigured."
+      )
+
+    if jax.default_backend().lower() != "cpu":
+      with jax.default_device(jax.devices("cpu")[0]):
+        with self.assertRaisesRegex(ValueError, "Unsupported backend"):
+          _ = jax_fn(inputs)
+        with tf2jax.config.override_config(
+            "xlacallmodule_strict_checks", False
+        ):
+          self.assertAllClose(jax_fn(inputs), tf_fn(inputs))
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/test_util.py` & `tf2jax-0.3.4/tf2jax/_src/test_util.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/_src/tf2jax.py` & `tf2jax-0.3.4/tf2jax/_src/tf2jax.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,26 @@
 import tree
 
 # Import usage logging here.
 
 from tensorflow.python.framework import op_def_registry  # pylint: disable=no-name-in-module
 from tensorflow.python.framework import ops as tf_ops  # pylint: disable=no-name-in-module
 
+try:
+  import tf2jax.experimental.ops  # pylint: disable=g-import-not-at-top,unused-import
+except ImportError:
+  logging.info(
+      "Proceeding without support for experimental ops, e.g. XlaCallModule.")
 
+
+ArrayLike = ops.ArrayLike
 SpecTree = Union[tf.TensorSpec, Iterable["SpecTree"], Mapping[str, "SpecTree"]]
 
+safe_zip = jax.util.safe_zip
+
 
 class AnnotatedFunction:
   """Callable function with additional metadata.
 
   The metadata includes: structured inputs and outputs (composed of
   tf.TensorSpec) and the original function signature.
   """
@@ -73,14 +82,15 @@
 
 
 _EMPTY_RETURN_OP_NAME = ops._EMPTY_RETURN_OP_NAME  # pylint: disable=protected-access
 _EMPTY_RETURN_VALUE = ops._EMPTY_RETURN_VALUE  # pylint: disable=protected-access
 
 
 _UNUSED_INPUT = object()
+_XLA_CALL_MODULE = "XlaCallModule"
 
 
 def _fix_jax_poly_shape(shape: Tuple[Any, ...]) -> Tuple[Any, ...]:
   good_shape = []
   for dim in shape:
     try:
       # This catches _DimPolynomial from jax2tf.
@@ -153,21 +163,23 @@
 
 
 class _LibraryFunction(NamedTuple):
   """A library function."""
   fn: Callable[..., Any]
   require_rng: bool
   # Optional fields (mainly) used by gradient functions.
-  params: Optional[Mapping[str, jnp.ndarray]] = None
+  params: Optional[Mapping[str, ArrayLike]] = None
   input_specs: Optional[Tuple[tf.TensorSpec, ...]] = None
   output_specs: Optional[Tuple[tf.TensorSpec, ...]] = None
   # If fn is a gradient function, this is the output specs for the original fn.
   orig_fn_output_specs: Optional[Tuple[tf.TensorSpec, ...]] = None
   # Whether an output is unmodified input to the function.
   output_is_input: Optional[Tuple[bool]] = None
+  # Inputs corresponding to VarHandleOp
+  variable_input_specs: Optional[Tuple[tf.TensorSpec, ...]] = None
 
   def __call__(self, *args, **kwargs):
     if self.params:
       return self.fn(self.params, *args, **kwargs)
     else:
       # Ignore parameters in inputs and outputs.
       return self.fn({}, *args, **kwargs)[0]
@@ -177,39 +189,42 @@
     named_args: Sequence[Tuple[str, jnp.ndarray]],
     inputs: Tuple[_TensorEdge, ...],
 ) -> Tuple[jnp.ndarray, ...]:
   """Extract inputs from named arguments."""
   if len(named_args) != len(inputs):
     raise ValueError(
         f"Expected {len(inputs)} arguments, received {len(named_args)}")
-  for (arg_name, _), inp in zip(named_args, inputs):
+  for (arg_name, _), inp in safe_zip(named_args, inputs):
     if arg_name != inp.op_name:
       raise ValueError(f"Expected inputs {inp.op_name}, found {arg_name}")
 
   unboxed_args = [
       arg[inp.idx] if isinstance(arg, (list, tuple)) else arg
-      for arg, inp in zip([x for _, x in named_args], inputs)
+      for arg, inp in safe_zip([x for _, x in named_args], inputs)
   ]
   return tuple(unboxed_args)
 
 
 class _OpNode:
   """Represents an Op."""
 
   def __init__(self, proto, library: Mapping[str, _LibraryFunction],
                node_map: Mapping[str, Any]):
     self.jax_func = ops.get_parser(proto.op)(proto)
     self.op = proto.op
     self.name = proto.name
 
+    inputs = [_TensorEdge.from_string(inp, node_map) for inp in proto.input]
+
     self.inner_fns = dict()
     if isinstance(self.jax_func, ops._HigherOrderFunction):
       self.inner_fns = self.jax_func.get_inner_functions(library)
+      for input_name in self.jax_func.get_additional_inputs(**self.inner_fns):
+        inputs.append(_TensorEdge.from_string(input_name, node_map))
 
-    inputs = [_TensorEdge.from_string(inp, node_map) for inp in proto.input]
     self.control_inputs = tuple([inp for inp in inputs if inp.is_control])
     self.inputs = tuple([inp for inp in inputs if not inp.is_control])
 
   @property
   def all_inputs(self) -> Tuple[_TensorEdge, ...]:
     return self.inputs + self.control_inputs
 
@@ -443,16 +458,19 @@
     raise
 
   graph = concrete_func.graph
   graphdef = graph.as_graph_def()
 
   num_flat_args = len(concrete_func.inputs) - len(concrete_func.captured_inputs)
   captures = list(
-      zip([inp.op.name for inp in concrete_func.inputs[num_flat_args:]],
-          [inp for inp in concrete_func.captured_inputs]))
+      safe_zip(
+          [inp.op.name for inp in concrete_func.inputs[num_flat_args:]],
+          [inp for inp in concrete_func.captured_inputs],
+      )
+  )
   func_variables = {v.handle.ref(): v for v in concrete_func.variables}
   variable_map = {
       k: func_variables[v.ref()] for k, v in captures if v.dtype == tf.resource
   }
   constants = {k: v.numpy() for k, v in captures if v.dtype != tf.resource}
 
   captured_input_names = tuple([
@@ -601,15 +619,15 @@
     grad_inputs = tuple([_TensorEdge(v.name) for v in self.grad_fn.input_specs])
 
     @jax.custom_gradient
     def fn(*args):
       eval_cache = _EvaluationCache(
           self.subgraph, named_args, self.output_node.inputs + grad_inputs)
       assert len(args) == len(self.unique_inputs)
-      for inp, val in zip(self.unique_inputs, args):
+      for inp, val in safe_zip(self.unique_inputs, args):
         if isinstance(eval_cache.outputs[inp.op_name], list):
           eval_cache.outputs[inp.op_name][inp.idx] = val
         elif isinstance(eval_cache.outputs[inp.op_name], tuple):
           old_outputs = eval_cache.outputs[inp.op_name]
           eval_cache.outputs[inp.op_name] = (
               old_outputs[:inp.idx] + (val,) + old_outputs[inp.idx + 1:])
         else:
@@ -890,22 +908,36 @@
     if isinstance(spec, tf.TensorSpec):
       input_names.append(spec.name)
     else:
       input_names.append(f"__static_arg_{static_arg_num}")
       static_arg_num += 1
   input_names = tuple(input_names)
   assert len(input_names) == len(set(input_names))
-  output_names = tuple([v.name for v in tree.flatten(structured_outputs)])
+  flat_output_specs = tree.flatten(structured_outputs)
+  output_names = tuple(
+      v.name for v in flat_output_specs if isinstance(v, tf.TensorSpec)
+  )
 
   unsupported = ops.get_unsupported_operations(
       [node.op for node in graphdef.node])
   if unsupported:
-    raise ValueError(f"Unsupported operations in graph: {list(unsupported)}\n"
-                     "Support for additional TensorFlow ops are added on an "
-                     "as-needed basis, please contact the library owner(s).")
+    err_message = f"Unsupported operations in graph: {list(unsupported)}"
+    if _XLA_CALL_MODULE in unsupported:
+      err_message += "\n"
+      err_message += (
+          f"`{_XLA_CALL_MODULE}` is generated by jax2tf.convert with native "
+          "serialization, this is partially supported in tf2jax (check for "
+          "import error if you see this message)."
+      )
+    err_message += "\n"
+    err_message += (
+        "Support for additional TensorFlow ops are added on an as-needed "
+        "basis, please contact the library owner(s)."
+    )
+    raise ValueError(err_message)
 
   # Extract variables.
   if tf.executing_eagerly():
     # Uniqueify variables with identical names.
     variables_tf = {}
     var_name_by_ref = {}
     for v in variable_map.values():
@@ -987,17 +1019,17 @@
 
     if len(inputs) != len(input_names):
       raise ValueError(
           f"Expected {len(input_names)} args, found {len(inputs)}.")
 
     inputs = tree.map_structure(
         lambda x: x if isinstance(x, jnp.ndarray) else np.array(x), inputs)
-    all_params = {**params, **constants}
+    all_params = dict(**params, **constants)
 
-    for inp, (path, spec) in zip(inputs, input_path_to_specs):
+    for inp, (path, spec) in safe_zip(inputs, input_path_to_specs):
       if not isinstance(spec, tf.TensorSpec):
         # A `None` spec denotes a Tensor argument that was unused in deepfunc.
         is_tracer = isinstance(inp, jax.core.Tracer)
         if spec is not None and (is_tracer or spec != inp):
           inp_type = "tracer" if is_tracer else "literal value"
           raise ValueError(
               f"Found unexpected {inp_type} `{inp}`, expected `{spec}` for "
@@ -1023,17 +1055,27 @@
             f"Found incompatible input dtype: {inp.dtype}, expected "
             f"{spec.dtype} for argument at {path}.\n"
             "If this is not an issue for you, the error can be disabled "
             "either tf2jax.update_config('strict_dtype_check', False) or the "
             "context manager "
             "tf2jax.override_config('strict_dtype_check', False)")
 
+    missing_params = [
+        var_by_node.get(v, v)
+        for v in captured_input_names
+        if var_by_node.get(v, v) not in all_params
+    ]
+    if missing_params:
+      raise ValueError(f"Some parameters are missing, {missing_params}.")
+
     full_inputs = inputs + tuple(
         [all_params[var_by_node.get(v, v)] for v in captured_input_names])
-    full_inputs = list(zip(input_names + captured_input_names, full_inputs))
+    full_inputs = list(
+        safe_zip(input_names + captured_input_names, full_inputs)
+    )
 
     if num_rng_required:
       rng_keys = list(jax.random.split(rng, num_rng_required))
     else:
       rng_keys = []
 
     updated_param_names = set()
@@ -1054,16 +1096,27 @@
         # Assign variables.
         for var_name, var_val in updated_params.items():
           eval_cache.outputs[var_name] = var_val
           updated_param_names.add(var_name)
 
         eval_cache.free_inputs(node)
 
-    flat_outputs = tuple([eval_cache.outputs[k.op_name] for k in output_args])
-    flat_outputs = [v for v in flat_outputs if v is not _EMPTY_RETURN_VALUE]
+    tensor_outputs = tuple([eval_cache.outputs[k.op_name] for k in output_args])
+    tensor_outputs = [v for v in tensor_outputs if v is not _EMPTY_RETURN_VALUE]
+
+    # Merge the tensor and non-tensor outputs.
+    output_idx = 0
+    flat_outputs = []
+    for spec in flat_output_specs:
+      if isinstance(spec, tf.TensorSpec):
+        flat_outputs.append(tensor_outputs[output_idx])
+        output_idx += 1
+      else:
+        flat_outputs.append(spec)
+    assert output_idx == len(tensor_outputs)
     collected_outputs = tree.unflatten_as(structured_outputs, flat_outputs)
 
     # Parameters after any assignment.
     new_params = {
         var_name: eval_cache.outputs[node_by_var[var_name]]
         for var_name in params.keys()
     }
@@ -1100,29 +1153,47 @@
             arg.name,
             tuple([proto.ret[arg.name]] + ["^" + v for v in proto.control_ret]),
             {"T": tf.as_dtype(arg.type)},
         ))
   graphdef = _GraphDef(tuple(input_nodes + list(proto.node_def) + output_nodes))
   output_is_input = tuple(output_is_input)
 
+  # VarHandleOp correspond to variables in checkpoints.
+  var_handle_ops = [n for n in proto.node_def if n.op == "VarHandleOp"]
+
   params = [
       inspect.Parameter(arg.name, inspect.Parameter.POSITIONAL_ONLY)
       for arg in proto.signature.input_arg
+  ] + [
+      inspect.Parameter(
+          arg.name.replace("/", "___"), inspect.Parameter.POSITIONAL_ONLY
+      )
+      for arg in var_handle_ops
   ]
   signature = inspect.Signature(params)
 
   structured_inputs = tuple([
       tf.TensorSpec(None, dtype=tf.as_dtype(arg.type), name=arg.name)
       for arg in proto.signature.input_arg
   ])
   structured_outputs = tuple([
       tf.TensorSpec(None, dtype=tf.as_dtype(arg.type), name=arg.name)
       for arg in proto.signature.output_arg
   ])
 
+  def node_to_spec(v):
+    return tf.TensorSpec(
+        shape=[dim.size for dim in v.attr["shape"].shape.dim],
+        dtype=tf.as_dtype(v.attr["dtype"].type),
+        name=v.name,
+    )
+
+  var_inputs = tuple(node_to_spec(v) for v in var_handle_ops)
+  structured_inputs = structured_inputs + var_inputs
+
   jax_func, jax_params = _convert(
       graphdef,
       signature,
       [structured_inputs, {}],
       structured_outputs,
       library=library)
   if jax_params:
@@ -1132,16 +1203,23 @@
   # Does any of the ops or inner functions require RNG?
   require_rng = any([n.op in _TF_RANDOM_OPS for n in proto.node_def])
   for node in proto.node_def:
     for attr in node.attr.values():
       if attr.func.name:
         require_rng = require_rng or library[attr.func.name].require_rng
 
-  return _LibraryFunction(jax_func, require_rng, None, structured_inputs,
-                          structured_outputs, output_is_input=output_is_input)
+  return _LibraryFunction(
+      fn=jax_func,
+      require_rng=require_rng,
+      params=None,
+      input_specs=structured_inputs,
+      output_specs=structured_outputs,
+      output_is_input=output_is_input,
+      variable_input_specs=var_inputs,
+  )
 
 
 def _filter_nodes(
     predicate: Callable[[tf.compat.v1.NodeDef], bool],
     graph: Any,
 ) -> Iterator[Tuple[tf.compat.v1.NodeDef, Any]]:
   """Filter nodes in a tf.Graph with a predicate."""
@@ -1199,15 +1277,15 @@
 
   # Gradient function can capture tensors in the outer function. Move them
   # into the arguments of the gradient function for conversion to JAX.
   variable_map = {}
   constant_map = {}
   external_capture_specs = []
   internal_capture_names = []
-  for inp, cap in zip(grad_inputs[num_flat_args:], grad_captured_inputs):
+  for inp, cap in safe_zip(grad_inputs[num_flat_args:], grad_captured_inputs):
     if cap.dtype == tf.resource:
       variable_map[inp.op.name] = func_variables[cap.ref()]
       internal_capture_names.append(inp.op.name)
     elif hasattr(cap, "numpy"):
       constant_map[inp.op.name] = cap.numpy()
       internal_capture_names.append(inp.op.name)
     else:
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/tf2jax_test.py` & `tf2jax-0.3.4/tf2jax/_src/tf2jax_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,20 +64,21 @@
 class ModelsTest(tf.test.TestCase, parameterized.TestCase):
 
   def _test_convert(self, tf_func, inputs):
     jax_func, jax_params = tf2jax.convert(
         tf.function(tf_func), np.zeros_like(inputs))
     jax_func = self.variant(jax_func)
 
-    jax_results, jax_params = jax_func(jax_params, inputs)
+    (jax_results, _), jax_params = jax_func(jax_params, inputs)
     tf_results, tf_params = tf_func(inputs)
 
     # Check outputs
-    for tf_res, jax_res in zip(
-        tree.flatten(tf_results), tree.flatten(jax_results)):
+    for tf_res, jax_res in jax.util.safe_zip(
+        tree.flatten(tf_results), tree.flatten(jax_results)
+    ):
       self.assertAllClose(tf_res.numpy(), jax_res, atol=1e-4)
 
     # Check params (batchnorm stats changed).
     for tf_var in tree.flatten(tf_params):
       jax_var = jax_params[tf_var.name.split(":")[0]]
       self.assertAllClose(tf_var.numpy(), jax_var, atol=1e-5)
 
@@ -513,10 +514,43 @@
     tf_outputs = forward(x)
 
     apply_fn, params = tf2jax.convert(forward, tf.TensorSpec((None, 5)))
     jax_outputs, _ = self.variant(apply_fn)(params, x)
 
     self.assertAllClose(tf_outputs, jax_outputs)
 
+  @chex.variants(with_jit=True, without_jit=True)
+  def test_none_in_outputs(self):
+    @tf.function
+    def tf_func(x):
+      return x + 1, None, x + 3.14
+
+    jax_func = tf2jax.convert_functional(tf_func, np.zeros((3, 2)))
+    inputs = np.ones((3, 2))
+    outputs = self.variant(jax_func)(inputs)
+
+    self.assertAllClose(inputs + 1, outputs[0])
+    self.assertIsNone(outputs[1])
+    self.assertAllClose(inputs + 3.14, outputs[2])
+
+  @chex.variants(with_jit=True, without_jit=True)
+  def test_missing_params(self):
+    variables = dict(
+        a=tf.Variable(3.14, trainable=True, name="aaa"),
+        b=tf.Variable(42.0, trainable=False, name="bbb"),
+    )
+
+    @tf.function
+    def tf_func(x):
+      return x + variables["a"] + variables["b"]
+
+    np_inputs = np.array(range(6), dtype=np.float32).reshape(3, 2)
+    jax_func, jax_params = tf2jax.convert(tf_func, np.zeros_like(np_inputs))
+
+    with self.assertRaisesRegex(
+        ValueError, r"Some parameters are missing, \[\'bbb\'\]."
+    ):
+      self.variant(jax_func)({"aaa": jax_params["aaa"]}, np_inputs)
+
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tf2jax-0.3.3/tf2jax/_src/utils.py` & `tf2jax-0.3.4/tf2jax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/_src/xla_utils.py` & `tf2jax-0.3.4/tf2jax/_src/xla_utils.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax/tf2jax_test.py` & `tf2jax-0.3.4/tf2jax/tf2jax_test.py`

 * *Files identical despite different names*

### Comparing `tf2jax-0.3.3/tf2jax.egg-info/PKG-INFO` & `tf2jax-0.3.4/tf2jax.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf2jax
-Version: 0.3.3
+Version: 0.3.4
 Summary: TF2JAX: Convert TensorFlow to JAX
 Home-page: https://github.com/deepmind/tf2jax
 Author: DeepMind
 Author-email: tf2jax-dev@google.com
 License: Apache 2.0
 Keywords: jax tensorflow conversion translate
 Classifier: Development Status :: 4 - Beta
@@ -203,15 +203,15 @@
 import tensorflow_hub as hub
 
 hub_model = hub.load("/tmp/blah")
 jax_func, jax_params = tf2jax.convert(tf.function(hub_model), tf.zeros_like(x))
 jax_outputs, updated_jax_params = jax_func(jax_params, x)
 ```
 
-## JAX to TensorFlow and Back Again.
+## JAX to TensorFlow and back again.
 
 `tf2jax.convert_functional` can convert the outputs of `jax2tf.convert` back
 into JAX code.
 
 ```python
 # Some JAX function.
 def forward(*inputs):
@@ -322,14 +322,57 @@
 operations from `reduce_window` operations generated by JAX2TF. This provides
 better performance because `reduce_window` implementation of these ops have
 O(N^2) complexity on CPU and GPU backends, and can suffer from long compilation
 times due to aggressive constant folding.
 
 See [jax2tf_cumulative_reduction] for more context.
 
+## JAX2TF Native Serialization and XlaCallModule.
+
+From JAX v0.4.7 and onward, `jax2tf.convert` preferred mode of operation (soon
+to be default) is **native serialization** in which the target function is
+lowered to [StableHLO] and wrapped in a single TensorFlow op, `XlaCallModule`.
+
+The new native serialization format will more faithfully reproduce the semantics
+of the target function, at the cost of some reduced flexibility for downstream
+processing as the computation graph is no longer exposed as a tf.Graph.
+
+`XlaCallModule` is supported by TF2JAX from v0.3.4 and onward.
+
+However as this makes use of a custom JAX primitive that aims to encapsulate
+[StableHLO] payload found in `XlaCallModule`, it does not possess JAX rules for
+transformations such as (but not limited to) batching and differentiation.
+
+* **Differentiation**: first order derivative of serialized function is
+still supported through custom gradients requested at serialization time with
+`jax2tf.convert(..., with_gradient=True)`. This is the default behaviour.
+* **Batching**: `jax.vmap` will fail, though users may be able to naively
+replicate the desired behavior with `jax.lax.map`, albeit with poorer
+performance.
+
+### Platform Specificity
+
+Natively serialized JAX programs are platform specific ([link](https://github.com/google/jax/blob/main/jax/experimental/jax2tf/README.md#natively-serialized-jax-modules-are-platform-specific)). Executing a natively
+serialized program on platforms other than the one for which it was lowered,
+would raise a ValueError, e.g.:
+
+```python
+ValueError: Unsupported backend: `cpu` not in `('tpu',)`.
+```
+
+This matches the behaviour of `XlaCallModule`.
+
+Users can disable this check via a config flag, but the resulting program may
+be slower or fail to execute completely.
+
+```python
+with tf2jax.override_config("xlacallmodule_strict_checks", False):
+  jax_func(np.zeros((20, 5), np.float32))
+```
+
 ## Limitations
 
 Currently, only a subset of TensorFlow ops are supported, and not necessarily
 all functionalities are supported for some ops. The code will fail fast. Support
 for additional TensorFlow ops are added on a as-needed basis. Please submit your
 requests via Github issues or send in your pull requests.
 
@@ -382,7 +425,8 @@
 
 [DeepMind JAX Ecosystem]: https://deepmind.com/blog/article/using-jax-to-accelerate-our-research "DeepMind JAX Ecosystem"
 [DeepMind JAX Ecosystem citation]: https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt "Citation"
 [JAX]: https://github.com/google/jax "JAX on GitHub"
 [TensorFlow]: https://github.com/tensorflow/tensorflow "TensorFlow on GitHub"
 [jax2tf documentation]: https://github.com/google/jax/blob/master/jax/experimental/jax2tf/README.md#calling-tensorflow-functions-from-jax "jax2tf documentation"
 [jax2tf_cumulative_reduction]: https://github.com/google/jax/blob/main/jax/experimental/jax2tf/jax2tf.py#L2172
+[StableHLO]: https://github.com/openxla/stablehlo
```

### Comparing `tf2jax-0.3.3/tf2jax.egg-info/SOURCES.txt` & `tf2jax-0.3.4/tf2jax.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 tf2jax/_src/ops_test.py
 tf2jax/_src/roundtrip_test.py
 tf2jax/_src/test_util.py
 tf2jax/_src/tf2jax.py
 tf2jax/_src/tf2jax_test.py
 tf2jax/_src/utils.py
 tf2jax/_src/xla_utils.py
-tf2jax/_src/experimental/__init__.py
-tf2jax/_src/experimental/mhlo.py
-tf2jax/_src/experimental/mhlo_test.py
-tf2jax/_src/experimental/ops.py
+tf2jax/experimental/__init__.py
+tf2jax/experimental/mhlo.py
+tf2jax/experimental/mhlo_test.py
+tf2jax/experimental/ops.py
+tf2jax/experimental/util.py
```

