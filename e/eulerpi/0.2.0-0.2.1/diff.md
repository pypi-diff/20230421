# Comparing `tmp/eulerpi-0.2.0.tar.gz` & `tmp/eulerpi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulerpi-0.2.0.tar", max compression
+gzip compressed data, was "eulerpi-0.2.1.tar", max compression
```

## Comparing `eulerpi-0.2.0.tar` & `eulerpi-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1117 2023-04-20 21:54:42.257745 eulerpi-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     4634 2023-04-20 21:54:42.257745 eulerpi-0.2.0/README.md
--rw-r--r--   0        0        0      564 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/__init__.py
--rw-r--r--   0        0        0      191 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/__init__.py
--rw-r--r--   0        0        0    10754 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/dense_grid.py
--rw-r--r--   0        0        0      355 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/dense_grid_types.py
--rw-r--r--   0        0        0     4609 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/inference.py
--rw-r--r--   0        0        0      514 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/inference_types.py
--rw-r--r--   0        0        0     3684 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/kde.py
--rw-r--r--   0        0        0    15213 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/model.py
--rw-r--r--   0        0        0    17486 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/result_manager.py
--rw-r--r--   0        0        0    17240 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/sampling.py
--rw-r--r--   0        0        0    20662 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/sparsegrid.py
--rw-r--r--   0        0        0     6393 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/core/transformations.py
--rw-r--r--   0        0        0    14800 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/CoronaData.csv
--rw-r--r--   0        0        0       94 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/__init__.py
--rw-r--r--   0        0        0     2767 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/corona/corona.py
--rw-r--r--   0        0        0     1295 2023-04-20 21:54:42.265745 eulerpi-0.2.0/eulerpi/examples/cpp/CMakeLists.txt
--rw-r--r--   0        0        0        0 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/cpp_model.hpp
--rw-r--r--   0        0        0     1191 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/cpp_plant.py
--rw-r--r--   0        0        0     2559 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/python_reference_plants.py
--rw-r--r--   0        0        0      357 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/cpp/wrapper.cpp
--rw-r--r--   0        0        0     1811 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
--rw-r--r--   0        0        0     1133 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_caffeine_model.py
--rw-r--r--   0        0        0     1564 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.py
--rw-r--r--   0        0        0     5493 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.xml
--rw-r--r--   0        0        0     2241 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/simple_models.py
--rw-r--r--   0        0        0   189602 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/ETF.csv
--rw-r--r--   0        0        0      268 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/ETF50.csv
--rw-r--r--   0        0        0       88 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/__init__.py
--rw-r--r--   0        0        0     5556 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/stock/stock.py
--rw-r--r--   0        0        0     5877 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv
--rw-r--r--   0        0        0     5046 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureData.csv
--rw-r--r--   0        0        0      215 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/__init__.py
--rw-r--r--   0        0        0     2136 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/examples/temperature/temperature.py
--rw-r--r--   0        0        0     2169 2023-04-20 21:54:42.269745 eulerpi-0.2.0/eulerpi/jax_extension.py
--rw-r--r--   0        0        0     2344 2023-04-20 21:54:42.269745 eulerpi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6058 1970-01-01 00:00:00.000000 eulerpi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1117 2023-04-21 01:14:59.791617 eulerpi-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     4704 2023-04-21 01:14:59.791617 eulerpi-0.2.1/README.md
+-rw-r--r--   0        0        0      564 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/__init__.py
+-rw-r--r--   0        0        0      191 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/__init__.py
+-rw-r--r--   0        0        0    10754 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/dense_grid.py
+-rw-r--r--   0        0        0      355 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/dense_grid_types.py
+-rw-r--r--   0        0        0     4609 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/inference.py
+-rw-r--r--   0        0        0      514 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/inference_types.py
+-rw-r--r--   0        0        0     3684 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/kde.py
+-rw-r--r--   0        0        0    15208 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/model.py
+-rw-r--r--   0        0        0    17486 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/result_manager.py
+-rw-r--r--   0        0        0    17240 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/sampling.py
+-rw-r--r--   0        0        0    20637 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/sparsegrid.py
+-rw-r--r--   0        0        0     6393 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/core/transformations.py
+-rw-r--r--   0        0        0    14800 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/CoronaData.csv
+-rw-r--r--   0        0        0       94 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/__init__.py
+-rw-r--r--   0        0        0     2767 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/corona/corona.py
+-rw-r--r--   0        0        0     1295 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0        0 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/cpp_model.hpp
+-rw-r--r--   0        0        0     1191 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/cpp_plant.py
+-rw-r--r--   0        0        0     2559 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/python_reference_plants.py
+-rw-r--r--   0        0        0      357 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/cpp/wrapper.cpp
+-rw-r--r--   0        0        0     1811 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml
+-rw-r--r--   0        0        0     1133 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_caffeine_model.py
+-rw-r--r--   0        0        0     1793 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.py
+-rw-r--r--   0        0        0     5493 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.xml
+-rw-r--r--   0        0        0     2241 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/simple_models.py
+-rw-r--r--   0        0        0   189602 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/ETF.csv
+-rw-r--r--   0        0        0      268 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/ETF50.csv
+-rw-r--r--   0        0        0       88 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/__init__.py
+-rw-r--r--   0        0        0     5556 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/stock/stock.py
+-rw-r--r--   0        0        0     5877 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv
+-rw-r--r--   0        0        0     5046 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureData.csv
+-rw-r--r--   0        0        0      215 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/examples/temperature/temperature.py
+-rw-r--r--   0        0        0     2169 2023-04-21 01:14:59.799617 eulerpi-0.2.1/eulerpi/jax_extension.py
+-rw-r--r--   0        0        0     2316 2023-04-21 01:14:59.803617 eulerpi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6128 1970-01-01 00:00:00.000000 eulerpi-0.2.1/PKG-INFO
```

### Comparing `eulerpi-0.2.0/LICENSE.md` & `eulerpi-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/README.md` & `eulerpi-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 <h1></h1>
 
 ![EPI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/blob/main/epi.png?raw=True "logo")
 
 <!-- The badges we want to display -->
 [![pages-build-deployment](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/pages/pages-build-deployment)
 [![Build & Publish Documentation](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/sphinx.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/sphinx.yml)
-[![CI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml)
+[![Publish to PyPI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/publish.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/publish.yml)
 [![pytest](https://img.shields.io/github/actions/workflow/status/Systems-Theory-in-Systems-Biology/EPI/ci.yml?label=pytest&logo=pytest)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml)
 
 [![flake8](https://img.shields.io/badge/flake8-checked-blue.svg)](https://flake8.pycqa.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE.md)
 [![Python](https://img.shields.io/badge/python-3.10-purple.svg)](https://www.python.org/)
+![PyPI](https://img.shields.io/pypi/v/eulerpi)
 
 Euler Parameter Inference (EPI) is a Python package for inverse parameter inference. It provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 
 ## Documentation
 
 The full documentation to this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
```

### Comparing `eulerpi-0.2.0/eulerpi/__init__.py` & `eulerpi-0.2.1/eulerpi/__init__.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/dense_grid.py` & `eulerpi-0.2.1/eulerpi/core/dense_grid.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/inference.py` & `eulerpi-0.2.1/eulerpi/core/inference.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/inference_types.py` & `eulerpi-0.2.1/eulerpi/core/inference_types.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/kde.py` & `eulerpi-0.2.1/eulerpi/core/kde.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/model.py` & `eulerpi-0.2.1/eulerpi/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     def param_dim(self):
         """The number of parameters of the model."""
         return len(self.amici_model.getParameterIds())
 
     @property
     def data_dim(self):
         """The number of observables of the model."""
-        return len(self.amici_model.getObservableIds())
+        return len(self.amici_model.getStateIds())
 
     def __init__(
         self,
         sbml_file: str,
         central_param: np.ndarray,
         param_limits: np.ndarray,
         param_names=None,
```

### Comparing `eulerpi-0.2.0/eulerpi/core/result_manager.py` & `eulerpi-0.2.1/eulerpi/core/result_manager.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/sampling.py` & `eulerpi-0.2.1/eulerpi/core/sampling.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/core/sparsegrid.py` & `eulerpi-0.2.1/eulerpi/core/sparsegrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,35 +455,33 @@
         pool.close()
         pool.join()
 
         # convert the results to a numpy array
         # Take care! The results here are for single points, therefore we cant use np.concatenate
         results = np.vstack(results)
 
-        print(results.shape)
-
         # save the results
         result_manager.save_overall(
             slice,
-            results[:, 0 : data.shape[1]],
-            results[:, data.shape[1] : data.shape[1] + slice.shape[0]],
-            results[:, data.shape[1] + slice.shape[0] :],
+            results[:, 0 : slice.shape[0]],
+            results[:, slice.shape[0] : slice.shape[0] + data.shape[1]],
+            results[:, slice.shape[0] + data.shape[1] :],
         )
         slice_name = result_manager.get_slice_name(slice)
-        overall_params[slice_name] = results[:, 0 : data.shape[1]]
+        overall_params[slice_name] = results[:, 0 : slice.shape[0]]
         overall_sim_results[slice_name] = results[
-            :, data.shape[1] : data.shape[1] + slice.shape[0]
+            :, slice.shape[0] : slice.shape[0] + data.shape[1]
         ]
         overall_density_evals[slice_name] = results[
-            :, data.shape[1] + slice.shape[0] :
+            :, slice.shape[0] + data.shape[1] :
         ]
         result_manager.save_inference_information(
             slice=slice,
             model=model,
-            inference_type=InferenceType.DENSE_GRID,
+            inference_type=InferenceType.SPARSE_GRID,
             num_processes=num_processes,
             num_levels=num_levels,
         )
 
     return (
         overall_params,
         overall_sim_results,
```

### Comparing `eulerpi-0.2.0/eulerpi/core/transformations.py` & `eulerpi-0.2.1/eulerpi/core/transformations.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/corona/CoronaData.csv` & `eulerpi-0.2.1/eulerpi/examples/corona/CoronaData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/corona/corona.py` & `eulerpi-0.2.1/eulerpi/examples/corona/corona.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/cpp/CMakeLists.txt` & `eulerpi-0.2.1/eulerpi/examples/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/cpp/cpp_model.hpp` & `eulerpi-0.2.1/eulerpi/examples/cpp/cpp_model.hpp`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/cpp/cpp_plant.py` & `eulerpi-0.2.1/eulerpi/examples/cpp/cpp_plant.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/cpp/python_reference_plants.py` & `eulerpi-0.2.1/eulerpi/examples/cpp/python_reference_plants.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml` & `eulerpi-0.2.1/eulerpi/examples/sbml/Caffeine_2Wks_Exponential_decay.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/sbml/sbml_caffeine_model.py` & `eulerpi-0.2.1/eulerpi/examples/sbml/sbml_caffeine_model.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/sbml/sbml_menten_model.xml` & `eulerpi-0.2.1/eulerpi/examples/sbml/sbml_menten_model.xml`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/simple_models.py` & `eulerpi-0.2.1/eulerpi/examples/simple_models.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/stock/ETF.csv` & `eulerpi-0.2.1/eulerpi/examples/stock/ETF.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/stock/stock.py` & `eulerpi-0.2.1/eulerpi/examples/stock/stock.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureArtificialParams.csv` & `eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureArtificialParams.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/temperature/TemperatureData.csv` & `eulerpi-0.2.1/eulerpi/examples/temperature/TemperatureData.csv`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/examples/temperature/temperature.py` & `eulerpi-0.2.1/eulerpi/examples/temperature/temperature.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/eulerpi/jax_extension.py` & `eulerpi-0.2.1/eulerpi/jax_extension.py`

 * *Files identical despite different names*

### Comparing `eulerpi-0.2.0/pyproject.toml` & `eulerpi-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eulerpi"
-version = "0.2.0"
+version = "0.2.1"
 description = "The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution."
 authors = ["Lars Kaiser <lars.g.kaiser@gmx.de>", "Sebastian Hoepfl <sebastian.hoepfl@ist.uni-stuttgart.de>", "Vincent Wagner <vincent.wagner@ist.uni-stuttgart.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -32,15 +32,14 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.2"
-pytest-datafiles = "^2.0.1"
 pyproject-flake8 = "^6.0.0.post1"
 sphinx-copybutton = "^0.5.1"
 sphinx = "^5"
 myst-parser = "^0.18.1"
 coverage = "^7.0.5"
 sphinx-togglebutton = "^0.3.2"
 ipykernel = "^6.21.2"
```

### Comparing `eulerpi-0.2.0/PKG-INFO` & `eulerpi-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulerpi
-Version: 0.2.0
+Version: 0.2.1
 Summary: The eulerian parameter inference (eulerpi) returns a parameter distribution, which is consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 Author: Lars Kaiser
 Author-email: lars.g.kaiser@gmx.de
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -31,21 +31,22 @@
 <h1></h1>
 
 ![EPI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/blob/main/epi.png?raw=True "logo")
 
 <!-- The badges we want to display -->
 [![pages-build-deployment](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/pages/pages-build-deployment)
 [![Build & Publish Documentation](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/sphinx.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/sphinx.yml)
-[![CI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml)
+[![Publish to PyPI](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/publish.yml/badge.svg)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/publish.yml)
 [![pytest](https://img.shields.io/github/actions/workflow/status/Systems-Theory-in-Systems-Biology/EPI/ci.yml?label=pytest&logo=pytest)](https://github.com/Systems-Theory-in-Systems-Biology/EPI/actions/workflows/ci.yml)
 
 [![flake8](https://img.shields.io/badge/flake8-checked-blue.svg)](https://flake8.pycqa.org/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE.md)
 [![Python](https://img.shields.io/badge/python-3.10-purple.svg)](https://www.python.org/)
+![PyPI](https://img.shields.io/pypi/v/eulerpi)
 
 Euler Parameter Inference (EPI) is a Python package for inverse parameter inference. It provides an implementation of the EPI algorithm, which takes observed data and a model as input and returns a parameter distribution consistent with the observed data by solving the inverse problem directly. In the case of a one-to-one mapping, this is the true underlying distribution.
 
 ## Documentation
 
 The full documentation to this software, including a detailed tutorial on how to use EPI and the api documentation, can be found under [Documentation](https://Systems-Theory-in-Systems-Biology.github.io/EPI/).
```

