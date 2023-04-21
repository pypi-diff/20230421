# Comparing `tmp/pyrlprob-2.0.1.tar.gz` & `tmp/pyrlprob-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.0.1.tar", last modified: Wed Mar  8 23:14:16 2023, max compression
+gzip compressed data, was "pyrlprob-2.0.2.tar", last modified: Fri Apr 21 21:40:33 2023, max compression
```

## Comparing `pyrlprob-2.0.1.tar` & `pyrlprob-2.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.355705 pyrlprob-2.0.1/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/LICENSE.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/MANIFEST.in
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-03-08 23:14:16.354705 pyrlprob-2.0.1/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.1/README.md
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyproject.toml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.197705 pyrlprob-2.0.1/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/__main__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    14512 2023-03-08 18:19:48.000000 pyrlprob-2.0.1/pyrlprob/base_funs.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/commands.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.162712 pyrlprob-2.0.1/pyrlprob/include/
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.223708 pyrlprob-2.0.1/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/mdp.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/problem.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.239715 pyrlprob-2.0.1/pyrlprob/tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.272715 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.1/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1549 2023-03-08 18:35:25.000000 pyrlprob-2.0.1/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1238 2023-03-08 18:20:43.000000 pyrlprob-2.0.1/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.284705 pyrlprob-2.0.1/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.339720 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5262 2023-03-08 18:32:36.000000 pyrlprob-2.0.1/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.350727 pyrlprob-2.0.1/pyrlprob/utils/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4637 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.1/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-03-08 23:14:16.211711 pyrlprob-2.0.1/pyrlprob.egg-info/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-03-08 23:14:16.000000 pyrlprob-2.0.1/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-03-08 23:14:16.000000 pyrlprob-2.0.1/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-03-08 23:14:16.000000 pyrlprob-2.0.1/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-03-08 23:14:16.000000 pyrlprob-2.0.1/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-03-08 23:14:16.000000 pyrlprob-2.0.1/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-03-08 23:14:16.355719 pyrlprob-2.0.1/setup.cfg
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-03-08 22:31:10.000000 pyrlprob-2.0.1/setup.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.700507 pyrlprob-2.0.2/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/LICENSE.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/MANIFEST.in
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-21 21:40:33.698510 pyrlprob-2.0.2/PKG-INFO
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.2/README.md
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyproject.toml
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.462508 pyrlprob-2.0.2/pyrlprob/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/__main__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.2/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/commands.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.415509 pyrlprob-2.0.2/pyrlprob/include/
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.499506 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/mdp.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/problem.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.526506 pyrlprob-2.0.2/pyrlprob/tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.573509 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.2/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.590507 pyrlprob-2.0.2/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.675507 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.2/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.692508 pyrlprob-2.0.2/pyrlprob/utils/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     4709 2023-04-21 21:23:43.000000 pyrlprob-2.0.2/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.2/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-21 21:40:33.482508 pyrlprob-2.0.2/pyrlprob.egg-info/
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-04-21 21:40:33.000000 pyrlprob-2.0.2/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-04-21 21:40:33.700512 pyrlprob-2.0.2/setup.cfg
+-rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-04-21 21:40:04.000000 pyrlprob-2.0.2/setup.py
```

### Comparing `pyrlprob-2.0.1/LICENSE.txt` & `pyrlprob-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/PKG-INFO` & `pyrlprob-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.1
+Version: 2.0.2
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.1/README.md` & `pyrlprob-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/__main__.py` & `pyrlprob-2.0.2/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/base_funs.py` & `pyrlprob-2.0.2/pyrlprob/base_funs.py`

 * *Files 4% similar despite different names*

```diff
@@ -207,16 +207,32 @@
         env_inst = env_inst.env
         config["env"] = type(env_inst)
 
     # No learning
     config["lr"] = 0.
 
     # Evaluation and callbacks config
+    config["create_env_on_driver"] = False
     config["evaluation_interval"] = 1
-    config["evaluation_num_episodes"] = int(evaluation_num_episodes/config["num_envs_per_worker"])
+    config["evaluation_num_workers"] = max(config["evaluation_num_workers"], 1)
+    if evaluation_num_episodes % config["num_envs_per_worker"]:
+        if evaluation_num_episodes % config["evaluation_num_workers"]:
+            config["evaluation_num_episodes"] = evaluation_num_episodes
+            config["num_envs_per_worker"] = 1
+            config["evaluation_num_workers"] = 1
+        else:
+            config["evaluation_num_episodes"] = evaluation_num_episodes
+            config["num_envs_per_worker"] = 1
+    else:
+        if evaluation_num_episodes % config["evaluation_num_workers"]:
+            config["evaluation_num_episodes"] = int(evaluation_num_episodes/config["num_envs_per_worker"])
+            config["evaluation_num_workers"] = 1
+        else:
+            config["evaluation_num_episodes"] = int(evaluation_num_episodes/config["num_envs_per_worker"])
+        
     config["evaluation_config"] = evaluation_config
     if custom_eval_function is not None:
         if callable(custom_eval_function):
                 config["custom_eval_function"] = custom_eval_function
         else:
             mod_name, fun_name = custom_eval_function.rsplit('.',1)
             mod = importlib.import_module(mod_name)
```

### Comparing `pyrlprob-2.0.1/pyrlprob/commands.py` & `pyrlprob-2.0.2/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.0.2/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/mdp.py` & `pyrlprob-2.0.2/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/problem.py` & `pyrlprob-2.0.2/pyrlprob/problem.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.0.2/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/landing1d_load.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 config:
   batch_mode: complete_episodes
   callbacks: TrainingCallbacks
   clip_param: 0.2
+  create_env_on_driver: false
   env: pyrlprob.tests.py_tests.pyLanding1DEnv
   env_config:
     H: 40
     Tmax: 1.227
     c: 2.349
     g: 1.0
     h0_max: 1.2
@@ -15,16 +16,16 @@
     tf: 1.397
     v0_max: -0.75
     v0_min: -0.85
     vf: 0.0
   evaluation_config:
     explore: false
   evaluation_interval: 1
-  evaluation_num_episodes: 1
-  evaluation_num_workers: 0
+  evaluation_num_episodes: 2
+  evaluation_num_workers: 2
   explore: true
   framework: tf
   gamma: 1.0
   ignore_worker_failures: true
   kl_coeff: 0.0
   lambda: 1.0
   log_level: INFO
@@ -33,43 +34,43 @@
     fcnet_activation: tanh
     fcnet_hiddens:
     - 64
     - 64
     free_log_std: true
     vf_share_layers: false
   num_cpus_for_driver: 1
-  num_cpus_per_worker: 3
-  num_envs_per_worker: 12
+  num_cpus_per_worker: 1
+  num_envs_per_worker: 5
   num_gpus: 0
   num_gpus_per_worker: 0
   num_sgd_iter: 10
-  num_workers: 1
-  remote_worker_envs: true
+  num_workers: 2
+  remote_worker_envs: false
   rollout_fragment_length: 40
-  sgd_minibatch_size: 240
+  sgd_minibatch_size: 160
   shuffle_sequences: true
-  train_batch_size: 1920
+  train_batch_size: 400
   use_critic: true
   use_gae: true
   vf_loss_coeff: 0.5
 custom_metrics:
 - cstr_viol
 eval_env_config:
   env_config:
     prng_seed: 0
 load:
   prev_exp_dirs:
-  - /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-03-08_11-32-46/PPO_pyrlprob.tests.py_tests.pyLanding1DEnv_9f3b4_00000_0_2023-03-08_11-32-46/
+  - /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-04-21_14-36-15/PPO_pyrlprob.tests.py_tests.pyLanding1DEnv_8b2d9_00000_0_2023-04-21_14-36-15/
   prev_last_cps:
-  - 100
-  trainer_dir: /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-03-08_11-32-46/
-num_eval_episodes: 64
+  - 1
+  trainer_dir: /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-04-21_14-36-15/
+num_eval_episodes: 28
 postproc_data:
   episode_step_data:
   - h
   - v
   - m
   - t
   - T
 run: ppo
 stop:
-  training_iteration: 200
+  training_iteration: 2
```

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/landing1d_py.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 run: ppo
 stop:
-  training_iteration: 100
+  training_iteration: 50
 custom_metrics:
 - cstr_viol
 postproc_data:
   episode_step_data: 
   - h
   - v
   - m
   - t
   - T
-num_eval_episodes: 64
+num_eval_episodes: 10
 eval_env_config:
   env_config:
     prng_seed: 0
 config:
-  num_workers: 1
-  num_envs_per_worker: 12
+  num_workers: 2
+  num_envs_per_worker: 5
   num_gpus: 0
-  num_cpus_per_worker: 3
+  num_cpus_per_worker: 1
   num_gpus_per_worker: 0
   num_cpus_for_driver: 1
-  remote_worker_envs: True
+  create_env_on_driver: False
+  remote_worker_envs: False
   rollout_fragment_length: 40
   batch_mode: complete_episodes
-  train_batch_size: 1920
+  train_batch_size: 400
   model:
     fcnet_hiddens: [64, 64]
     fcnet_activation: tanh
     vf_share_layers: False
     free_log_std: True
   gamma: 1.
   log_level: INFO
   framework: tf
   explore: True
   ignore_worker_failures: True
   evaluation_interval: 1
-  evaluation_num_episodes: 1
+  evaluation_num_episodes: 2
   evaluation_config:
     explore: False
-  evaluation_num_workers: 0
+  evaluation_num_workers: 2
   use_critic: True
   use_gae: True
   lambda: 1.
   kl_coeff: 0.
-  sgd_minibatch_size: 240
+  sgd_minibatch_size: 160
   shuffle_sequences: True
   num_sgd_iter: 10
   lr: 1.0e-04
   vf_loss_coeff: 0.5
   clip_param: 0.2
   callbacks:
     TrainingCallbacks
```

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.0.2/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.0.2/pyrlprob/tests/test_landing1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     with open(os.path.join(__location__, "landing1d_load.yaml"), 'w') as outfile:
         yaml.dump(config_new_dict, outfile)
     
     #Training, evaluation and postprocessing of pre-trained model
     config_new = os.path.join(__location__, "landing1d_load.yaml")
     LandingProblemPretrained = RLProblem(config_new)
     trainer_dir, exp_dirs, last_cps, _ = \
-        LandingProblemPretrained.solve()
+        LandingProblemPretrained.solve(debug=False)
 
     #Plot of metric trend
     plt.style.use("seaborn")
     plt.style.use("seaborn")
     matplotlib.rc('font', size=20)
     fig = plot_metric("episode_reward",
                       exp_dirs,
```

### Comparing `pyrlprob-2.0.1/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.0.2/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/utils/__init__.py` & `pyrlprob-2.0.2/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.0.2/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob/utils/callbacks.py` & `pyrlprob-2.0.2/pyrlprob/utils/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
         info = episode.last_info_for()
 
         if info is not None:
             if "episode_step_data" in info:
                 for key in info["episode_step_data"].keys():
                     episode.hist_data[key] = episode.user_data[key]
                     episode.hist_data[key + "_length"] = [len(episode.user_data[key])]
+                    print("episode_step_data end callback: data added")
             if "episode_end_data" in info:
                 for key, item in info["episode_end_data"].items():
                     if isinstance(item, Iterable):
                         episode.hist_data[key] = [item[-1]]
                     else:
                         episode.hist_data[key] = [item]
             if "custom_metrics" in info:
```

### Comparing `pyrlprob-2.0.1/pyrlprob/utils/plots.py` & `pyrlprob-2.0.2/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.0.2/pyrlprob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.1
+Version: 2.0.2
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrlprob-2.0.1/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.0.2/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.1/setup.py` & `pyrlprob-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.0.1',
+    version='2.0.2',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
```

