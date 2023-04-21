# Comparing `tmp/openqaoa-0.1.2.tar.gz` & `tmp/openqaoa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openqaoa-0.1.2.tar", last modified: Thu Mar 23 12:37:57 2023, max compression
+gzip compressed data, was "openqaoa-0.1.3.tar", last modified: Fri Apr 21 10:55:20 2023, max compression
```

## Comparing `openqaoa-0.1.2.tar` & `openqaoa-0.1.3.tar`

### file list

```diff
@@ -1,183 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.141259 openqaoa-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-23 12:36:04.000000 openqaoa-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-03-23 12:37:57.141259 openqaoa-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-03-23 12:36:04.000000 openqaoa-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-23 12:36:04.000000 openqaoa-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 12:37:57.141259 openqaoa-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-23 12:36:04.000000 openqaoa-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.121259 openqaoa-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.121259 openqaoa-0.1.2/src/openqaoa-azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.121259 openqaoa-0.1.2/src/openqaoa-azure/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-azure/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-azure/backends/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.121259 openqaoa-0.1.2/src/openqaoa-braket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-braket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-braket/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-braket/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-braket/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-braket/backends/qaoa_braket_qpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27222 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/baseworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/algorithms/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/jobs/managed_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/qaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14897 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    23721 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/algorithms/workflow_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/basebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/cost_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/devices_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_analytical_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/derivatives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/derivatives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33489 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/derivatives/derivative_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/derivatives/qfim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.125259 openqaoa-0.1.2/src/openqaoa-core/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/logger_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/CANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/SPSA.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/iCANS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/fourier/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/is_independent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/quantum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.129258 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/qaoa_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/optimizers/training_vqa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.133258 openqaoa-0.1.2/src/openqaoa-core/problems/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/knapsack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/maximumcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/minimumvertexcover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/numberpartition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/shortestpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/problems/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.133258 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.133258 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20161 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.133258 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    58031 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.133258 openqaoa-0.1.2/src/openqaoa-pyquil/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-pyquil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.137258 openqaoa-0.1.2/src/openqaoa-pyquil/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-pyquil/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-pyquil/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.137258 openqaoa-0.1.2/src/openqaoa-qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.137258 openqaoa-0.1.2/src/openqaoa-qiskit/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-qiskit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-qiskit/backends/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-03-23 12:36:04.000000 openqaoa-0.1.2/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.137258 openqaoa-0.1.2/src/openqaoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-03-23 12:37:57.000000 openqaoa-0.1.2/src/openqaoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-23 12:37:57.000000 openqaoa-0.1.2/src/openqaoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:37:57.000000 openqaoa-0.1.2/src/openqaoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-23 12:37:57.000000 openqaoa-0.1.2/src/openqaoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-23 12:37:57.000000 openqaoa-0.1.2/src/openqaoa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:37:57.141259 openqaoa-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_analytical_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_aws_managed_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_circuit_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_custom_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    45726 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_optimizers_pennylane.py
--rw-r--r--   0 runner    (1001) docker     (123)    27168 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_parameters_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    40114 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_problems.py
--rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_pyquil_qvm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_qpu_braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_qpu_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_qpu_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_rqaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_sample_from_wavefunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_sim_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_simulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41780 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (123)    82513 2023-03-23 12:36:04.000000 openqaoa-0.1.2/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.937017 openqaoa-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-21 10:53:10.000000 openqaoa-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-21 10:55:20.937017 openqaoa-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-04-21 10:53:10.000000 openqaoa-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 10:53:10.000000 openqaoa-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:55:20.941017 openqaoa-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-21 10:53:10.000000 openqaoa-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-azure/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-azure/backends/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.909016 openqaoa-0.1.3/src/openqaoa-braket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-braket/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/gates_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10121 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-braket/backends/qaoa_braket_qpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28209 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/baseworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/managed_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28190 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.913016 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/algorithms/workflow_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/basebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/cost_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/devices_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/gates_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/plugin_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_analytical_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29828 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/derivatives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33489 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/derivative_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/derivatives/qfim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/logger_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/CANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/SPSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/iCANS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.917016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31659 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/is_independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34509 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/quantum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.921016 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/qaoa_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/optimizers/training_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/binpacking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/maximalindependentset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/maximumcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/minimumvertexcover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/numberpartition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/portfoliooptimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/shortestpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/problems/vehiclerouting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.925016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17246 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21328 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57894 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-pyquil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-pyquil/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/gates_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backend_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.929016 openqaoa-0.1.3/src/openqaoa-qiskit/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/gates_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16054 2023-04-21 10:53:10.000000 openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.933016 openqaoa-0.1.3/src/openqaoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 10:55:20.000000 openqaoa-0.1.3/src/openqaoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:55:20.937017 openqaoa-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_analytical_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_aws_managed_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36050 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_circuit_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_custom_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11791 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_pyquil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gate_applicators_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47713 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9670 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_optimizers_pennylane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_parameters_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66604 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_pyquil_qvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13835 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22623 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_qpu_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21036 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_rqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_sample_from_wavefunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30630 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_sim_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43760 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27559 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95997 2023-04-21 10:53:10.000000 openqaoa-0.1.3/tests/test_workflows.py
```

### Comparing `openqaoa-0.1.2/LICENSE` & `openqaoa-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/PKG-INFO` & `openqaoa-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: openqaoa
-Version: 0.1.2
-Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
-Home-page: https://github.com/entropicalabs/openqaoa
-Author: Entropica Labs
-License: MIT
-Keywords: quantum optimisation SDK
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: all
-License-File: LICENSE
-
 <div align="center">
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo_offW.png" width="650">
   <img alt="OpenQAOA" src="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo.png" width="650">
 </picture>
 
@@ -44,34 +25,39 @@
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
 Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
 
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPi. First, create a virtual environment with python3.8+ and then simply pip install openqaoa with the following command
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 
-```bash
+```
 pip install openqaoa
 ```
 
 Alternatively, you can install manually directly from the GitHub repository by
 
 1. Clone the git repository:
 
-```bash
-git clone git@github.com:entropicalabs/openqaoa.git
+```
+git clone https://github.com/entropicalabs/openqaoa.git
 ```
 
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** for the environment.
+2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 
-3. After cloning the repository `cd openqaoa` and pip install in edit mode. Use the following command for a vanilla install with the `scipy` optimizers:
+3. After cloning the repository `cd openqaoa` and pip install the package. 
 
-```bash
-pip install -e .
+```
+pip install .
+```
+If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
+
+```
+pip install .[tests]
 ```
 
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
 The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
@@ -98,22 +84,23 @@
 
 | Device location  | Device Name |
 | ------------- | ------------- |
 | `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
+| [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
 
 ## Running the tests
 
 To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
 
-> :warning: **Some tests require authentication**: all tests flagged `api` or `qpu` require valid qpu crendentials to be specified in `tests/credentials.json`
+> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
-> :warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
 
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at openqaoa@entropicalabs.com.
+We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.2/README.md` & `openqaoa-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: openqaoa
+Version: 0.1.3
+Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
+Home-page: https://github.com/entropicalabs/openqaoa
+Author: Entropica Labs
+License: MIT
+Keywords: quantum optimisation SDK
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8, <3.11
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+Provides-Extra: all
+License-File: LICENSE
+
 <div align="center">
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo_offW.png" width="650">
   <img alt="OpenQAOA" src="https://github.com/entropicalabs/openqaoa/blob/main/.github/images/openqaoa_logo.png" width="650">
 </picture>
 
@@ -25,34 +44,39 @@
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
 Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
 
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPi. First, create a virtual environment with python3.8+ and then simply pip install openqaoa with the following command
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 
-```bash
+```
 pip install openqaoa
 ```
 
 Alternatively, you can install manually directly from the GitHub repository by
 
 1. Clone the git repository:
 
-```bash
-git clone git@github.com:entropicalabs/openqaoa.git
+```
+git clone https://github.com/entropicalabs/openqaoa.git
 ```
 
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** for the environment.
+2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 
-3. After cloning the repository `cd openqaoa` and pip install in edit mode. Use the following command for a vanilla install with the `scipy` optimizers:
+3. After cloning the repository `cd openqaoa` and pip install the package. 
 
-```bash
-pip install -e .
+```
+pip install .
+```
+If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
+
+```
+pip install .[tests]
 ```
 
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
 The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
@@ -79,22 +103,23 @@
 
 | Device location  | Device Name |
 | ------------- | ------------- |
 | `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
+| [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
 
 ## Running the tests
 
 To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
 
-> :warning: **Some tests require authentication**: all tests flagged `api` or `qpu` require valid qpu crendentials to be specified in `tests/credentials.json`
+> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
-> :warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
 
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at openqaoa@entropicalabs.com.
+We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.2/setup.py` & `openqaoa-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "pandas>=1.3.5",
     "sympy>=1.10.1",
     "numpy>=1.22.3",
     "networkx>=2.8",
     "matplotlib>=3.4.3",
     "scipy>=1.8",
     "qiskit>=0.36.1",
+    "qiskit-ibm-provider",
     "pyquil>=3.1.0",
     "docplex>=2.23.1",
     "autograd>=1.4",
     "semantic_version>=2.10",
     "autoray>=0.3.1",
     "azure-quantum",
     "qdk",
@@ -83,14 +84,22 @@
         "": "src",
         "openqaoa": "src/openqaoa-core",
         "openqaoa_braket": "src/openqaoa-braket",
         "openqaoa_qiskit": "src/openqaoa-qiskit",
         "openqaoa_pyquil": "src/openqaoa-pyquil",
         "openqaoa_azure": "src/openqaoa-azure",
     },
+    entry_points={
+        "openqaoa.plugins": [
+            "qiskit = openqaoa_qiskit.backend_config",
+            "braket = openqaoa_braket.backend_config",
+            "pyquil = openqaoa_pyquil.backend_config",
+            "azure = openqaoa_azure.backend_config"
+        ]
+    },
     url="https://github.com/entropicalabs/openqaoa",
     install_requires=requirements,
     license="MIT",
     description="OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `openqaoa-0.1.2/src/openqaoa-azure/backends/devices.py` & `openqaoa-0.1.3/src/openqaoa-azure/backends/devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         Quantum Workspace.
 
         Parameters
         ----------
         device_name: `str`
             The name of the Azure remote QPU/Simulator to be used
         resource_id: `str`
-            resource_id
+            The resource_id of the Workplace
         az_location: `str`
-            az_location
+            The location of the Azure Workplace. e.g. "westus"
         """
 
         self.resource_id = resource_id
         self.location = az_location
         self.device_name = device_name
         self.device_location = "azure"
```

### Comparing `openqaoa-0.1.2/src/openqaoa-braket/backends/devices.py` & `openqaoa-0.1.3/src/openqaoa-braket/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-braket/backends/qaoa_braket_qpu.py` & `openqaoa-0.1.3/src/openqaoa-braket/backends/qaoa_braket_qpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from braket.circuits import Circuit
 from braket.circuits.gates import H
 from braket.circuits.result_types import Probability
 from braket.circuits.free_parameter import FreeParameter
 from braket.jobs.metrics import log_metric
 
 from .devices import DeviceAWS
+from .gates_braket import BraketGateApplicator
 from openqaoa.backends.basebackend import (
     QAOABaseBackendShotBased,
     QAOABaseBackendCloud,
     QAOABaseBackendParametric,
 )
 from openqaoa.qaoa_components import QAOADescriptor
 from openqaoa.qaoa_components.variational_parameters.variational_baseparams import (
@@ -149,14 +150,16 @@
     def parametric_qaoa_circuit(self) -> Circuit:
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
         the circuit.
         """
         parametric_circuit = Circuit()
+        gate_applicator = BraketGateApplicator()
+
         if self.prepend_state:
             parametric_circuit += self.prepend_state
 
         # Initial state is all |+>
         if self.init_hadamard:
             for each_qubit in self.problem_reg:
                 parametric_circuit += H.h(each_qubit)
@@ -167,18 +170,16 @@
             if each_gate.gate_label.type.value in ["MIXER", "COST"]:
                 angle_param = FreeParameter(each_gate.gate_label.__repr__())
                 self.braket_parameter_list.append(angle_param)
                 each_gate.angle_value = angle_param
             decomposition = each_gate.decomposition("standard")
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0]()
-                parametric_circuit = gate.apply_braket_gate(
-                    *each_tuple[1], parametric_circuit
-                )
+                gate = each_tuple[0](gate_applicator, *each_tuple[1])
+                gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit += self.append_state
 
         # TODO: needs to be fixed --> measurement operations on problem qubits
         parametric_circuit += Probability.probability()
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/baseworkflow.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/baseworkflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,26 @@
 from ..utilities import delete_keys_from_dict, is_valid_uuid, generate_uuid
 from ..backends.qaoa_backend import (
     DEVICE_NAME_TO_OBJECT_MAPPER,
     DEVICE_ACCESS_OBJECT_MAPPER,
 )
 
 
+def check_compiled(func):
+    def wrapper(self, *args, **kwargs):
+        result = func(self, *args, **kwargs)
+        if self.compiled:
+            raise ValueError(
+                "Cannot change properties of the object after compilation."
+            )
+        return result
+
+    return wrapper
+
+
 class Workflow(ABC):
     """
     Abstract class to represent an optimizer
 
     It's basic usage consists of
 
      #. Initialization
@@ -91,15 +103,14 @@
             "algorithm": None,  # qaoa or rqaoa
             "description": None,
             "run_by": None,
             "provider": None,
             "target": None,
             "cloud": None,
             "client": None,
-            "qubit_number": None,  # it is set automatically in the compilation from the problem object
             "execution_time_start": None,
             "execution_time_end": None,
         }
 
         # Initialize the experiment tags
         self.exp_tags = {}
 
@@ -115,40 +126,41 @@
             except:
                 raise ValueError("The exp_tags attribute is not json serializable")
 
         return super().__setattr__(__name, __value)
 
     def set_header(
         self,
-        project_id: str,
-        description: str,
-        run_by: str,
-        provider: str,
-        target: str,
-        cloud: str,
-        client: str,
+        project_id: str = None,
+        description: str = None,
+        run_by: str = None,
+        provider: str = None,
+        target: str = None,
+        cloud: str = None,
+        client: str = None,
         experiment_id: str = None,
     ):
         """
         Method to set the identification stamps of the optimizer object in self.header.
 
         Parameters
         ----------
         TODO : document the parameters
         """
+        if project_id is not None:
+            if not is_valid_uuid(project_id):
+                raise ValueError(
+                    "The project_id is not a valid uuid, example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
+                )
 
-        if not is_valid_uuid(project_id):
-            raise ValueError(
-                "The project_id is not a valid uuid, example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
-            )
-
-        if experiment_id != None:
+        if experiment_id is not None:
             if not is_valid_uuid(experiment_id):
                 raise ValueError(
-                    "The experiment_id is not a valid uuid, example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
+                    "The experiment_id is not a valid uuid, \
+                        example of a valid uuid: 8353185c-b175-4eda-9628-b4e58cb0e41b"
                 )
             else:
                 self.header["experiment_id"] = experiment_id
 
         self.header["project_id"] = project_id
         self.header["description"] = description
         self.header["run_by"] = run_by
@@ -172,28 +184,30 @@
         tags: `dict`
             Dictionary containing the tags to be added to the experiment.
             If the tag already exists, it will be overwritten.
         """
 
         self.exp_tags = {**self.exp_tags, **tags}
 
+    @check_compiled
     def set_device(self, device: DeviceBase):
         """ "
         Specify the device to be used by the QAOA.
 
         Parameters
         ----------
         location: `str`
             Can be either local, qcs, or ibmq
         name: `str`
             The name of the device to be used, for local simulators please refer to `q.local_simulators`.
             For cloud providers please refer to the provider's naming conventions
         """
         self.device = device
 
+    @check_compiled
     def set_backend_properties(self, **kwargs):
         """
         Set the backend properties
 
         Parameters
         -------------------
             device: DeviceBase
@@ -232,14 +246,15 @@
                 raise ValueError(
                     f"Specified argument `{value}` for `{key}` in set_backend_properties is not supported"
                 )
 
         self.backend_properties = BackendProperties(**kwargs)
         return None
 
+    @check_compiled
     def set_classical_optimizer(self, **kwargs):
         """
         Set the parameters for the classical optimizer to be used in the optimizers workflow
 
         Parameters
         ----------
             method: str
@@ -316,35 +331,35 @@
         assert isinstance(problem, QUBO), "The problem must be converted into QUBO form"
         self.problem = problem
 
         # the atomic id is generated every time that it is compiled
         self.header["atomic_id"] = generate_uuid()
 
         # header is updated with the qubit number of the problem
-        self.header["qubit_number"] = self.problem.n
+        self.set_exp_tags({"qubit_number": self.problem.n})
 
     def optimize():
         raise NotImplementedError
 
     def _serializable_dict(
-        self, complex_to_string: bool = False, intermediate_mesurements: bool = True
+        self, complex_to_string: bool = False, intermediate_measurements: bool = True
     ):
         """
         Returns a dictionary with all values and attributes of the object that we want to
         return in `asdict` and `dump(s)` methods in a dictionary.
         The returned dictionary has two keys: header and data. The header contains all the data
         that can identify the experiment, while the data contains all the input and output data
         of the experiment (also the experiment tags).
 
         Parameters
         ----------
         complex_to_string: bool
             If True, converts all complex numbers to strings. This is useful for
             JSON serialization, for the `dump(s)` methods.
-        intermediate_mesurements: bool
+        intermediate_measurements: bool
             If True, intermediate measurements are included in the dump.
             If False, intermediate measurements are not included in the dump.
             Default is True.
         """
 
         # create the final data dictionary
         data = {}
@@ -362,16 +377,16 @@
         for item in ["noise_model", "append_state", "prepend_state"]:
             if data["input_parameters"]["backend_properties"][item] is not None:
                 data["input_parameters"]["backend_properties"][item] = str(
                     data["input_parameters"]["backend_properties"][item]
                 )
 
         data["result"] = (
-            self.result.asdict(False, complex_to_string, intermediate_mesurements)
-            if not self.result in [None, {}]
+            self.result.asdict(False, complex_to_string, intermediate_measurements)
+            if self.result not in [None, {}]
             else None
         )
 
         # create the final header dictionary
         header = self.header.copy()
         header["metadata"] = {
             **self.exp_tags.copy(),
@@ -418,15 +433,15 @@
         exclude_keys : List[str]
             A list of keys to exclude from the returned dictionary.
         options : dict
             A dictionary of options to pass to the method that creates the dictionary to dump.
                 complex_to_string : bool
                     If True, converts complex numbers to strings. If False,
                     complex numbers are not converted to strings.
-                intermediate_mesurements : bool
+                intermediate_measurements : bool
                     If True, includes the intermediate measurements in the results.
                     If False, only the final measurements are included.
 
         Returns
         -------
         dict
         """
@@ -450,15 +465,15 @@
             The number of spaces to indent the result in the json file.
             If None, the result is not indented.
         exclude_keys : List[str]
             A list of keys to exclude from the json string.
         options : dict
             A dictionary of options to pass to the method that creates
             the dictionary to dump.
-        intermediate_mesurements : bool
+        intermediate_measurements : bool
             If True, includes the intermediate measurements in the results.
             If False, only the final measurements are included.
 
         Returns
         -------
         str
         """
@@ -475,15 +490,15 @@
                 indent=indent,
             )
 
     def dump(
         self,
         file_name: str = "",
         file_path: str = "",
-        prepend_id: bool = True,
+        prepend_id: bool = False,
         indent: int = 2,
         compresslevel: int = 0,
         exclude_keys: List[str] = [],
         overwrite: bool = False,
         options: dict = {},
     ):
         """
@@ -493,69 +508,85 @@
 
         Parameters
         ----------
         file_name : str
             The name of the json file.
         file_path : str
             The path where the json file will be saved.
+        prepend_id : bool
+            If True, the name will have the following format: '{project_id}--{experiment_id}--{atomic_id}--{file_name}.json'.
+            If False, the name will have the following format: '{file_name}.json'.
+            Default is False.
         indent : int
             The number of spaces to indent the result in the json file.
             If None, the result is not indented.
         compresslevel : int
             The compression level to use. If 0, no compression is used and a json file is saved.
             If 1, the fastest compression method is used. If 9, the slowest
             but most effective compression method is used. And a .gz file is saved.
         exclude_keys : List[str]
             A list of keys that should not be included in the json file.
         overwrite : bool
             If True, overwrites the file if it already exists. If False,
             raises an error if the file already exists.
         options : dict
             A dictionary of options to pass to the method that creates the dictionary to dump.
-        intermediate_mesurements : bool
+        intermediate_measurements : bool
             If True, includes the intermediate measurements in the results.
             If False, only the final measurements are included.
         """
 
         options = {**options, **{"complex_to_string": True}}
 
+        project_id = (
+            self.header["project_id"]
+            if not self.header["project_id"] is None
+            else "None"
+        )
+
         # get the full name
-        if prepend_id == False and file_name == "":
-            raise ValueError("If prepend_id is False, file_name must be specified.")
-        elif prepend_id == False:
+        if prepend_id is False and file_name == "":
+            raise ValueError(
+                "dump method missing argument: 'file_name'. Otherwise 'prepend_id' must be specified as True."
+            )
+        elif prepend_id is False:
             file = file_path + file_name
         elif file_name == "":
             file = (
                 file_path
+                + project_id
+                + "--"
                 + self.header["experiment_id"]
                 + "--"
                 + self.header["atomic_id"]
             )
         else:
             file = (
                 file_path
+                + project_id
+                + "--"
                 + self.header["experiment_id"]
                 + "--"
                 + self.header["atomic_id"]
                 + "--"
                 + file_name
             )
 
         # adding .json extension if not present and adding .gz extension if compresslevel is not 0 and not present
         file = file + ".json" if ".json" != file[-5:] else file
         if compresslevel != 0:
             file = file + ".gz" if ".gz" != file[-3:] else file
 
         # checking if the file already exists, and raising an error if it does and overwrite is False
-        if overwrite == False and exists(file):
+        if overwrite is False and exists(file):
             raise FileExistsError(
                 f"The file {file} already exists. Please change the name of the file or set overwrite=True."
             )
 
-        ## saving the file
+        # saving the file
         if compresslevel == 0:  # if compresslevel is 0, save as json file
             with open(file, "w") as f:
                 if exclude_keys == []:
                     json.dump(self._serializable_dict(**options), f, indent=indent)
                 else:
                     json.dump(
                         delete_keys_from_dict(
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/jobs/managed_job.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/jobs/managed_job.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/qaoa_result.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     delete_keys_from_dict,
 )
 from ...backends.basebackend import QAOABaseBackend, QAOABaseBackendStatevector
 from ...backends.qaoa_analytical_sim import QAOABackendAnalyticalSimulator
 
 
 def most_probable_bitstring(cost_hamiltonian, measurement_outcomes):
-
+    """
+    Computing the most probable bitstring
+    """
     mea_out = list(measurement_outcomes.values())
     index_likliest_states = np.argwhere(mea_out == np.max(mea_out))
     # degeneracy = len(index_likliest_states)
     solutions_bitstrings = [
         list(measurement_outcomes.keys())[e[0]] for e in index_likliest_states
     ]
 
@@ -50,15 +52,17 @@
     def __init__(
         self,
         log: "Logger",
         method: Type[str],
         cost_hamiltonian: Type[Hamiltonian],
         type_backend: Type[QAOABaseBackend],
     ):
-
+        """
+        init method
+        """
         self.__type_backend = type_backend
         self.method = method
         self.cost_hamiltonian = cost_hamiltonian
 
         self.evals = {
             "number_of_evals": log.func_evals.best[0],
             "jac_evals": log.jac_func_evals.best[0],
@@ -112,15 +116,15 @@
         if log.n_shots.history != []:
             self.n_shots = log.n_shots.history
 
     def asdict(
         self,
         keep_cost_hamiltonian: bool = True,
         complex_to_string: bool = False,
-        intermediate_mesurements: bool = True,
+        intermediate_measurements: bool = True,
         exclude_keys: List[str] = [],
     ):
         """
         Returns a dictionary with the results of the optimization, where the dictionary is serializable.
         If the backend is a statevector backend, the measurement outcomes will be the statevector,
         meaning that it is a list of complex numbers, which is not serializable.
         If that is the case, and complex_to_string is true the complex numbers are converted to strings.
@@ -128,15 +132,15 @@
         Parameters
         ----------
         keep_cost_hamiltonian: `bool`
             If True, the cost hamiltonian is kept in the dictionary. If False, it is removed.
         complex_to_string: `bool`
             If True, the complex numbers are converted to strings. If False, they are kept as complex numbers.
             This is useful for the JSON serialization.
-        intermediate_mesurements: bool, optional
+        intermediate_measurements: bool, optional
             If True, intermediate measurements are included in the dump.
             If False, intermediate measurements are not included in the dump.
             Default is True.
         exclude_keys: `list[str]`
             A list of keys to exclude from the returned dictionary.
 
         Returns
@@ -148,60 +152,84 @@
         return_dict = {}
         return_dict["method"] = self.method
         if keep_cost_hamiltonian:
             return_dict["cost_hamiltonian"] = convert2serialize(self.cost_hamiltonian)
         return_dict["evals"] = self.evals
         return_dict["most_probable_states"] = self.most_probable_states
 
-        complx_to_str = (
+        complex_to_str = (
             lambda x: str(x)
             if isinstance(x, np.complex128) or isinstance(x, complex)
             else x
         )
 
         # if the backend is a statevector backend, the measurement outcomes will be the statevector,
         # meaning that it is a list of complex numbers, which is not serializable.
         # If that is the case, and complex_to_string is true the complex numbers are converted to strings.
-        if complex_to_string and issubclass(
-            self.__type_backend, QAOABaseBackendStatevector
-        ):
+        if complex_to_string:
             return_dict["intermediate"] = {}
             for key, value in self.intermediate.items():
-                if (
-                    intermediate_mesurements == False and "measurement" in key
-                ):  # if intermediate_mesurements is false, the intermediate measurements are not included in the dump
-                    return_dict["intermediate"][key] = []
-                elif "measurement" in key and (
-                    isinstance(value, list) or isinstance(value, np.ndarray)
+                # Measurements and Cost may require casting
+                if "measurement" in key:
+                    if len(value) > 0:
+                        if intermediate_measurements is False:
+                            # if intermediate_measurements is false, the intermediate measurements are not included
+                            return_dict["intermediate"][key] = []
+                        elif isinstance(
+                            value[0], np.ndarray
+                        ):  # Statevector -> convert complex to str
+                            return_dict["intermediate"][key] = [
+                                [complex_to_str(item) for item in list_]
+                                for list_ in value
+                                if (
+                                    isinstance(list_, list)
+                                    or isinstance(list_, np.ndarray)
+                                )
+                            ]
+                        else:  # All other case -> cast numpy into
+                            return_dict["intermediate"][key] = [
+                                {k_: int(v_) for k_, v_ in v.items()} for v in value
+                            ]
+                    else:
+                        pass
+                elif "cost" == key and (
+                    isinstance(value[0], np.float64) or isinstance(value[0], np.float32)
                 ):
-                    return_dict["intermediate"][key] = [
-                        [complx_to_str(item) for item in list_]
-                        for list_ in value
-                        if (isinstance(list_, list) or isinstance(list_, np.ndarray))
-                    ]
+                    return_dict["intermediate"][key] = [float(item) for item in value]
                 else:
                     return_dict["intermediate"][key] = value
 
             return_dict["optimized"] = {}
             for key, value in self.optimized.items():
+                # If wavefunction do complex to str
                 if "measurement" in key and (
                     isinstance(value, list) or isinstance(value, np.ndarray)
                 ):
                     return_dict["optimized"][key] = [
-                        complx_to_str(item) for item in value
+                        complex_to_str(item) for item in value
                     ]
+                # if dictionary, convert measurement values to integers
+                elif "measurement" in key and (isinstance(value, dict)):
+                    return_dict["optimized"][key] = {
+                        k: int(v) for k, v in value.items()
+                    }
                 else:
                     return_dict["optimized"][key] = value
+
+                if "cost" in key and (
+                    isinstance(value, np.float64) or isinstance(value, np.float32)
+                ):
+                    return_dict["optimized"][key] = float(value)
         else:
             return_dict["intermediate"] = self.intermediate
             return_dict["optimized"] = self.optimized
 
         # if we are using a shot adaptive optimizer, we need to add the number of shots to the result,
         # so if attribute n_shots is not empty, it is added to the dictionary
-        if getattr(self, "n_shots", None) != None:
+        if getattr(self, "n_shots", None) is not None:
             return_dict["n_shots"] = self.n_shots
 
         return (
             return_dict
             if exclude_keys == []
             else delete_keys_from_dict(return_dict, exclude_keys)
         )
@@ -229,15 +257,15 @@
         result = cls.__new__(cls)
 
         # set the attributes of the new instance, using the dictionary
         for key, value in dictionary.items():
             setattr(result, key, value)
 
         # if there is an input cost hamiltonian, it is added to the result
-        if cost_hamiltonian != None:
+        if cost_hamiltonian is not None:
             result.cost_hamiltonian = cost_hamiltonian
 
         # if the measurement_outcomes are strings, they are converted to complex numbers
         if not isinstance(
             result.optimized["measurement_outcomes"], dict
         ) and isinstance(result.optimized["measurement_outcomes"][0], str):
             for i in range(len(result.optimized["measurement_outcomes"])):
@@ -277,15 +305,15 @@
         Returns
         -------
         `dict`
             The count dictionary obtained either throught the statevector or
             the actual measurement counts.
         """
 
-        if type(measurement_outcomes) == type(np.array([])):
+        if isinstance(measurement_outcomes, type(np.array([]))):
             measurement_outcomes = qaoa_probabilities(measurement_outcomes)
 
         return measurement_outcomes
 
     def plot_cost(
         self, figsize=(10, 8), label="Cost", linestyle="--", color="b", ax=None
     ):
@@ -331,15 +359,14 @@
         self,
         n_states_to_keep=None,
         figsize=(10, 8),
         label="Probability distribution",
         color="tab:blue",
         ax=None,
     ):
-
         """
         Helper function to plot the probabilities corresponding to each basis states
         (with prob != 0) obtained from the optimized result
 
         Parameters
         ----------
         n_states_to_keep: 'int
@@ -355,15 +382,15 @@
         ax: 'matplotlib.axes._subplots.AxesSubplot'
             Axis on which to plot the graph. Deafults to None
         """
 
         outcome = self.optimized["measurement_outcomes"]
 
         # converting to counts dictionary if outcome is statevector
-        if type(outcome) == type(np.array([])):
+        if isinstance(outcome, type(np.array([]))):
             outcome = self.get_counts(outcome)
             # setting norm to 1 since it might differ slightly for statevectors due to numerical preicision
             norm = np.float64(1)
         else:
             # needed to be able to divide the tuple by 'norm'
             norm = np.float64(sum(outcome.values()))
 
@@ -403,15 +430,15 @@
 
         # formatting labels
         labels = [
             r"$\left|{}\right>$".format(state) for state in states[:n_states_to_keep]
         ]
         labels.append("rest")
 
-        # represent the bar with the addition of all the remaining probabilites
+        # represent the bar with the addition of all the remaining probabilities
         rest = sum(probs[n_states_to_keep:])
 
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
 
         colors = [color for _ in range(n_states_to_keep)] + ["xkcd:magenta"]
 
@@ -466,15 +493,15 @@
             Axis on which to plot the graph. If none is given, a new figure will be created.
 
         """
 
         if ax is None:
             ax = plt.subplots(figsize=figsize)[1]
 
-        ## creating a list of parameters to plot
+        # creating a list of parameters to plot
         # if param_to_plot is not given, plot all the parameters
         if param_to_plot is None:
             param_to_plot = list(range(len(self.n_shots[0])))
         # if param_to_plot is a single value, convert to list
         elif type(param_to_plot) == int:
             param_to_plot = [param_to_plot]
         # if param_to_plot is not a list, raise error
@@ -500,40 +527,42 @@
         if len(param_to_plot) == 1:
             if type(label) == str:
                 label = [label]
             if type(color) == str:
                 color = [color]
 
         # if param_top_plot is a list and label or color are not lists, raise error
-        if (type(label) != list) or (type(color) != list and color != None):
+        if (type(label) != list) or (type(color) != list and color is not None):
             raise TypeError("`label` and `color` must be list of str")
         # if label is a list, check that all the elements are strings
-        for l in label:
-            assert type(l) == str, "`label` must be a list of strings"
+        for lab in label:
+            assert type(lab) == str, "`label` must be a list of strings"
         # if color is a list, check that all the elements are strings
-        if color != None:
+        if color is not None:
             for c in color:
                 assert type(c) == str, "`color` must be a list of strings"
 
         # if label and color are lists, check if they have the same length as param_to_plot
         if len(label) != len(param_to_plot) or (
-            color != None and len(color) != len(param_to_plot)
+            color is not None and len(color) != len(param_to_plot)
         ):
             raise ValueError(
-                f"`param_to_plot`, `label` and `color` must have the same length, `param_to_plot` is a list of {len(param_to_plot)} elements"
+                f"`param_to_plot`, `label` and `color` must have the same length, \
+                    `param_to_plot` is a list of {len(param_to_plot)} elements"
             )
 
         # linestyle must be a string or a list of strings, if it is a string, convert it to a list of strings
         if type(linestyle) != str and type(linestyle) != list:
             raise TypeError("`linestyle` must be str or list")
         elif type(linestyle) == str:
             linestyle = [linestyle for _ in range(len(param_to_plot))]
         elif len(linestyle) != len(param_to_plot):
             raise ValueError(
-                f"`linestyle` must have the same length as param_to_plot (length of `param_to_plot` is {len(param_to_plot)}), or be a string"
+                f"`linestyle` must have the same length as param_to_plot \
+                    (length of `param_to_plot` is {len(param_to_plot)}), or be a string"
             )
         else:
             for ls in linestyle:
                 assert type(ls) == str, "`linestyle` must be a list of strings"
 
         # plot the evolution of the number of shots for each parameter that is in param_to_plot
         transposed_n_shots = np.array(self.n_shots).T
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from typing import List, Callable, Optional
-import requests
+from typing import List, Callable, Optional, Union, Dict
+from copy import deepcopy
+import numpy as np
+
 from .qaoa_result import QAOAResult
 from ..workflow_properties import CircuitProperties
-from ..baseworkflow import Workflow
-from ...backends.devices_core import DeviceLocal, DeviceBase
+from ..baseworkflow import Workflow, check_compiled
+from ...backends import QAOABackendAnalyticalSimulator
+from ...backends.devices_core import DeviceLocal
 from ...backends.qaoa_backend import get_qaoa_backend
 from ...problems import QUBO
 from ...qaoa_components import (
     Hamiltonian,
     QAOADescriptor,
     create_qaoa_variational_params,
 )
+from ...qaoa_components.variational_parameters.variational_baseparams import (
+    QAOAVariationalBaseParams,
+)
 from ...utilities import get_mixer_hamiltonian, generate_timestamp
 from ...optimizers.qaoa_optimizer import get_optimizer
 
 
 class QAOA(Workflow):
     """
     A class implementing a QAOA workflow end to end.
@@ -111,14 +117,15 @@
         """
         super().__init__(device)
         self.circuit_properties = CircuitProperties()
 
         # change header algorithm to qaoa
         self.header["algorithm"] = "qaoa"
 
+    @check_compiled
     def set_circuit_properties(self, **kwargs):
         """
         Specify the circuit properties to construct QAOA circuit
 
         Parameters
         ----------
         qubit_register: `list`
@@ -249,19 +256,32 @@
 
         self.optimizer = get_optimizer(
             vqa_object=self.backend,
             variational_params=self.variate_params,
             optimizer_dict=self.classical_optimizer.asdict(),
         )
 
+        # Set the header properties
+        self.header["target"] = self.device.device_name
+        self.header["cloud"] = self.device.device_location
+
+        metadata = {
+            "p": self.circuit_properties.p,
+            "param_type": self.circuit_properties.param_type,
+            "init_type": self.circuit_properties.init_type,
+            "optimizer_method": self.classical_optimizer.method,
+        }
+
+        self.set_exp_tags(tags=metadata)
+
         self.compiled = True
 
         if verbose:
             print("\t \033[1m ### Summary ###\033[0m")
-            print(f"OpenQAOA has been compiled with the following properties")
+            print("OpenQAOA has been compiled with the following properties")
             print(
                 f"Solving QAOA with \033[1m {self.device.device_name} \033[0m on"
                 f"\033[1m{self.device.device_location}\033[0m"
             )
             print(
                 f"Using p={self.circuit_properties.p} with {self.circuit_properties.param_type}"
                 f"parameters initialized as {self.circuit_properties.init_type}"
@@ -283,33 +303,129 @@
         return None
 
     def optimize(self, verbose=False):
         """
         A method running the classical optimisation loop
         """
 
-        if self.compiled == False:
+        if self.compiled is False:
             raise ValueError("Please compile the QAOA before optimizing it!")
 
         # timestamp for the start of the optimization
         self.header["execution_time_start"] = generate_timestamp()
 
         self.optimizer.optimize()
         # TODO: result and qaoa_result will differ
         self.result = self.optimizer.qaoa_result
 
         # timestamp for the end of the optimization
         self.header["execution_time_end"] = generate_timestamp()
 
         if verbose:
-            print(f"optimization completed.")
+            print("Optimization completed.")
         return
 
+    def evaluate_circuit(
+        self,
+        params: Union[List[float], Dict[str, List[float]], QAOAVariationalBaseParams],
+    ):
+        """
+        A method to evaluate the QAOA circuit at a given set of parameters
+
+        Parameters
+        ----------
+        params: list or dict or QAOAVariationalBaseParams or None
+            List of parameters or dictionary of parameters. Which will be used to evaluate the QAOA circuit.
+            If None, the variational parameters of the QAOA object will be used.
+
+        Returns
+        -------
+        result: dict
+            A dictionary containing the results of the evaluation:
+            - "expectation": the expectation value of the cost Hamiltonian
+            - "uncertainty": the uncertainty of the expectation value of the cost Hamiltonian
+            - "measurement_results": either the state of the QAOA circuit output (if the QAOA circuit is
+            evaluated on a state simulator) or the counts of the QAOA circuit output
+            (if the QAOA circuit is evaluated on a QPU or shot-based simulator)
+        """
+
+        # before evaluating the circuit we check that the QAOA object has been compiled
+        if self.compiled is False:
+            raise ValueError("Please compile the QAOA before optimizing it!")
+
+        # Check the type of the input parameters and save them as a
+        # QAOAVariationalBaseParams object at the variable `params_obj`
+
+        # if the parameters are passed as a dictionary we copy and update the variational parameters of the QAOA object
+        if isinstance(params, dict):
+            params_obj = deepcopy(self.variate_params)
+            # we check that the dictionary contains all the parameters of the QAOA object that are not empty
+            for key, value in params_obj.asdict().items():
+                if value.size > 0:
+                    assert (
+                        key in params.keys()
+                    ), f"The parameter `{key}` is missing from the input dictionary"
+            params_obj.update_from_dict(params)
+
+        # if the parameters are passed as a list we copy and update the variational parameters of the QAOA object
+        elif isinstance(params, list) or isinstance(params, np.ndarray):
+            assert len(params) == len(
+                self.variate_params
+            ), "The number of parameters does not match the number of parameters in the QAOA circuit"
+            params_obj = deepcopy(self.variate_params)
+            params_obj.update_from_raw(params)
+
+        # if the parameters are passed as a QAOAVariationalBaseParams object we just take it as it is
+        elif isinstance(params, QAOAVariationalBaseParams):
+            # check whether the input params object is supported for circuit evaluation
+            assert (
+                len(self.variate_params.mixer_1q_angles) == len(params.mixer_1q_angles)
+                and len(self.variate_params.mixer_2q_angles)
+                == len(self.variate_params.mixer_2q_angles)
+                and len(self.variate_params.cost_1q_angles)
+                == len(self.variate_params.cost_1q_angles)
+                and len(self.variate_params.cost_2q_angles)
+                == len(self.variate_params.cost_2q_angles)
+            ), "Specify a supported params object"
+            params_obj = params
+
+        # if the parameters are passed in a different format, we raise an error
+        else:
+            raise TypeError(
+                f"The input params must be a list or a dictionary. Instead, received {type(params)}"
+            )
+
+        # Evaluate the QAOA circuit and return the results
+        output_dict = {
+            "cost": None,
+            "uncertainty": None,
+            "measurement_results": None,
+        }
+        # if the backend is the analytical simulator, we just return the expectation value of the cost Hamiltonian
+        if isinstance(self.backend, QAOABackendAnalyticalSimulator):
+            output_dict.update({"cost": self.backend.expectation(params_obj)[0]})
+
+        else:
+            cost, uncertainty = self.backend.expectation_w_uncertainty(params_obj)
+            measurement_results = (
+                self.backend.measurement_outcomes
+                if isinstance(self.backend.measurement_outcomes, dict)
+                else self.backend.measurement_outcomes.tolist()
+            )
+            output_dict.update(
+                {
+                    "cost": cost,
+                    "uncertainty": uncertainty,
+                    "measurement_results": measurement_results,
+                }
+            )
+        return output_dict
+
     def _serializable_dict(
-        self, complex_to_string: bool = False, intermediate_mesurements: bool = True
+        self, complex_to_string: bool = False, intermediate_measurements: bool = True
     ):
         """
         Returns all values and attributes of the object that we want to return in
         `asdict` and `dump(s)` methods in a dictionary.
 
         Parameters
         ----------
@@ -318,24 +434,24 @@
             This is useful for JSON serialization.
 
         Returns
         -------
         serializable_dict: dict
             A dictionary containing all the values and attributes of the object
             that we want to return in `asdict` and `dump(s)` methods.
-        intermediate_mesurements: bool
+        intermediate_measurements: bool
             If True, intermediate measurements are included in the dump.
             If False, intermediate measurements are not included in the dump.
             Default is True.
         """
 
         # we call the _serializable_dict method of the parent class,
         # specifying the keys to delete from the results dictionary
         serializable_dict = super()._serializable_dict(
-            complex_to_string, intermediate_mesurements
+            complex_to_string, intermediate_measurements
         )
 
         # we add the keys of the QAOA object that we want to return
         serializable_dict["data"]["input_parameters"]["circuit_properties"] = dict(
             self.circuit_properties
         )
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,29 @@
     It stores the results of the RQAOA optimization as a dictionary. With some custom methods.
     """
 
     def asdict(
         self,
         keep_cost_hamiltonian: bool = True,
         complex_to_string: bool = False,
-        intermediate_mesurements: bool = True,
+        intermediate_measurements: bool = True,
         exclude_keys: List[str] = [],
     ):
         """
         Returns the results as a full dictionary, meaning that the objects of the
         intermediate steps are also converted to dictionaries.
 
         Parameters
         ----------
         keep_cost_hamiltonian : bool, optional
             If True, the cost Hamiltonian is kept in the dictionary, by default True.
         complex_to_string : bool, optional
             If True, the complex numbers are converted to strings, by default False.
             This is useful for JSON serialization.
-        intermediate_mesurements: bool, optional
+        intermediate_measurements: bool, optional
             If True, intermediate measurements are included in the dump. If False,
             intermediate measurements are not included in the dump.
             Default is True.
         exclude_keys: `list[str]`, optional
             A list of keys to exclude from the returned dictionary.
 
         Returns
@@ -51,15 +51,15 @@
             results["intermediate_steps"].append(
                 {
                     "counter": step["counter"],
                     "problem": step["problem"].asdict(),
                     "qaoa_results": step["qaoa_results"].asdict(
                         keep_cost_hamiltonian,
                         complex_to_string,
-                        intermediate_mesurements,
+                        intermediate_measurements,
                     ),
                     "exp_vals_z": step["exp_vals_z"].tolist(),
                     "corr_matrix": step["corr_matrix"].tolist(),
                 }
             )
         return (
             results
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 max_terms_and_stats.update({max_spin: max_val})
 
             # Set the spin value to 0 to check for the next one
             Z[max_spin] = 0
 
     # Flag if we have have not been able to extract any relation for the terms
     if max_terms_and_stats == {}:
-        print(f"All expectation values are 0: Breaking degeneracy by fixing a qubit\n")
+        print("All expectation values are 0: Breaking degeneracy by fixing a qubit\n")
         max_terms_and_stats = {(0,): -1.0}
 
     return max_terms_and_stats
 
 
 def ada_max_terms(exp_vals_z: np.ndarray, corr_matrix: np.ndarray, n_max: int):
     """
@@ -128,15 +128,15 @@
                 max_terms_and_stats.update({max_spin: max_val})
 
             # Set the spin value to 0 to check for the next one
             Z[max_spin] = 0
 
     # Flag if we have have not been able to extract any relation for the terms
     if max_terms_and_stats == {}:
-        print(f"All expectation values are 0: Breaking degeneracy by fixing a qubit\n")
+        print("All expectation values are 0: Breaking degeneracy by fixing a qubit\n")
         max_terms_and_stats = {(0,): -1.0}
 
     # Correlation average magnitude
     avg_mag_stats = np.round(np.mean(np.abs(list(max_terms_and_stats.values()))), 10)
 
     # Select only the ones above average
     max_terms_and_stats = {
@@ -391,15 +391,15 @@
     # Define new QUBO problem as a dictionary
     old_register = set([spin for term in problem.terms for spin in term])
     new_problem_dict = {}
 
     # get a set of all the spins to be eliminated
     eliminated_spins = set()
     for spin in spin_map.keys():
-        if spin != spin_map[spin][1] or spin_map[spin][1] == None:
+        if spin != spin_map[spin][1] or spin_map[spin][1] is None:
             eliminated_spins.add(spin)
 
     # Scan all terms and weights
     for term, weight in zip(problem.terms, problem.weights):
         # Bias terms
         if len(term) == 1:
             # Extract spin from the map
@@ -601,15 +601,16 @@
         )
 
     return full_solution
 
 
 def solution_for_vanishing_instances(hamiltonian: Hamiltonian, spin_map: dict):
     """
-    Constructs the final solution of the smallest non vanishing problem by fixing the vanishing spins arbitrarily to 1 while obeying the correlations identified by the last run of QAOA before the problem vanished.
+    Constructs the final solution of the smallest non vanishing problem by fixing the vanishing spins arbitrarily to 1
+    while obeying the correlations identified by the last run of QAOA before the problem vanished.
     Computing the classical energy of the generated string.
 
     Parameters
     ----------
     spin_map: `dict`
         Spin map containing the correlations and eliminations of the smallest non-vanishing
         problem statement.
@@ -617,20 +618,22 @@
         Hamiltonian object containing the smallest non vanishing problem statement.
 
     Returns
     -------
     cl_energy: `float`
         The energy of the solution wrt the cost Hamiltonian.
     cl_ground_state: `list`
-        The (single) classical solution to the problem reconstructed accordingly to the last spin map. Represented as a binary string and then cast to a list to match the output of the `ground_state_hamiltonian` function which is used usually.
+        The (single) classical solution to the problem reconstructed accordingly to the last spin map.
+        Represented as a binary string and then cast to a list to match the output of the
+        `ground_state_hamiltonian` function which is used usually.
     """
     cl_ground_state = ""
 
     for spin in spin_map.keys():
-        if spin_map[spin][1] == None:
+        if spin_map[spin][1] is None:
             cl_ground_state += "1"
         else:
             # fix according to correlation factor
             factor = spin_map[spin][0]
             parent = spin_map[spin][1]
 
             if factor == 1.0:
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import numpy as np
 
 from .rqaoa_workflow_properties import RqaoaParameters
-from ..baseworkflow import Workflow
+from ..baseworkflow import Workflow, check_compiled
 from ..qaoa import QAOA
 from ..workflow_properties import CircuitProperties
 from ...backends.devices_core import DeviceLocal, DeviceBase
 from ...problems import QUBO
 from ...utilities import (
     ground_state_hamiltonian,
     exp_val_hamiltonian_termwise,
@@ -145,14 +145,15 @@
         super().__init__(device)  # use the parent class to initialize
         self.circuit_properties = CircuitProperties()
         self.rqaoa_parameters = RqaoaParameters()
 
         # change algorithm name to rqaoa
         self.header["algorithm"] = "rqaoa"
 
+    @check_compiled
     def set_circuit_properties(self, **kwargs):
         """
         Specify the circuit properties to construct the QAOA circuits
 
         Parameters
         ----------
             qubit_register: `list`
@@ -207,14 +208,15 @@
                     f"Specified argument {key} is not supported by the circuit"
                 )
 
         self.circuit_properties = CircuitProperties(**kwargs)
 
         return None
 
+    @check_compiled
     def set_rqaoa_parameters(self, **kwargs):
         """
         Specify the parameters to run a desired RQAOA program.
 
         Parameters
         ----------
         rqaoa_type: `int`
@@ -488,15 +490,15 @@
 
         # set compiled to false
         self.compiled = False
 
         # dump the object if dump is true
         if dump:
             self.dump(
-                **{**dump_options, **{"options": {"intermediate_mesurements": False}}}
+                **{**dump_options, **{"options": {"intermediate_measurements": False}}}
             )
 
         if verbose:
             print(f"RQAOA optimization completed.")
 
         return
 
@@ -542,15 +544,15 @@
             # max Number of spins to eliminate
             n = self.rqaoa_parameters.steps[counter]
 
         # If the step eliminates more spins than available, reduce step to match cutoff
         return (n_qubits - n_cutoff) if (n_qubits - n_cutoff) < n else n
 
     def _serializable_dict(
-        self, complex_to_string: bool = False, intermediate_mesurements: bool = True
+        self, complex_to_string: bool = False, intermediate_measurements: bool = True
     ):
         """
         Returns all values and attributes of the object that we want to
         return in `asdict` and `dump(s)` methods in a dictionary.
 
         Parameters
         ----------
@@ -559,23 +561,23 @@
             If False, complex numbers are converted to lists of real and imaginary parts.
 
         Returns
         -------
         serializable_dict: dict
             Dictionary containing all the values and attributes of the object
             that we want to return in `asdict` and `dump(s)` methods.
-        intermediate_mesurements: bool
+        intermediate_measurements: bool
             If True, intermediate measurements are included in the dump. If False,
             intermediate measurements are not included in the dump.
             Default is True.
         """
         # we call the _serializable_dict method of the parent class,
         # specifying the keys to delete from the results dictionary
         serializable_dict = super()._serializable_dict(
-            complex_to_string, intermediate_mesurements
+            complex_to_string, intermediate_measurements
         )
 
         # we add the keys of the RQAOA object that we want to return
         serializable_dict["data"]["input_parameters"]["circuit_properties"] = dict(
             self.circuit_properties
         )
         serializable_dict["data"]["input_parameters"]["rqaoa_parameters"] = dict(
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,18 +49,19 @@
         ----------
         rqaoa_type: `int`
             String specifying the RQAOA scheme under which eliminations are computed. The two methods are 'custom' and
             'adaptive'. Defaults to "custom".
         n_max: `int`
             Maximum number of eliminations allowed at each step when using the adaptive method. Defaults to 1.
         steps: `Union[list,int]`
-            Elimination schedule for the RQAOA algorithm. If an integer is passed, it sets the number of spins eliminated
-            at each step. If a list is passed, the algorithm will follow the list to select how many spins to eliminate
-            at each step. Note that the list needs enough elements to specify eliminations from the initial number of qubits
-            up to the cutoff value. If the list contains more, the algorithm will follow instructions until the cutoff value
+            Elimination schedule for the RQAOA algorithm. If an integer is passed, it sets the number of spins
+            eliminated at each step. If a list is passed, the algorithm will follow the list to select
+            how many spins to eliminate at each step. Note that the list needs enough elements to specify
+            eliminations from the initial number of qubits up to the cutoff value. If the list contains more,
+            the algorithm will follow instructions until the cutoff value
             is reached. Defaults to 1.
         n_cutoff: `int`
             Cutoff value at which the RQAOA algorithm obtains the solution classically. Defaults to 5.
         original_hamiltonian: `Hamiltonian`
             Hamiltonian encoding the original problem fed into the RQAOA algorithm. Defaults to None.
         counter: `int`
             Variable to count the step in the schedule. If counter = 3 the next step is schedule[3].
@@ -70,30 +71,31 @@
         self.n_max = n_max
         self.steps = steps
         self.n_cutoff = n_cutoff
         self.original_hamiltonian = original_hamiltonian
         self.counter = counter
 
         # check if the rqaoa type is correct
-        if not self.rqaoa_type in ALLOWED_RQAOA_TYPES:
+        if self.rqaoa_type not in ALLOWED_RQAOA_TYPES:
             self.compiled = False
             raise Exception(
                 f'rqaoa_type {self.rqaoa_type} is not supported. Please select "adaptive" or "custom".'
             )
 
         # check if the parameters given are in accordance with the rqaoa_type
         if self.rqaoa_type == "adaptive":
             if self.steps != 1:
                 raise ValueError(
-                    f"When using the adaptive method, the `steps` parameter is not required.  \
+                    "When using the adaptive method, the `steps` parameter is not required.  \
                     The parameter that specifies the maximum number of eliminations per step is `n_max`."
                 )
             if self.counter != 0:
                 raise ValueError(
-                    f"When using the adaptive method, the `counter` parameter is not required."
+                    "When using the adaptive method, the `counter` parameter is not required."
                 )
         else:
             if self.n_max != 1:
                 raise ValueError(
-                    f"When using the custom method, the `n_max` parameter is not required.  \
-                    The parameter that specifies the number of eliminations is `steps`, which can be a string or a list."
+                    "When using the custom method, the `n_max` parameter is not required.  \
+                    The parameter that specifies the number of eliminations is `steps`,\
+                          which can be a string or a list."
                 )
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/algorithms/workflow_properties.py` & `openqaoa-0.1.3/src/openqaoa-core/algorithms/workflow_properties.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/basebackend.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/basebackend.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/cost_function.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/cost_function.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/devices_core.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/devices_core.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_analytical_sim.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_analytical_sim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_backend.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,65 @@
 from typing import Union, Optional, List
 import numpy as np
 
+from .plugin_finder import plugin_finder_dict
 from .qaoa_vectorized import QAOAvectorizedBackendSimulator
 from .qaoa_analytical_sim import QAOABackendAnalyticalSimulator
 from .devices_core import DeviceBase, DeviceLocal
 from .basebackend import QuantumCircuitBase, QAOABaseBackend
 from ..qaoa_components import QAOADescriptor
-from openqaoa_braket.backends import DeviceAWS, QAOAAWSQPUBackend
-from openqaoa_qiskit.backends import (
-    DeviceQiskit,
-    QAOAQiskitQPUBackend,
-    QAOAQiskitBackendShotBasedSimulator,
-    QAOAQiskitBackendStatevecSimulator,
-)
-from openqaoa_azure.backends import DeviceAzure
-from openqaoa_pyquil.backends import (
-    DevicePyquil,
-    QAOAPyQuilQPUBackend,
-    QAOAPyQuilWavefunctionSimulatorBackend,
-)
-
-
-DEVICE_NAME_TO_OBJECT_MAPPER = {
-    "qiskit.qasm_simulator": QAOAQiskitBackendShotBasedSimulator,
-    "qiskit.shot_simulator": QAOAQiskitBackendShotBasedSimulator,
-    "qiskit.statevector_simulator": QAOAQiskitBackendStatevecSimulator,
-    "vectorized": QAOAvectorizedBackendSimulator,
-    "pyquil.statevector_simulator": QAOAPyQuilWavefunctionSimulatorBackend,
-    "analytical_simulator": QAOABackendAnalyticalSimulator,
-}
-
-DEVICE_ACCESS_OBJECT_MAPPER = {
-    DeviceQiskit: QAOAQiskitQPUBackend,
-    DevicePyquil: QAOAPyQuilQPUBackend,
-    DeviceAWS: QAOAAWSQPUBackend,
-    DeviceAzure: QAOAQiskitQPUBackend,
-}
 
+PLUGIN_DICT = plugin_finder_dict()
+
+def _create_mappers(input_plugin_dict: dict) -> dict:
+    
+    DEVICE_NAME_TO_OBJECT_MAPPER = dict()
+    DEVICE_ACCESS_OBJECT_MAPPER = dict()
+    
+    DEVICE_NAME_TO_OBJECT_MAPPER["vectorized"] = QAOAvectorizedBackendSimulator
+    DEVICE_NAME_TO_OBJECT_MAPPER["analytical_simulator"] = QAOABackendAnalyticalSimulator
+    
+    for each_entry_key, each_entry_value in input_plugin_dict.items():
+        if hasattr(each_entry_value, 'device_access'):
+            DEVICE_ACCESS_OBJECT_MAPPER.update(each_entry_value.device_access)
+        if hasattr(each_entry_value, 'device_name_to_obj'):
+            DEVICE_NAME_TO_OBJECT_MAPPER.update(each_entry_value.device_name_to_obj)
+        
+    return DEVICE_NAME_TO_OBJECT_MAPPER, DEVICE_ACCESS_OBJECT_MAPPER
+
+DEVICE_NAME_TO_OBJECT_MAPPER, DEVICE_ACCESS_OBJECT_MAPPER = _create_mappers(PLUGIN_DICT)
 
 def _backend_arg_mapper(
     backend_obj: QAOABaseBackend,
     n_shots: Optional[int] = None,
     seed_simulator: Optional[int] = None,
     qiskit_simulation_method: Optional[str] = None,
     noise_model=None,
     active_reset: Optional[bool] = None,
     rewiring=None,
     disable_qubit_rewiring: Optional[bool] = None,
     initial_qubit_mapping=None,
 ):
-
+    
     BACKEND_ARGS_MAPPER = {
         QAOABackendAnalyticalSimulator: {},
         QAOAvectorizedBackendSimulator: {},
-        QAOAQiskitBackendStatevecSimulator: {},
-        QAOAPyQuilWavefunctionSimulatorBackend: {},
-        QAOAQiskitBackendShotBasedSimulator: {
-            "n_shots": n_shots,
-            "seed_simulator": seed_simulator,
-            "qiskit_simulation_method": qiskit_simulation_method,
-            "noise_model": noise_model,
-            "initial_qubit_mapping": initial_qubit_mapping,
-        },
-        QAOAQiskitQPUBackend: {
-            "n_shots": n_shots,
-            "initial_qubit_mapping": initial_qubit_mapping,
-        },
-        QAOAPyQuilQPUBackend: {
-            "n_shots": n_shots,
-            "active_reset": active_reset,
-            "rewiring": rewiring,
-            "initial_qubit_mapping": initial_qubit_mapping,
-        },
-        QAOAAWSQPUBackend: {
-            "n_shots": n_shots,
-            "disable_qubit_rewiring": disable_qubit_rewiring,
-            "initial_qubit_mapping": initial_qubit_mapping,
-        },
     }
+    
+    local_vars = locals()
+    
+    for each_plugin_entrypoint in PLUGIN_DICT.values():
+        if hasattr(each_plugin_entrypoint, 'backend_args'):
+            for each_key, each_value in each_plugin_entrypoint.backend_args.items():
+                # Convert list of accepted parameters into a dictionary with
+                # the name of the variable as a key and the local value of the 
+                # variable
+                var_values = [local_vars[each_name] for each_name in each_value]
+                input_dict = {each_key: dict(zip(each_value, var_values))}
+                BACKEND_ARGS_MAPPER.update(input_dict)
 
     final_backend_kwargs = {
         key: value
         for key, value in BACKEND_ARGS_MAPPER[backend_obj].items()
         if value is not None
     }
     return final_backend_kwargs
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/backends/qaoa_vectorized.py` & `openqaoa-0.1.3/src/openqaoa-core/backends/qaoa_vectorized.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Union, List, Tuple, Type, Optional
 import numpy as np
 from copy import copy
 from scipy.sparse import csc_matrix, kron, diags
 from scipy.sparse.linalg import expm
 
 from .basebackend import QAOABaseBackendStatevector
+from .gates_vectorized import VectorizedGateApplicator
 from ..qaoa_components import QAOADescriptor, Hamiltonian
 from ..qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
 from ..utilities import generate_uuid, round_value
 
 
@@ -816,30 +817,32 @@
         params:
             ``QAOAVariationalBaseParams`` object that contains rotation angles and gates to be applied.
 
         Returns
         -------
             None
         """
+        gates_applicator = VectorizedGateApplicator()
+        
         # generate a job id for the wavefunction evaluation
         self.job_id = generate_uuid()
 
         # reset the wavefunction back to its initialisation state
         self.reset_circuit()
 
         # Assign angles and apply gates
         self.assign_angles(params)
 
         low_level_gate_list = []
         for each_gate in self.abstract_circuit:
             low_level_gate_list.extend(each_gate.decomposition("trivial"))
 
         for each_tuple in low_level_gate_list:
-            gate = each_tuple[0]()
-            gate.apply_vector_gate(*each_tuple[1], self)
+            gate = each_tuple[0](gates_applicator, *each_tuple[1])
+            gate.apply_gate(self)
 
         # Handle append state
         if self.append_state is not None:
 
             # Flatten (2,...,2) shaped wfn into a 2**n-dim column vector before multiplying with unitary matrix, ...
             self.wavefn = np.matmul(self.append_state, self.wavefn.flatten())
             # then re-shape it back to (2,...,2)
@@ -886,15 +889,15 @@
         """
 
         self.qaoa_circuit(params)
 
         # Reshape wavefunction
         wavefn_ = self.wavefn
 
-        self.measurement_outcomes = self.wavefn.flatten()
+        self.measurement_outcomes = wavefn_.flatten()
 
         # Compute the expectation value and its standard deviation
         ham_wf = self.ham_op * wavefn_
         exp_val = np.real(np.vdot(wavefn_, ham_wf))
 
         out = exp_val
 
@@ -918,15 +921,15 @@
         """
 
         self.qaoa_circuit(params)
 
         # Reshape wavefunction
         wavefn_ = self.wavefn
 
-        self.measurement_outcomes = self.wavefn.flatten()
+        self.measurement_outcomes = wavefn_.flatten()
 
         # Compute the expectation value and its standard deviation
         ham_wf = self.ham_op * wavefn_
         exp_val = np.real(np.vdot(wavefn_, ham_wf))
 
         exp_val_sq = np.real(np.vdot(ham_wf, ham_wf))
         std_dev = (exp_val_sq - exp_val**2) ** 0.5
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/derivatives/derivative_functions.py` & `openqaoa-0.1.3/src/openqaoa-core/derivatives/derivative_functions.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/derivatives/qfim.py` & `openqaoa-0.1.3/src/openqaoa-core/derivatives/qfim.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/logger_vqa.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/logger_vqa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/CANS.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/CANS.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/SPSA.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/SPSA.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/iCANS.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/iCANS.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/natural_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/newton_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/rmsprop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/optimization_methods/stochastic_grad_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/fourier/reconstruct.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/is_independent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/is_independent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/matrix_manipulation.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/multi_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/quantum.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/quantum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/single_dispatch.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/math/utils.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/math/utils.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/fft.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/random.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/random.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/tensor.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/numpy/wrapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/optimization_methods_pennylane.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/qaoa_optimizer.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/qaoa_optimizer.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/optimizers/training_vqa.py` & `openqaoa-0.1.3/src/openqaoa-core/optimizers/training_vqa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/converters.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from collections import defaultdict
 from typing import Union
+
 import numpy as np
 
 from .qubo import QUBO
 
 
 class FromDocplex2IsingModel(object):
     def __init__(
         self,
         model,
         multipliers: Union[float, list] = None,
         unbalanced_const: bool = False,
         strength_ineq: list = [0.1, 0.5],
     ):
-
         """
         Creates an instance to translate Docplex models to its Ising Model representation
 
         Parameters
         ----------
         model : Docplex model
             It is an object that has the mathematical expressions (cost function and
@@ -26,23 +26,27 @@
         multipliters: [float, integer, list]
             The strength of the penalties of the cost function
         heuristic: bool
             If the method for the inequality constraints is used. This method
             implement a novel approach that do not required slack variables.
         strength_ineq: List[float, float]
             Lagrange multipliers of the penalization term using the unbalanced
-            constrained method.
-            For the penalty => \lambda_2 * \zeta**2 - \lambda_1 * \zeta  || strength_ineq = [a, b]
-            Usually lambda_2 < lambda_1. Please refere to the paper:
-                Unbalanced penalizations: A novel approach of inequality constraints
-                codification in quantum optimization problems.
-        """
+            penalization method.
+            For the unbalanced penalization => - \lambda_1 h(x) + \lambda_2 * h(x)**2
+            where h(x) >= 0 is the inequality constraint.
+            strength_ineq = [\lambda_1, \lambda_2]
+            Usually \lambda_2 < \lambda_1. Please refer to the paper:
+                Unbalanced penalization: A new approach to encode inequality constraints
+                of combinatorial problems for quantum optimization algorithms
+                https://arxiv.org/abs/2211.13914
 
+        """
+        # assign the docplex Model
         self.model = model.copy()
-
+        self.model_name = model.name
         # save the index in a dict
         self.idx_terms = {}
         for x in self.model.iter_variables():
             self.idx_terms[x] = x.index
             if x.vartype.short_name != "binary":
                 TypeError(f"Variable {x.vartype.short_name} is not allowed.")
         # if unbalanced constraint  approach
@@ -55,16 +59,16 @@
         """
         Adds linear expresions to the objective function stored in self.qubo_dict.
 
         Parameters
         ----------
         expr : model.objective_expr
             A docplex model attribute.
-        """
 
+        """
         for x, weight in expr.get_linear_part().iter_terms():
             self.qubo_dict[(self.idx_terms[x],)] += weight
 
     def quadratic_expr(self, expr):
         """
         Adds quadratic terms to the objective function stored in self.qubo_dict.
 
@@ -97,16 +101,16 @@
         multiplier : float
             Lagrange multiplier of the penalty
 
         Returns
         -------
         penalty : docplex.mp.quad.QuadExpr
             Penalty that will be added to the cost function.
-        """
 
+        """
         penalty = multiplier * (expression) ** 2
         return penalty
 
     @staticmethod
     def bounds(linear_expression):
         """
         Generates the limits of a linear term
@@ -168,22 +172,23 @@
         constraint : docplex.mp.constr.LinearConstraint
             DESCRIPTION.
 
         Returns
         -------
         new_exp : docplex.mp.linear.LinearExpr
             The equality constraint representation of the inequality constraint.
+
         """
 
         if constraint.sense_string == "LE":  # Less or equal inequality constraint
             new_exp = constraint.get_right_expr() + -1 * constraint.get_left_expr()
         elif constraint.sense_string == "GE":  # Great or equal inequality constriant
             new_exp = constraint.get_left_expr() + -1 * constraint.get_right_expr()
         else:
-            AttributeError(
+            raise AttributeError(
                 f"It is not possible to implement constraint {constraint.sense_string}."
             )
 
         lower_bound, upper_bound = self.bounds(new_exp)
         slack_lim = upper_bound  # Slack var limit
 
         if slack_lim > 0:
@@ -207,52 +212,51 @@
             )  # restrict the last term to fit the upper bound
 
         return new_exp
 
     def inequality_to_unbalanced_penalty(self, constraint):
         """
         Inequality constraint based on an unbalanced penality function described in
-        detail in the paper: "Unbalanced penalizations: A novel approach of
-        inequality constraints codification in quantum optimization problems""
+        detail in the paper: https://arxiv.org/abs/2211.13914
 
         Parameters
         ----------
         constraint : DOcplex inequality constraint
             Inequality constraints in a DOcplex format.
 
         Returns
         -------
         penalty : DOcplex term
             Quadratic programing penalization term.
-        """
 
+        """
         if constraint.sense_string == "LE":  # Less or equal inequality constraint
             new_exp = constraint.get_right_expr() + -1 * constraint.get_left_expr()
         elif constraint.sense_string == "GE":  # Great or equal inequality constriant
             new_exp = constraint.get_left_expr() + -1 * constraint.get_right_expr()
         else:
-            AttributeError(
+            raise AttributeError(
                 f"It is not possible to implement constraint {constraint.sense_string}."
             )
         strength = self.strength_ineq
-        penalty = strength[0] * new_exp**2 - strength[1] * new_exp
+        penalty = -strength[0] * new_exp + strength[1] * new_exp**2
         return penalty
 
     def multipliers_generators(self):
         """
         Penality term size adapter, this is the Lagrange multiplier of the cost
         function penalties for every constraint if the multiplier is not indicated
         by the user.
 
         Returns
         -------
         float
             the multiplier resized by the cost function limits.
-        """
 
+        """
         cost_func = self.model.objective_expr
         l_bound_linear, u_bound_linear = self.bounds(cost_func.get_linear_part())
         l_bound_quad, u_bound_quad = self.quadratic_bounds(
             cost_func.iter_quad_triplets()
         )
         return 1.0 + (u_bound_linear - l_bound_linear) + (u_bound_quad - l_bound_quad)
 
@@ -264,29 +268,30 @@
         ----------
         multiplier : List
             For each constraint a multiplier, if None it automatically is selected.
 
         Returns
         -------
         None.
+
         """
 
         constraints_list = list(self.model.iter_linear_constraints())
         n_constraints = len(constraints_list)
 
         if (
             multipliers is None
         ):  # Default penalties are choosen from the bounds of the objective func.
             multipliers = n_constraints * [self.multipliers_generators()]
 
         elif np.isscalar(multipliers):
             multipliers = n_constraints * [multipliers]
 
         elif type(multipliers) not in [list, np.ndarray]:
-            TypeError(f"{type(multipliers)} is not a accepted format")
+            raise TypeError(f"{type(multipliers)} is not a accepted format")
 
         for cn, constraint in enumerate(constraints_list):
             if (
                 constraint.sense_string == "EQ"
             ):  # Equality constraint added as a penalty.
                 left_exp = constraint.get_left_expr()
                 right_exp = constraint.get_right_expr()
@@ -294,22 +299,20 @@
                 penalty = self.equality_to_penalty(expression, multipliers[cn])
             elif constraint.sense_string in [
                 "LE",
                 "GE",
             ]:  # Inequality constraint added as a penalty with additional slack variables.
                 constraint.name = f"C{cn}"
                 if self.unbalanced:
-                    penalty = multipliers[cn] * self.inequality_to_unbalanced_penalty(
-                        constraint
-                    )
+                    penalty = self.inequality_to_unbalanced_penalty(constraint)
                 else:
                     ineq2eq = self.inequality_to_equality(constraint)
                     penalty = self.equality_to_penalty(ineq2eq, multipliers[cn])
             else:
-                TypeError("This is not a valid constraint.")
+                raise TypeError("This is not a valid constraint.")
 
             self.linear_expr(penalty)
             self.quadratic_expr(penalty)
             self.constant += penalty.constant
             self.objective_qubo += penalty
 
     @staticmethod
@@ -327,23 +330,22 @@
         qubo_weights : List
             coefficients of the variables
 
 
         Returns
         -------
         Ising Model stored on QUBO class
-        """
 
+        """
         ising_terms, ising_weights = [], []
         linear_terms = np.zeros(n_variables)
 
         constant_term = 0
         # Process the given terms and weights
         for weight, term in zip(qubo_weights, qubo_terms):
-
             if len(term) == 2:
                 u, v = term
 
                 if u != v:
                     ising_terms.append([u, v])
                     ising_weights.append(weight / 4)
                 else:
@@ -354,15 +356,15 @@
                 constant_term += weight / 4
             elif len(term) == 1:
                 linear_terms[term[0]] -= weight / 2
                 constant_term += weight / 2
             elif len(term) == 0:
                 constant_term += weight
             else:
-                TypeError(f"Term {term} is not recognized!")
+                raise TypeError(f"Term {term} is not recognized!")
 
         for variable, linear_term in enumerate(linear_terms):
             ising_terms.append([variable])
             ising_weights.append(linear_term)
 
         ising_terms.append([])
         ising_weights.append(constant_term)
@@ -416,14 +418,15 @@
         ]  # The right term is for adding the constant part of the QUBO
 
         weights = list(self.qubo_dict.values()) + [self.constant]
 
         n_variables = self.model.number_of_variables
         # QUBO docplex
         qubo_docplex = self.model.copy()
+        qubo_docplex.name = self.model_name
         qubo_docplex.clear_constraints()
         qubo_docplex.remove_objective()
         qubo_docplex.minimize(self.objective_qubo)
         # Ising Hamiltonian of the QUBO
         ising_model = self.qubo_to_ising(n_variables, terms, weights)
 
         return qubo_docplex, ising_model
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/helper_functions.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/helper_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from .problem import Problem
 from .knapsack import Knapsack, SlackFreeKnapsack
 from .maximumcut import MaximumCut
 from .minimumvertexcover import MinimumVertexCover
 from .numberpartition import NumberPartition
 from .shortestpath import ShortestPath
 from .tsp import TSP
+from .vehiclerouting import VRP
+from .maximalindependentset import MIS
+from .binpacking import BinPacking
 from .qubo import QUBO
 
 
 def create_problem_from_dict(problem_instance: dict) -> Problem:
     """
     Creates an object of the class corresponding to the problem type
     in the input instance, with the same attributes as the input instance.
@@ -35,14 +38,17 @@
         "tsp": TSP,
         "number_partition": NumberPartition,
         "maximum_cut": MaximumCut,
         "knapsack": Knapsack,
         "slack_free_knapsack": SlackFreeKnapsack,
         "minimum_vertex_cover": MinimumVertexCover,
         "shortest_path": ShortestPath,
+        "vehicle_routing": VRP,
+        "maximal_independent_set": MIS,
+        "bin_packing": BinPacking,
     }
 
     # check if the problem type is in the mapper
     assert (
         problem_instance["problem_type"] in problem_mapper
     ), f"Problem type {problem_instance['problem_type']} not supported."
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/knapsack.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/knapsack.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/maximumcut.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/maximumcut.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/minimumvertexcover.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/minimumvertexcover.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/numberpartition.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/numberpartition.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/problem.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/problem.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/qubo.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/qubo.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/shortestpath.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/shortestpath.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/problems/tsp.py` & `openqaoa-0.1.3/src/openqaoa-core/problems/tsp.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         self.qubit_2 = qubit_2
         self.gate_label = GateMapLabel(n_qubits=2, gatemap_type=GateMapType.FIXED)
 
     @property
     def _decomposition_standard(self) -> List[Tuple]:
 
         return [
-            (CX, [[self.qubit_1, self.qubit_2]]),
-            (CX, [[self.qubit_2, self.qubit_1]]),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
+            (CX, [self.qubit_2, self.qubit_1]),
+            (CX, [self.qubit_1, self.qubit_2]),
         ]
 
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
 
         return [
             (
@@ -76,19 +76,20 @@
             (
                 RX,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, -np.pi / 2)],
             ),
             (
                 RiSWAP,
                 [
-                    [self.qubit_1, self.qubit_2],
+                    self.qubit_1,
+                    self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, np.pi),
                 ],
             ),
-            (CZ, [[self.qubit_1, self.qubit_2]]),
+            (CZ, [self.qubit_1, self.qubit_2]),
             # X gate decomposition
             (RZ, [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
             (
                 RX,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RZ, [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
@@ -178,15 +179,16 @@
     def _decomposition_trivial(self) -> List[Tuple]:
 
         low_level_gate = eval(type(self).__name__.strip("GateMap"))
         return [
             (
                 low_level_gate,
                 [
-                    [self.qubit_1, self.qubit_2],
+                    self.qubit_1,
+                    self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class RXXGateMap(TwoQubitRotationGateMap):
@@ -200,23 +202,23 @@
             ),
             (RX, [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
             (
                 RY,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RZ,
                 [
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RY,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
             (
                 RY,
@@ -242,23 +244,23 @@
                 RX,
                 [self.qubit_1, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (
                 RX,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RZ,
                 [
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RY,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, -np.pi / 2)],
             ),
             (
                 RX,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, -np.pi / 2)],
@@ -272,45 +274,45 @@
 
         return [
             (
                 RY,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RZ,
                 [
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RY,
                 [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi / 2)],
             ),
             (RX, [self.qubit_2, RotationAngle(lambda x: x, self.gate_label, np.pi)]),
         ]
 
 
 class RZZGateMap(TwoQubitRotationGateMap):
     @property
     def _decomposition_standard(self) -> List[Tuple]:
 
         return [
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
             (
                 RZ,
                 [
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
-            (CX, [[self.qubit_1, self.qubit_2]]),
+            (CX, [self.qubit_1, self.qubit_2]),
         ]
 
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
 
         return [
             (
@@ -326,15 +328,16 @@
                     self.qubit_2,
                     RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             ),
             (
                 CPHASE,
                 [
-                    [self.qubit_1, self.qubit_2],
+                    self.qubit_1,
+                    self.qubit_2,
                     RotationAngle(lambda x: -2 * x, self.gate_label, self.angle_value),
                 ],
             ),
         ]
 
 
 class RYZGateMap(TwoQubitRotationGateMap):
@@ -359,19 +362,17 @@
     @property
     def _decomposition_standard2(self) -> List[Tuple]:
 
         return [
             (
                 RiSWAP,
                 [
-                    [
-                        self.qubit_1,
-                        self.qubit_2,
-                        RotationAngle(lambda x: x, self.gate_label, self.angle_value),
-                    ]
+                    self.qubit_1,
+                    self.qubit_2,
+                    RotationAngle(lambda x: x, self.gate_label, self.angle_value),
                 ],
             )
         ]
 
 
 class RotationGateMapFactory(object):
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         self.qubit_indices, self.pauli_str = self._sort_pauli_op(
             qubit_indices, pauli_str
         )
 
         # Store phase accumulated from simplification
         self.phase = phase
 
+    def __hash__(self) -> int:
+        return hash((self.qubit_indices, self.pauli_str, self.phase))
+
     @staticmethod
     def _sort_pauli_op(qubit_indices: Tuple[int], pauli_str: str):
         """
         Sort the Pauli Operator in increasing order of qubit indices.
 
         Parameters
         ----------
@@ -259,20 +262,21 @@
         """
         return len(self.qubit_indices)
 
     def __eq__(self, other_pauli_op):
         """
         Check whether two pauli_operators are equivalent, by comparing qubit indices and pauli strings.
         """
-        condition1 = (
-            True if self.qubit_indices == other_pauli_op.qubit_indices else False
+        tuple_1 = (self.qubit_indices, self.pauli_str, self.phase)
+        tuple_2 = (
+            other_pauli_op.qubit_indices,
+            other_pauli_op.pauli_str,
+            other_pauli_op.phase,
         )
-        condition2 = True if self.pauli_str == other_pauli_op.pauli_str else False
-
-        return condition1 and condition2
+        return tuple_1 == tuple_2
 
     def __copy__(self):
         """
         Create a new `PauliOp` by copying the current one.
         """
         copied_pauli_op = self.__class__.__new__(self.__class__)
         for attribute, value in vars(self).items():
@@ -475,14 +479,16 @@
                     pauli_str = term.pauli_str
                     self.terms.append(PauliOp(pauli_str, new_indices))
                 else:
                     self.terms.append(term)
 
                 # Update the coefficients with phase from Pauli Operators
                 self.coeffs.append(coeff * term.phase)
+                # after absorbing the phase in coeff, set the phase in term to 1
+                term.phase = 1
 
         if divide_into_singles_and_pairs:
             self._divide_into_singles_pairs()
 
     @property
     def qureg(self):
         """
@@ -541,14 +547,40 @@
 
         # Generate expression
         hamiltonian_expression = Symbol(str(self.constant))
         for term, coeff in zip(self.terms, self.coeffs):
             hamiltonian_expression += Symbol(str(coeff) + term.__str__())
         return hamiltonian_expression
 
+    # A function that outputs a dictionary of the Hamiltonian terms and coefficients
+    def hamiltonian_dict(self, classical: bool = True):
+        """
+        Generates a dictionary of the Hamiltonian terms and coefficients.
+
+        Parameters
+        ----------
+        classical: `bool`, optional
+            If true, returns a dictionary containing only qubit indices as terms
+            else returns a dictionary containing PauliOp objects as terms.
+
+        Returns
+        -------
+        `dict`
+            Dictionary of the Hamiltonian terms and coefficients.
+        """
+        hamiltonian_dict = {}
+        for term, coeff in zip(self.terms, self.coeffs):
+            if classical:
+                hamiltonian_dict[tuple(term.qubit_indices)] = coeff
+            else:
+                hamiltonian_dict[term] = coeff
+            # add the constant term
+            hamiltonian_dict[()] = self.constant
+        return hamiltonian_dict
+
     def __add__(self, other_hamiltonian):
         """
         Add two Hamiltonians in place updating `self`
 
         Parameters
         ----------
         other_hamiltonian: `Hamiltonian`
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/ansatz_constructor/rotationangle.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/annealingparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         v: List[Union[int, float]],
         u: List[Union[int, float]],
     ):
         # setup reg, qubits_singles and qubits_pairs
         super().__init__(qaoa_descriptor)
         assert q is not None, f"Depth q for {type(self).__name__} must be specified"
         self.q = q
-        self.u = u
         self.v = v
+        self.u = u
         self.betas = dct(self.v, n=self.p)
         self.gammas = dst(self.u, n=self.p)
 
     def __repr__(self):
         string = "Fourier Parameterisation:\n"
         string += "\tp: " + str(self.p) + "\n"
         string += "\tq: " + str(self.q) + "\n"
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py`

 * *Files 10% similar despite different names*

```diff
@@ -128,14 +128,63 @@
             The parameters in a 1D array. Has the same output format as the
             expected input of ``self.update_from_raw``. Hence corresponds to
             the flattened `parameters` in `__init__()`
 
         """
         raise NotImplementedError()
 
+    def update_from_dict(self, new_values: dict):
+        """
+        Update all the parameters from a dictionary.
+
+        The input has the same format as the output of ``self.asdict()``.
+
+        Parameters
+        ----------
+        new_values: `dict`
+            A dictionary with the new parameters. Must have the same keys as
+            the output of ``self.asdict()``.
+
+        """
+
+        assert isinstance(new_values, dict), f"Expected dict, got {type(new_values)}"
+
+        for key, value in new_values.items():
+            if key not in self.asdict().keys():
+                raise KeyError(
+                    f"'{key}' not in {self.__class__.__name__}, expected keys: {list(self.asdict().keys())}"
+                )
+            else:
+                if getattr(self, key).shape != np.array(value).shape:
+                    raise ValueError(
+                        f"Shape of '{key}' does not match. Expected shape {getattr(self, key).shape}, got {np.array(value).shape}."
+                    )
+
+        raw_params = []
+        for key, value in self.asdict().items():
+            if key in new_values.keys():
+                raw_params += list(np.array(new_values[key]).flatten())
+            else:
+                raw_params += list(np.array(value).flatten())
+
+        self.update_from_raw(raw_params)
+
+    def asdict(self) -> dict:
+        """
+        Return the parameters as a dictionary.
+
+        Returns
+        -------
+        dict:
+            The parameters as a dictionary. Has the same output format as the
+            expected input of ``self.update_from_dict``.
+
+        """
+        return {k[2:]: v for k, v in self.__dict__.items() if k[0:2] == "__"}
+
     @classmethod
     def linear_ramp_from_hamiltonian(
         cls, qaoa_descriptor: QAOADescriptor, time: float = None
     ):
         """Alternative to ``__init__`` that already fills ``parameters``.
 
         Calculate initial parameters from register, terms, weights
```

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py` & `openqaoa-0.1.3/src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-core/utilities.py` & `openqaoa-0.1.3/src/openqaoa-core/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,14 +744,17 @@
 
         # Add contribution to total energy
         energy += prob * config_energy
 
     # Normalize with respect to the number of shots
     energy *= 1 / shots
 
+    # Add constant term in Hamiltonian
+    energy += hamiltonian.constant
+
     return energy
 
 
 def energy_spectrum_hamiltonian(hamiltonian: Hamiltonian) -> np.ndarray:
     """
     Computes exactly the energy spectrum of the hamiltonian defined by terms
     and weights and its corresponding configuration of variables. Uses
@@ -1587,50 +1590,44 @@
         return True
     except ValueError:
         # If it's a value error, then the string is not a valid string for a UUID.
         return False
 
 
 def permute_counts_dictionary(
-    counts_dictionary: dict, final_qubit_layout: List[int]
+    counts_dictionary: dict, permutation_order: List[int]
 ) -> dict:
     """Permutes the order of the qubits in the counts dictionary to the
     original order if SWAP gates were used leading to modified qubit layout.
     Parameters
     ----------
     counts_dictionary : `dict`
         The measurement outcomes obtained from the Simulator/QPU
-    original_qubit_layout: List[int]
-        The qubit layout in which the qubits were initially
-    final_qubit_layout: List[int]
-        The final qubit layout after application of SWAPs
+    permutation_order: List[int]
+        The qubit order to permute the dictionary with
 
     Returns
     -------
     `dict`
         The permuted counts dictionary with qubits in the original place
     """
 
     # Create a mapping of original positions to final positions
-    original_qubit_layout = list(range(len(final_qubit_layout)))
+    # original order always goes from 0 -> n-1
+    original_order = list(range(len(permutation_order)))
     mapping = {
-        original_qubit_layout[i]: final_qubit_layout[i]
-        for i in range(len(original_qubit_layout))
+        original_order[i]: permutation_order[i] for i in range(len(original_order))
     }
     permuted_counts = {}
 
-    for basis, counts in counts_dictionary.items():
-
-        def permute_string(basis_state: str = basis, mapping: dict = mapping):
-            # Use the mapping to permute the string
-            permuted_string = "".join(
-                [basis_state[mapping[i]] for i in range(len(basis_state))]
-            )
-            return permuted_string
-
+    for basis_state, counts in counts_dictionary.items():
+        # Use the mapping to permute the string
+        permuted_string = "".join(
+            [basis_state[mapping[i]] for i in range(len(basis_state))]
+        )
         permuted_counts.update({permuted_string: counts})
 
     return permuted_counts
 
 
 ################################################################################
 # CHECKING FUNCTION
@@ -1715,15 +1712,15 @@
 
 def dicke_wavefunction(excitations, n_qubits):
     """
     Generate the k-excitations dicke statevector
 
     Parameters
     ----------
-    excitations: str
+    excitations: int
         The number of excitations in the basis
 
     n_qubits: int
         The number of qubits in the register
 
     Returns
     -------
```

### Comparing `openqaoa-0.1.2/src/openqaoa-pyquil/backends/devices.py` & `openqaoa-0.1.3/src/openqaoa-pyquil/backends/devices.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py` & `openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from collections import Counter
 import numpy as np
 from pyquil import Program, gates, quilbase
 from typing import List, Optional
 import warnings
 
 from .devices import DevicePyquil
+from .gates_pyquil import PyquilGateApplicator
 from openqaoa.backends.basebackend import (
     QAOABaseBackendShotBased,
     QAOABaseBackendCloud,
     QAOABaseBackendParametric,
 )
 from openqaoa.qaoa_components import QAOADescriptor
 from openqaoa.qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
 from openqaoa.qaoa_components.ansatz_constructor.gatemap import RZZGateMap, SWAPGateMap
+from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
 from openqaoa.utilities import generate_uuid
 
 
 def check_edge_connectivity(executable: Program, device: DevicePyquil):
 
     '''
     Check that the program does not contain 2-qubit terms that is not present
@@ -189,14 +191,16 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         `pyquil.Program`
             A pyquil.Program object.
         """
+        gates_applicator = PyquilGateApplicator()
+        
         if self.active_reset:
             parametric_circuit = Program(gates.RESET())
         else:
             parametric_circuit = Program()
 
         if self.rewiring != None:
             if self.rewiring in [
@@ -243,35 +247,29 @@
             if isinstance(each_gate, RZZGateMap) or isinstance(each_gate, SWAPGateMap):
                 decomposition = each_gate.decomposition("standard2")
             else:
                 decomposition = each_gate.decomposition("standard")
 
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0]()
-                if len(each_tuple[1]) == 1:
-                    qubits, rotation_angle = each_tuple[1][0], None
-                elif len(each_tuple[1]) == 2:
-                    qubits, rotation_angle = each_tuple[1]
+                if type(each_tuple[1][-1]) == RotationAngle:
+                    rotation_angle = each_tuple[1][-1]
+                    qubits = each_tuple[1][:-1]
                 else:
-                    raise ValueError(
-                        f"Specified an incorrect gate decomposition {each_tuple[1]}"
-                    )
-                if isinstance(qubits, list):
-                    new_qubits = [self.qubit_mapping[qubit] for qubit in qubits]
-                else:
-                    new_qubits = self.qubit_mapping[qubits]
+                    rotation_angle = None
+                    qubits = each_tuple[1]
+                if not isinstance(qubits, list):
+                    qubits = [qubits]
+                new_qubits = [self.qubit_mapping[qubit] for qubit in qubits]
+                    
                 if rotation_angle is None:
-                    parametric_circuit = gate.apply_pyquil_gate(
-                        new_qubits, parametric_circuit
-                    )
+                    gate = each_tuple[0](gates_applicator, *new_qubits)
                 else:
-                    parametric_circuit = gate.apply_pyquil_gate(
-                        new_qubits, rotation_angle, parametric_circuit
-                    )
+                    gate = each_tuple[0](gates_applicator, *new_qubits, rotation_angle)
+                gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit += self.append_state
 
         if self.final_mapping is None:
             for i, qbit in enumerate(self.problem_reg):
                 parametric_circuit += gates.MEASURE(self.qubit_mapping[qbit], ro[i])
```

### Comparing `openqaoa-0.1.2/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py` & `openqaoa-0.1.3/src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Tuple
 import numpy as np
 
 from pyquil import Program, gates
 from pyquil.api import WavefunctionSimulator
 
+from .gates_pyquil import PyquilGateApplicator
 from openqaoa.backends.basebackend import QAOABaseBackendStatevector
 from openqaoa.qaoa_components import QAOADescriptor
 from openqaoa.qaoa_components.variational_parameters.variational_baseparams import (
     QAOAVariationalBaseParams,
 )
 from openqaoa.qaoa_components.ansatz_constructor.gatemap import (
     RXGateMap,
@@ -54,15 +55,16 @@
         params: `QAOAVariationalBaseParams`
 
         Returns
         -------
         `pyquil.Program`
                 A pyquil.Program object.
         """
-
+        gates_applicator = PyquilGateApplicator()
+        
         self.assign_angles(params)
 
         circuit = Program()
         if self.prepend_state:
             circuit += self.prepend_state
 
         # Initial state is all |+>
@@ -78,16 +80,16 @@
                 in QAOAPyQuilWavefunctionSimulatorBackend.PYQUIL_ROTATIONGATES_LIBRARY
             ):
                 decomposition = each_gate.decomposition("trivial")
             else:
                 decomposition = each_gate.decomposition("standard")
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                low_gate = each_tuple[0]()
-                circuit = low_gate.apply_pyquil_gate(*each_tuple[1], circuit)
+                gate = each_tuple[0](gates_applicator, *each_tuple[1])
+                gate.apply_gate(circuit)
 
         if self.append_state:
             circuit += self.append_state
 
         return circuit
 
     def wavefunction(self, params: QAOAVariationalBaseParams):
```

### Comparing `openqaoa-0.1.2/src/openqaoa-qiskit/backends/devices.py` & `openqaoa-0.1.3/src/openqaoa-qiskit/backends/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qiskit import IBMQ
+from qiskit_ibm_provider import IBMProvider
 from qiskit_aer import AerSimulator
 from typing import List
 from openqaoa.backends.devices_core import DeviceBase
 
 
 class DeviceQiskit(DeviceBase):
     """
@@ -77,15 +77,15 @@
         """
 
         self.provider_connected = self._check_provider_connection()
 
         if self.provider_connected == False:
             return self.provider_connected
 
-        self.available_qpus = [backend.name() for backend in self.provider.backends()]
+        self.available_qpus = [backend.name for backend in self.provider.backends()]
 
         if self.device_name == "":
             return self.provider_connected
 
         self.qpu_connected = self._check_backend_connection()
 
         if self.provider_connected and self.qpu_connected:
@@ -108,24 +108,32 @@
 
     def _check_provider_connection(self) -> bool:
         """
         Private method for checking connection with provider.
         """
 
         try:
-            self.provider = IBMQ.load_account()
-            if any([self.hub, self.group, self.project]):
-                self.provider = IBMQ.get_provider(
-                    hub=self.hub, group=self.group, project=self.project
-                )
+            #Use default
+            self.provider = IBMProvider()
+            #Unless exact instance is specified
+            if all([self.hub, self.group, self.project]):
+                instance_name = self.hub + '/' + self.group + '/' + self.project
+                assert instance_name in self.provider.instances()
+                self.provider = IBMProvider(instance=instance_name)
+            elif any([self.hub, self.group, self.project]):
+                #if only partially specified, print warning.
+                raise Exception("You've only partially specified the instance name. Either"
+                                "the hub, group or project is missing. hub: {}, group: {}, project: {}.\n"
+                                "The default instance will be used instead. (This default can "
+                                "be specified when doing `IBMProvider.save_account`)")
             return True
         except Exception as e:
             print(
                 "An Exception has occured when trying to connect with the provider."
                 "Please note that you are required to set up your IBMQ account locally first."
                 "See: https://quantum-computing.ibm.com/lab/docs/iql/manage/account/ibmq"
-                "for how to save your IBMQ account locally: {}".format(e)
+                "for how to save your IBMQ account locally. \n {}".format(e)
             )
             return False
 
     def connectivity(self) -> List[List[int]]:
         return self.backend_device.configuration().coupling_map
```

### Comparing `openqaoa-0.1.2/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py` & `openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import time
 from typing import Optional, List
 import warnings
 
 # IBM Qiskit imports
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister, transpile
-from qiskit.providers.ibmq.job import (
-    IBMQJobApiError,
-    IBMQJobInvalidStateError,
-    IBMQJobFailureError,
-    IBMQJobTimeoutError,
+from qiskit_ibm_provider.job.exceptions import (
+    IBMJobApiError,
+    IBMJobInvalidStateError,
+    IBMJobFailureError,
+    IBMJobTimeoutError,
 )
 from qiskit.circuit import Parameter
 
 from .devices import DeviceQiskit
+from .gates_qiskit import QiskitGateApplicator
 from openqaoa.backends.basebackend import (
     QAOABaseBackendShotBased,
     QAOABaseBackendCloud,
     QAOABaseBackendParametric,
 )
 from openqaoa.qaoa_components import QAOADescriptor
 from openqaoa.qaoa_components.variational_parameters.variational_baseparams import (
@@ -91,27 +92,25 @@
 
         if self.device.provider_connected and self.device.qpu_connected:
             self.backend_qpu = self.device.backend_device
         elif self.device.provider_connected and self.device.qpu_connected in [
             False,
             None,
         ]:
-            if type(self.device).__name__ == "DeviceAzure":
-                raise Exception(
-                    "Connection to Azure was made. Error connecting to the specified backend."
-                )
-            else:
-                raise Exception(
-                    "Connection to IBMQ was made. Error connecting to the specified backend."
+            raise Exception(
+                "Connection to {} was made. Error connecting to the specified backend.".format(
+                    self.device.device_location.upper()
                 )
+            )
+
         else:
-            if type(self.device).__name__ == "DeviceAzure":
-                raise Exception("Error connecting to Azure.")
-            else:
-                raise Exception("Error connecting to IBMQ.")
+
+            raise Exception(
+                "Error connecting to {}.".format(self.device.device_location.upper())
+            )
 
         if self.device.n_qubits < self.n_qubits:
             raise Exception(
                 "There are lesser qubits on the device than the number of qubits required for the circuit."
             )
         # For parametric circuits
         self.parametric_circuit = self.parametric_qaoa_circuit
@@ -160,14 +159,15 @@
         ----------
             params:
                 Object of type QAOAVariationalBaseParams
         """
         # self.reset_circuit()
         creg = ClassicalRegister(len(self.problem_reg))
         parametric_circuit = QuantumCircuit(self.qureg, creg)
+        gate_applicator = QiskitGateApplicator()
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.problem_reg)
 
@@ -177,18 +177,16 @@
             if each_gate.gate_label.type.value in ["MIXER", "COST"]:
                 angle_param = Parameter(each_gate.gate_label.__repr__())
                 self.qiskit_parameter_list.append(angle_param)
                 each_gate.angle_value = angle_param
             decomposition = each_gate.decomposition("standard")
             # using the list above, construct the circuit
             for each_tuple in decomposition:
-                gate = each_tuple[0]()
-                parametric_circuit = gate.apply_ibm_gate(
-                    *each_tuple[1], parametric_circuit
-                )
+                gate = each_tuple[0](gate_applicator, *each_tuple[1])
+                gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit = parametric_circuit.compose(self.append_state)
 
         # only measure the problem qubits
         if self.final_mapping is None:
             parametric_circuit.measure(self.problem_reg, creg)
@@ -237,20 +235,20 @@
 
             while api_contact == False:
                 try:
                     self.job_id = job.job_id()
                     counts = job.result().get_counts()
                     api_contact = True
                     job_state = True
-                except (IBMQJobApiError, IBMQJobTimeoutError):
+                except (IBMJobApiError, IBMJobTimeoutError):
                     print("There was an error when trying to contact the IBMQ API.")
                     job_state = True
                     no_of_api_retries += 1
                     time.sleep(5)
-                except (IBMQJobFailureError, IBMQJobInvalidStateError):
+                except (IBMJobFailureError, IBMJobInvalidStateError):
                     print("There was an error with the state of the Job in IBMQ.")
                     no_of_job_retries += 1
                     break
 
                 if no_of_api_retries >= max_api_retries:
                     raise ConnectionError(
                         "Number of API Retries exceeded Maximum allowed."
```

### Comparing `openqaoa-0.1.2/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py` & `openqaoa-0.1.3/src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.providers.aer import AerSimulator
 from qiskit.providers.aer.noise import NoiseModel
 from qiskit.opflow.primitive_ops import PauliSumOp
 from qiskit.quantum_info import Statevector
 from qiskit.circuit import Parameter
 
+from .gates_qiskit import QiskitGateApplicator
 from openqaoa.backends.basebackend import (
     QAOABaseBackendParametric,
     QAOABaseBackendShotBased,
     QAOABaseBackendStatevector,
 )
 from openqaoa.qaoa_components import QAOADescriptor
 from openqaoa.qaoa_components.variational_parameters.variational_baseparams import (
@@ -145,14 +146,15 @@
         """
         Creates a parametric QAOA circuit, given the qubit pairs, single qubits with biases,
         and a set of circuit angles. Note that this function does not actually run
         the circuit.
         """
         # self.reset_circuit()
         parametric_circuit = QuantumCircuit(self.qureg)
+        gate_applicator = QiskitGateApplicator()
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.qureg)
 
@@ -168,18 +170,16 @@
                 in QAOAQiskitBackendShotBasedSimulator.QISKIT_GATEMAP_LIBRARY
             ):
                 decomposition = each_gate.decomposition("trivial")
             else:
                 decomposition = each_gate.decomposition("standard")
             # Create Circuit
             for each_tuple in decomposition:
-                low_gate = each_tuple[0]()
-                parametric_circuit = low_gate.apply_ibm_gate(
-                    *each_tuple[1], parametric_circuit
-                )
+                gate = each_tuple[0](gate_applicator,*each_tuple[1])
+                gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit = parametric_circuit.compose(self.append_state)
         parametric_circuit.measure_all()
 
         return parametric_circuit
 
@@ -360,14 +360,15 @@
         Parameters
         ----------
             params:
                 Object of type QAOAVariationalBaseParams
         """
         # self.reset_circuit()
         parametric_circuit = QuantumCircuit(self.qureg)
+        gate_applicator = QiskitGateApplicator()
 
         if self.prepend_state:
             parametric_circuit = parametric_circuit.compose(self.prepend_state)
         # Initial state is all |+>
         if self.init_hadamard:
             parametric_circuit.h(self.qureg)
 
@@ -383,18 +384,16 @@
                 in QAOAQiskitBackendStatevecSimulator.QISKIT_GATEMAP_LIBRARY
             ):
                 decomposition = each_gate.decomposition("trivial")
             else:
                 decomposition = each_gate.decomposition("standard")
             # Create Circuit
             for each_tuple in decomposition:
-                low_gate = each_tuple[0]()
-                parametric_circuit = low_gate.apply_ibm_gate(
-                    *each_tuple[1], parametric_circuit
-                )
+                gate = each_tuple[0](gate_applicator,*each_tuple[1])
+                gate.apply_gate(parametric_circuit)
 
         if self.append_state:
             parametric_circuit = parametric_circuit.compose(self.append_state)
 
         return parametric_circuit
 
     def wavefunction(
```

### Comparing `openqaoa-0.1.2/src/openqaoa.egg-info/PKG-INFO` & `openqaoa-0.1.3/src/openqaoa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openqaoa
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenQAOA is a python open-source multi-backend Software Development Kit to create, customise and execute the Quantum Approximate Optimisation Algorithm (QAOA) on Noisy Intermediate-Scale Quantum (NISQ) devices, and simulators
 Home-page: https://github.com/entropicalabs/openqaoa
 Author: Entropica Labs
 License: MIT
 Keywords: quantum optimisation SDK
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -44,34 +44,39 @@
 
 Please, consider [joining our discord](https://discord.gg/ana76wkKBd) if you want to be part of our community and participate in the OpenQAOA's development. 
 
 Check out OpenQAOA website [https://openqaoa.entropicalabs.com/](https://openqaoa.entropicalabs.com/)
 
 ## Installation instructions
 
-You can install the latest version of OpenQAOA directly from PyPi. First, create a virtual environment with python3.8+ and then simply pip install openqaoa with the following command
+You can install the latest version of OpenQAOA directly from PyPI. First, create a virtual environment with python3.8, 3.9, 3.10 and then pip install openqaoa with the following command
 
-```bash
+```
 pip install openqaoa
 ```
 
 Alternatively, you can install manually directly from the GitHub repository by
 
 1. Clone the git repository:
 
-```bash
-git clone git@github.com:entropicalabs/openqaoa.git
 ```
+git clone https://github.com/entropicalabs/openqaoa.git
+```
+
+2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** (or newer) for the environment.
 
-2. Creating a python `virtual environment` for this project is recommended. (for instance, using conda). Instructions on how to create a virtual environment can be found [here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands). Make sure to use **python 3.8** for the environment.
+3. After cloning the repository `cd openqaoa` and pip install the package. 
 
-3. After cloning the repository `cd openqaoa` and pip install in edit mode. Use the following command for a vanilla install with the `scipy` optimizers:
+```
+pip install .
+```
+If you are interested in running the tests or the docs you can do so my using the installment modifiers `[docs]` and `[tests]`. For example,
 
-```bash
-pip install -e .
+```
+pip install .[tests]
 ```
 
 Should you face any issue during the installation, please drop us an email at openqaoa@entropicalabs.com or open an issue!
 
 ## Getting started
 
 The documentation for OpenQAOA can be found [here](https://el-openqaoa.readthedocs.io/en/latest/).
@@ -98,22 +103,23 @@
 
 | Device location  | Device Name |
 | ------------- | ------------- |
 | `local`  | `['qiskit.shot_simulator', 'qiskit.statevector_simulator', 'qiskit.qasm_simulator', 'vectorized', 'pyquil.statevector_simulator']`  |
 | [Amazon Braket](https://docs.aws.amazon.com/braket/latest/developerguide/braket-devices.html)    | IonQ, Rigetti, OQC, and simulators |
 | [IBMQ](https://quantum-computing.ibm.com/)    | Please check the IBMQ backends available to your account |
 | [Rigetti QCS](https://qcs.rigetti.com/sign-in)     | Aspen-11, Aspen-M-1, and QVM simulator |
+| [Azure](https://azure.microsoft.com/en-us/products/quantum) | IonQ, Quantinuum, Rigetti, QCI |
 
 
 ## Running the tests
 
 To run the test, first, make sure to have installed all the optional testing dependencies by running `pip install .[tests]` (note, the braket must to be escaped if you are using the popular zsh shell), and then just type `pytest tests/.` from the project's root folder.
 
-> :warning: **Some tests require authentication**: all tests flagged `api` or `qpu` require valid qpu crendentials to be specified in `tests/credentials.json`
+> :warning: **Some tests require authentication**: Please, check the flags in `pytest.ini`. Currently these testes are marked `qpu`, `api`, `docker_aws`, `braket_api`, `sim`
 
-> :warning: **Some tests require authentication**: Please, note that the PyQuil-Rigetti tests contained in `test_pyquil_qvm.py` requires an active `qvm` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html))
+> :warning: **Some tests require Rigetti's QVM or a valid AWS Jobs docker**: Please, note these tests are marked as `qvm` and `docker_aws` (see Rigetti's documentation [here](https://pyquil-docs.rigetti.com/en/v3.1.0/qvm.html) for more information).
 
 ## Contributing and feedback
 
 If you find any bugs or errors, have feature requests, or code you would like to contribute, feel free to open an issue or send us a pull request on GitHub.
 
-We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at openqaoa@entropicalabs.com.
+We are always interested to hear about projects built with EntropicaQAOA. If you have an application you'd like to tell us about, drop us an email at [openqaoa@entropicalabs.com](mailto:openqaoa@entropicalabs.com)
```

### Comparing `openqaoa-0.1.2/src/openqaoa.egg-info/SOURCES.txt` & `openqaoa-0.1.3/src/openqaoa.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/openqaoa-azure/__init__.py
+src/openqaoa-azure/backend_config.py
 src/openqaoa-azure/backends/__init__.py
 src/openqaoa-azure/backends/devices.py
 src/openqaoa-braket/__init__.py
+src/openqaoa-braket/backend_config.py
 src/openqaoa-braket/backends/__init__.py
 src/openqaoa-braket/backends/devices.py
+src/openqaoa-braket/backends/gates_braket.py
 src/openqaoa-braket/backends/qaoa_braket_qpu.py
 src/openqaoa-core/__init__.py
 src/openqaoa-core/_version.py
 src/openqaoa-core/utilities.py
 src/openqaoa-core/algorithms/__init__.py
 src/openqaoa-core/algorithms/baseworkflow.py
 src/openqaoa-core/algorithms/workflow_properties.py
 src/openqaoa-core/algorithms/jobs/__init__.py
 src/openqaoa-core/algorithms/jobs/managed_job.py
 src/openqaoa-core/algorithms/qaoa/__init__.py
+src/openqaoa-core/algorithms/qaoa/qaoa_benchmark.py
 src/openqaoa-core/algorithms/qaoa/qaoa_result.py
 src/openqaoa-core/algorithms/qaoa/qaoa_workflow.py
 src/openqaoa-core/algorithms/rqaoa/__init__.py
 src/openqaoa-core/algorithms/rqaoa/rqaoa_result.py
 src/openqaoa-core/algorithms/rqaoa/rqaoa_utils.py
 src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow.py
 src/openqaoa-core/algorithms/rqaoa/rqaoa_workflow_properties.py
 src/openqaoa-core/backends/__init__.py
 src/openqaoa-core/backends/basebackend.py
 src/openqaoa-core/backends/cost_function.py
 src/openqaoa-core/backends/devices_core.py
+src/openqaoa-core/backends/gates_vectorized.py
+src/openqaoa-core/backends/plugin_finder.py
 src/openqaoa-core/backends/qaoa_analytical_sim.py
 src/openqaoa-core/backends/qaoa_backend.py
 src/openqaoa-core/backends/qaoa_device.py
 src/openqaoa-core/backends/qaoa_vectorized.py
 src/openqaoa-core/derivatives/__init__.py
 src/openqaoa-core/derivatives/derivative_functions.py
 src/openqaoa-core/derivatives/qfim.py
@@ -72,24 +78,28 @@
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/gradient_descent.py
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/momentum.py
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/nesterov_momentum.py
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rms_prop.py
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/rotosolve.py
 src/openqaoa-core/optimizers/pennylane/pennylane_optimizers/spsa.py
 src/openqaoa-core/problems/__init__.py
+src/openqaoa-core/problems/binpacking.py
 src/openqaoa-core/problems/converters.py
 src/openqaoa-core/problems/helper_functions.py
 src/openqaoa-core/problems/knapsack.py
+src/openqaoa-core/problems/maximalindependentset.py
 src/openqaoa-core/problems/maximumcut.py
 src/openqaoa-core/problems/minimumvertexcover.py
 src/openqaoa-core/problems/numberpartition.py
+src/openqaoa-core/problems/portfoliooptimization.py
 src/openqaoa-core/problems/problem.py
 src/openqaoa-core/problems/qubo.py
 src/openqaoa-core/problems/shortestpath.py
 src/openqaoa-core/problems/tsp.py
+src/openqaoa-core/problems/vehiclerouting.py
 src/openqaoa-core/qaoa_components/__init__.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/__init__.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/baseparams.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/gatemap.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/gatemaplabel.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/gates.py
 src/openqaoa-core/qaoa_components/ansatz_constructor/hamiltonianmapper.py
@@ -100,36 +110,46 @@
 src/openqaoa-core/qaoa_components/variational_parameters/extendedparams.py
 src/openqaoa-core/qaoa_components/variational_parameters/fourierparams.py
 src/openqaoa-core/qaoa_components/variational_parameters/standardparams.py
 src/openqaoa-core/qaoa_components/variational_parameters/variational_baseparams.py
 src/openqaoa-core/qaoa_components/variational_parameters/variational_params_converters.py
 src/openqaoa-core/qaoa_components/variational_parameters/variational_params_factory.py
 src/openqaoa-pyquil/__init__.py
+src/openqaoa-pyquil/backend_config.py
 src/openqaoa-pyquil/backends/__init__.py
 src/openqaoa-pyquil/backends/devices.py
+src/openqaoa-pyquil/backends/gates_pyquil.py
 src/openqaoa-pyquil/backends/qaoa_pyquil_qpu.py
 src/openqaoa-pyquil/backends/qaoa_pyquil_sim.py
 src/openqaoa-qiskit/__init__.py
+src/openqaoa-qiskit/backend_config.py
 src/openqaoa-qiskit/backends/__init__.py
 src/openqaoa-qiskit/backends/devices.py
+src/openqaoa-qiskit/backends/gates_qiskit.py
 src/openqaoa-qiskit/backends/qaoa_qiskit_qpu.py
 src/openqaoa-qiskit/backends/qaoa_qiskit_sim.py
 src/openqaoa.egg-info/PKG-INFO
 src/openqaoa.egg-info/SOURCES.txt
 src/openqaoa.egg-info/dependency_links.txt
+src/openqaoa.egg-info/entry_points.txt
 src/openqaoa.egg-info/requires.txt
 src/openqaoa.egg-info/top_level.txt
 tests/test_all.py
 tests/test_analytical_simulator.py
 tests/test_aws_managed_jobs.py
 tests/test_backends.py
+tests/test_benchmark.py
 tests/test_circuit_routing.py
 tests/test_converters.py
 tests/test_custom_mixer.py
 tests/test_derivative.py
+tests/test_gate_applicators_braket.py
+tests/test_gate_applicators_pyquil.py
+tests/test_gate_applicators_qiskit.py
+tests/test_gate_applicators_vectorized.py
 tests/test_gates.py
 tests/test_imports.py
 tests/test_logger.py
 tests/test_notebooks.py
 tests/test_operators.py
 tests/test_optimizers.py
 tests/test_optimizers_pennylane.py
```

### Comparing `openqaoa-0.1.2/src/openqaoa.egg-info/requires.txt` & `openqaoa-0.1.3/src/openqaoa.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pandas>=1.3.5
 sympy>=1.10.1
 numpy>=1.22.3
 networkx>=2.8
 matplotlib>=3.4.3
 scipy>=1.8
 qiskit>=0.36.1
+qiskit-ibm-provider
 pyquil>=3.1.0
 docplex>=2.23.1
 autograd>=1.4
 semantic_version>=2.10
 autoray>=0.3.1
 azure-quantum
 qdk
```

### Comparing `openqaoa-0.1.2/tests/test_analytical_simulator.py` & `openqaoa-0.1.3/tests/test_analytical_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
         try:
             q.optimize()
         except:
             exception = True
         assert exception, "Extended params didn't fail"
 
         # Testing for Fourier params
+        q = QAOA()
+        q.set_device(analytical_device)
         q.set_circuit_properties(
             p=1, param_type="fourier", init_type="rand", mixer_hamiltonian="x"
         )
         exception = False
         try:
             q.optimize()
         except:
```

### Comparing `openqaoa-0.1.2/tests/test_aws_managed_jobs.py` & `openqaoa-0.1.3/tests/test_aws_managed_jobs.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   limitations under the License.
 
 import os
 import pytest
 import unittest
 import networkx as nw
 from braket.jobs.local import LocalQuantumJob
+from unittest.mock import MagicMock
 
 from openqaoa.problems import MinimumVertexCover
 from openqaoa.algorithms import AWSJobs
 from openqaoa.algorithms import QAOA, RQAOA
 from openqaoa.backends import create_device
 
 
@@ -51,16 +52,18 @@
         # the S3 location where the SDK would store the task results by default for the job
         os.environ["AMZN_BRAKET_TASK_RESULTS_S3_URI"] = ""
         # the S3 location where the job results would be stored, as specified in CreateJob request’s OutputDataConfig
         os.environ["AMZN_BRAKET_JOB_RESULTS_S3_PATH"] = ""
         # the string that should be passed to CreateQuantumTask’s jobToken parameter for quantum tasks created in the job container
         # os.environ["AMZN_BRAKET_JOB_TOKEN"] = ''
 
+        self.n_qubits = 10
+
         self.vc = MinimumVertexCover(
-            nw.circulant_graph(10, [1]), field=1.0, penalty=10
+            nw.circulant_graph(self.n_qubits, [1]), field=1.0, penalty=10
         ).qubo
 
     def testOsEnvironAssignment(self):
 
         qaoa_workflow = AWSJobs(algorithm="QaoA")
         assert qaoa_workflow.algorithm == "qaoa"
         assert qaoa_workflow.input_dir == "./tests/jobs_test_input/"
@@ -76,18 +79,27 @@
 
         input_data_path = os.path.join(
             os.environ["AMZN_BRAKET_INPUT_DIR"], "input_data/"
         )
 
         # Create the qubo and the qaoa
         q = QAOA()
+        q.set_classical_optimizer(maxiter='5')
         q.set_device(
             create_device("aws", "arn:aws:braket:::device/quantum-simulator/amazon/sv1")
         )
-        q.set_classical_optimizer(maxiter="5")
+        
+        ### The following lines are needed to fool the github actions into correctly executing q.compile() !!
+        q.device.check_connection = MagicMock(return_value = True)
+        q.device.qpu_connected = True
+        q.device.provider_connected = True
+        q.device.n_qubits = self.n_qubits
+        q.device.backend_device = ''
+        q.device.aws_region = 'us-east-1'
+
         q.compile(self.vc)
         q.dump(
             file_name="openqaoa_params.json",
             file_path=input_data_path,
             prepend_id=False,
             overwrite=True,
         )
@@ -97,14 +109,15 @@
             source_module="./tests/jobs_test_input/aws_braket_source_module/openqaoa_qaoa_script.py",
             image_uri="amazon-braket-oq-dev",
             input_data={"input_data": input_data_path},
         )
 
         assert (job.state() == "COMPLETED") and (job.result() != None) == True
 
+
     @pytest.mark.docker_aws
     def testLocalJobRQAOA(self):
         """Test an end-to-end rqaoa running on a local docker instance"""
 
         input_data_path = os.path.join(
             os.environ["AMZN_BRAKET_INPUT_DIR"], "input_data/"
         )
@@ -112,14 +125,23 @@
         # Create the rqaoa
         r = RQAOA()
         r.set_rqaoa_parameters(n_cutoff=6)
         r.set_classical_optimizer(maxiter=3, save_intermediate=False)
         r.set_device(
             create_device("aws", "arn:aws:braket:::device/quantum-simulator/amazon/sv1")
         )
+        
+        ### The following lines are needed to fool the github actions into correctly executing q.compile() !!
+        r.device.check_connection = MagicMock(return_value = True)
+        r.device.qpu_connected = True
+        r.device.provider_connected = True
+        r.device.n_qubits = self.n_qubits
+        r.device.backend_device = ''
+        r.device.aws_region = 'us-east-1'
+
         r.compile(self.vc)
         r.dump(
             file_name="openqaoa_params.json",
             file_path=input_data_path,
             prepend_id=False,
             overwrite=True,
         )
```

### Comparing `openqaoa-0.1.2/tests/test_backends.py` & `openqaoa-0.1.3/tests/test_backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
 import json
-import os
 import pytest
 import subprocess
 
 from openqaoa.backends.qaoa_backend import (
     get_qaoa_backend,
     DEVICE_NAME_TO_OBJECT_MAPPER,
     DEVICE_ACCESS_OBJECT_MAPPER,
@@ -34,20 +33,21 @@
 class TestingBackendLocal(unittest.TestCase):
     """
     These tests check that the methods of the local backends are working properly.
     """
 
     def test_get_counts_and_expectation_n_shots(self):
         """
-        Check that the .get_counts admit n_shots as an argument, and works properly for the backend of all local devices.
-        Also check that .expectation and .expecation_w_uncertainty methods admit n_shots as an argument for the QAOABaseBackendShotBased backends.
+        Check that the .get_counts admit n_shots as an argument, and works properly for
+          the backend of all local devices.
+        Also check that .expectation and .expecation_w_uncertainty methods admit n_shots
+         as an argument for the QAOABaseBackendShotBased backends.
         """
 
         for device_name in DEVICE_NAME_TO_OBJECT_MAPPER.keys():
-
             # Analytical device doesn't have any of those so we are skipping it in the tests.
             if device_name in ["analytical_simulator"]:
                 continue
 
             qaoa_descriptor, variational_params_std = get_params()
 
             device = create_device(location="local", name=device_name)
@@ -58,33 +58,36 @@
             assert (
                 sum(
                     backend.get_counts(
                         params=variational_params_std, n_shots=58
                     ).values()
                 )
                 == 58
-            ), "`n_shots` is not being respected for the local simulator `{}` when calling backend.get_counts(n_shots=58).".format(
+            ), "`n_shots` is not being respected for the local simulator `{}` when \
+                calling backend.get_counts(n_shots=58).".format(
                 device_name
             )
             if isinstance(backend, QAOABaseBackendShotBased):
                 try:
                     backend.expectation(params=variational_params_std, n_shots=58)
                 except Exception:
                     raise Exception(
-                        "backend.expectation does not admit `n_shots` as an argument for the local simulator `{}`.".format(
+                        "backend.expectation does not admit `n_shots` as an argument \
+                            for the local simulator `{}`.".format(
                             device_name
                         )
                     )
                 try:
                     backend.expectation_w_uncertainty(
                         params=variational_params_std, n_shots=58
                     )
                 except Exception:
                     raise Exception(
-                        "backend.expectation_w_uncertainty does not admit `n_shots` as an argument for the local simulator `{}`.".format(
+                        "backend.expectation_w_uncertainty does not admit `n_shots` \
+                            as an argument for the local simulator `{}`.".format(
                             device_name
                         )
                     )
 
 
 class TestingBackendQPUs(unittest.TestCase):
     """
@@ -92,15 +95,14 @@
 
     For all of these tests, credentials.json MUST be filled with the appropriate
     credentials.
     """
 
     @pytest.mark.qpu
     def setUp(self):
-
         self.HUB = "ibm-q"
         self.GROUP = "open"
         self.PROJECT = "main"
 
         bashCommand = "az resource list"
         process = subprocess.Popen(bashCommand.split(), stdout=subprocess.PIPE)
         output, error = process.communicate()
@@ -118,90 +120,98 @@
                 if each_json["name"] == "TestingOpenQAOA"
             ][0]
             self.RESOURCE_ID = output_json_s["id"]
             self.AZ_LOCATION = output_json_s["location"]
 
     @pytest.mark.qpu
     def test_get_counts_and_expectation_n_shots(self):
-        """Check that the .get_counts, .expectation and .expecation_w_uncertainty methods admit n_shots as an argument for the backends of all QPUs."""
+        """
+        TODO: test needs to be updated as DEVICE_ACCESS_OBJECT_MAPPER is now dynamically filled
+        based on whether a module exists.
+
+        Check that the .get_counts, .expectation and .expecation_w_uncertainty methods
+        admit n_shots as an argument for the backends of all QPUs.
+        """
 
         list_device_attributes = [
             {
-                "QPU": "Qiskit",
-                "device_name": "ibmq_qasm_simulator",
-                "hub": self.HUB,
-                "group": self.GROUP,
-                "project": self.PROJECT,
+                "QPU": "Azure",
+                "device_name": "rigetti.sim.qvm",
+                "resource_id": self.RESOURCE_ID,
+                "az_location": self.AZ_LOCATION,
+            },
+            {
+                "QPU": "AWS",
+                "device_name": "arn:aws:braket:::device/quantum-simulator/amazon/sv1",
             },
             {
                 "QPU": "Pyquil",
                 "device_name": "2q-qvm",
                 "as_qvm": True,
                 "execution_timeout": 3,
                 "compiler_timeout": 3,
             },
             {
-                "QPU": "AWS",
-                "device_name": "arn:aws:braket:::device/quantum-simulator/amazon/sv1",
-            },
-            {
-                "QPU": "Azure",
-                "device_name": "rigetti.sim.qvm",
-                "resource_id": self.RESOURCE_ID,
-                "az_location": self.AZ_LOCATION,
+                "QPU": "Qiskit",
+                "device_name": "ibmq_qasm_simulator",
+                "hub": self.HUB,
+                "group": self.GROUP,
+                "project": self.PROJECT,
             },
         ]
 
         assert len(list_device_attributes) == len(
             DEVICE_ACCESS_OBJECT_MAPPER
-        ), "The number of QPUs in the list of tests is not the same as the number of QPUs in the DEVICE_ACCESS_OBJECT_MAPPER. The list should be updated."
-
+        ), "The number of QPUs in the list of tests is not the same as the number of QPUs in \
+             the DEVICE_ACCESS_OBJECT_MAPPER. The list should be updated."
+        print(DEVICE_ACCESS_OBJECT_MAPPER.items(), list_device_attributes)
         for (device, backend), device_attributes in zip(
             DEVICE_ACCESS_OBJECT_MAPPER.items(), list_device_attributes
         ):
-
             qaoa_descriptor, variational_params_std = get_params()
 
             QPU_name = device_attributes.pop("QPU")
             print("Testing {} backend.".format(QPU_name))
 
             # if QPU_name in ["AWS", 'Qiskit']:
             #     print(f"Skipping test for {QPU_name} backend.")
             #     continue
 
             try:
+                print(device, device_attributes)
                 device = device(**device_attributes)
                 backend = backend(
                     qaoa_descriptor=qaoa_descriptor,
                     device=device,
                     cvar_alpha=1,
                     n_shots=100,
                     prepend_state=None,
                     append_state=None,
                     init_hadamard=True,
                 )
 
-                # Check that the .get_counts, .expectation and .expectation_w_variance methods admit n_shots as an argument
+                # Check that the .get_counts, .expectation and .expectation_w_variance methods
+                # admit n_shots as an argument
                 assert (
                     sum(
                         backend.get_counts(
                             params=variational_params_std, n_shots=58
                         ).values()
                     )
                     == 58
-                ), "`n_shots` is not being respected when calling .get_counts(n_shots=58).".format(
+                ), "`n_shots` is not being respected \
+                    when calling .get_counts(n_shots=58) for QPU `{}`.".format(
                     QPU_name
                 )
                 backend.expectation(params=variational_params_std, n_shots=58)
                 backend.expectation_w_uncertainty(
                     params=variational_params_std, n_shots=58
                 )
 
             except Exception as e:
-
                 raise e from type(e)(f"Error raised for `{QPU_name}`: " + str(e))
 
             print("Test passed for {} backend.".format(QPU_name))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.2/tests/test_circuit_routing.py` & `openqaoa-0.1.3/tests/test_circuit_routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # unit testing for circuit routing functionality in OQ
 import unittest
 import numpy as np
-from typing import List, Callable, Optional
+from typing import List, Optional
 import pytest
 
-from openqaoa import QAOA
+from openqaoa import QAOA, create_device, QUBO
 from openqaoa.qaoa_components import (
     create_qaoa_variational_params,
     QAOADescriptor,
     PauliOp,
     Hamiltonian,
 )
 from openqaoa.utilities import X_mixer_hamiltonian
-from openqaoa.backends import QAOAvectorizedBackendSimulator, create_device
-from openqaoa.problems import NumberPartition, QUBO, Knapsack, MaximumCut, ShortestPath
+from openqaoa.problems import NumberPartition, Knapsack, MaximumCut, ShortestPath
 from openqaoa_pyquil.backends import DevicePyquil, QAOAPyQuilQPUBackend
 from openqaoa.backends.devices_core import DeviceBase
 from openqaoa.qaoa_components.ansatz_constructor.gatemap import SWAPGateMap
 
 
 class TestingQAOAPyquilQVM_QR(unittest.TestCase):
 
@@ -31,15 +30,14 @@
         Tests that QAOADescriptor with a trivial `routing_function` input (with no swaps) returns identical
         results as QAOADescriptor with no `routing_function` input, by comparing output of seeded QVM run.
         Different values of p, arguments, and cost hamiltonian coefficients are tested.
 
         """
 
         def routing_function_test1(device, problem_to_solve):
-
             # tuples ordered from 0,n, both SWAP and ising gates
             gate_list_indices = [[0, 1]]
 
             # True for SWAP
             swap_mask = [False]
 
             # {QPU: (0 to n index)}
@@ -113,15 +111,14 @@
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=5, compiler_timeout=5
         )
         device_pyquil.quantum_computer.qam.random_seed = seed
 
         for i in range(len(p_lst)):
-
             p = p_lst[i]
             args = args_lst[i]
             cost_hamil = cost_hamil_lst[i]
 
             # With routing
             mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
             qaoa_descriptor = QAOADescriptor(
@@ -162,22 +159,21 @@
             )
             expt_pyquil_no_qr = backend_obj_pyquil.expectation(variate_params)
 
             self.assertAlmostEqual(expt_pyquil_w_qr, expt_pyquil_no_qr)
 
     def test_cancelled_swap(self):
         """
-        Tests that QAOADescriptor with a trivial `routing_function` input (with two swaps that cancel each other) returns identical
-        results as QAOADescriptor with no `routing_function` input, by comparing output of seeded QVM run.
-        Different values of p, arguments, and cost hamiltonian coefficients are tested.
-
+        Tests that QAOADescriptor with a trivial `routing_function` input (with two swaps that cancel each other)
+        returns identical results as QAOADescriptor with no `routing_function` input,
+        by comparing output of seeded QVM run. Different values of p, arguments,
+        and cost hamiltonian coefficients are tested.
         """
 
         def routing_function_test1(device, problem_to_solve):
-
             # tuples ordered from 0,n, both SWAP and ising gates
             gate_list_indices = [[0, 1], [0, 1], [0, 1]]
 
             # True for SWAP
             swap_mask = [True, True, False]
 
             # {QPU: (0 to n index)}
@@ -251,15 +247,14 @@
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=5, compiler_timeout=5
         )
         device_pyquil.quantum_computer.qam.random_seed = seed
 
         for i in range(len(p_lst)):
-
             p = p_lst[i]
             args = args_lst[i]
             cost_hamil = cost_hamil_lst[i]
 
             # With routing
             mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
             qaoa_descriptor = QAOADescriptor(
@@ -310,15 +305,14 @@
 
         Note : Even with a fixed seed, insertion of swaps changes measurement statistics.
         Final assertion is therefore only up to a tolerance, chosen by eyeballing results for a chosen seed.
 
         """
 
         def routing_function_test1(device, problem_to_solve):
-
             # tuples ordered from 0,n, both SWAP and ising gates
             gate_list_indices = [[0, 1], [0, 1]]
 
             # True for SWAP
             swap_mask = [True, False]
 
             # {QPU: (0 to n index)}
@@ -392,15 +386,14 @@
 
         device_pyquil = DevicePyquil(
             device_name="2q-qvm", as_qvm=True, execution_timeout=10, compiler_timeout=10
         )
         device_pyquil.quantum_computer.qam.random_seed = seed
 
         for i in range(len(p_lst)):
-
             p = p_lst[i]
             args = args_lst[i]
             cost_hamil = cost_hamil_lst[i]
 
             # With routing
             mixer_hamil = X_mixer_hamiltonian(n_qubits=2)
             qaoa_descriptor = QAOADescriptor(
@@ -450,15 +443,14 @@
         Tests QAOADescriptor with different devices.
         results as QAOADescriptor with no `routing_function` input, by comparing output of seeded QVM run.
         Different values of p, arguments, and cost hamiltonian coefficients are tested.
 
         """
 
         def routing_function_test1(device, problem_to_solve):
-
             # tuples ordered from 0,n, both SWAP and ising gates
             gate_list_indices = [[0, 1], [1, 0], [0, 1]]
 
             # True for SWAP
             swap_mask = [True, True, False]
 
             # {QPU: (0 to n index)}
@@ -496,15 +488,14 @@
 
         device_name_lst = ["2q-qvm", "3q-qvm", "Aspen-M-3"]
 
         shots = 2
         seed = 1
 
         for i in range(len(p_lst)):
-
             p = p_lst[i]
             args = args_lst[i]
             cost_hamil = cost_hamil_lst[i]
 
             device_pyquil = DevicePyquil(
                 device_name=device_name_lst[i],
                 as_qvm=True,
@@ -599,17 +590,18 @@
             self.swap_mask,
             self.initial_physical_to_logical_mapping,
             self.final_logical_qubit_order,
         )
 
 
 class TestingQubitRouting(unittest.TestCase):
-    @pytest.mark.qpu
     def setUp(self):
-
+        """
+        Test edge cases
+        """
         # case qubits device > qubits problem (IBM NAIROBI)
         self.IBM_NAIROBI_KNAPSACK = ExpectedRouting(
             qubo=Knapsack.random_instance(n_items=3, seed=20).qubo,
             device_location="ibmq",
             device_name="ibm_nairobi",
             qpu_credentials={
                 "hub": "ibm-q",
@@ -878,15 +870,15 @@
                 0: 5,
                 7: 6,
             },
             final_logical_qubit_order=[2, 3, 6, 1, 4, 5, 0],
         )
 
         # case qubits device == qubits problem (RIGETTI)
-        self.RIGETTI_MACUT = ExpectedRouting(
+        self.RIGETTI_MAXCUT = ExpectedRouting(
             qubo=MaximumCut.random_instance(
                 n_nodes=9, edge_probability=0.9, seed=20
             ).qubo,
             device_location="qcs",
             device_name="9q-square-qvm",
             qpu_credentials={
                 "as_qvm": True,
@@ -1128,15 +1120,14 @@
 
         assert (
             gate_indices_list_new == expected_gate_indices_list
         ), "The qubits used in the gates are not correct"
 
     @pytest.mark.qpu
     def test_qubit_routing(self):
-
         for i, case in enumerate(self.list_of_cases):
             print("Test case {} out of {}:".format(i + 1, len(self.list_of_cases)))
             self.__compare_results(case, p=i % 4 + 1)
             print("Test passed for case: {}".format(case.values_input()))
 
 
 if __name__ == "__main__":
```

### Comparing `openqaoa-0.1.2/tests/test_converters.py` & `openqaoa-0.1.3/tests/test_converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def test_unbalanced_penalizations(self):
         """
         Test the equality and inequality constraints are encoded in the QUBO
         model using the unblanaced penalization method.
 
         """
-        weights = [3.85, 0.25, -1.15]
+        weights = [4.25, -0.95, -2.45]
         # Creating a basic docplex model
         mdl = Model("Test inequal")  # Docplex model
         num_z = 2  # Number of variables
         z = mdl.binary_var_list(num_z, name="Z")  # docplex variables
         objective = mdl.sum(z) - 2 * z[0] + z[1] * z[0] + 5  # objective function
         # Adding constraints
         mdl.add_constraint(mdl.sum(z[i] for i in range(num_z)) == 1)
```

### Comparing `openqaoa-0.1.2/tests/test_custom_mixer.py` & `openqaoa-0.1.3/tests/test_custom_mixer.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_derivative.py` & `openqaoa-0.1.3/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_gates.py` & `openqaoa-0.1.3/tests/test_gates.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,401 +24,414 @@
     RYY,
     RZZ,
     RZX,
     CPHASE,
     RiSWAP,
 )
 from openqaoa.qaoa_components.ansatz_constructor.rotationangle import RotationAngle
+from openqaoa_braket.backends.gates_braket import BraketGateApplicator
+from openqaoa_qiskit.backends.gates_qiskit import QiskitGateApplicator
+from openqaoa_pyquil.backends.gates_pyquil import PyquilGateApplicator
 
 
 class TestingGate(unittest.TestCase):
+    
+    def setUp(self):
+        
+        self.braket_gate_applicator = BraketGateApplicator()
+        self.qiskit_gate_applicator = QiskitGateApplicator()
+        self.pyquil_gate_applicator = PyquilGateApplicator()
+    
     def test_braket_gates_1q(self):
+        
+        # Braket Gate Applicator
+        gate_applicator = self.braket_gate_applicator
 
         # One Qubit Gate Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], FreeParameter("test_angle"))
-
+        
         empty_circuit = Circuit()
-        llgate = RY()
-        output_circuit = llgate.apply_braket_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RY(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.Ry.ry(0, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = RX()
-        output_circuit = llgate.apply_braket_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RX(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.Rx.rx(0, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = RZ()
-        output_circuit = llgate.apply_braket_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RZ(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.Rz.rz(0, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
     def test_braket_gates_2q(self):
+        
+        # Braket Gate Applicator
+        gate_applicator = self.braket_gate_applicator
 
         # Two Qubit Gate Tests
         empty_circuit = Circuit()
-        llgate = CZ()
-        output_circuit = llgate.apply_braket_gate([0, 1], empty_circuit)
+        llgate = CZ(gate_applicator, 0, 1)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = Circuit()
         test_circuit += braketgates.CZ.cz(0, 1)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = CX(mode="CX")
-        output_circuit = llgate.apply_braket_gate([0, 1], empty_circuit)
+        llgate = CX(gate_applicator, 0, 1)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = Circuit()
         test_circuit += braketgates.CNot.cnot(0, 1)
 
         self.assertEqual(test_circuit, output_circuit)
 
     def test_braket_gates_2q_w_gates(self):
+        
+        # Braket Gate Applicator
+        gate_applicator = self.braket_gate_applicator
 
         # Two Qubit Gate with Angles Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], FreeParameter("test_angle"))
 
         empty_circuit = Circuit()
-        llgate = RXX()
-        output_circuit = llgate.apply_braket_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RXX(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.XX.xx(0, 1, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = RYY()
-        output_circuit = llgate.apply_braket_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RYY(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.YY.yy(0, 1, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = RZZ()
-        output_circuit = llgate.apply_braket_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RZZ(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.ZZ.zz(0, 1, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = CPHASE()
-        output_circuit = llgate.apply_braket_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = CPHASE(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.CPhaseShift.cphaseshift(0, 1, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
         empty_circuit = Circuit()
-        llgate = RiSWAP()
-        output_circuit = llgate.apply_braket_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RiSWAP(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
         output_circuit = output_circuit.make_bound_circuit({"test_angle": np.pi})
 
         test_circuit = Circuit()
         test_circuit += braketgates.XY.xy(0, 1, np.pi)
 
         self.assertEqual(test_circuit, output_circuit)
 
     def test_ibm_gates_1q(self):
+        
+        # Qiskit Gate Applicator
+        gate_applicator = self.qiskit_gate_applicator
 
         # One Qubit Gate Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], np.pi)
 
         empty_circuit = QuantumCircuit(1)
-        llgate = RY()
-        output_circuit = llgate.apply_ibm_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RY(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(1)
         test_circuit.ry(np.pi, 0)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(1)
-        llgate = RX()
-        output_circuit = llgate.apply_ibm_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RX(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(1)
         test_circuit.rx(np.pi, 0)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(1)
-        llgate = RZ()
-        output_circuit = llgate.apply_ibm_gate(0, rotation_angle_obj, empty_circuit)
+        llgate = RZ(gate_applicator, 0, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(1)
         test_circuit.rz(np.pi, 0)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
     def test_ibm_gates_2q(self):
+        
+        # Qiskit Gate Applicator
+        gate_applicator = self.qiskit_gate_applicator
 
         # Two Qubit Gate Tests
         empty_circuit = QuantumCircuit(2)
-        llgate = CZ()
-        output_circuit = llgate.apply_ibm_gate([0, 1], empty_circuit)
+        llgate = CZ(gate_applicator, 0, 1)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.cz(0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(2)
-        llgate = CX(mode="CX")
-        output_circuit = llgate.apply_ibm_gate([0, 1], empty_circuit)
+        llgate = CX(gate_applicator, 0, 1)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.cx(0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
-        empty_circuit = QuantumCircuit(2)
-        llgate = CX(mode="CZ")
-        output_circuit = llgate.apply_ibm_gate([0, 1], empty_circuit)
-
-        test_circuit = QuantumCircuit(2)
-        test_circuit.ry(np.pi / 2, 1)
-        test_circuit.rx(np.pi, 1)
-        test_circuit.cz(0, 1)
-        test_circuit.ry(np.pi / 2, 1)
-        test_circuit.rx(np.pi, 1)
-
-        self.assertEqual(
-            test_circuit.to_instruction().definition,
-            output_circuit.to_instruction().definition,
-        )
+#         empty_circuit = QuantumCircuit(2)
+#         llgate = CX(gate_applicator)
+#         output_circuit = llgate.apply_ibm_gate([0, 1], empty_circuit)
+
+#         test_circuit = QuantumCircuit(2)
+#         test_circuit.ry(np.pi / 2, 1)
+#         test_circuit.rx(np.pi, 1)
+#         test_circuit.cz(0, 1)
+#         test_circuit.ry(np.pi / 2, 1)
+#         test_circuit.rx(np.pi, 1)
+
+#         self.assertEqual(
+#             test_circuit.to_instruction().definition,
+#             output_circuit.to_instruction().definition,
+#         )
 
     def test_ibm_gates_2q_w_gates(self):
+        
+        # Qiskit Gate Applicator
+        gate_applicator = self.qiskit_gate_applicator
 
         # Two Qubit Gate with Angles Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], np.pi)
 
         empty_circuit = QuantumCircuit(2)
-        llgate = RXX()
-        output_circuit = llgate.apply_ibm_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RXX(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.rxx(np.pi, 0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(2)
-        llgate = RYY()
-        output_circuit = llgate.apply_ibm_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RYY(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.ryy(np.pi, 0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(2)
-        llgate = RZZ()
-        output_circuit = llgate.apply_ibm_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RZZ(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.rzz(np.pi, 0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(2)
-        llgate = RZX()
-        output_circuit = llgate.apply_ibm_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = RZX(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.rzx(np.pi, 0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
         empty_circuit = QuantumCircuit(2)
-        llgate = CPHASE()
-        output_circuit = llgate.apply_ibm_gate(
-            [0, 1], rotation_angle_obj, empty_circuit
-        )
+        llgate = CPHASE(gate_applicator, 0, 1, rotation_angle_obj)
+        output_circuit = llgate.apply_gate(empty_circuit)
 
         test_circuit = QuantumCircuit(2)
         test_circuit.crz(np.pi, 0, 1)
 
         self.assertEqual(
             test_circuit.to_instruction().definition,
             output_circuit.to_instruction().definition,
         )
 
     def test_pyquil_gates_1q(self):
+        
+        # Pyquil Gate Applicator
+        gate_applicator = self.pyquil_gate_applicator
 
         # One Qubit Gate Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], np.pi)
 
         empty_program = Program()
-        llgate = RY()
-        output_program = llgate.apply_pyquil_gate(0, rotation_angle_obj, empty_program)
+        llgate = RY(gate_applicator, 0, rotation_angle_obj)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_RY(np.pi, 0))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
         empty_program = Program()
-        llgate = RX()
-        output_program = llgate.apply_pyquil_gate(0, rotation_angle_obj, empty_program)
+        llgate = RX(gate_applicator, 0, rotation_angle_obj)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_RX(np.pi, 0))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
         empty_program = Program()
-        llgate = RZ()
-        output_program = llgate.apply_pyquil_gate(0, rotation_angle_obj, empty_program)
+        llgate = RZ(gate_applicator, 0, rotation_angle_obj)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_RZ(np.pi, 0))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
     def test_pyquil_gates_2q(self):
+        
+        # Pyquil Gate Applicator
+        gate_applicator = self.pyquil_gate_applicator
 
         # Two Qubit Gate Tests
         empty_program = Program()
-        llgate = CZ()
-        output_program = llgate.apply_pyquil_gate([0, 1], empty_program)
+        llgate = CZ(gate_applicator, 0, 1)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_CZ(0, 1))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
         empty_program = Program()
-        llgate = CX()
-        output_program = llgate.apply_pyquil_gate([0, 1], empty_program)
+        llgate = CX(gate_applicator, 0, 1)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_CX(0, 1))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
     def test_pyquil_gates_2q_w_gates(self):
+        
+        # Pyquil Gate Applicator
+        gate_applicator = self.pyquil_gate_applicator
 
         # Two Qubit Gate with Angles Tests
         rotation_angle_obj = RotationAngle(lambda x: x, [], np.pi)
 
         empty_program = Program()
-        llgate = CPHASE()
-        output_program = llgate.apply_pyquil_gate(
-            [0, 1], rotation_angle_obj, empty_program
-        )
+        llgate = CPHASE(gate_applicator, 0, 1, rotation_angle_obj)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_CPHASE(np.pi, 0, 1))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
             instr.name for instr in test_program if type(instr) == quilbase.Gate
         ]
         self.assertEqual(output_gate_names, test_gate_names)
 
         empty_program = Program()
-        llgate = RiSWAP()
-        output_program = llgate.apply_pyquil_gate(
-            [0, 1], rotation_angle_obj, empty_program
-        )
+        llgate = RiSWAP(gate_applicator, 0, 1, rotation_angle_obj)
+        output_program = llgate.apply_gate(empty_program)
 
         test_program = Program().inst(p_XY(np.pi, 0, 1))
 
         output_gate_names = [
             instr.name for instr in output_program if type(instr) == quilbase.Gate
         ]
         test_gate_names = [
```

### Comparing `openqaoa-0.1.2/tests/test_imports.py` & `openqaoa-0.1.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_logger.py` & `openqaoa-0.1.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_notebooks.py` & `openqaoa-0.1.3/tests/test_notebooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Tests to run the notebooks. They work by converting the notebooks
 to a python script via nbconvert and then running the resulting .py file.
 """
 import nbformat
 from nbconvert.preprocessors import ExecutePreprocessor
 import pytest
 
-import sys, os
+import sys
+import os
 
 myPath = os.path.dirname(os.path.abspath(__file__))
 sys.path.insert(0, myPath + "/../")
 
 
 def notebook_test_function(name):
-
     with open(name, encoding="utf-8") as f:
         nb = nbformat.read(f, as_version=4)
 
     ep = ExecutePreprocessor(timeout=600, kernel_name="env")
 
     ep.preprocess(nb)
 
@@ -71,20 +71,28 @@
     notebook_test_function("./examples/10_workflows_on_Amazon_braket.ipynb")
 
 
 def test_11_Mixer_example():
     notebook_test_function("./examples/11_Mixer_example.ipynb")
 
 
+def test_13_optimizers():
+    notebook_test_function("./examples/13_optimizers.ipynb")
+
+
+@pytest.mark.qpu
+def test_14_benchmark():
+    notebook_test_function("./examples/14_qaoa_benchmark.ipynb")
+
+
 def test_X_dumping_data():
     notebook_test_function("./examples/X_dumping_data.ipynb")
 
 
-### Community Tutorials
-
+# Community Tutorials
 # @pytest.mark.notebook
 def test_tutorial_quantum_approximate_optimization_algorithm():
     notebook_test_function(
         "./examples/community_tutorials/01_tutorial_quantum_approximate_optimization_algorithm.ipynb"
     )
```

### Comparing `openqaoa-0.1.2/tests/test_operators.py` & `openqaoa-0.1.3/tests/test_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1252,10 +1252,68 @@
 
         # Check exception message
         self.assertEqual(
             "Hamiltonian only supports Linear and Quadratic terms",
             str(context.exception),
         )
 
+    def test_hamiltonian_dict(self):
+        """Test if the method produces
+        the correct dictionary corresponding to the Hamiltonian.
+
+        It creates a dictionary of the form
+        {(i, j): coeff} where i, j are the indices of the qubits if
+        argument `classical` is set true in the function otherwise,
+        produces a dictionary of the form {PauliOp}: coeff}
+        """
+
+        # TEST 1
+        # Define Hamiltonian attributes
+        terms = [[0, 1], [0, 2], [1, 2]]
+        coefficients = [1, 0.5, 0.5]
+        constant = 2
+
+        # Generate Hamiltonian
+        hamiltonian = Hamiltonian.classical_hamiltonian(terms, coefficients, constant)
+
+        # Generate dictionary
+        hamiltonian_dict = hamiltonian.hamiltonian_dict()
+
+        # Correct dictionary
+        correct_dict = {(0, 1): 1, (0, 2): 0.5, (1, 2): 0.5, (): 2}
+
+        # Test if dictionary was correctly computed
+        assert (
+            hamiltonian_dict == correct_dict
+        ), f"Hamiltonian dictionary did not yield correct dictionary"
+
+        # TEST 2
+        terms = [PauliOp("XX", (0, 1)), PauliOp("YY", (0, 2))]
+        coeffs = [1, 0.5]
+        constant = 0
+
+        # Generate Hamiltonian
+        hamiltonian = Hamiltonian(terms, coeffs, constant)
+
+        # Generate dictionaries
+        hamiltonian_dict_indices = hamiltonian.hamiltonian_dict(classical=True)
+        hamiltonian_dict_pauliop = hamiltonian.hamiltonian_dict(classical=False)
+
+        # Correct dictionaries
+        correct_dict_indices = {(0, 1): 1, (0, 2): 0.5, (): 0}
+        correct_dict_pauliop = {
+            PauliOp("XX", (0, 1)): 1,
+            PauliOp("YY", (0, 2)): 0.5,
+            (): 0,
+        }
+
+        assert (
+            hamiltonian_dict_indices == correct_dict_indices
+        ), "Hamiltonian dictionary did not yield correct dictionary"
+
+        assert (
+            hamiltonian_dict_pauliop == correct_dict_pauliop
+        ), "Hamiltonian dictionary did not yield correct dictionary"
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.2/tests/test_optimizers.py` & `openqaoa-0.1.3/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_optimizers_pennylane.py` & `openqaoa-0.1.3/tests/test_optimizers_pennylane.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_parameters.py` & `openqaoa-0.1.3/tests/test_parameters.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from scipy.fft import dst, dct
 
 from openqaoa.qaoa_components import *
 from openqaoa.utilities import X_mixer_hamiltonian, XY_mixer_hamiltonian
 from openqaoa.qaoa_components.ansatz_constructor.gatemaplabel import GateMapType
 from openqaoa.qaoa_components.variational_parameters.variational_params_factory import (
     PARAMS_CLASSES_MAPPER,
+    VARIATIONAL_PARAMS_DICT_KEYS,
 )
 
 register = [0, 1, 2]
 terms = [[0, 1], [2], [0, 2]]
 weights = [1, 0.5, -2.0]
 
 terms_wo_bias = [[0, 1], [1, 2]]
@@ -580,99 +581,161 @@
                 init_type="rand",
                 q=1,
                 total_annealing_time=1,
             )
 
             self.assertEqual(variate_params.__str__(), variate_params.__repr__())
 
-    # # Plot Tests
+    def test_qaoa_variational_params_asdict(self):
 
-    # def test_StandardParams_plot(self):
+        p = 4
+        q = 2
 
-    #     register_wo_bias = [0, 1, 2]
-    #     terms_wo_bias = [[0, 1], [0, 2]]
-    #     weights_wo_bias = [1, -2.0]
-
-    #     p = 5
-    #     hyperparams = HyperParams(terms,weights,register,p)
-    #     params = StandardParams.linear_ramp_from_hamiltonian(hyperparams)
-    #     fig, ax = plt.subplots()
-    #     params.plot(ax=ax)
-    #     # plt.show()
-
-    #     p = 8
-    #     hyperparams = HyperParams(terms,weights,register,p)
-    #     params = StandardParams(hyperparams,([0.1]*p, [0.2]*p))
-    #     fig, ax = plt.subplots()
-    #     params.plot(ax=ax)
-    #     # plt.show()
-
-    #     p = 2
-    #     hyperparams = HyperParams(terms_wo_bias,weights_wo_bias,register_wo_bias,p)
-    #     params = StandardParams(hyperparams,([5]*p, [10]*p))
-    #     fig, ax = plt.subplots()
-    #     params.plot(ax=ax)
-    #     # plt.show()
-
-    # def test_ExtendedParams_plot(self):
-
-    #     register_wo_bias = [0, 1, 2]
-    #     terms_wo_bias = [[0, 1], [0, 2]]
-    #     weights_wo_bias = [1, -2.0]
-
-    #     p = 5
-    #     hyperparams = HyperParams(terms_wo_bias,weights_wo_bias,register_wo_bias,p)
-    #     params = ExtendedParams.linear_ramp_from_hamiltonian(hyperparams, p)
-    #     fig, ax = plt.subplots()
-    #     params.plot(ax=ax)
-    #     # plt.show()
-
-    #     p = 8
-    #     hyperparams = HyperParams(terms_wo_bias,weights_wo_bias,register_wo_bias,p)
-    #     params = ExtendedParams(hyperparams,
-    #                             ([0.1] * p*len(register),
-    #                             [],
-    #                             [0.2] * p*len(weights_wo_bias)))
-    #     fig, ax = plt.subplots()
-    #     params.plot(ax=ax)
-    #     # plt.show()
-
-    # def test_extended_get_constraints(self):
-    #     register = [0,1,2,3]
-    #     terms = [[0, 1], [1, 2], [2, 3], [3, 0]]
-    #     weights = [0.1, 0.3, 0.5, -0.7]
-    #     p = 2
-
-    #     hyperparams = HyperParams(terms,weights,register,p)
-    #     params = ExtendedParams.linear_ramp_from_hamiltonian(hyperparams)
-
-    #     actual_constraints = params.get_constraints()
-
-    #     expected_constraints = [(0, 2 * np.pi), (0, 2 * np.pi),
-    #                             (0, 2 * np.pi), (0, 2 * np.pi),
-    #                             (0, 2 * np.pi), (0, 2 * np.pi),
-    #                             (0, 2 * np.pi), (0, 2 * np.pi),
-    #                             (0, 2 * np.pi / weights[0]),
-    #                             (0, 2 * np.pi / weights[1]),
-    #                             (0, 2 * np.pi / weights[2]),
-    #                             (0, 2 * np.pi / weights[3]),
-    #                             (0, 2 * np.pi / weights[0]),
-    #                             (0, 2 * np.pi / weights[1]),
-    #                             (0, 2 * np.pi / weights[2]),
-    #                             (0, 2 * np.pi / weights[3])]
-
-    #     assert(np.allclose(expected_constraints, actual_constraints))
-
-    #     cost_function = QAOACostVector(params)
-    #     np.random.seed(0)
-    #     random_angles = np.random.uniform(-100, 100, size=len(params.raw()))
-    #     value = cost_function(random_angles)
-
-    #     normalised_angles = [random_angles[i] % actual_constraints[i][1]
-    #                         for i in range(len(params.raw()))]
-    #     normalised_value = cost_function(normalised_angles)
+        number_of_params = {
+            "standard": {"betas": p, "gammas": p},
+            "standard_w_bias": {"betas": p, "gammas_singles": p, "gammas_pairs": p},
+            "extended": {
+                "betas_singles": len(register) * p,
+                "betas_pairs": 0,
+                "gammas_singles": sum([1 for term in terms if len(term) == 1]) * p,
+                "gammas_pairs": sum([1 for term in terms if len(term) == 2]) * p,
+            },
+            "fourier": {"v": q, "u": q},
+            "fourier_extended": {
+                "v_singles": len(register) * q,
+                "v_pairs": 0,
+                "u_singles": sum([1 for term in terms if len(term) == 1]) * q,
+                "u_pairs": sum([1 for term in terms if len(term) == 2]) * q,
+            },
+            "fourier_w_bias": {"v": q, "u_singles": q, "u_pairs": q},
+            "annealing": {"schedule": p},
+        }
 
-    #     assert(np.allclose(value, normalised_value))
+        qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=p)
+
+        for each_key_value in PARAMS_CLASSES_MAPPER.keys():
+
+            # create the variational params object
+            variate_params = create_qaoa_variational_params(
+                qaoa_descriptor,
+                params_type=each_key_value,
+                init_type="rand",
+                q=q,
+                total_annealing_time=2,
+            )
+
+            # get the dict and check that it is a dict
+            variate_params_dict = variate_params.asdict()
+            assert isinstance(
+                variate_params_dict, dict
+            ), f"asdict() should return a dict, it did not for type: '{each_key_value}'."
+
+            # check that the keys are correct
+            expected_keys = VARIATIONAL_PARAMS_DICT_KEYS[each_key_value]
+            for key in [
+                "q",
+                "total_annealing_time",
+            ]:  # from expected_keys, remove the "q" and "total_annealing_time" keys, if there are any
+                if key in expected_keys:
+                    expected_keys.remove(key)
+            assert set(variate_params_dict.keys()) == set(
+                expected_keys
+            ), f"asdict() should return a dict with the correct keys, it did not for type: '{each_key_value}'."
+
+            # check that the number of values is correct
+            for key, value in variate_params_dict.items():
+                assert (
+                    value.size == number_of_params[each_key_value][key]
+                ), f"asdict() should return a dict with the correct number of values, it did not for type: '{each_key_value}'. \
+                \n Expected {number_of_params[each_key_value][key]} values for key '{key}', but got {value.size} values."
+
+            # check that the values are correct
+            list_params_raw = []
+            for key, value in variate_params_dict.items():
+                list_params_raw += value.flatten().tolist()
+
+            assert np.allclose(
+                list_params_raw, variate_params.raw().tolist()
+            ), f"asdict() should return a dict with the correct values, it did not for type: '{each_key_value}'."
+
+    def test_qaoa_variational_params_update_from_dict(self):
+
+        qaoa_descriptor = QAOADescriptor(cost_hamiltonian, mixer_hamiltonian, p=2)
+
+        for each_key_value in PARAMS_CLASSES_MAPPER.keys():
+            variate_params = create_qaoa_variational_params(
+                qaoa_descriptor,
+                params_type=each_key_value,
+                init_type="rand",
+                q=1,
+                total_annealing_time=1,
+            )
+
+            # get the params as a dict
+            variate_params_dict = variate_params.asdict()
+
+            # create a new dict with random values
+            new_dict = {
+                k: np.random.rand(*v.shape) for k, v in variate_params_dict.items()
+            }
+
+            # update the variational params object with the new dict
+            variate_params.update_from_dict(new_dict)
+
+            # check that the values are correct
+            for key, value in variate_params.asdict().items():
+                assert np.allclose(
+                    value, new_dict[key]
+                ), f"update_from_dict() should update the values correctly, it did not for type: '{each_key_value}'."
+
+            # check that if we pass in a dict with the wrong keys, an error is raised
+            wrong_dict = new_dict
+            wrong_dict["wrong_key"] = np.random.rand(1)
+            error = False
+            try:
+                variate_params.update_from_dict(wrong_dict)
+            except:
+                error = True
+            assert (
+                error
+            ), f"update_from_dict() should raise an error if the dict has the wrong keys, it did not for type: '{each_key_value}'."
+
+            # check that if we pass in a dict with more values than expected, an error is raised
+            wrong_dict = new_dict
+            wrong_dict.pop("wrong_key")
+            for key in wrong_dict.keys():
+                wrong_dict[key] = np.append(wrong_dict[key], np.random.rand(1))
+            error = False
+            try:
+                variate_params.update_from_dict(wrong_dict)
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"update_from_dict() should raise an error if the dict has more values than expected, it did not for type: '{each_key_value}'."
+
+            # check that if we pass in a dict with less values than expected, an error is raised
+            wrong_dict = new_dict
+            for key in wrong_dict.keys():
+                wrong_dict[key] = wrong_dict[key][:-2]
+            error = False
+            try:
+                variate_params.update_from_dict(wrong_dict)
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"update_from_dict() should raise an error if the dict has less values than expected, it did not for type: '{each_key_value}'."
+
+            # check that if we pass something that is not a dict, an error is raised
+            error = False
+            try:
+                variate_params.update_from_dict(1)
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"update_from_dict() should raise an error if the input is not a dict, it did not for type: '{each_key_value}'."
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.2/tests/test_parameters_plots.py` & `openqaoa-0.1.3/tests/test_parameters_plots.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_problems.py` & `openqaoa-0.1.3/tests/test_problems.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     QUBO,
     TSP,
     Knapsack,
     ShortestPath,
     SlackFreeKnapsack,
     MaximumCut,
     MinimumVertexCover,
+    VRP,
+    PortfolioOptimization,
+    MIS,
+    BinPacking,
 )
 from openqaoa.utilities import convert2serialize
 from openqaoa.problems.helper_functions import create_problem_from_dict
 
 
 def terms_list_equality(terms_list1, terms_list2):
     """
@@ -26,16 +30,33 @@
     else:
         for term1, term2 in zip(terms_list1, terms_list2):
             bool = True if (term1 == term2 or term1 == term2[::-1]) else False
 
     return bool
 
 
-class TestProblem(unittest.TestCase):
+def terms_list_isclose(terms_list1, terms_list2):
+    """
+    Check if the distance between two terms list
+    where the order of edges do not matter.
+    """
+    if len(terms_list1) != len(terms_list2):
+        bool = False
+    else:
+        for term1, term2 in zip(terms_list1, terms_list2):
+            bool = (
+                True
+                if np.isclose(term1, term2) or np.isclose(term1, term2[::-1])
+                else False
+            )
+
+    return bool
+
 
+class TestProblem(unittest.TestCase):
     # TESTING QUBO CLASS METHODS
     def test_qubo_terms_and_weight_same_size(self):
         """
         Test that creating a QUBO problem with invalid terms and weights
         sizes raises an exception and check the constant is detected correctly
         """
         n = 2
@@ -785,15 +806,14 @@
             -10.361716714885624,
             -10.424148382787205,
             -9.797225258452029,
             -11.038545614372802,
         ]
         expected_constant = 62.51983851122417
         tsp_qubo = TSP(city_coordinates).qubo
-        print(tsp_qubo.weights)
         self.assertTrue(terms_list_equality(expected_terms, tsp_qubo.terms))
         self.assertEqual(expected_weights, tsp_qubo.weights)
         self.assertEqual(expected_constant, tsp_qubo.constant)
 
     def test_tsp_random_instance(self):
         """Testing the random_instance method of the TSP problem class"""
         rng = np.random.default_rng(1234)
@@ -885,24 +905,24 @@
         distance_matrix = [[1, 2.3], [-2, 3]]
         with self.assertRaises(ValueError) as e:
             TSP(distance_matrix=distance_matrix)
         self.assertEqual("Distances should be positive", str(e.exception))
 
         # Graph type-check
         G = nx.complete_graph(5)
-        for (u, v) in G.edges():
+        for u, v in G.edges():
             G[u][v]["weight"] = "a"
 
         with self.assertRaises(TypeError) as e:
             TSP(G=G)
         self.assertEqual(
             "The edge weights must be of type float or int", str(e.exception)
         )
 
-        for (u, v) in G.edges():
+        for u, v in G.edges():
             G[u][v]["weight"] = -2.0
 
         with self.assertRaises(ValueError) as e:
             TSP(G=G)
         self.assertEqual("Edge weights should be positive", str(e.exception))
 
     # TESTING SHORTESTPATH PROBLEM CLASS
@@ -963,25 +983,25 @@
             2.5,
         ]
         sp_qubo_terms = [[1, 2], [2, 3], [0, 1], [1, 3], [0, 3], [0], [1], [2], [3]]
         sp_qubo_weights = [0.5, 0.5, -1.0, 0.5, -1.0, -0.5, -0.5, -0.5, -0.5]
         sp_qubo_constant = 2.5
 
         gr = nx.generators.fast_gnp_random_graph(3, 1, seed=1234)
-        for (u, v) in gr.edges():
+        for u, v in gr.edges():
             gr.edges[u, v]["weight"] = 1
         for w in gr.nodes():
             gr.nodes[w]["weight"] = 1
         source, dest = 0, 2
         sp = ShortestPath(gr, source, dest)
         n_variables = sp.G.number_of_nodes() + sp.G.number_of_edges() - 2
         bin_terms, bin_weights = sp.terms_and_weights()
         terms, weights = QUBO.convert_qubo_to_ising(n_variables, bin_terms, bin_weights)
         qubo = sp.qubo
-        print(terms)
+
         self.assertTrue(terms_list_equality(bin_terms, sp_terms))
         self.assertEqual(list(bin_weights), sp_weights)
         self.assertTrue(terms_list_equality(terms, conv_sp_terms))
         self.assertEqual(list(weights), conv_sp_weights)
         self.assertTrue(terms_list_equality(sp_qubo_terms, qubo.terms))
         self.assertEqual(sp_qubo_weights, qubo.weights)
         self.assertEqual(sp_qubo_constant, qubo.constant)
@@ -989,22 +1009,22 @@
     def test_shortestpath_random_instance(self):
         """Test random instance method of Shortest Path problem class"""
         sp_rand_terms = [[1, 2], [2, 3], [0, 1], [1, 3], [0, 3], [0], [1], [2], [3]]
         sp_rand_weights = [0.5, 0.5, -1.0, 0.5, -1.0, -0.5, -0.5, -0.5, -0.5]
         sp_rand_constant = 2.5
 
         gr = nx.generators.fast_gnp_random_graph(3, 1, seed=1234)
-        for (u, v) in gr.edges():
+        for u, v in gr.edges():
             gr.edges[u, v]["weight"] = 1.0
         for w in gr.nodes():
             gr.nodes[w]["weight"] = 1.0
         sp_prob = ShortestPath.random_instance(
             n_nodes=3, edge_probability=1, seed=1234, source=0, dest=2
         ).qubo
-        print(sp_prob.terms)
+
         self.assertTrue(terms_list_equality(sp_rand_terms, sp_prob.terms))
         self.assertEqual(sp_rand_weights, sp_prob.weights)
         self.assertEqual(sp_rand_constant, sp_prob.constant)
 
         self.assertEqual(sp_prob.terms, ShortestPath(gr, 0, 2).qubo.terms)
         self.assertEqual(sp_prob.weights, ShortestPath(gr, 0, 2).qubo.weights)
         self.assertEqual(sp_prob.constant, ShortestPath(gr, 0, 2).qubo.constant)
@@ -1028,14 +1048,396 @@
             nx.set_node_attributes(G, values=node_dict, name="weight")
 
             shortest_path_problem = ShortestPath(G, 0, -1)
             shortest_path_qubo = shortest_path_problem.qubo
 
         self.assertRaises(Exception, test_assertion_fn)
 
+    # TESTING VRP PROBLEM CLASS
+
+    def test_vrp_terms_weights_constant(self):
+        """Testing VRP problem creation"""
+        pos = [[4, 1], [4, 4], [3, 3]]  # nodes position x, y
+        n_vehicles = 1
+        n_nodes = len(pos)
+        G = nx.Graph()
+        G.add_nodes_from(range(n_nodes))
+        for i in range(n_nodes - 1):
+            for j in range(i + 1, n_nodes):
+                r = np.sqrt((pos[i][0] - pos[j][0]) ** 2 + (pos[i][1] - pos[j][1]) ** 2)
+                G.add_weighted_edges_from([(i, j, r)])
+        vrp_qubo = VRP(G, pos, n_vehicles).qubo
+        expected_terms = [[0, 1], [0, 2], [1, 2], [0], [1], [2]]
+        expected_weights = [2.0, 2.0, 2.0, 6.5, 6.881966011250105, 7.292893218813452]
+        expected_constant = 21.32514076993644
+
+        self.assertTrue(terms_list_equality(expected_terms, vrp_qubo.terms))
+        self.assertEqual(expected_weights, vrp_qubo.weights)
+        self.assertEqual(expected_constant, vrp_qubo.constant)
+
+    def test_vrp_random_instance(self):
+        """Testing the random_instance method of the VRP problem class"""
+        seed = 1234
+        np.random.seed(seed)
+        n_nodes = 3
+        n_vehicles = 1
+        G = nx.Graph()
+        G.add_nodes_from(range(n_nodes))
+        pos = [[0, 0]]
+        pos += [list(2 * np.random.rand(2) - 1) for _ in range(n_nodes - 1)]
+        for i in range(n_nodes - 1):
+            for j in range(i + 1, n_nodes):
+                r = np.sqrt((pos[i][0] - pos[j][0]) ** 2 + (pos[i][1] - pos[j][1]) ** 2)
+                G.add_weighted_edges_from([(i, j, r)])
+
+        vrp_prob = VRP(G, pos, n_vehicles).qubo
+        vrp_prob_random = VRP.random_instance(
+            n_nodes=n_nodes, n_vehicles=n_vehicles, seed=seed
+        ).qubo
+
+        self.assertTrue(terms_list_equality(vrp_prob_random.terms, vrp_prob.terms))
+        self.assertEqual(vrp_prob_random.weights, vrp_prob.weights)
+        self.assertEqual(vrp_prob_random.constant, vrp_prob.constant)
+
+    def test_vrp_random_instance_unbalanced(self):
+        """
+        Testing the random_instance method of the VRP problem class using the
+        unbalanced penalization method
+        """
+        seed = 1234
+        np.random.seed(seed)
+        n_nodes = 8
+        n_vehicles = 2
+        n_vars = n_nodes * (n_nodes - 1) // 2
+
+        vrp_prob_random = VRP.random_instance(
+            n_nodes=n_nodes,
+            n_vehicles=n_vehicles,
+            seed=seed,
+            method="unbalanced",
+            penalty=3 * [0.1],
+        ).qubo
+
+        self.assertTrue(vrp_prob_random.n == n_vars)
+        self.assertTrue(vrp_prob_random.weights[0] == 0.05)
+        self.assertTrue(vrp_prob_random.weights[-1] == -0.688413325464513)
+        self.assertTrue(vrp_prob_random.terms[0] == [0, 1])
+        self.assertTrue(vrp_prob_random.terms[-1] == [27])
+
+    def test_vrp_plot(self):
+        """
+        Testing the random_instance method of the VRP problem class using the
+        unbalanced penalization method
+        """
+        import matplotlib.pyplot as plt
+
+        seed = 1234
+        np.random.seed(seed)
+        n_nodes = 8
+        n_vehicles = 2
+
+        vrp_prob_random = VRP.random_instance(
+            n_nodes=n_nodes,
+            n_vehicles=n_vehicles,
+            seed=seed
+        )
+        vrp_sol = vrp_prob_random.classical_solution()
+        vrp_sol_str = vrp_prob_random.classical_solution(string=True)
+
+        self.assertTrue(isinstance(vrp_prob_random.plot_solution(vrp_sol), plt.Figure))
+        self.assertTrue(isinstance(vrp_prob_random.plot_solution(vrp_sol_str), plt.Figure))
+
+    def test_vrp_type_checking(self):
+        """
+        Checks if the type-checking returns the right error.
+        """
+        # Wrong method is called
+        with self.assertRaises(ValueError) as e:
+            VRP.random_instance(n_nodes=6, n_vehicles=2, method="method")
+        self.assertEqual(
+            "The method 'method' is not valid.",
+            str(e.exception),
+        )
+        # Penalization terms in unblanced method is not equal to three
+        with self.assertRaises(ValueError) as e:
+            VRP.random_instance(
+                n_nodes=6, n_vehicles=2, method="unbalanced", penalty=[0.1]
+            )
+        self.assertEqual(
+            "The penalty must have 3 parameters [lambda_0, lambda_1, lambda_2]",
+            str(e.exception),
+        )
+
+        # paths with an unfeasible solution
+        with self.assertRaises(ValueError) as e:
+            vrp = VRP.random_instance(n_nodes=6, n_vehicles=2, seed=1234)
+            sol = vrp.classical_solution()
+            sol["x_0_1"] = (
+                sol["x_0_1"] + 1
+            ) % 2  # Changing one value in the solution to make it an unfeasible solution
+            vrp.paths_subtours(sol)
+        self.assertEqual(
+            "Solution provided does not fulfill all the path conditions.",
+            str(e.exception),
+        )
+        # subtours with an unfeasible direction (broke subtour)
+        with self.assertRaises(ValueError) as e:
+            vrp = VRP.random_instance(
+                n_nodes=10, n_vehicles=2, subtours=[[]], seed=1234
+            )
+            sol = vrp.classical_solution()
+            sol["x_1_2"] = (
+                sol["x_1_2"] + 1
+            ) % 2  # Changing one value in the solution to make it an unfeasible solution
+            vrp.paths_subtours(sol)
+        self.assertEqual(
+            "The subtours in the solution are broken.",
+            str(e.exception),
+        )
+        # Test unfeasible problem does not return classical solution
+        with self.assertRaises(ValueError) as e:
+            vrp = VRP.random_instance(n_nodes=3, n_vehicles=3, seed=1234)
+            sol = vrp.classical_solution()
+            vrp.paths_subtours(sol)
+        self.assertEqual(
+            "Solution not found: integer infeasible.",
+            str(e.exception),
+        )
+        # Test wrong graph input
+        with self.assertRaises(TypeError) as e:
+            G = [[0, 1, 2], [1, 2, 3]]
+            vrp = VRP(G, pos=[[0, 1], [1, 2]], n_vehicles=2)
+        self.assertEqual(
+            "Input problem graph must be a networkx Graph.",
+            str(e.exception),
+        )
+        # Test different size between graph nodes and x, y positions in pos
+        with self.assertRaises(ValueError) as e:
+            G = nx.Graph()
+            G.add_nodes_from(range(3))
+            vrp = VRP(G, pos=[[0, 1], [1, 2]], n_vehicles=2)
+        self.assertEqual(
+            "The number of nodes in G is 3 while the x, y coordinates in pos is 2",
+            str(e.exception),
+        )
+        # Test different size between colors and number of vehicles
+        with self.assertRaises(ValueError) as e:
+            seed = 1234
+            vrp = VRP.random_instance(n_nodes=6, n_vehicles=2, seed=seed)
+            vrp.plot_solution(vrp.classical_solution(), colors=["tab:blue"])
+        self.assertEqual(
+            "The length of colors 1 and the number of vehicles 2 do not match",
+            str(e.exception),
+        )
+
+    # TESTING PORTFOLIO OPTIMIZATION PROBLEM CLASS
+
+    def test_portfoliooptimization_terms_weights_constant(self):
+        """Test terms,weights,constant of QUBO generated by Portfolio Optimization class"""
+
+        po_terms = [[0, 1], [0, 2], [1, 2], [0], [1], [2]]
+        po_weights = [0.505, 0.505, 0.505, 0.535, 0.535, 0.535]
+        po_constant = 0.8799999999999999
+
+        mu = [0.1, 0.1, 0.1]
+        sigma = [[0.01, 0.01, 0.01], [0.01, 0.01, 0.01], [0.01, 0.01, 0.01]]
+        risk_factor = 0.1
+        budget = 2
+        penalty = 1
+
+        qubo = PortfolioOptimization(mu, sigma, risk_factor, budget, penalty).qubo
+        terms, weights = qubo.terms, qubo.weights
+        constant = qubo.constant
+
+        self.assertEqual(weights, po_weights)
+        self.assertEqual(terms, po_terms)
+        self.assertEqual(po_constant, constant)
+
+    def test_portfoliooptimization_random_instance(self):
+        """Test random instance method of Portfolio Optimization problem class"""
+        seed = 1234
+        np.random.seed(seed)
+        num_assets = 3
+        risk_factor = 0.1
+        budget = 2
+        penalty = 1
+        mu_bounds = [-0.1, 0.1]
+        sigma_bounds = [-0.01, 0.01]
+        mu = [
+            (mu_bounds[1] - mu_bounds[0]) * np.random.rand() + mu_bounds[0]
+            for _ in range(num_assets)
+        ]
+        sigma = [[0 for i in range(num_assets)] for j in range(num_assets)]
+        for i in range(num_assets):
+            for j in range(num_assets):
+                sigma[i][j] = (
+                    sigma_bounds[1] - sigma_bounds[0]
+                ) * np.random.rand() + sigma_bounds[0]
+
+        qubo = PortfolioOptimization(mu, sigma, risk_factor, budget, penalty).qubo
+
+        qubo_random = PortfolioOptimization.random_instance(
+            mu_bounds=mu_bounds,
+            sigma_bounds=sigma_bounds,
+            risk_factor=risk_factor,
+            budget=budget,
+            seed=seed,
+            penalty=penalty,
+            num_assets=num_assets,
+        ).qubo
+        self.assertEqual(qubo.weights, qubo_random.weights)
+        self.assertEqual(qubo.terms, qubo_random.terms)
+        self.assertEqual(qubo.constant, qubo_random.constant)
+
+    def test_portfoliooptimization_classical_sol(self):
+        """Test the portfolio optimization set random instance method classical solution"""
+
+        seed = 1234
+        np.random.seed(seed)
+        po_sol = PortfolioOptimization.random_instance(
+            num_assets=10, seed=seed
+        ).classical_solution()
+
+        sol = {
+            "asset_0": 0,
+            "asset_1": 0,
+            "asset_2": 0,
+            "asset_3": 1,
+            "asset_4": 1,
+            "asset_5": 0,
+            "asset_6": 0,
+            "asset_7": 1,
+            "asset_8": 1,
+            "asset_9": 1,
+        }
+
+        self.assertEqual(po_sol, sol)
+
+    def test_portfoliooptimization_plot(self):
+        """Test portfolio optmization random instance method"""
+        import matplotlib.pyplot as plt
+
+        seed = 1234
+        porfolitooptimization_random_prob = PortfolioOptimization.random_instance(
+            num_assets=12, budget=8, seed=seed
+        )
+        sol = porfolitooptimization_random_prob.classical_solution()
+        figure = porfolitooptimization_random_prob.plot_solution(sol)
+        self.assertTrue(isinstance(figure, plt.Figure))
+        fig, ax = plt.subplots(figsize=(5, 5))
+        self.assertTrue(
+            porfolitooptimization_random_prob.plot_solution(sol, ax=ax) == None)
+
+    # TESTING MAXIMAL INDEPENDENT SET PROBLEM
+
+    def test_mis_terms_weights_constant(self):
+        """Test that MaximumCut creates a correct QUBO from the provided graph"""
+
+        gr = nx.generators.random_graphs.fast_gnp_random_graph(n=5, p=0.8, seed=1234)
+        gr_edges = [
+            [0, 3],
+            [0, 4],
+            [1, 2],
+            [1, 3],
+            [2, 4],
+            [3, 4],
+            [0],
+            [1],
+            [2],
+            [3],
+            [4],
+        ]
+        gr_weights = [0.5, 0.5, 0.5, 0.5, 0.5, 0.5, -0.5, -0.5, -0.5, -1.0, -1.0]
+
+        mis_prob_qubo = MIS(gr).qubo
+
+        self.assertTrue(terms_list_equality(gr_edges, mis_prob_qubo.terms))
+        self.assertEqual(gr_weights, mis_prob_qubo.weights)
+        self.assertEqual(0.5, mis_prob_qubo.constant)
+
+    def test_mis_random_problem(self):
+        """Test MaximumCut random instance method"""
+
+        seed = 1234
+        gr = nx.generators.random_graphs.fast_gnp_random_graph(n=10, p=0.8, seed=seed)
+        mis_manual_prob = MIS(gr).qubo
+
+        np.random.seed(1234)
+        mis_random_prob = MIS.random_instance(
+            n_nodes=10, edge_probability=0.8, seed=seed
+        ).qubo
+
+        self.assertTrue(
+            terms_list_equality(mis_manual_prob.terms, mis_random_prob.terms)
+        )
+        self.assertEqual(mis_manual_prob.weights, mis_random_prob.weights)
+        self.assertEqual(mis_manual_prob.constant, mis_random_prob.constant)
+
+    def test_mis_type_checking(self):
+        """
+        Checks if the type-checking returns the right error.
+        """
+
+        # graph type-check
+        graph_list = [(1, 2), {"node1": 1, "node2": 2}, np.array([1, 2])]
+
+        for each_graph in graph_list:
+            with self.assertRaises(TypeError) as e:
+                MIS(G=each_graph)
+            self.assertEqual(
+                "Input problem graph must be a networkx Graph.", str(e.exception)
+            )
+
+    def test_mis_classical_sol(self):
+        """Test the maximal independent set random instance method classical solution"""
+
+        seed = 1234
+        np.random.seed(seed)
+        mis_sol = MIS.random_instance(
+            n_nodes=10, edge_probability=0.7, seed=seed
+        ).classical_solution()
+
+        sol = {
+            "x_0": 1,
+            "x_1": 1,
+            "x_2": 0,
+            "x_3": 0,
+            "x_4": 0,
+            "x_5": 0,
+            "x_6": 0,
+            "x_7": 0,
+            "x_8": 1,
+            "x_9": 0,
+        }
+
+        self.assertEqual(mis_sol, sol)
+
+    def test_mis_plot(self):
+        """Test maximal independent set random instance method"""
+        from matplotlib.pyplot import Figure
+
+        seed = 1234
+        mis_random_prob = MIS.random_instance(
+            n_nodes=10, edge_probability=0.7, seed=seed
+        )
+        sol = {
+            "x_0": 1,
+            "x_1": 1,
+            "x_2": 0,
+            "x_3": 0,
+            "x_4": 0,
+            "x_5": 0,
+            "x_6": 0,
+            "x_7": 0,
+            "x_8": 1,
+            "x_9": 0,
+        }
+        fig = mis_random_prob.plot_solution(sol)
+        self.assertTrue(isinstance(fig, Figure))
+
     def __generate_random_problems(self):
         problems_random_instances = {
             "tsp": TSP.random_instance(n_cities=randint(2, 15)),
             "number_partition": NumberPartition.random_instance(
                 n_numbers=randint(2, 15)
             ),
             "maximum_cut": MaximumCut.random_instance(
@@ -1047,26 +1449,33 @@
             ),
             "minimum_vertex_cover": MinimumVertexCover.random_instance(
                 n_nodes=randint(2, 15), edge_probability=random()
             ),
             "shortest_path": ShortestPath.random_instance(
                 n_nodes=randint(3, 15), edge_probability=random()
             ),
+            "vehicle_routing": VRP.random_instance(),
+            "maximal_independent_set": MIS.random_instance(
+                n_nodes=randint(3, 15), edge_probability=random()
+            ),
+            "bin_packing": BinPacking.random_instance(),
         }
         qubo_random_instances = {
             k: v.qubo for k, v in problems_random_instances.items()
         }
         qubo_random_instances["generic_qubo"] = QUBO.random_instance(randint(2, 15))
-
         return problems_random_instances, qubo_random_instances
 
     def test_problem_instance(self):
         """
         Test problem instance method of the QUBO class.
-        From the random instance of all the different problems, we generate the QUBO problem out of it and then we check if the problem instance attribute is correct, by comparing the keys of the problem instance with the expected keys.
+        From the random instance of all the different problems, we generate the
+        QUBO problem out of it and then we check if the problem instance
+        attribute is correct, by comparing the keys of the problem instance
+        with the expected keys.
         """
 
         _, qubos = self.__generate_random_problems()
 
         expected_keys = {
             "tsp": ["problem_type", "n_cities", "G", "A", "B"],
             "number_partition": ["problem_type", "numbers", "n_numbers"],
@@ -1085,14 +1494,37 @@
                 "weights",
                 "weight_capacity",
                 "penalty",
                 "n_items",
             ],
             "minimum_vertex_cover": ["problem_type", "G", "field", "penalty"],
             "shortest_path": ["problem_type", "G", "source", "dest"],
+            "vehicle_routing": [
+                "problem_type",
+                "G",
+                "pos",
+                "n_vehicles",
+                "depot",
+                "subtours",
+                "method",
+                "penalty",
+            ],
+            "maximal_independent_set": ["problem_type", "G", "penalty"],
+            "bin_packing": [
+                "problem_type",
+                "weights",
+                "weight_capacity",
+                "penalty",
+                "n_items",
+                "method",
+                "simplifications",
+                "n_bins",
+                "min_bins",
+                "solution",
+            ],
             "generic_qubo": ["problem_type"],
         }
 
         for k, v in qubos.items():
             assert (
                 list(v.problem_instance.keys()) == expected_keys[k]
             ), "Problem instance keys are not correct for problem type {}".format(k)
@@ -1109,14 +1541,17 @@
             "tsp": TSP,
             "number_partition": NumberPartition,
             "maximum_cut": MaximumCut,
             "knapsack": Knapsack,
             "slack_free_knapsack": SlackFreeKnapsack,
             "minimum_vertex_cover": MinimumVertexCover,
             "shortest_path": ShortestPath,
+            "maximal_independent_set": MIS,
+            "bin_packing": BinPacking,
+            "vehicle_routing": VRP,
         }
 
         problems, qubos = self.__generate_random_problems()
 
         for type in qubos:
             if type == "generic_qubo":
                 continue
@@ -1139,15 +1574,14 @@
     def test_qubo_from_dict(self):
         """
         Test qubo from dict method of the QUBO class.
         """
 
         _, qubos = self.__generate_random_problems()
         for _, qubo in qubos.items():
-
             qubo_dict = qubo.asdict()
 
             new_qubo = QUBO.from_dict(qubo_dict)
 
             for term, new_term in zip(qubo.terms, new_qubo.terms):
                 assert set(term) == set(
                     new_term
@@ -1156,19 +1590,412 @@
                 )
 
                 assert set(qubo.weights) == set(
                     new_qubo.weights
                 ), "QUBO from dict method is not correct for problem type {}".format(
                     qubo.problem_instance["problem_type"]
                 )
-
+                
                 for key in qubo.__dict__:
                     if key != "terms" and key != "weights":
                         assert (
                             qubo.__dict__[key] == new_qubo.__dict__[key]
                         ), "QUBO from dict method is not correct for problem type {}".format(
                             qubo.problem_instance["problem_type"]
                         )
 
+    # TESTING BINPACKING CLASS
+    def test_binpacking_terms_weights_constant(self):
+        """Test that BinPacking creates a correct QUBO from the provided weights and terms"""
+
+        terms = [
+            [2, 3],
+            [4, 5],
+            [0, 2],
+            [0, 4],
+            [0, 6],
+            [2, 4],
+            [2, 6],
+            [4, 6],
+            [1, 3],
+            [1, 5],
+            [1, 7],
+            [3, 5],
+            [3, 7],
+            [5, 7],
+            [0],
+            [1],
+            [2],
+            [3],
+            [4],
+            [5],
+            [6],
+            [7],
+        ]
+
+        weights = [
+            1.5,
+            1.5,
+            -0.75,
+            -1.0,
+            -1.5,
+            0.5,
+            0.75,
+            1.0,
+            -0.75,
+            -1.0,
+            -1.5,
+            0.5,
+            0.75,
+            1.0,
+            1.25,
+            1.25,
+            -0.875,
+            -0.875,
+            -1.1666666666666665,
+            -1.1666666666666665,
+            -1.75,
+            -1.75,
+        ]
+        constant = 10.083333333333332
+        weights_list = [3, 4]
+        weight_capacity = 6
+        binpacking_prob_qubo = BinPacking(
+            weights_list, weight_capacity, simplifications=False
+        ).qubo
+        self.assertTrue(terms_list_equality(terms, binpacking_prob_qubo.terms))
+        self.assertTrue(terms_list_isclose(weights, binpacking_prob_qubo.weights))
+        self.assertTrue(np.isclose(constant, binpacking_prob_qubo.constant))
+
+    def test_binpacking_terms_weights_constant_simplified(self):
+        """Test that BinPacking creates a correct QUBO from the provided weights and terms"""
+
+        terms = [
+            [1, 2],
+            [1, 3],
+            [2, 3],
+            [4, 5],
+            [4, 6],
+            [5, 6],
+            [1, 4],
+            [1, 7],
+            [4, 7],
+            [2, 5],
+            [8, 2],
+            [8, 5],
+            [0, 3],
+            [0, 6],
+            [0, 9],
+            [3, 6],
+            [9, 3],
+            [9, 6],
+            [0],
+            [1],
+            [2],
+            [3],
+            [4],
+            [5],
+            [6],
+            [7],
+            [8],
+            [9],
+        ]
+
+        weights = [
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            0.2,
+            0.28,
+            0.35,
+            0.2,
+            0.4,
+            0.5,
+            -0.4,
+            -0.5,
+            -1.0,
+            0.2,
+            0.4,
+            0.5,
+            0.4,
+            -1.08,
+            -0.96,
+            -1.36,
+            -1.1,
+            -0.95,
+            -1.45,
+            -0.14,
+            0.1,
+            -0.9,
+        ]
+        constant = 9.29
+        weights_list = [3, 4, 5]
+        weight_capacity = 10
+        binpacking_prob_qubo = BinPacking(weights_list, weight_capacity).qubo
+
+        self.assertTrue(terms_list_equality(terms, binpacking_prob_qubo.terms))
+        self.assertTrue(terms_list_isclose(weights, binpacking_prob_qubo.weights))
+        self.assertTrue(np.isclose(constant, binpacking_prob_qubo.constant))
+
+    def test_binpacking_terms_weights_constant_unbalanced(self):
+        """Test that BinPacking creates a correct QUBO from the provided weights and terms
+        using the unbalanced penalization encoding"""
+        terms = [
+            [1, 2],
+            [1, 3],
+            [2, 3],
+            [4, 5],
+            [4, 6],
+            [5, 6],
+            [1, 4],
+            [2, 5],
+            [0, 3],
+            [0, 6],
+            [3, 6],
+            [0],
+            [1],
+            [2],
+            [3],
+            [4],
+            [5],
+            [6],
+        ]
+
+        weights = [
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            1.0,
+            0.05,
+            0.05,
+            -0.1,
+            -0.125,
+            0.05,
+            -0.475,
+            -0.97,
+            -0.91,
+            -1.01,
+            -0.9625,
+            -0.8875,
+            -1.0125,
+        ]
+        constant = 6.8775
+
+        weights_list = [3, 4, 5]
+        weight_capacity = 10
+        binpacking_prob_qubo = BinPacking(
+            weights_list, weight_capacity, method="unbalanced"
+        ).qubo
+
+        self.assertTrue(terms_list_equality(terms, binpacking_prob_qubo.terms))
+        self.assertTrue(terms_list_isclose(weights, binpacking_prob_qubo.weights))
+        self.assertTrue(np.isclose(constant, binpacking_prob_qubo.constant))
+
+    def test_binpacking_terms_penalizations_terms_unbalanced(self):
+        """Test that BinPacking creates a correct QUBO from the provided weights and terms
+        using the unbalanced penalization encoding given the penalization terms"""
+        terms = [[1, 2], [0, 2], [0], [1], [2]]
+
+        weights = [0.5, -0.25, -0.25, -0.0625, -0.125]
+        constant = 1.953125
+
+        weights_list = [3, 4]
+        weight_capacity = 8
+        penalty = [1, 1, 1]
+        binpacking_prob_qubo = BinPacking(
+            weights_list,
+            weight_capacity,
+            penalty=penalty,
+            method="unbalanced",
+            simplifications=True,
+        ).qubo
+
+        self.assertTrue(terms_list_equality(terms, binpacking_prob_qubo.terms))
+        self.assertTrue(terms_list_isclose(weights, binpacking_prob_qubo.weights))
+        self.assertTrue(np.isclose(constant, binpacking_prob_qubo.constant))
+
+    def test_binpacking_terms_penalizations_terms_slack(self):
+        """Test that BinPacking creates a correct QUBO from the provided weights and terms
+        using the unbalanced penalization encoding"""
+        terms = [[1, 2], [1, 3], [0, 2], [0, 4], [2, 4], [0], [1], [2], [3], [4]]
+
+        weights = [
+            0.5,
+            0.15625,
+            -0.25,
+            -0.5,
+            0.25,
+            -0.25,
+            0.03125,
+            -0.125,
+            0.0390625,
+            -0.25,
+        ]
+        constant = 2.7890625
+
+        weights_list = [3, 4]
+        weight_capacity = 8
+        penalty = [1]
+        binpacking_prob_qubo = BinPacking(
+            weights_list,
+            weight_capacity,
+            penalty=penalty,
+            method="slack",
+            simplifications=True,
+        ).qubo
+
+        self.assertTrue(terms_list_equality(terms, binpacking_prob_qubo.terms))
+        self.assertTrue(terms_list_isclose(weights, binpacking_prob_qubo.weights))
+        self.assertTrue(np.isclose(constant, binpacking_prob_qubo.constant))
+
+    def test_binpacking_random_problem(self):
+        """Test Bin Packing random instance method"""
+
+        seed = 1234
+        np.random.seed(seed)
+        min_weight = 1
+        max_weight = 7
+        n_items = 3
+        weight_capacity = 15
+        weights = list(np.random.randint(min_weight, max_weight, n_items))
+        binpacking_manual_prob = BinPacking(weights, weight_capacity).qubo
+
+        binpacking_random_prob = BinPacking.random_instance(
+            n_items=3, seed=seed, weight_capacity=weight_capacity
+        ).qubo
+
+        self.assertTrue(
+            terms_list_equality(
+                binpacking_manual_prob.terms, binpacking_random_prob.terms
+            )
+        )
+        self.assertEqual(binpacking_manual_prob.weights, binpacking_random_prob.weights)
+        self.assertEqual(
+            binpacking_manual_prob.constant, binpacking_random_prob.constant
+        )
+
+    def test_binpacking_classical_sol(self):
+        """Test the Bin Packing random instance method classical solution"""
+
+        seed = 1234
+        np.random.seed(seed)
+        binpacking_sol = BinPacking.random_instance(
+            n_items=3, seed=seed
+        ).classical_solution()
+
+        sol = {
+            "y_0": 1,
+            "y_1": 0,
+            "y_2": 0,
+            "x_0_0": 1,
+            "x_0_1": 0,
+            "x_0_2": 0,
+            "x_1_0": 1,
+            "x_1_1": 0,
+            "x_1_2": 0,
+            "x_2_0": 1,
+            "x_2_1": 0,
+            "x_2_2": 0,
+        }
+
+        self.assertEqual(binpacking_sol, sol)
+
+    def test_binpacking_plot(self):
+        """Test Bin Packing random instance method"""
+        from matplotlib.pyplot import Figure
+
+        seed = 1234
+        binpacking_random_prob = BinPacking.random_instance(n_items=3, seed=seed)
+        sol = {
+            "y_0": 1,
+            "y_1": 0,
+            "y_2": 0,
+            "x_0_0": 1,
+            "x_0_1": 0,
+            "x_0_2": 0,
+            "x_1_0": 1,
+            "x_1_1": 0,
+            "x_1_2": 0,
+            "x_2_0": 1,
+            "x_2_1": 0,
+            "x_2_2": 0,
+        }
+        fig = binpacking_random_prob.plot_solution(sol)
+        self.assertTrue(isinstance(fig, Figure))
+
+    def test_binpacking_method_checking(self):
+        """
+        Checks if the method-checking returns the right error.
+        """
+        weights = [3, 5, 7]
+        weight_capacity = 15
+        method = "random"
+        with self.assertRaises(ValueError) as e:
+            BinPacking(weights, weight_capacity, method=method)
+        self.assertEqual(
+            f"The method '{method}' is not a valid method. Choose between 'slack' and 'unbalanced'",
+            str(e.exception),
+        )
+
+    def test_binpacking_random_problem_checking(self):
+        """
+        Checks if the random min_weight equal to max_weight returns the right error.
+        """
+        min_weight = 5
+        max_weight = 5
+        with self.assertRaises(ValueError) as e:
+            BinPacking.random_instance(min_weight=min_weight, max_weight=max_weight)
+        self.assertEqual(
+            f"min_weight: {min_weight} must be < max_weight:{max_weight}",
+            str(e.exception),
+        )
+
+    def test_binpacking_classical_sol_checking(self):
+        """
+        Checks if the unfeasible classical solution returns the right error.
+        """
+        weights = [10, 10]
+        weight_capacity = 8
+        with self.assertRaises(ValueError) as e:
+            BinPacking(
+                weights=weights, weight_capacity=weight_capacity
+            ).classical_solution()
+        self.assertEqual("solution not found: integer infeasible", str(e.exception))
+
+    def test_binpacking_input_weights(self):
+        """
+        Checks if the unfeasible classical solution returns the right error.
+        """
+        weights = [10.1, 10]
+        weight_capacity = 8
+        with self.assertRaises(TypeError) as e:
+            BinPacking(
+                weights=weights, weight_capacity=weight_capacity
+            ).classical_solution()
+        self.assertEqual(
+            f"The weights must be integer numbers. Format {type(weights[0])} found.",
+            str(e.exception),
+        )
+
+    def test_binpacking_input_weight_capacity(self):
+        """
+        Checks if the unfeasible classical solution returns the right error.
+        """
+        weights = [10, 10]
+        weight_capacity = 8.1
+        with self.assertRaises(TypeError) as e:
+            BinPacking(
+                weights=weights, weight_capacity=weight_capacity
+            ).classical_solution()
+        self.assertEqual(
+            f"The weight_capacity must be integer. Format {type(weight_capacity)} found.",
+            str(e.exception),
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.2/tests/test_pyquil_qvm.py` & `openqaoa-0.1.3/tests/test_pyquil_qvm.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_qpu_braket.py` & `openqaoa-0.1.3/tests/test_qpu_braket.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """This Object tests the QAOA Braket QPU Backend objects, which is tasked with the
     creation and execution of a QAOA circuit for the selected QPU provider and
     backend.
 
     These tests require authentication through the AWS CLI.
     """
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_circuit_angle_assignment_qpu_backend(self):
         """
         A tests that checks if the circuit created by the AWS Backend
         has the appropriate angles assigned before the circuit is executed.
         Checks the circuit created on the AWS Backend.
         """
 
@@ -83,15 +83,15 @@
         main_circuit.rx(0, -2 * betas[1])
         main_circuit.rx(1, -2 * betas[1])
         main_circuit.rx(2, -2 * betas[1])
         main_circuit.probability()
 
         self.assertEqual(main_circuit, qpu_circuit)
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_circuit_angle_assignment_qpu_backend_w_hadamard(self):
         """
         Checks for consistent if init_hadamard is set to True.
         """
 
         nqubits = 3
         p = 2
@@ -145,15 +145,15 @@
         main_circuit.rx(0, -2 * betas[1])
         main_circuit.rx(1, -2 * betas[1])
         main_circuit.rx(2, -2 * betas[1])
         main_circuit.probability()
 
         self.assertEqual(main_circuit, qpu_circuit)
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_prepend_circuit(self):
         """
         Checks if prepended circuit has been prepended correctly.
         """
 
         nqubits = 3
         p = 1
@@ -204,15 +204,15 @@
         main_circuit.rx(0, -2 * betas[0])
         main_circuit.rx(1, -2 * betas[0])
         main_circuit.rx(2, -2 * betas[0])
         main_circuit.probability()
 
         self.assertEqual(main_circuit, qpu_circuit)
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_append_circuit(self):
         """
         Checks if appended circuit is appropriately appended to the back of the
         QAOA Circuit.
         """
 
         nqubits = 3
@@ -264,17 +264,16 @@
         main_circuit.x(0)
         main_circuit.x(1)
         main_circuit.x(2)
         main_circuit.probability()
 
         self.assertEqual(main_circuit, qpu_circuit)
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_prepend_exception(self):
-
         """
         Test that the error catching for a prepend ciruit larger than the problem
         circuit is invalid
         """
 
         nqubits = 3
         p = 1
@@ -293,30 +292,32 @@
         cost_hamil = Hamiltonian(
             [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
             weights,
             1,
         )
         mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=p)
-        variate_params = QAOAVariationalStandardParams(qaoa_descriptor, betas, gammas)
+
+        # Try to create the variate params
+        _ = QAOAVariationalStandardParams(qaoa_descriptor, betas, gammas)
 
         aws_device = DeviceAWS("arn:aws:braket:::device/quantum-simulator/amazon/sv1")
 
         try:
-            aws_backend = QAOAAWSQPUBackend(
+            # Try to create the AWS backend
+            _ = QAOAAWSQPUBackend(
                 qaoa_descriptor, aws_device, shots, prepend_circuit, None, True, 1.0
             )
         except Exception as e:
             self.assertEqual(
                 str(e), "Cannot attach a bigger circuit to the QAOA routine"
             )
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_exceptions_in_init(self):
-
         """
         Testing the Exceptions in the init function of the QAOAAWSQPUBackend
         """
 
         nqubits = 3
         p = 1
         weights = [1, 1, 1]
@@ -327,15 +328,17 @@
         cost_hamil = Hamiltonian(
             [PauliOp("ZZ", (0, 1)), PauliOp("ZZ", (1, 2)), PauliOp("ZZ", (0, 2))],
             weights,
             1,
         )
         mixer_hamil = X_mixer_hamiltonian(n_qubits=nqubits)
         qaoa_descriptor = QAOADescriptor(cost_hamil, mixer_hamil, p=p)
-        variate_params = QAOAVariationalStandardParams(qaoa_descriptor, betas, gammas)
+
+        # Try instantiating the variate params
+        _ = QAOAVariationalStandardParams(qaoa_descriptor, betas, gammas)
 
         # If the user's aws credentials is not correct.
         mock_device = Mock()
         mock_device.configure_mock(
             **{
                 "check_connection.return_value": False,
                 "provider_connected.return_value": False,
@@ -375,17 +378,16 @@
             )
 
         # Correct device arn (Errorless)
         aws_device = DeviceAWS("arn:aws:braket:::device/quantum-simulator/amazon/sv1")
 
         QAOAAWSQPUBackend(qaoa_descriptor, aws_device, shots, None, None, True, 1.0)
 
-    @pytest.mark.qpu
+    @pytest.mark.braket_api
     def test_remote_qubit_overflow(self):
-
         """
         If the user creates a circuit that is larger than the maximum circuit size
         that is supported by the QPU. An Exception should be raised with the
         appropriate error message alerting the user to the error.
         """
 
         shots = 100
@@ -408,17 +410,16 @@
             braket_backend.expectation(variate_params)
         except Exception as e:
             self.assertEqual(
                 str(e),
                 "There are lesser qubits on the device than the number of qubits required for the circuit.",
             )
 
-    @pytest.mark.qpu
+    @pytest.mark.sim
     def test_remote_integration_qpu_run(self):
-
         """
         Run a toy example in manual mode to make sure everything works as
         expected for a remote backend
         """
 
         shots = 100
```

### Comparing `openqaoa-0.1.2/tests/test_qpu_devices.py` & `openqaoa-0.1.3/tests/test_qpu_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,41 +26,50 @@
 
     @pytest.mark.api
     def setUp(self):
 
         self.HUB = "ibm-q"
         self.GROUP = "open"
         self.PROJECT = "main"
+        self.INSTANCE = "ibm-q/open/main"
 
     @pytest.mark.api
     def test_changing_provider(self):
 
         """
         This test checks that the specified hub,group and project in the
         initialisation of DeviceQiskit changes the provider to the appropriate
         destination.
         """
 
         device_obj = DeviceQiskit(device_name="ibmq_manila")
         device_obj.check_connection()
 
-        self.assertEqual(device_obj.provider.credentials.hub, self.HUB)
-        self.assertEqual(device_obj.provider.credentials.group, self.GROUP)
-        self.assertEqual(device_obj.provider.credentials.project, self.PROJECT)
-
-        device_obj2 = DeviceQiskit(device_name="ibmq_manila", hub="ibm-q-startup")
-        device_obj2.check_connection()
-        self.assertEqual(device_obj2.provider.credentials.hub, "ibm-q-startup")
+        provider_instances = device_obj.provider.instances()
+
+        if len(provider_instances) >= 2:
+
+            for each_item in provider_instances[:2]:
+
+                [hub, group, project] = each_item.split("/")
+                device_obj2 = DeviceQiskit(
+                    device_name="ibmq_manila", hub=hub, group=group, project=project
+                )
+                device_obj2.check_connection()
+
+                self.assertEqual(device_obj2.provider._account.instance, each_item)
 
     @pytest.mark.api
     def test_check_connection_provider_no_backend_wrong_hub_group_project(self):
 
         """
-        If the wrong hub, group or project is specified, check_connection should
+        Hub, group and project must always be specified together.
+        If either the hub, group or project is wrongly specified, check_connection should
         return False.
+        If not all 3 are specified, check_connection should return False.
         The provider_connected attribute should be updated to False.
         Since the API Token is loaded from save_account, the api token will be
         checked by Qiskit.
         """
 
         for each_combi in itertools.product(
             ["invalid_hub", None], ["invalid_group", None], ["invalid_project", None]
@@ -164,27 +173,27 @@
 
         device_obj = DeviceLocal("unsupported_device")
 
         self.assertEqual(device_obj.check_connection(), False)
 
 
 class TestingDeviceAWS(unittest.TestCase):
-
     """These tests check the Object used to access AWS Braket and their
     available QPUs can be established.
 
     For any tests using provided credentials, the tests will only pass if those
     details provided are correct/valid with AWS Braket.
     """
 
-    @pytest.mark.api
+    @pytest.mark.braket_api
     def test_changing_aws_region(self):
 
         device_obj = DeviceAWS(
-            device_name="arn:aws:braket:::device/quantum-simulator/amazon/sv1"
+            device_name="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
+            aws_region="us-east-1",
         )
 
         device_obj.check_connection()
         default_region = device_obj.aws_region
 
         self.assertEqual("us-east-1", default_region)
 
@@ -194,43 +203,43 @@
         )
 
         device_obj.check_connection()
         custom_region = device_obj.aws_region
 
         self.assertEqual("us-west-1", custom_region)
 
-    @pytest.mark.api
+    @pytest.mark.braket_api
     def test_changing_s3_bucket_names(self):
 
         device_obj = DeviceAWS(
             device_name="arn:aws:braket:::device/quantum-simulator/amazon/sv1",
             s3_bucket_name="random_new_name",
         )
 
         device_obj.check_connection()
         custom_bucket = device_obj.s3_bucket_name
 
         self.assertEqual("random_new_name", custom_bucket)
 
-    @pytest.mark.api
+    @pytest.mark.braket_api
     def test_check_connection_provider_no_backend_provided_credentials(self):
 
         """
         If no information about the device name, but the credentials
         used are correct, check_connection should return True.
         The provider_connected attribute should be updated to True.
         """
 
         device_obj = DeviceAWS(device_name="")
 
         self.assertEqual(device_obj.check_connection(), True)
         self.assertEqual(device_obj.provider_connected, True)
         self.assertEqual(device_obj.qpu_connected, None)
 
-    @pytest.mark.api
+    @pytest.mark.braket_api
     def test_check_connection_provider_right_backend_provided_credentials(self):
 
         """
         If the correct device name is provided and the credentials
         used are correct, check_connection should return True.
         The provider_connected attribute should be updated to True.
         The qpu_connected attribute should be updated to True.
@@ -243,15 +252,15 @@
 
         device_obj = DeviceAWS(device_name=valid_qpu_name)
 
         self.assertEqual(device_obj.check_connection(), True)
         self.assertEqual(device_obj.provider_connected, True)
         self.assertEqual(device_obj.qpu_connected, True)
 
-    @pytest.mark.api
+    @pytest.mark.braket_api
     def test_check_connection_provider_wrong_backend_provided_credentials(self):
 
         """
         If device name provided is incorrect, and not empty, and the credentials
         used are correct, check_connection should return False.
         The provider_connected attribute should be updated to True.
         The qpu_connected attribute should be updated to False.
@@ -292,15 +301,15 @@
                 for each_json in output_json
                 if each_json["name"] == "TestingOpenQAOA"
             ][0]
             self.RESOURCE_ID = output_json_s["id"]
             self.AZ_LOCATION = output_json_s["location"]
 
     @pytest.mark.api
-    def test_check_connection_provider_no_resource_id(self):
+    def test_check_connection_provider_no_resource_id_or_az_location(self):
 
         """
         If no information about about the workspace is provided, the resource id
         or az location, check_connection and provider_connected should return False.
         """
 
         for resource_id, az_location in itertools.product(
@@ -316,36 +325,40 @@
                 )
 
                 self.assertEqual(device_obj.check_connection(), False)
                 self.assertEqual(device_obj.provider_connected, False)
                 self.assertEqual(device_obj.qpu_connected, None)
 
     @pytest.mark.api
-    def test_check_connection_provider_no_backend_provided_credentials(self):
+    def test_check_connection_provider_no_backend_provided_resource_id_and_az_location(
+        self,
+    ):
 
         """
-        If no information about the device name, but the credentials
-        used are correct, check_connection should return True.
+        If no information about the device name, but the resource id and azure
+        location used are correct, check_connection should return True.
         The provider_connected attribute should be updated to True.
         """
 
         device_obj = DeviceAzure(
             device_name="", resource_id=self.RESOURCE_ID, az_location=self.AZ_LOCATION
         )
 
         self.assertEqual(device_obj.check_connection(), True)
         self.assertEqual(device_obj.provider_connected, True)
         self.assertEqual(device_obj.qpu_connected, None)
 
     @pytest.mark.api
-    def test_check_connection_provider_right_backend_provided_credentials(self):
+    def test_check_connection_provider_right_backend_provided_resource_id_and_az_location(
+        self,
+    ):
 
         """
-        If the correct device name is provided and the credentials
-        used are correct, check_connection should return True.
+        If the correct device name is provided and the resource id and azure
+        location used are correct, check_connection should return True.
         The provider_connected attribute should be updated to True.
         The qpu_connected attribute should be updated to True.
         """
 
         device_obj = DeviceAzure(
             device_name="", resource_id=self.RESOURCE_ID, az_location=self.AZ_LOCATION
         )
@@ -360,19 +373,21 @@
         )
 
         self.assertEqual(device_obj.check_connection(), True)
         self.assertEqual(device_obj.provider_connected, True)
         self.assertEqual(device_obj.qpu_connected, True)
 
     @pytest.mark.api
-    def test_check_connection_provider_wrong_backend_provided_credentials(self):
+    def test_check_connection_provider_wrong_backend_provided_resource_id_and_az_location(
+        self,
+    ):
 
         """
-        If device name provided is incorrect, and not empty, and the credentials
-        used are correct, check_connection should return False.
+        If device name provided is incorrect, and not empty, and the resource id
+        and azure location used are correct, check_connection should return False.
         The provider_connected attribute should be updated to True.
         The qpu_connected attribute should be updated to False.
         """
 
         device_obj = DeviceAzure(
             device_name="invalid_backend",
             resource_id=self.RESOURCE_ID,
```

### Comparing `openqaoa-0.1.2/tests/test_result_object.py` & `openqaoa-0.1.3/tests/test_result_object.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_results.py` & `openqaoa-0.1.3/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_rqaoa.py` & `openqaoa-0.1.3/tests/test_rqaoa.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_sample_from_wavefunction.py` & `openqaoa-0.1.3/tests/test_sample_from_wavefunction.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_sim_qiskit.py` & `openqaoa-0.1.3/tests/test_sim_qiskit.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_simulators.py` & `openqaoa-0.1.3/tests/test_simulators.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_utilities.py` & `openqaoa-0.1.3/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,43 +504,87 @@
         Tests the function that computes the expectation value of a classical Hamiltonian
         for a dictionary containing measurement counts.
 
         The test consists in computing the expectation value from a given Hamiltonian
         and a given measurement counts dictionary.
         """
 
+        ## First test - Ring of Disagrees
+
         # Number of qubits
         n_qubits = 10
 
         # Define edges and weights determining the problem graph
         edges = [(i, i + 1) for i in range(n_qubits - 1)] + [(0, n_qubits - 1)]
         weights = [1 for _ in range(len(edges))]
+        constant = 10
 
         # Hamiltonian
-        hamiltonian = Hamiltonian.classical_hamiltonian(edges, weights, constant=0)
+        hamiltonian = Hamiltonian.classical_hamiltonian(edges, weights, constant)
 
         # Input measurement counts dictionary
         input_measurement_counts = {
             "0101010101": 10,
             "1010101010": 10,
             "0000000000": 10,
             "1111111111": 10,
             "1111111110": 10,
         }
 
         # Obtain energy expectation value
         energy = energy_expectation(hamiltonian, input_measurement_counts)
 
         # Correct energy
-        correct_energy = 1.2
+        correct_energy = 11.2
+
+        # Test energy was computed correctly
+        assert np.allclose(
+            energy, correct_energy
+        ), f"The energy expectation value for rings of disagrees was not computed correctly"
+
+        ## Second test - Minimum Vertex Cover on a Ring
+
+        # Number of qubits
+        n_qubits = 10
+
+        # Edges of the graph
+        edges = [(i, i + 1) for i in range(n_qubits - 1)] + [(0, n_qubits - 1)]
+
+        # Define graph and add edges
+        G = nx.Graph()
+        G.add_edges_from(edges)
+
+        # QUBO instance of the problem
+        field = 1.0
+        penalty = 10.0
+        mvc = MinimumVertexCover(G, field=field, penalty=penalty).qubo
+
+        # Minimum Vertex Cover Hamiltonian
+        hamiltonian = Hamiltonian.classical_hamiltonian(
+            mvc.terms, mvc.weights, mvc.constant
+        )
+
+        # Input measurement counts dictionary
+        input_measurement_counts = {
+            "0101010101": 10,
+            "1010101010": 10,
+            "0000000000": 10,
+            "1111111111": 10,
+        }
+
+        # Obtain energy expectation value
+        energy = energy_expectation(hamiltonian, input_measurement_counts)
+
+        # Correct energy
+        correct_energy = 30
 
         # Test energy was computed correctly
         assert np.allclose(
             energy, correct_energy
-        ), f"The energy expectation value was not computed correctly"
+        ), f"The energy expectation value for Minimum Vertex Cover was not computed correctly"
 
     def test_energy_spectrum_hamiltonian(self):
         """
         Tests the function that computes the exact energy spectrum from a given classical Hamiltonian.
 
         The test consists in computing the spectrum of a given classical Hamiltonian.
         """
@@ -1176,10 +1220,31 @@
         generated_timestamp = generate_timestamp()
 
         # Test that the timestamp has been generated correctly
         assert is_valid_timestamp(
             generated_timestamp
         ), f"Timestamp has not been generated correctly"
 
+    def test_permute_counts_dictionary(self):
+        """
+        Tests the function that permutes the counts dictionary: permute_counts_dictionary.
+        """
+
+        # Input dictionary
+        input_dict = {"011011": 1, "000111": 2, "000000": 3}
+
+        # Permute the dictionary
+        output_dict = permute_counts_dictionary(
+            input_dict, permutation_order=[4, 5, 3, 0, 1, 2]
+        )
+
+        # Expected dictionary
+        expected_dict = {"110011": 1, "111000": 2, "000000": 3}
+
+        # Test that the dictionary has been permuted correctly
+        assert (
+            output_dict == expected_dict
+        ), f"Dictionary has not been permuted correctly"
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `openqaoa-0.1.2/tests/test_vectorized.py` & `openqaoa-0.1.3/tests/test_vectorized.py`

 * *Files identical despite different names*

### Comparing `openqaoa-0.1.2/tests/test_workflows.py` & `openqaoa-0.1.3/tests/test_workflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-import json, os, gzip
+import json
+import os
+import gzip
 import unittest
 import networkx as nw
 import numpy as np
 import datetime
+from copy import deepcopy
 
 from qiskit.providers.fake_provider import FakeVigo
 from qiskit.providers.aer.noise import NoiseModel
 from qiskit.providers.aer import QasmSimulator
 
 from openqaoa import QAOA, RQAOA
+from openqaoa.problems import NumberPartition
 from openqaoa.algorithms import QAOAResult, RQAOAResult
 from openqaoa.algorithms.baseworkflow import Workflow
 from openqaoa.utilities import X_mixer_hamiltonian, XY_mixer_hamiltonian, is_valid_uuid
 from openqaoa.algorithms.workflow_properties import (
     BackendProperties,
     ClassicalOptimizer,
     CircuitProperties,
 )
 from openqaoa.algorithms.rqaoa.rqaoa_workflow_properties import RqaoaParameters
 from openqaoa.backends import create_device, DeviceLocal
-from openqaoa.backends.devices_core import SUPPORTED_LOCAL_SIMULATORS
+from openqaoa.backends.cost_function import cost_function
+
+# from openqaoa.backends.devices_core import SUPPORTED_LOCAL_SIMULATORS
 from openqaoa.qaoa_components import (
     Hamiltonian,
     QAOADescriptor,
     QAOAVariationalStandardParams,
     QAOAVariationalStandardWithBiasParams,
     QAOAVariationalExtendedParams,
     QAOAVariationalFourierParams,
@@ -42,24 +48,24 @@
 from openqaoa_pyquil.backends import DevicePyquil
 from openqaoa_pyquil.backends import QAOAPyQuilWavefunctionSimulatorBackend
 from openqaoa_qiskit.backends import DeviceQiskit
 from openqaoa_qiskit.backends import (
     QAOAQiskitBackendShotBasedSimulator,
     QAOAQiskitBackendStatevecSimulator,
 )
+from openqaoa_azure.backends import DeviceAzure
 
-
-ALLOWED_LOCAL_SIMUALTORS = SUPPORTED_LOCAL_SIMULATORS
-LOCAL_DEVICES = ALLOWED_LOCAL_SIMUALTORS + ["6q-qvm", "Aspen-11"]
+from openqaoa.qaoa_components.variational_parameters.variational_params_factory import (
+    PARAMS_CLASSES_MAPPER,
+)
 
 
 def _compare_qaoa_results(dict_old, dict_new):
-
     for key in dict_old.keys():
-        if key == "cost_hamiltonian":  ## CHECK WHAT DO WITH THIS
+        if key == "cost_hamiltonian":  # CHECK WHAT DO WITH THIS
             pass
         elif key == "_QAOAResult__type_backend":
             if issubclass(dict_old[key], QAOABaseBackendStatevector):
                 assert (
                     dict_new[key] == QAOABaseBackendStatevector
                 ), "Type of backend is not correct."
             else:
@@ -76,26 +82,29 @@
                     ), "Optimized params are not the same."
         elif key == "intermediate":
             for key2 in dict_old[key].keys():
                 if key2 == "measurement_outcomes":
                     for step in range(len(dict_old[key][key2])):
                         assert np.all(
                             dict_old[key][key2][step] == dict_new[key][key2][step]
-                        ), "Intermediate params are not the same."
+                        ), f"Intermediate params are not the same. Expected {dict_old[key][key2][step]} but \
+                            received {dict_new[key][key2][step]}"
                 else:
                     assert (
                         dict_old[key][key2] == dict_new[key][key2]
-                    ), "Intermediate params are not the same."
+                    ), f"Intermediate params are not the same. Expected {dict_old[key][key2]}, but \
+                        received {dict_new[key][key2]}"
         else:
             assert dict_old[key] == dict_new[key], f"'{key}' is not the same"
 
 
 def _test_keys_in_dict(obj, expected_keys):
     """
-    private function to test the keys. It recursively tests the keys of the nested dictionaries, or lists of dictionaries
+    private function to test the keys.
+    It recursively tests the keys of the nested dictionaries, or lists of dictionaries
     """
 
     if isinstance(obj, dict):
         for key in obj:
             if key in expected_keys.keys():
                 expected_keys[key] = True
 
@@ -112,24 +121,22 @@
 class TestingVanillaQAOA(unittest.TestCase):
 
     """
     Unit test based testing of the QAOA workflow class
     """
 
     def test_vanilla_qaoa_default_values(self):
-
         q = QAOA()
         assert q.circuit_properties.p == 1
         assert q.circuit_properties.param_type == "standard"
         assert q.circuit_properties.init_type == "ramp"
         assert q.device.device_location == "local"
         assert q.device.device_name == "vectorized"
 
     def test_end_to_end_vectorized(self):
-
         g = nw.circulant_graph(6, [1])
         vc = MinimumVertexCover(g, field=1.0, penalty=10).qubo
 
         q = QAOA()
         q.set_classical_optimizer(optimization_progress=True)
         q.compile(vc)
         q.optimize()
@@ -171,28 +178,34 @@
                 **{"hub": "***", "group": "***", "project": "***"},
             )
         )
         assert type(q.device) == DeviceQiskit
         assert q.device.device_name == "place_holder"
         assert q.device.device_location == "ibmq"
 
+        q.set_device(
+            create_device(
+                "azure", name="place_holder", resource_id="***", az_location="***"
+            )
+        )
+        assert type(q.device) == DeviceAzure
+        assert q.device.device_name == "place_holder"
+        assert q.device.device_location == "azure"
+
     def test_compile_before_optimise(self):
         """
         Assert that compilation has to be called before optimisation
         """
-        g = nw.circulant_graph(6, [1])
-        # vc = MinimumVertexCover(g, field =1.0, penalty=10).qubo
 
         q = QAOA()
         q.set_classical_optimizer(optimization_progress=True)
 
         self.assertRaises(ValueError, lambda: q.optimize())
 
     def test_cost_hamil(self):
-
         g = nw.circulant_graph(6, [1])
         problem = MinimumVertexCover(g, field=1.0, penalty=10)
         qubo_problem = problem.qubo
 
         test_hamil = Hamiltonian.classical_hamiltonian(
             terms=qubo_problem.terms,
             coeffs=qubo_problem.weights,
@@ -205,15 +218,14 @@
 
         self.assertEqual(q.cost_hamil.expression, test_hamil.expression)
         self.assertEqual(
             q.qaoa_descriptor.cost_hamiltonian.expression, test_hamil.expression
         )
 
     def test_set_circuit_properties_fourier_q(self):
-
         """
         The value of q should be None if the param_type used is not fourier.
         Else if param_type is fourier, fourier_extended or fourier_w_bias, it
         should be the value of q, if it is provided.
         """
 
         fourier_param_types = ["fourier", "fourier_extended", "fourier_w_bias"]
@@ -225,15 +237,14 @@
             self.assertEqual(q.circuit_properties.q, 1)
 
         q.set_circuit_properties(param_type="standard", q=1)
 
         self.assertEqual(q.circuit_properties.q, None)
 
     def test_set_circuit_properties_annealing_time_linear_ramp_time(self):
-
         """
         Check that linear_ramp_time and annealing_time are updated appropriately
         as the value of p is changed.
         """
 
         q = QAOA()
 
@@ -244,17 +255,17 @@
 
         q.set_circuit_properties(p=2)
 
         self.assertEqual(q.circuit_properties.annealing_time, 0.7 * 2)
         self.assertEqual(q.circuit_properties.linear_ramp_time, 0.7 * 2)
 
     def test_set_circuit_properties_qaoa_descriptor_mixer_x(self):
-
         """
-        Checks if the X mixer created by the X_mixer_hamiltonian method and the automated methods in workflows do the same thing.
+        Checks if the X mixer created by the X_mixer_hamiltonian method
+        and the automated methods in workflows do the same thing.
 
         For each qubit, there should be 1 RXGateMap per layer of p.
         """
 
         nodes = 6
         edge_probability = 0.6
         g = nw.generators.fast_gnp_random_graph(n=nodes, p=edge_probability)
@@ -278,17 +289,17 @@
             self.assertEqual(each_gatemap_name, "RXGateMap")
 
         for j in range(2):
             for i in range(6):
                 self.assertEqual(q.qaoa_descriptor.mixer_blocks[j][i].qubit_1, i)
 
     def test_set_circuit_properties_qaoa_descriptor_mixer_xy(self):
-
         """
-        Checks if the XY mixer created by the XY_mixer_hamiltonian method and the automated methods in workflows do the same thing.
+        Checks if the XY mixer created by the XY_mixer_hamiltonian method
+        and the automated methods in workflows do the same thing.
 
         Depending on the qubit connectivity selected. (chain, full or star)
         For each pair of connected qubits, there should be 1 RXXGateMap and RYYGateMap per layer of p.
         """
 
         g_c = nw.circulant_graph(6, [1])
         g_f = nw.complete_graph(6)
@@ -324,15 +335,14 @@
             for i in range(0, len(q.qaoa_descriptor.mixer_qubits_pairs), 2):
                 self.assertEqual(q.qaoa_descriptor.mixer_qubits_pairs[i], "RXXGateMap")
                 self.assertEqual(
                     q.qaoa_descriptor.mixer_qubits_pairs[i + 1], "RYYGateMap"
                 )
 
     def test_set_circuit_properties_variate_params(self):
-
         """
         Ensure that the Varitional Parameter Object created based on the input string , param_type, is correct.
 
         TODO: Check if q=None is the appropriate default.
         """
 
         param_type_names = [
@@ -354,24 +364,22 @@
 
         nodes = 6
         edge_probability = 0.6
         g = nw.generators.fast_gnp_random_graph(n=nodes, p=edge_probability)
         problem = MinimumVertexCover(g, field=1.0, penalty=10)
 
         for i in range(len(object_types)):
-
             q = QAOA()
             q.set_circuit_properties(param_type=param_type_names[i], q=1)
 
             q.compile(problem=problem.qubo)
 
             self.assertEqual(type(q.variate_params), object_types[i])
 
     def test_set_circuit_properties_change(self):
-
         """
         Ensure that once a property has beefn changed via set_circuit_properties.
         The attribute has been appropriately updated.
         Updating all attributes at the same time.
         """
 
         #         default_pairings = {'param_type': 'standard',
@@ -411,17 +419,17 @@
 
         q.set_circuit_properties(**update_pairings)
 
         for each_key, each_value in update_pairings.items():
             self.assertEqual(getattr(q.circuit_properties, each_key), each_value)
 
     def test_set_circuit_properties_rejected_values(self):
-
         """
-        Some properties of CircuitProperties Object return a ValueError if the specified property has not been whitelisted in the code.
+        Some properties of CircuitProperties Object return a ValueError
+        if the specified property has not been whitelisted in the code.
         This checks that the ValueError is raised if the argument is not whitelisted.
         """
 
         q = QAOA()
 
         self.assertRaises(
             ValueError, lambda: q.set_circuit_properties(param_type="wrong name")
@@ -431,15 +439,14 @@
         )
         self.assertRaises(
             ValueError, lambda: q.set_circuit_properties(mixer_hamiltonian="wrong name")
         )
         self.assertRaises(ValueError, lambda: q.set_circuit_properties(p=-1))
 
     def test_set_backend_properties_change(self):
-
         """
         Ensure that once a property has been changed via set_backend_properties.
         The attribute has been appropriately updated.
         Updating all attributes at the same time.
         """
 
         default_pairings = {
@@ -465,15 +472,14 @@
 
         q.set_backend_properties(**update_pairings)
 
         for each_key, each_value in update_pairings.items():
             self.assertEqual(getattr(q.backend_properties, each_key), each_value)
 
     def test_set_backend_properties_check_backend_vectorized(self):
-
         """
         Check if the backend returned by set_backend_properties is correct
         Based on the input device.
         Also Checks if defaults from workflows are used in the backend.
         """
 
         nodes = 6
@@ -492,15 +498,14 @@
         self.assertEqual(q.backend.prepend_state, None)
         self.assertEqual(q.backend.append_state, None)
         self.assertEqual(q.backend.cvar_alpha, 1)
 
         self.assertRaises(AttributeError, lambda: q.backend.n_shots)
 
     def test_set_backend_properties_check_backend_vectorized_w_custom(self):
-
         """
         Check if the backend returned by set_backend_properties is correct
         Based on the input device.
         Uses custom values for attributes in backend_properties and checks if the
         backend object responds appropriately.
         """
 
@@ -534,15 +539,14 @@
         self.assertEqual((q.backend.prepend_state == prepend_state_rand).all(), True)
         self.assertEqual((q.backend.append_state == append_state_rand).all(), True)
         self.assertEqual(q.backend.cvar_alpha, 1)
 
         self.assertRaises(AttributeError, lambda: q.backend.n_shots)
 
     def test_set_backend_properties_check_backend_vectorized_error_values(self):
-
         """
         If the values provided from the workflows are incorrect, we should
         receive the appropriate error messages from the vectorized backend.
 
         Checks:
         Incorrect size of prepend state and append state.
         """
@@ -572,15 +576,14 @@
         update_pairings = {"prepend_state": None, "append_state": append_state_rand}
 
         q.set_backend_properties(**update_pairings)
 
         self.assertRaises(ValueError, lambda: q.compile(problem=qubo_problem))
 
     def test_set_backend_properties_check_backend_qiskit_qasm(self):
-
         """
         Check if the backend returned by set_backend_properties is correct
         Based on the input device. For qiskit qasm simulator.
         Also Checks if defaults from workflows are used in the backend.
         """
 
         nodes = 6
@@ -598,15 +601,14 @@
         self.assertEqual(q.backend.init_hadamard, True)
         self.assertEqual(q.backend.prepend_state, None)
         self.assertEqual(q.backend.append_state, None)
         self.assertEqual(q.backend.cvar_alpha, 1)
         self.assertEqual(q.backend.n_shots, 100)
 
     def test_set_backend_properties_check_backend_qiskit_statevector(self):
-
         """
         Check if the backend returned by set_backend_properties is correct
         Based on the input device. For qiskit statevector simulator.
         Also Checks if defaults from workflows are used in the backend.
         """
 
         nodes = 6
@@ -627,15 +629,14 @@
         self.assertEqual(q.backend.prepend_state, None)
         self.assertEqual(q.backend.append_state, None)
         self.assertEqual(q.backend.cvar_alpha, 1)
 
         self.assertRaises(AttributeError, lambda: q.backend.n_shots)
 
     def test_set_backend_properties_check_backend_pyquil_statevector(self):
-
         """
         Check if the backend returned by set_backend_properties is correct
         Based on the input device. For pyquil statevector simulator.
         Also Checks if defaults from workflows are used in the backend.
         """
 
         nodes = 6
@@ -656,15 +657,14 @@
         self.assertEqual(q.backend.prepend_state, None)
         self.assertEqual(q.backend.append_state, None)
         self.assertEqual(q.backend.cvar_alpha, 1)
 
         self.assertRaises(AttributeError, lambda: q.backend.n_shots)
 
     def test_set_classical_optimizer_defaults(self):
-
         """
         Check if the fields in the default classical_optimizer dict are correct
         """
 
         default_pairings = {
             "optimize": True,
             "method": "cobyla",
@@ -683,31 +683,29 @@
         }
 
         q = QAOA()
 
         for each_key, each_value in default_pairings.items():
             self.assertEqual(getattr(q.classical_optimizer, each_key), each_value)
 
-            if each_value != None:
-                self.assertEqual(q.classical_optimizer.asdict()[each_key], each_value)
+            # if each_value is None: LD --> I don't think we really need this test, since asdict()
+            #     assert isinstance(q.classical_optimizer.each_key, None)
 
     def test_set_classical_optimizer_jac_hess_casing(self):
-
         """
         jac and hess should be in lower case if it is a string.
         """
 
         q = QAOA()
         q.set_classical_optimizer(jac="JaC", hess="HeSS")
 
         self.assertEqual(q.classical_optimizer.jac, "jac")
         self.assertEqual(q.classical_optimizer.hess, "hess")
 
     def test_set_classical_optimizer_method_selectors(self):
-
         """
         Different methods would return different Optimizer classes.
         Check that the correct class is returned.
         """
 
         nodes = 6
         edge_probability = 0.6
@@ -764,29 +762,29 @@
                 assert is_valid_uuid(
                     qaoa.header["experiment_id"]
                 ), "The experiment_id is not a valid uuid."
             elif key == "algorithm":
                 assert qaoa.header["algorithm"] == "qaoa"
             else:
                 assert (
-                    value == None
+                    value is None
                 ), "The value of the key {} (of the dictionary qaoa.header) is not None, when it should be.".format(
                     key
                 )
 
         # save the experiment_id
         experiment_id = qaoa.header["experiment_id"]
 
         # set the header
         qaoa.set_header(
             project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
             description="test",
-            run_by="raul",
+            run_by="OpenQAOA",
             provider="-",
-            target="-",
+            target="vectorized",
             cloud="local",
             client="-",
         )
 
         # check that the experiment_id has not changed, since it is not set in the set_header method
         assert (
             qaoa.header["experiment_id"] == experiment_id
@@ -795,31 +793,32 @@
         # now set the experiment_id
         experiment_id = experiment_id[:-2] + "00"
 
         # set the header
         qaoa.set_header(
             project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
             description="test",
-            run_by="raul",
+            run_by="OpenQAOA",
             provider="-",
-            target="-",
+            target="vectorized",
             cloud="local",
             client="-",
             experiment_id=experiment_id,
         )
 
-        # check if the header values are set to the correct values, except for the qubit_number, atomic_id, execution_time_start, and execution_time_end (which are set to None)
+        # check if the header values are set to the correct values, except for the
+        # qubit_number, atomic_id, execution_time_start, and execution_time_end (which are set to None)
         dict_values = {
             "experiment_id": experiment_id,
             "project_id": "8353185c-b175-4eda-9628-b4e58cb0e41b",
             "algorithm": "qaoa",
             "description": "test",
-            "run_by": "raul",
+            "run_by": "OpenQAOA",
             "provider": "-",
-            "target": "-",
+            "target": "vectorized",
             "cloud": "local",
             "client": "-",
             "qubit_number": None,
             "atomic_id": None,
             "execution_time_start": None,
             "execution_time_end": None,
         }
@@ -829,16 +828,18 @@
             ), "The value of the key {} (of the dictionary qaoa.header) is not correct.".format(
                 key
             )
 
         # compile the QAOA object
         qaoa.compile(problem=QUBO.random_instance(n=8))
 
-        # check if the header values are still set to the correct values, except for execution_time_start, and execution_time_end (which are set to None).
-        # Now atomic_id should be set to a valid uuid. And qubit_number should be set to 8 (number of qubits of the problem)
+        # check if the header values are still set to the correct values, except for execution_time_start, and
+        # execution_time_end (which are set to None).
+        # Now atomic_id should be set to a valid uuid.
+        # And qubit_number should be set to 8 (number of qubits of the problem)
         dict_values["qubit_number"] = 8
         for key, value in qaoa.header.items():
             if key not in ["atomic_id"]:
                 assert (
                     dict_values[key] == value
                 ), "The value of the key {} (of the dictionary qaoa.header) is not correct.".format(
                     key
@@ -849,15 +850,16 @@
 
         # save the atomic_id
         atomic_id = qaoa.header["atomic_id"]
 
         # optimize the QAOA object
         qaoa.optimize()
 
-        # check if the header values are still set to the correct values, now everything should be set to a valid value (execution_time_start and execution_time_end should be integers>1672933928)
+        # check if the header values are still set to the correct values, now everything should be set to a valid value
+        # (execution_time_start and execution_time_end should be integers>1672933928)
         dict_values["atomic_id"] = atomic_id
         for key, value in qaoa.header.items():
             if key not in ["execution_time_start", "execution_time_end"]:
                 assert (
                     dict_values[key] == value
                 ), "The value of the key {} (of the dictionary qaoa.header) is not correct.".format(
                     key
@@ -871,34 +873,34 @@
 
         # test if an error is raised when the project_id is not a valid string
         error = False
         try:
             qaoa.set_header(
                 project_id="test",
                 description="test",
-                run_by="raul",
+                run_by="OpenQAOA",
                 provider="-",
-                target="-",
+                target="vectorized",
                 cloud="local",
                 client="-",
             )
         except:
             error = True
         assert error, "The project_id is not valid string, but no error was raised."
 
         # test if an error is raised when the experiment_id is not a valid string
         error = False
         try:
             qaoa.set_header(
                 project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
                 experiment_id="test",
                 description="test",
-                run_by="raul",
+                run_by="OpenQAOA",
                 provider="-",
-                target="-",
+                target="vectorized",
                 cloud="local",
                 client="-",
             )
         except:
             error = True
         assert error, "The experiment_id is not valid string, but no error was raised."
 
@@ -909,18 +911,25 @@
 
         qaoa = QAOA()
         qaoa.set_exp_tags(tags={"tag1": "value1", "tag2": "value2"})
         qaoa.set_exp_tags(tags={"tag1": "value9"})
         qaoa.compile(problem=QUBO.random_instance(n=8))
         qaoa.optimize()
 
-        assert qaoa.exp_tags == {
+        tags = {
             "tag1": "value9",
             "tag2": "value2",
-        }, "Experiment tags are not set correctly."
+            "init_type": "ramp",
+            "optimizer_method": "cobyla",
+            "p": 1,
+            "param_type": "standard",
+            "qubit_number": 8,
+        }
+
+        assert qaoa.exp_tags == tags, "Experiment tags are not set correctly."
 
         error = False
         try:
             qaoa.set_exp_tags(tags={"tag1": complex(1, 2)})
         except:
             error = True
         assert error, "Experiment tag values should be primitives."
@@ -964,17 +973,17 @@
         # qaoa
         qaoa = QAOA()
         qaoa.compile(problem=QUBO.random_instance(n=8))
         # set the header
         qaoa.set_header(
             project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
             description="test",
-            run_by="raul",
+            run_by="OpenQAOA",
             provider="-",
-            target="-",
+            target="vectorized",
             cloud="local",
             client="-",
         )
         qaoa.optimize()
 
         # check QAOA asdict
         self.__test_expected_keys(qaoa.asdict(), method="asdict")
@@ -994,78 +1003,89 @@
             json.loads(qaoa.dumps(exclude_keys=exclude_keys)),
             exclude_keys,
             method="dumps",
         )
 
         # check QAOA dump
         file_name = "test_dump_qaoa.json"
-        experiment_id, atomic_id = (
+        project_id, experiment_id, atomic_id = (
+            qaoa.header["project_id"],
             qaoa.header["experiment_id"],
             qaoa.header["atomic_id"],
         )
-        full_name = f"{experiment_id}--{atomic_id}--{file_name}"
+        full_name = f"{project_id}--{experiment_id}--{atomic_id}--{file_name}"
 
-        qaoa.dump(file_name, indent=None)
+        qaoa.dump(file_name, indent=None, prepend_id=True)
         assert os.path.isfile(full_name), "Dump file does not exist"
         with open(full_name, "r") as file:
             assert file.read() == qaoa.dumps(
                 indent=None
             ), "Dump file does not contain the correct data"
         os.remove(full_name)
 
-        # check RQAOA dump whitout prepending the experiment_id and atomic_id
+        # check QAOA dump whitout prepending the experiment_id and atomic_id
         qaoa.dump(file_name, indent=None, prepend_id=False)
         assert os.path.isfile(
             file_name
         ), "Dump file does not exist, when not prepending the experiment_id and atomic_id"
 
-        # check RQAOA dump fails when the file already exists
+        # check QAOA dump fails when the file already exists
         error = False
         try:
             qaoa.dump(file_name, indent=None, prepend_id=False)
         except FileExistsError:
             error = True
         assert error, "Dump file does not fail when the file already exists"
 
         # check that we can overwrite the file
         qaoa.dump(file_name, indent=None, prepend_id=False, overwrite=True)
         assert os.path.isfile(file_name), "Dump file does not exist, when overwriting"
         os.remove(file_name)
 
-        # check RQAOA dump fails when prepend_id is True and file_name is not given
+        # check QAOA dump fails when prepend_id is True and file_name is not given
         error = False
         try:
             qaoa.dump(prepend_id=False)
         except ValueError:
             error = True
         assert (
             error
         ), "Dump file does not fail when prepend_id is True and file_name is not given"
 
-        # check you can dump to a file with no arguments
-        qaoa.dump()
+        # check QAOA dump with no arguments
+        error = False
+        try:
+            qaoa.dump()
+        except ValueError:
+            error = True
+        assert (
+            error
+        ), "Dump file does not fail when no arguments are given, should be the same as dump(prepend_id=False)"
+
+        # check you can dump to a file with no arguments, just prepend_id=True
+        qaoa.dump(prepend_id=True)
         assert os.path.isfile(
-            f"{experiment_id}--{atomic_id}.json"
+            f"{project_id}--{experiment_id}--{atomic_id}.json"
         ), "Dump file does not exist, when no name is given"
-        os.remove(f"{experiment_id}--{atomic_id}.json")
+        os.remove(f"{project_id}--{experiment_id}--{atomic_id}.json")
 
         # check QAOA dump deleting some keys
         exclude_keys = ["schedule", "singlet"]
-        qaoa.dump(file_name, exclude_keys=exclude_keys, indent=None)
+        qaoa.dump(file_name, exclude_keys=exclude_keys, indent=None, prepend_id=True)
         assert os.path.isfile(
             full_name
         ), "Dump file does not exist, when deleting some keys"
         with open(full_name, "r") as file:
             assert file.read() == qaoa.dumps(
                 exclude_keys=exclude_keys, indent=None
             ), "Dump file does not contain the correct data, when deleting some keys"
         os.remove(full_name)
 
         # check QAOA dump with compression
-        qaoa.dump(file_name, compresslevel=2, indent=None)
+        qaoa.dump(file_name, compresslevel=2, indent=None, prepend_id=True)
         assert os.path.isfile(
             full_name + ".gz"
         ), "Dump file does not exist, when compressing"
         with gzip.open(full_name + ".gz", "rb") as file:
             assert (
                 file.read() == qaoa.dumps(indent=None).encode()
             ), "Dump file does not contain the correct data, when compressing"
@@ -1172,19 +1192,19 @@
         # test the keys, it will set the keys to True if they are found
         _test_keys_in_dict(obj, expected_keys)
 
         # Check if the dictionary has all the expected keys except the ones that were not included
         for key, value in expected_keys.items():
             if key not in exclude_keys:
                 assert (
-                    value == True
+                    value is True
                 ), f'Key "{key}" not found in the dictionary, when using "{method}" method.'
             else:
                 assert (
-                    value == False
+                    value is False
                 ), f'Key "{key}" was found in the dictionary, but it should not be there, when using "{method}" method.'
 
         """
         to get the list of expected keys, run the following code:
 
             def get_keys(obj, list_keys):
                 if isinstance(obj, dict):
@@ -1218,30 +1238,26 @@
 
         # run rqaoa with different devices, and save the objcets in a list
         qaoas = []
         for device in [
             create_device(location="local", name="qiskit.shot_simulator"),
             create_device(location="local", name="vectorized"),
         ]:
-
             q = QAOA()
             q.set_device(device)
             q.set_circuit_properties(
                 p=1, param_type="extended", init_type="rand", mixer_hamiltonian="x"
             )
             q.set_backend_properties(n_shots=50)
-            q.set_classical_optimizer(maxiter=10, optimization_progress=True)
+            q.set_classical_optimizer(maxiter=2, optimization_progress=True)
             q.set_exp_tags({"add_tag": "test"})
             q.set_header(
                 project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
                 description="test",
-                run_by="raul",
-                provider="-",
-                target="-",
-                cloud="local",
+                run_by="oq",
                 client="-",
             )
 
             # test that you can convert the rqaoa object to a dictionary and then load it before optimization
             _ = QAOA.from_dict(q.asdict())
             _.compile(maxcut_qubo)
             _.optimize()
@@ -1251,17 +1267,17 @@
 
             # compile and optimize the original rqaoa object
             q.compile(maxcut_qubo)
             q.optimize()
 
             qaoas.append(q)
 
-        # for each rqaoa object, create a new rqaoa object from dict, json string, json file, and compressed json file and compare them with the original object
+        # for each rqaoa object, create a new rqaoa object from dict, json string, json file,
+        # and compressed json file and compare them with the original object
         for q in qaoas:
-
             new_q_list = []
 
             # get new qaoa from dict
             new_q_list.append(QAOA.from_dict(q.asdict()))
             # get new qaoa from json string
             new_q_list.append(QAOA.loads(q.dumps()))
             # get new qaoa from json file
@@ -1270,15 +1286,14 @@
             os.remove("test.json")  # delete file test.json
             # get new qaoa from compressed json file
             q.dump("test.json", prepend_id=False, compresslevel=3)
             new_q_list.append(QAOA.load("test.json.gz"))
             os.remove("test.json.gz")  # delete file test.json
 
             for new_q in new_q_list:
-
                 # check that the new object is an QAOA object
                 assert isinstance(new_q, QAOA), "new_r is not an RQAOA object"
 
                 # check that the attributes of the new object are of the correct type
                 attributes_types = [
                     ("header", dict),
                     ("exp_tags", dict),
@@ -1325,14 +1340,277 @@
             RQAOA.from_dict(q.asdict())
         except Exception:
             error = True
         assert (
             error
         ), "RQAOA.from_dict should raise an error when using a QAOA dictionary"
 
+    def test_qaoa_evaluate_circuit(self):
+        """
+        test the evaluate_circuit method
+        """
+
+        # problem
+        problem = MinimumVertexCover.random_instance(
+            n_nodes=6, edge_probability=0.8
+        ).qubo
+
+        # run qaoa with different param_type, and save the objcets in a list
+        qaoas = []
+        for param_type in PARAMS_CLASSES_MAPPER.keys():
+            q = QAOA()
+            q.set_circuit_properties(p=3, param_type=param_type, init_type="rand")
+            q.compile(problem)
+            qaoas.append(q)
+
+        # for each qaoa object, test the evaluate_circuit method
+        for q in qaoas:
+            # evaluate the circuit with random dict of params
+            params = {
+                k: np.random.rand(*v.shape)
+                for k, v in q.variate_params.asdict().items()
+            }
+            result = q.evaluate_circuit(params)
+            assert (
+                abs(result["cost"]) >= 0
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` \
+                should return a cost, here cost is {result['cost']}"
+            assert (
+                abs(result["uncertainty"]) > 0
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return an uncertanty, \
+                here uncertainty is {result['uncertainty']}"
+            assert (
+                len(result["measurement_results"]) > 0
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return \
+                a wavefunction when using a state-based simulator"
+
+            # evaluate the circuit with a list of params, taking the params from the dict,
+            # so we should get the same result
+            params2 = []
+            for value in params.values():
+                params2 += value.flatten().tolist()
+            result2 = q.evaluate_circuit(params2)
+            assert (
+                result == result2
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return the same result \
+                when passing a dict or a list of params"
+
+            # evaluate the circuit with np.ndarray of params, taking the params from the dict,
+            # so we should get the same result
+            result2 = q.evaluate_circuit(np.array(params2))
+            assert (
+                result == result2
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return the same result \
+                when passing a dict or a list of params"
+
+            # evaluate the circuit with the params as a QAOAVariationalBaseParams object,
+            # so we should get the same result
+            params_obj = deepcopy(q.variate_params)
+            params_obj.update_from_raw(params2)
+            result3 = q.evaluate_circuit(params_obj)
+            assert (
+                result == result3
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return the same result \
+                when passing a dict or a list of params"
+
+            # run the circuit with the params manually, we should get the same result
+            result4 = {}
+            (
+                result4["cost"],
+                result4["uncertainty"],
+            ) = q.backend.expectation_w_uncertainty(params_obj)
+            result4["measurement_results"] = q.backend.wavefunction(params_obj)
+            assert (
+                result == result4
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should return the same result when \
+                  passing the optimized params manually"
+
+            # evaluate the circuit with a wrong input, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit(1)
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error when \
+                  passing a wrong input"
+
+            # evaluate the circuit with a list longer than it should, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit(params2 + [1])
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error when \
+                passing a list longer than it should"
+
+            # evaluate the circuit with a list shorter than it should, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit(params2[:-1])
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error when \
+                passing a list shorter than it should"
+
+            # evaluate the circuit with a dict with a wrong key, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit({**params, "wrong_key": 1})
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error \
+                when passing a dict with a wrong key"
+
+            # evaluate the circuit with a dict with a value longer than it should, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit(
+                    {**params, list(params.keys())[0]: np.random.rand(40)}
+                )
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error when \
+                passing a dict with a value longer than it should"
+
+            # evaluate the circuit without passing any param, it should raise an error
+            error = False
+            try:
+                q.evaluate_circuit()
+            except Exception:
+                error = True
+            assert (
+                error
+            ), f"param_type={q.circuit_properties.param_type}. `evaluate_circuit` should raise an error when \
+                  not passing any param"
+
+        # check that it works with shots
+        q = QAOA()
+        device = create_device(location="local", name="qiskit.qasm_simulator")
+        q.set_device(device)
+        q.set_circuit_properties(p=3)
+
+        # try to evaluate the circuit before compiling
+        error = False
+        try:
+            q.evaluate_circuit()
+        except Exception:
+            error = True
+        assert (
+            error
+        ), f"param_type={param_type}. `evaluate_circuit` should raise an error if the circuit is not compiled"
+
+        # compile and evaluate the circuit, and check that the result is correct
+        q.compile(problem)
+        result = q.evaluate_circuit([1, 2, 1, 2, 1, 2])
+        assert isinstance(
+            result["measurement_results"], dict
+        ), "When using a shot-based simulator, `evaluate_circuit` should return a dict of counts"
+        assert (
+            abs(result["cost"]) >= 0
+        ), "When using a shot-based simulator, `evaluate_circuit` should return a cost"
+        assert (
+            abs(result["uncertainty"]) > 0
+        ), "When using a shot-based simulator, `evaluate_circuit` should return an uncertanty"
+
+        cost = cost_function(
+            result["measurement_results"],
+            q.backend.qaoa_descriptor.cost_hamiltonian,
+            q.backend.cvar_alpha,
+        )
+        cost_sq = cost_function(
+            result["measurement_results"],
+            q.backend.qaoa_descriptor.cost_hamiltonian.hamiltonian_squared,
+            q.backend.cvar_alpha,
+        )
+        uncertainty = np.sqrt(cost_sq - cost**2)
+        assert (
+            np.round(cost, 12) == result["cost"]
+        ), "When using a shot-based simulator, `evaluate_circuit` not returning the correct cost"
+        assert (
+            np.round(uncertainty, 12) == result["uncertainty"]
+        ), "When using a shot-based simulator, `evaluate_circuit` not returning the correct uncertainty"
+
+        # check that it works with analytical simulator
+        q = QAOA()
+        device = create_device(location="local", name="analytical_simulator")
+        q.set_device(device)
+        q.set_circuit_properties(p=1, param_type="standard")
+        q.compile(problem)
+        result = q.evaluate_circuit([1, 2])
+        assert (
+            abs(result["cost"]) >= 0
+        ), "When using an analytical simulator, `evaluate_circuit` should return a cost"
+        assert (
+            result["uncertainty"] is None
+        ), "When using an analytical simulator, `evaluate_circuit` should return uncertainty None"
+        assert (
+            result["measurement_results"] is None
+        ), "When using an analytical simulator, `evaluate_circuit` should return no measurement results"
+
+    def test_change_properties_after_compilation(self):
+        device = create_device(location="local", name="qiskit.shot_simulator")
+        q = QAOA()
+        q.compile(QUBO.random_instance(4))
+
+        with self.assertRaises(ValueError):
+            q.set_device(device)
+        with self.assertRaises(ValueError):
+            q.set_circuit_properties(
+                p=1, param_type="standard", init_type="rand", mixer_hamiltonian="x"
+            )
+        with self.assertRaises(ValueError):
+            q.set_backend_properties(prepend_state=None, append_state=None)
+        with self.assertRaises(ValueError):
+            q.set_classical_optimizer(
+                maxiter=100, method="vgd", jac="finite_difference"
+            )
+
+    def test_numpy_serialize(self):
+        np_qubo = NumberPartition([1, 2, 3]).qubo
+
+        q = QAOA()
+        q.compile(np_qubo)
+        q.optimize()
+
+        # add numpy results
+        numpy_dict = {
+            "000": np.int64(85),
+            "100": np.int64(85),
+            "010": np.int64(85),
+            "111": 12,
+        }
+        numpy_cost = np.float64(85.123)
+
+        q.result.optimized["intermediate"] = [
+            numpy_cost,
+            numpy_cost,
+            numpy_cost,
+            0.123,
+            -123.123,
+        ]
+        q.result.intermediate["measurement_outcomes"] = [
+            numpy_dict,
+            numpy_dict,
+            numpy_dict,
+        ]
+        q.result.optimized["measurement_outcomes"] = numpy_dict
+        q.result.optimized["cost"] = numpy_cost
+
+        q.dumps()
+
 
 class TestingRQAOA(unittest.TestCase):
     """
     Unit test based testing of the RQAOA workflow class
     """
 
     def _test_default_values(self, x):
@@ -1341,15 +1619,15 @@
         """
 
         # circuit_properties
         cp = x.circuit_properties
         assert cp.param_type == "standard"
         assert cp.init_type == "ramp"
         assert cp.p == 1
-        assert cp.q == None
+        assert cp.q is None
         assert cp.mixer_hamiltonian == "x"
 
         # device
         d = x.device
         assert d.device_location == "local"
         assert d.device_name == "vectorized"
 
@@ -1359,15 +1637,15 @@
         """
         r = RQAOA()
 
         assert r.rqaoa_parameters.rqaoa_type == "custom"
         assert r.rqaoa_parameters.n_cutoff == 5
         assert r.rqaoa_parameters.n_max == 1
         assert r.rqaoa_parameters.steps == 1
-        assert r.rqaoa_parameters.original_hamiltonian == None
+        assert r.rqaoa_parameters.original_hamiltonian is None
         assert r.rqaoa_parameters.counter == 0
 
         self._test_default_values(r)
 
     def test_rqaoa_compile_and_qoao_default_values(self):
         """
         Test creation of the qaoa object and its default values
@@ -1387,16 +1665,15 @@
         param_type="standard",
         mixer="x",
         method="cobyla",
         maxiter=15,
         name_device="qiskit.statevector_simulator",
         return_object=False,
     ):
-
-        if problem == None:
+        if problem is None:
             problem = MaximumCut.random_instance(
                 n_nodes=8, edge_probability=0.5, seed=2
             ).qubo
 
         r = RQAOA()
         qiskit_device = create_device(location="local", name=name_device)
         r.set_device(qiskit_device)
@@ -1416,18 +1693,15 @@
             optimization_progress=True,
             cost_progress=True,
             parameter_log=True,
         )
         r.set_header(
             project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
             description="header",
-            run_by="raul",
-            provider="-",
-            target="-",
-            cloud="local",
+            run_by="OpenQAOA",
             client="-",
         )
         r.set_exp_tags(tags={"tag1": "value1", "tag2": "value2"})
         r.compile(problem)
         r.optimize()
 
         if return_object:
@@ -1459,15 +1733,14 @@
             exception = True
 
         assert (
             exception
         ), "RQAOA should not be able to optimize twice without compilation"
 
     def test_example_1_adaptive_custom(self):
-
         # Number of qubits
         n_qubits = 12
 
         # Elimination schemes
         Nmax = [1, 2, 3, 4]
         schedules = [1, [1, 2, 1, 2, 7]]
         n_cutoff = 5
@@ -1497,15 +1770,14 @@
 
         # Check computed solutions are among the correct ones
         for solution in solutions:
             for key in solution:
                 assert solution[key] == exact_soutions[key]
 
     def test_example_2_adaptive_custom(self):
-
         # Elimination scheme
         n_cutoff = 3
 
         # Define problem instance (Ring graph 10 qubits)
         graph = nw.circulant_graph(10, [1])
         problem = MinimumVertexCover(graph, field=1, penalty=10).qubo
 
@@ -1519,15 +1791,14 @@
 
         # Check computed solutions are among the correct ones
         for solution in solutions:
             for key in solution:
                 assert solution[key] == exact_soutions[key]
 
     def test_example_3_adaptive_custom(self):
-
         # Elimination scheme
         step = 2
         nmax = 4
         n_cutoff = 3
 
         # Define problem instance (Ring graph 10 qubits)
         graph = nw.complete_graph(10)
@@ -1554,15 +1825,14 @@
 
         # Check computed solutions are among the correct ones
         for solution in solutions:
             for key in solution:
                 assert solution[key] == exact_soutions[key]
 
     def test_example_4_adaptive_custom(self):
-
         # Number of qubits
         n_qubits = 10
 
         # Elimination schemes
         Nmax = [1, 2, 3, 4]
         schedules = [1, 2, 3]
         n_cutoff = 3
@@ -1869,21 +2139,22 @@
             json.loads(rqaoa.dumps(exclude_keys=exclude_keys)),
             exclude_keys,
             method="dumps",
         )
 
         # check RQAOA dump
         file_name = "test_dump_rqaoa.json"
-        experiment_id, atomic_id = (
+        project_id, experiment_id, atomic_id = (
+            rqaoa.header["project_id"],
             rqaoa.header["experiment_id"],
             rqaoa.header["atomic_id"],
         )
-        full_name = f"{experiment_id}--{atomic_id}--{file_name}"
+        full_name = f"{project_id}--{experiment_id}--{atomic_id}--{file_name}"
 
-        rqaoa.dump(file_name, indent=None)
+        rqaoa.dump(file_name, prepend_id=True, indent=None)
         assert os.path.isfile(full_name), "Dump file does not exist"
         with open(full_name, "r") as file:
             assert file.read() == rqaoa.dumps(
                 indent=None
             ), "Dump file does not contain the correct data"
         os.remove(full_name)
 
@@ -1912,35 +2183,45 @@
             rqaoa.dump(prepend_id=False)
         except ValueError:
             error = True
         assert (
             error
         ), "Dump file does not fail when prepend_id is True and file_name is not given"
 
-        # check you can dump to a file with no arguments
-        rqaoa.dump()
+        # check RQAOA dump with no arguments
+        error = False
+        try:
+            rqaoa.dump()
+        except ValueError:
+            error = True
+        assert (
+            error
+        ), "Dump file does not fail when no arguments are given, should be the same as dump(prepend_id=False)"
+
+        # check you can dump to a file with no arguments, just prepend_id=True
+        rqaoa.dump(prepend_id=True)
         assert os.path.isfile(
-            f"{experiment_id}--{atomic_id}.json"
+            f"{project_id}--{experiment_id}--{atomic_id}.json"
         ), "Dump file does not exist, when no name is given"
-        os.remove(f"{experiment_id}--{atomic_id}.json")
+        os.remove(f"{project_id}--{experiment_id}--{atomic_id}.json")
 
         # check RQAOA dump deleting some keys
         exclude_keys = ["schedule", "singlet"]
-        rqaoa.dump(file_name, exclude_keys=exclude_keys, indent=None)
+        rqaoa.dump(file_name, exclude_keys=exclude_keys, indent=None, prepend_id=True)
         assert os.path.isfile(
             full_name
         ), "Dump file does not exist, when deleting some keys"
         with open(full_name, "r") as file:
             assert file.read() == rqaoa.dumps(
                 exclude_keys=exclude_keys, indent=None
             ), "Dump file does not contain the correct data, when deleting some keys"
         os.remove(full_name)
 
         # check RQAOA dump with compression
-        rqaoa.dump(file_name, compresslevel=2, indent=None)
+        rqaoa.dump(file_name, compresslevel=2, indent=None, prepend_id=True)
         assert os.path.isfile(
             full_name + ".gz"
         ), "Dump file does not exist, when compressing"
         with gzip.open(full_name + ".gz", "rb") as file:
             assert (
                 file.read() == rqaoa.dumps(indent=None).encode()
             ), "Dump file does not contain the correct data, when compressing"
@@ -2073,19 +2354,19 @@
         # test the keys, it will set the keys to True if they are found
         _test_keys_in_dict(obj, expected_keys)
 
         # Check if the dictionary has all the expected keys except the ones that were not included
         for key, value in expected_keys.items():
             if key not in exclude_keys:
                 assert (
-                    value == True
+                    value is True
                 ), f'Key "{key}" not found in the dictionary, when using "{method}" method.'
             else:
                 assert (
-                    value == False
+                    value is False
                 ), f'Key "{key}" was found in the dictionary, but it should not be there, when using "{method}" method.'
 
         """
         to get the list of expected keys, run the following code:
 
             def get_keys(obj, list_keys):
                 if isinstance(obj, dict):
@@ -2107,50 +2388,55 @@
         """
 
     def test_rqaoa_dumping_step_by_step(self):
         """
         test dumping the RQAOA object step by step
         """
 
+        project_id = "d3a6f03b-1484-423a-8432-38e57c4e9ec7"
+
         # define the problem
         problem = QUBO.random_instance(n=8)
         problem.set_metadata(
             {"metadata_key1": "metadata_value1", "metadata_key2": "metadata_value2"}
         )
 
-        # define the RQAOA object
         r = RQAOA()
-
-        # set experimental tags
+        r.set_header(project_id=project_id)
         r.set_exp_tags({"tag1": "value1", "tag2": "value2"})
-
-        # set the classical optimizer
         r.set_classical_optimizer(optimization_progress=True)
-
-        # compile the problem
         r.compile(problem)
 
         # optimize the problem while dumping the data at each step
         r.optimize(
             dump=True,
             dump_options={
                 "file_name": "test_dumping_step_by_step",
                 "compresslevel": 2,
                 "indent": None,
+                "prepend_id": True,
             },
         )
 
         # create list of expected file names
         experiment_id, atomic_id = r.header["experiment_id"], r.header["atomic_id"]
         file_names = {
-            id: experiment_id + "--" + id + "--" + "test_dumping_step_by_step.json.gz"
+            id: project_id
+            + "--"
+            + experiment_id
+            + "--"
+            + id
+            + "--"
+            + "test_dumping_step_by_step.json.gz"
             for id in r.result["atomic_ids"].values()
         }
         file_names[atomic_id] = (
-            experiment_id
+            project_id
+            + "--"
+            + experiment_id
             + "--"
             + atomic_id
             + "--"
             + "test_dumping_step_by_step.json.gz"
         )
 
         # check if the files exist
@@ -2163,19 +2449,17 @@
             with gzip.open(file_name, "rb") as file:
                 files[atomic_id] = json.loads(file.read().decode())
 
         rqaoa_files, qaoa_files = 0, 0
 
         # check if the files have the expected keys
         for atomic_id, dictionary in files.items():
-
             file_name = file_names[atomic_id]
 
             if r.header["atomic_id"] == atomic_id:  # rqaoa files
-
                 rqaoa_files += 1
 
                 assert (
                     dictionary["header"]["experiment_id"] == r.header["experiment_id"]
                 ), f"File {file_name} has a different experiment_id than the RQAOA object."
                 assert (
                     dictionary["header"]["atomic_id"] == r.header["atomic_id"]
@@ -2188,15 +2472,14 @@
                 for step in dictionary["data"]["result"]["intermediate_steps"]:
                     assert (
                         step["qaoa_results"]["intermediate"]["measurement_outcomes"]
                         == []
                     ), f"File {file_name} has intermediate mesuraments, but it should not have them."
 
             else:  # qaoa files
-
                 qaoa_files += 1
 
                 assert (
                     dictionary["header"]["atomic_id"] == atomic_id
                 ), f"File {file_name} has a different atomic_id than expected."
                 assert (
                     dictionary["header"]["algorithm"] == "qaoa"
@@ -2234,30 +2517,29 @@
 
         # run rqaoa with different devices, and save the objcets in a list
         rqaoas = []
         for device in [
             create_device(location="local", name="qiskit.shot_simulator"),
             create_device(location="local", name="vectorized"),
         ]:
-
             r = RQAOA()
             r.set_device(device)
             r.set_circuit_properties(
                 p=1, param_type="extended", init_type="rand", mixer_hamiltonian="x"
             )
             r.set_backend_properties(n_shots=50)
             r.set_classical_optimizer(maxiter=10, optimization_progress=True)
             r.set_rqaoa_parameters(rqaoa_type="adaptive", n_cutoff=3)
             r.set_exp_tags({"tag1": "value1", "tag2": "value2"})
             r.set_header(
                 project_id="8353185c-b175-4eda-9628-b4e58cb0e41b",
                 description="test",
-                run_by="raul",
+                run_by="OpenQAOA",
                 provider="-",
-                target="-",
+                target="vectorized",
                 cloud="local",
                 client="-",
             )
 
             # test that you can convert the rqaoa object to a dictionary and then load it before optimization
             _ = RQAOA.from_dict(r.asdict())
             _.compile(maxcut_qubo)
@@ -2268,17 +2550,17 @@
 
             # compile and optimize the original rqaoa object
             r.compile(maxcut_qubo)
             r.optimize()
 
             rqaoas.append(r)
 
-        # for each rqaoa object, create a new rqaoa object from dict, json string, json file, and compressed json file and compare them with the original object
+        # for each rqaoa object, create a new rqaoa object from dict, json string, json file,
+        # and compressed json file and compare them with the original object
         for r in rqaoas:
-
             new_r_list = []
 
             # get new qaoa from dict
             new_r_list.append(RQAOA.from_dict(r.asdict()))
             # get new qaoa from json string
             new_r_list.append(RQAOA.loads(r.dumps()))
             # get new qaoa from json file
@@ -2287,15 +2569,14 @@
             os.remove("test.json")  # delete file test.json
             # get new qaoa from compressed json file
             r.dump("test.json", prepend_id=False, compresslevel=3)
             new_r_list.append(RQAOA.load("test.json.gz"))
             os.remove("test.json.gz")  # delete file test.json
 
             for new_r in new_r_list:
-
                 # check that the new object is an RQAOA object
                 assert isinstance(new_r, RQAOA), "new_r is not an RQAOA object"
 
                 # check that the attributes of the new object are of the correct type
                 attributes_types = [
                     ("header", dict),
                     ("exp_tags", dict),
@@ -2362,10 +2643,30 @@
             Workflow.from_dict(r.asdict())
         except Exception:
             error = True
         assert (
             error
         ), "Optimizer.from_dict should raise an error when using a RQAOA dictionary"
 
+    def test_change_properties_after_compilation(self):
+        device = create_device(location="local", name="qiskit.shot_simulator")
+        r = RQAOA()
+        r.compile(QUBO.random_instance(4))
+
+        with self.assertRaises(ValueError):
+            r.set_device(device)
+        with self.assertRaises(ValueError):
+            r.set_circuit_properties(
+                p=1, param_type="standard", init_type="rand", mixer_hamiltonian="x"
+            )
+        with self.assertRaises(ValueError):
+            r.set_backend_properties(prepend_state=None, append_state=None)
+        with self.assertRaises(ValueError):
+            r.set_classical_optimizer(
+                maxiter=100, method="vgd", jac="finite_difference"
+            )
+        with self.assertRaises(ValueError):
+            r.set_rqaoa_parameters(rqaoa_type="adaptive", n_cutoff=3, n_steps=3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

