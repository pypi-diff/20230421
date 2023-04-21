# Comparing `tmp/CUQIpy-0.3.0.tar.gz` & `tmp/CUQIpy-0.3.0.post0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-0.3.0.tar", last modified: Wed Feb 22 09:49:07 2023, max compression
+gzip compressed data, was "CUQIpy-0.3.0.post0.dev5.tar", last modified: Fri Apr 21 10:13:04 2023, max compression
```

## Comparing `CUQIpy-0.3.0.tar` & `CUQIpy-0.3.0.post0.dev5.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.363677 CUQIpy-0.3.0/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-02-22 09:49:07.000000 CUQIpy-0.3.0/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-02-22 09:49:07.000000 CUQIpy-0.3.0/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:49:07.000000 CUQIpy-0.3.0/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-22 09:49:07.000000 CUQIpy-0.3.0/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-22 09:49:07.000000 CUQIpy-0.3.0/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.363677 CUQIpy-0.3.0/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.367677 CUQIpy-0.3.0/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.367677 CUQIpy-0.3.0/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_cauchy_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_laplace_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.371677 CUQIpy-0.3.0/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52310 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:49:07.375677 CUQIpy-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    27722 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-22 09:48:56.000000 CUQIpy-0.3.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.658964 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-04-21 10:13:04.000000 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-21 10:13:04.000000 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:13:04.000000 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-21 10:13:04.000000 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 10:13:04.000000 CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.658964 CUQIpy-0.3.0.post0.dev5/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_cauchy_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_laplace_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.662964 CUQIpy-0.3.0.post0.dev5/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52310 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.666965 CUQIpy-0.3.0.post0.dev5/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:13:04.670965 CUQIpy-0.3.0.post0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-21 10:12:55.000000 CUQIpy-0.3.0.post0.dev5/tests/test_utilities.py
```

### Comparing `CUQIpy-0.3.0/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.3.0
+Version: 0.3.0.post0.dev5
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.3.0/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-0.3.0.post0.dev5/CUQIpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 cuqi/data/camera.npz
 cuqi/data/cat.npz
 cuqi/data/satellite.mat
 cuqi/density/__init__.py
 cuqi/density/_density.py
 cuqi/distribution/__init__.py
 cuqi/distribution/_beta.py
+cuqi/distribution/_cauchy.py
 cuqi/distribution/_cauchy_diff.py
 cuqi/distribution/_custom.py
 cuqi/distribution/_distribution.py
 cuqi/distribution/_gamma.py
 cuqi/distribution/_gaussian.py
 cuqi/distribution/_gmrf.py
 cuqi/distribution/_inverse_gamma.py
```

### Comparing `CUQIpy-0.3.0/LICENSE` & `CUQIpy-0.3.0.post0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/PKG-INFO` & `CUQIpy-0.3.0.post0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.3.0
+Version: 0.3.0.post0.dev5
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.3.0/README.md` & `CUQIpy-0.3.0.post0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/array/_array.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/array/_array.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/config.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/data/_data.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/data/astronaut.npz` & `CUQIpy-0.3.0.post0.dev5/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/data/camera.npz` & `CUQIpy-0.3.0.post0.dev5/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/data/cat.npz` & `CUQIpy-0.3.0.post0.dev5/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/data/satellite.mat` & `CUQIpy-0.3.0.post0.dev5/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/density/_density.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/diagnostics.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_beta.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_cauchy_diff.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_cauchy_diff.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_custom.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_custom.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_distribution.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_gamma.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_gaussian.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gaussian.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_gmrf.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_gmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_joint_distribution.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_laplace.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_laplace_diff.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_laplace_diff.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_lmrf.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_lmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_lognormal.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_normal.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_posterior.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/distribution/_uniform.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/geometry/__init__.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/geometry/_geometry.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/likelihood/__init__.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/likelihood/_likelihood.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/likelihood/_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/model/_model.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/model/_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/operator/_operator.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/pde/_pde.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/pde/_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/problem/_problem.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/problem/_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_conjugate.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_conjugate_approx.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_cwmh.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_gibbs.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_hmc.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_mh.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_pcn.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_rto.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/sampler/_sampler.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/sampler/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/samples/_samples.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/samples/_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/solver/_solver.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/testproblem/_testproblem.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/testproblem/_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/cuqi/utilities/_utilities.py` & `CUQIpy-0.3.0.post0.dev5/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/pyproject.toml` & `CUQIpy-0.3.0.post0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_abstract_distribution_density.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_abstract_distribution_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_bayesian_inversion.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_bayesian_inversion.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_density.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_distribution.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from math import isnan
 import cuqi
 import numpy as np
 import scipy as sp
+import scipy.stats as scipy_stats
 import scipy.sparse as sps
 
 from pytest import approx
 import pytest
 
 def test_Normal_mean_standard():
     assert cuqi.distribution.Normal(0,1).mean == approx(0.0)
@@ -631,7 +632,38 @@
 def test_Laplace_diff_should_not_allow_non_zero_location():
     """" Laplace_diff should not allow non-zero location. """
     with pytest.raises(ValueError):
         cuqi.distribution.Laplace_diff(np.ones(5), 1)
 
     with pytest.raises(ValueError):
         cuqi.distribution.Laplace_diff(lambda x: x, 1)
+
+def test_Cauchy_against_scipy():
+    """ Test Cauchy distribution logpdf, cdf, pdf, gradient """
+
+    x = cuqi.distribution.Cauchy(np.random.randn(5), np.abs(np.random.rand(5)))
+
+    val = np.random.randn(5)
+
+    # Test logpdf
+    assert np.allclose(x.logpdf(val), np.sum(scipy_stats.cauchy.logpdf(val, loc=x.location, scale=x.scale)))
+
+    # Test pdf
+    assert np.allclose(x.pdf(val), np.prod(scipy_stats.cauchy.pdf(val, loc=x.location, scale=x.scale)))
+
+    # Test cdf
+    assert np.allclose(x.cdf(val), np.sum(scipy_stats.cauchy.cdf(val, loc=x.location, scale=x.scale)))
+
+    # Test gradient
+    assert np.allclose(x.gradient(val), cuqi.utilities.approx_derivative(x.logpdf, val))
+
+def test_Cauchy_out_of_range_values():
+    """ Test that the logpdf is -inf for values outside the support """
+
+    x = cuqi.distribution.Cauchy(np.random.randn(5), np.abs(np.random.rand(5)))
+
+    x.scale[0] = 0 # This is not a valid scale
+
+    val = np.random.randn(5)
+
+    # Test logpdf
+    assert np.allclose(x.logpdf(val), -np.inf)
```

### Comparing `CUQIpy-0.3.0/tests/test_geometry.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_joint_distribution.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_likelihood.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_model.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_pde.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_pde.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_problem.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_sampler.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_samples.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_solver.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_testproblem.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.3.0/tests/test_utilities.py` & `CUQIpy-0.3.0.post0.dev5/tests/test_utilities.py`

 * *Files identical despite different names*

