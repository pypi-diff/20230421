# Comparing `tmp/jaxsim-0.1.dev118.tar.gz` & `tmp/jaxsim-0.1.dev135.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev118.tar", last modified: Fri Nov 11 09:56:44 2022, max compression
+gzip compressed data, was "jaxsim-0.1.dev135.tar", last modified: Fri Apr 21 08:24:38 2023, max compression
```

## Comparing `jaxsim-0.1.dev118.tar` & `jaxsim-0.1.dev135.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.991368 jaxsim-0.1.dev118/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.995368 jaxsim-0.1.dev118/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (122)      915 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1547 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3585 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1856 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.991368 jaxsim-0.1.dev118/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.995368 jaxsim-0.1.dev118/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.995368 jaxsim-0.1.dev118/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (122)     8180 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (122)    33459 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1962 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (122)     2010 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2006 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1564 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    18797 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10928 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5666 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.999368 jaxsim-0.1.dev118/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6180 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (122)     4075 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (122)     9028 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (122)    11035 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4538 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10365 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (122)     8505 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4026 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)    10213 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1374 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      330 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:44.003369 jaxsim-0.1.dev118/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      731 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2022-11-11 09:56:23.000000 jaxsim-0.1.dev118/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-11 09:56:43.995368 jaxsim-0.1.dev118/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      207 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-11 09:56:43.000000 jaxsim-0.1.dev118/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33921 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev118/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev135/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/.gitignore` & `jaxsim-0.1.dev135/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/LICENSE` & `jaxsim-0.1.dev135/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/PKG-INFO` & `jaxsim-0.1.dev135/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev118
+Version: 0.1.dev135
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -53,14 +53,16 @@
 - Support of SDF models (and, upon conversion, URDF models).
 - Collision detection between bodies and uneven ground surface.
 - Continuous soft contacts model with no friction cone approximations.
 - Full support of inertial properties of bodies.
 - Revolute, prismatic, and fixed joints support.
 - Integrators: forward Euler, semi-implicit Euler, Runge-Kutta 4.
 - High-level classes to compute multi-body dynamics quantities from simulation state.
+- High-level classes supporting both object-oriented and functional programming.
+- Optional validation of JAX pytrees to prevent JIT re-compilation. 
 
 Planned features:
 
 - Reinforcement Learning module developed in JAX.
 - Finalization of differentiable physics through the simulation.
 
 [jax]: https://github.com/google/jax/
@@ -107,14 +109,25 @@
 [PFS]: http://sdformat.org/tutorials?tut=pose_frame_semantics
 
 ## Contributing
 
 Pull requests are welcome. 
 For major changes, please open an issue first to discuss what you would like to change.
 
+## Citing
+
+```bibtex
+@software{ferigo_jaxsim_2022,
+  author = {Diego Ferigo and Silvio Traversaro and Daniele Pucci},
+  title = {{JAXsim}: A Physics Engine in Reduced Coordinates for Control and Robot Learning},
+  url = {http://github.com/ami-iit/jaxsin},
+  year = {2022},
+}
+```
+
 ## Maintainers
 
 | [<img src="https://github.com/diegoferigo.png" width="40">][df] | [@diegoferigo][df] |
 |:---------------------------------------------------------------:|:------------------:|
 
 [df]: https://github.com/diegoferigo
```

### Comparing `jaxsim-0.1.dev118/README.md` & `jaxsim-0.1.dev135/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 - Support of SDF models (and, upon conversion, URDF models).
 - Collision detection between bodies and uneven ground surface.
 - Continuous soft contacts model with no friction cone approximations.
 - Full support of inertial properties of bodies.
 - Revolute, prismatic, and fixed joints support.
 - Integrators: forward Euler, semi-implicit Euler, Runge-Kutta 4.
 - High-level classes to compute multi-body dynamics quantities from simulation state.
+- High-level classes supporting both object-oriented and functional programming.
+- Optional validation of JAX pytrees to prevent JIT re-compilation. 
 
 Planned features:
 
 - Reinforcement Learning module developed in JAX.
 - Finalization of differentiable physics through the simulation.
 
 [jax]: https://github.com/google/jax/
@@ -69,14 +71,25 @@
 [PFS]: http://sdformat.org/tutorials?tut=pose_frame_semantics
 
 ## Contributing
 
 Pull requests are welcome. 
 For major changes, please open an issue first to discuss what you would like to change.
 
+## Citing
+
+```bibtex
+@software{ferigo_jaxsim_2022,
+  author = {Diego Ferigo and Silvio Traversaro and Daniele Pucci},
+  title = {{JAXsim}: A Physics Engine in Reduced Coordinates for Control and Robot Learning},
+  url = {http://github.com/ami-iit/jaxsin},
+  year = {2022},
+}
+```
+
 ## Maintainers
 
 | [<img src="https://github.com/diegoferigo.png" width="40">][df] | [@diegoferigo][df] |
 |:---------------------------------------------------------------:|:------------------:|
 
 [df]: https://github.com/diegoferigo
```

### Comparing `jaxsim-0.1.dev118/setup.cfg` & `jaxsim-0.1.dev135/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/__init__.py` & `jaxsim-0.1.dev135/src/jaxsim/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,37 @@
-from . import high_level, logging, math, sixd
+from . import logging
+
+
+# Follow upstream development in https://github.com/google/jax/pull/13304
+def _jnp_options() -> None:
+
+    import os
+
+    from jax.config import config
+
+    # Enable by default
+    if not ("JAX_ENABLE_X64" in os.environ and os.environ["JAX_ENABLE_X64"] == "0"):
+        logging.info("Enabling JAX to use 64bit precision")
+        config.update("jax_enable_x64", True)
 
+        import jax.numpy as jnp
+        import numpy as np
+
+        if jnp.empty(0, dtype=float).dtype != jnp.empty(0, dtype=np.float64).dtype:
+            logging.warning("Failed to enable 64bit precision in JAX")
+
+
+def _np_options() -> None:
 
-def _np_options():
     import numpy as np
 
     np.set_printoptions(precision=5, suppress=True, linewidth=150, threshold=10_000)
 
 
-def _is_editable():
+def _is_editable() -> bool:
 
     import importlib.util
     import pathlib
     import site
 
     # Get the ModuleSpec of jaxsim
     jaxsim_spec = importlib.util.find_spec(name="jaxsim")
@@ -29,12 +49,19 @@
 
 # Initialize the logging verbosity
 if _is_editable():
     logging.configure(level=logging.LoggingLevel.DEBUG)
 else:
     logging.configure(level=logging.LoggingLevel.WARNING)
 
+# Configure JAX
+_jnp_options()
+
 # Initialize the numpy print options
 _np_options()
 
+del _jnp_options
 del _np_options
 del _is_editable
+
+from . import high_level, logging, math, sixd
+from .simulation.simulator import JaxSim
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev135/src/jaxsim/high_level/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev135/src/jaxsim/high_level/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev135/src/jaxsim/high_level/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import pathlib
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Tuple, Union, Any
 
 import jax.experimental.ode
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
 
 import jaxsim
@@ -71,14 +71,15 @@
     tf_model_state: jaxsim.physics.model.physics_model_state.PhysicsModelState = (
         dataclasses.field(repr=False)
     )
     tf_contact_state: jaxsim.physics.algos.soft_contacts.SoftContactsState = (
         dataclasses.field(repr=False)
     )
 
+    aux: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
 @jax_dataclasses.pytree_dataclass
 class Model(JaxsimDataclass):
 
     model_name: str = jax_dataclasses.static_field()
     physics_model: physics.model.physics_model.PhysicsModel = dataclasses.field(
         repr=False
@@ -756,14 +757,17 @@
 
         if joint_names is None:
             joint_names = self.joint_names()
 
         if positions.size != len(joint_names):
             raise ValueError("Wrong arguments size", positions.size, len(joint_names))
 
+        if positions.size == 0:
+            return
+
         # TODO: joint position limits
 
         self.data.model_state.joint_positions = (
             self.data.model_state.joint_positions.at[
                 self._joint_indices(joint_names=joint_names)
             ].set(positions)
         )
@@ -774,14 +778,17 @@
 
         if joint_names is None:
             joint_names = self.joint_names()
 
         if velocities.size != len(joint_names):
             raise ValueError("Wrong arguments size", velocities.size, len(joint_names))
 
+        if velocities.size == 0:
+            return
+
         # TODO: joint velocity limits
 
         self.data.model_state.joint_velocities = (
             self.data.model_state.joint_velocities.at[
                 self._joint_indices(joint_names=joint_names)
             ].set(velocities)
         )
@@ -941,14 +948,24 @@
             dt=(tf - t0),
             t0_model_data=t0_model_data,
             t0_model_input_real=t0_model_input_real.physics_model,
             t0_base_acceleration=t0_model_acceleration[0:6],
             t0_joint_acceleration=t0_model_acceleration[6:],
             tf_model_state=tf_model_state,
             tf_contact_state=tf_contact_state,
+            aux={
+                "t0": jax.tree_util.tree_map(
+                    lambda l: l[0],
+                    aux,
+                ),
+                "tf": jax.tree_util.tree_map(
+                    lambda l: l[-1],
+                    aux,
+                ),
+            },
         )
 
     # ===============
     # Private methods
     # ===============
 
     def inertial_to_active_representation(
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/logging.py` & `jaxsim-0.1.dev135/src/jaxsim/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     info("Configuring the 'jaxsim' logger")
 
     handler = logging.StreamHandler()
     fmt = "%(name)s[%(process)d] %(levelname)s %(message)s"
     handler.setFormatter(fmt=coloredlogs.ColoredFormatter(fmt=fmt))
     _logger().addHandler(hdlr=handler)
 
-    # Workaround for double logging caused by abseil handlers
-    # https://github.com/abseil/abseil-py/issues/99
+    # Do not propagate the messages to handlers of parent loggers
+    # (preventing duplicate logging)
     _logger().propagate = False
 
     set_logging_level(level=level)
 
 
 def debug(msg: str = "") -> None:
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev135/src/jaxsim/math/adjoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -69,7 +69,20 @@
             [
                 [R, Skew.vee(matrix=o_x_R @ R.T)],
                 [0, 0, 0, 1],
             ]
         )
 
         return H
+
+    @staticmethod
+    def inverse(adjoint: jtp.Matrix) -> jtp.Matrix:
+
+        A_X_B = adjoint
+        A_H_B = Adjoint.to_transform(adjoint=A_X_B)
+
+        A_R_B = A_H_B[0:3, 0:3]
+        A_o_B = A_H_B[0:3, 3]
+
+        return Adjoint.from_rotation_and_translation(
+            rotation=A_R_B, translation=A_o_B, inverse=True
+        )
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev135/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev135/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev135/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev135/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev135/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev135/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev135/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev135/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/parser.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,36 +40,28 @@
         raise RuntimeError("Failed to find any model in SDF resource")
 
     # Assume the SDF resource has only one model, or the desired model name is given
     sdf_models = {m.name: m for m in sdf_element.models()}
     sdf_model = (
         sdf_element.models()[0] if len(sdf_models) == 1 else sdf_models[model_name]
     )
-    logging.debug(msg=f"Found model '{sdf_model.name}' in SDF resource")
 
-    # Detect fixed-base models by checking the existence of joints having world as parent
-    sdf_joints_with_world_parent = [
-        j for j in sdf_model.joints() if j.parent == "world"
-    ]
-    fixed_base = len(sdf_joints_with_world_parent) > 0
+    # Log model name
+    logging.debug(msg=f"Found model '{sdf_model.name}' in SDF resource")
 
+    # Log type of base link
     logging.debug(
         msg="Model '{}' is {}".format(
-            sdf_model.name, "fixed-base" if fixed_base else "floating-base"
+            sdf_model.name,
+            "fixed-base" if sdf_model.is_fixed_base() else "floating-base",
         )
     )
 
-    # We extract the link connected to 'world', and consider it as base link.
-    # Instead, for floating-base models, we consider the first link as base link.
-    base_link_name = (
-        sdf_joints_with_world_parent[0].name
-        if fixed_base
-        else sdf_model.links()[0].name
-    )
-    logging.debug(msg=f"Considering '{base_link_name}' as base link")
+    # Log detected base link
+    logging.debug(msg=f"Considering '{sdf_model.get_canonical_link()}' as base link")
 
     # Pose of the model
     if sdf_model.pose is None:
         model_pose = kinematic_graph.RootPose()
 
     else:
         W_H_M = sdf_model.pose.transform()
@@ -99,15 +91,15 @@
 
     # =========================
     # Process fixed-base models
     # =========================
 
     # In this case, we need to get the pose of the joint that connects the base link
     # to the world and combine their pose
-    if fixed_base:
+    if sdf_model.is_fixed_base():
 
         # Create a massless word link
         world_link = descriptions.LinkDescription(
             name="world", mass=0, inertia=np.zeros(shape=(6, 6))
         )
 
         # Gather joints connecting fixed-base models to the world.
@@ -237,15 +229,15 @@
 
         if l.name not in links_dict:
             continue
 
         if l.pose is None:
             continue
 
-        if l.name == base_link_name:
+        if l.name == sdf_model.get_canonical_link():
             continue
 
         if l.name not in joint_dict:
             raise ValueError(f"Failed to find parent joint of link '{l.name}'")
 
         if l.pose.relative_to != joint_dict[l.name]:
             msg = "Pose of link '{}' is not expressed wrt its parent joint '{}'"
@@ -281,16 +273,16 @@
                 collisions.append(sphere_collision)
 
     return SDFData(
         model_name=sdf_model.name,
         link_descriptions=links,
         joint_descriptions=joints,
         collision_shapes=collisions,
-        fixed_base=fixed_base,
-        base_link_name=base_link_name,
+        fixed_base=sdf_model.is_fixed_base(),
+        base_link_name=sdf_model.get_canonical_link(),
         model_pose=model_pose,
         sdf_model=sdf_model,
     )
 
 
 def build_model_from_sdf(sdf: Union[Path, str]) -> descriptions.ModelDescription:
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/parsers/sdf/utils.py` & `jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ) -> Tuple[PropagateKinematicsCarry, None]:
 
         i_X_λi, W_X_i = carry
 
         i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
         i_X_λi = i_X_λi.at[i].set(i_X_λi_i)
 
-        W_X_i_i = W_X_i[λ[i]] @ jnp.linalg.inv(i_X_λi[i])
+        W_X_i_i = W_X_i[λ[i]] @ Adjoint.inverse(i_X_λi[i])
         W_X_i = W_X_i.at[i].set(W_X_i_i)
 
         return (i_X_λi, W_X_i), None
 
     (_, W_X_i), _ = jax.lax.scan(
         f=propagate_kinematics,
         init=propagate_kinematics_carry,
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import jaxsim.parsers
 import jaxsim.physics
 import jaxsim.typing as jtp
 from jaxsim.parsers.descriptions import JointDescriptor, JointType
 from jaxsim.physics import default_gravity
 from jaxsim.sixd import se3
-from jaxsim.utils import JaxsimDataclass, tracing
+from jaxsim.utils import JaxsimDataclass, not_tracing
 
 from .ground_contact import GroundContact
 from .physics_model_state import PhysicsModelState
 
 
 @pytree_dataclass
 class PhysicsModel(JaxsimDataclass):
@@ -56,15 +56,15 @@
             initial_state = PhysicsModelState.zero(physics_model=self)
             object.__setattr__(self, "initial_state", initial_state)
 
     @staticmethod
     def build_from(
         model_description: jaxsim.parsers.descriptions.model.ModelDescription,
         gravity: jtp.Vector = default_gravity(),
-    ):
+    ) -> "PhysicsModel":
 
         if gravity.size != 3:
             raise ValueError(gravity.size)
 
         # Currently, we assume that the link frame matches the frame of its parent joint
         for l in model_description:
             if not jnp.allclose(l.pose, jnp.eye(4)):
@@ -175,15 +175,15 @@
             _joint_friction_static=joint_friction_static,
             _joint_friction_viscous=joint_friction_viscous,
             _joint_limit_spring=joint_limit_spring,
             _joint_limit_damper=joint_limit_damper,
             gravity=jnp.hstack([gravity.squeeze(), np.zeros(3)]),
             is_floating_base=True,
             gc=GroundContact.build_from(model_description=model_description),
-            description=(model_description),
+            description=model_description,
         )
 
         # Floating-base models
         if not model_description.fixed_base:
             return physics_model
 
         # Fixed-base models
@@ -273,16 +273,17 @@
 
         return self._jtype_dict[joint_index]
 
     def joint_transforms(self, q: jtp.Vector) -> jtp.Array:
 
         from jaxsim.math.joint import jcalc
 
-        if not tracing(q) and q.shape[0] != self.dofs():
-            raise ValueError(q.shape)
+        if not_tracing(q):
+            if q.shape[0] != self.dofs():
+                raise ValueError(q.shape)
 
         Xj = jnp.stack(
             [jnp.zeros(shape=(6, 6))]
             + [
                 jcalc(jtyp=self.jtype(index + 1), q=joint_position)[0]
                 for index, joint_position in enumerate(q)
             ]
@@ -290,16 +291,17 @@
 
         return Xj
 
     def motion_subspaces(self, q: jtp.Vector) -> jtp.Array:
 
         from jaxsim.math.joint import jcalc
 
-        if not tracing(q) and q.shape[0] != self.dofs():
-            raise ValueError(q.shape)
+        if not_tracing(var=q):
+            if q.shape[0] != self.dofs():
+                raise ValueError(q.shape)
 
         SS = jnp.stack(
             [jnp.vstack(jnp.zeros(6))]
             + [
                 jcalc(jtyp=self.jtype(index + 1), q=joint_position)[1]
                 for index, joint_position in enumerate(q)
             ]
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/integrators.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/ode.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 def compute_contact_forces(
     physics_model: PhysicsModel,
     ode_state: ode_data.ODEState,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[jtp.Matrix, jtp.Matrix, jtp.Matrix]:
 
-    # Compute position and linear velocity (inertial representation)
-    # of all model's collidable points
+    # Compute position and linear mixed velocity of all model's collidable points
+    # collidable_points_kinematics
     pos_cp, vel_cp = collidable_points_pos_vel(
         model=physics_model,
         q=ode_state.physics_model.joint_positions,
         qd=ode_state.physics_model.joint_velocities,
         xfb=ode_state.physics_model.xfb(),
     )
 
@@ -105,43 +105,51 @@
             terrain=terrain,
         )
 
     # =====================
     # Joint position limits
     # =====================
 
-    # Get the joint position limits
-    s_min, s_max = jnp.array(
-        [j.position_limit for j in physics_model.description.joints_dict.values()]
-    ).T
-
-    # Get the spring/damper parameters of joint limits enforcement
-    # k_spring = jnp.array(list(physics_model._joint_limit_spring.values()))
-    k_damper = jnp.array(list(physics_model._joint_limit_damper.values()))
-
-    # Compute the joint torques that enforce joint limits
-    s = ode_state.physics_model.joint_positions
-    # sd = ode_state.physics_model.joint_velocities
-    tau_min = jnp.where(s <= s_min, k_damper * (s_min - s), 0)
-    tau_max = jnp.where(s >= s_max, k_damper * (s_max - s), 0)
-    tau_limit = tau_max + tau_min
+    if physics_model.dofs() > 0:
+
+        # Get the joint position limits
+        s_min, s_max = jnp.array(
+            [j.position_limit for j in physics_model.description.joints_dict.values()]
+        ).T
+
+        # Get the spring/damper parameters of joint limits enforcement
+        k_damper = jnp.array(list(physics_model._joint_limit_damper.values()))
+
+        # Compute the joint torques that enforce joint limits
+        s = ode_state.physics_model.joint_positions
+        tau_min = jnp.where(s <= s_min, k_damper * (s_min - s), 0)
+        tau_max = jnp.where(s >= s_max, k_damper * (s_max - s), 0)
+        tau_limit = tau_max + tau_min
+
+    else:
+        tau_limit = jnp.zeros_like(ode_input.physics_model.tau)
 
     # ==============
     # Joint friction
     # ==============
 
-    # Static and viscous joint friction parameters
-    kc = jnp.array(list(physics_model._joint_friction_static.values()))
-    kv = jnp.array(list(physics_model._joint_friction_viscous.values()))
-
-    # Compute the joint friction torque
-    tau_friction = -(
-        jnp.diag(kc) @ jnp.sign(ode_state.physics_model.joint_positions)
-        + jnp.diag(kv) @ ode_state.physics_model.joint_velocities
-    )
+    if physics_model.dofs() > 0:
+
+        # Static and viscous joint friction parameters
+        kc = jnp.array(list(physics_model._joint_friction_static.values()))
+        kv = jnp.array(list(physics_model._joint_friction_viscous.values()))
+
+        # Compute the joint friction torque
+        tau_friction = -(
+            jnp.diag(kc) @ jnp.sign(ode_state.physics_model.joint_positions)
+            + jnp.diag(kv) @ ode_state.physics_model.joint_velocities
+        )
+
+    else:
+        tau_friction = jnp.zeros_like(ode_input.physics_model.tau)
 
     # ========================
     # Compute forward dynamics
     # ========================
 
     # Compute the total forces applied to the bodies
     total_forces = ode_input.physics_model.f_ext + contact_forces_links
@@ -237,13 +245,14 @@
     W_nud_WB = jnp.hstack([W_a_WB.squeeze(), qdd.squeeze()])
 
     # Build the auxiliary data
     aux_dict = dict(
         model_acceleration=W_nud_WB,
         ode_input=ode_input,
         ode_input_real=ode_input_real,
+        contact_forces_links=contact_forces_links,
         contact_forces_points=contact_forces_points,
         tangential_deformation_dot=tangential_deformation_dot,
     )
 
     # Return the state derivative as a generic PyTree, and the dict with auxiliary info
     return state_derivative, aux_dict
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 import jax
 import jax.numpy as jnp
 import jax_dataclasses
 
 import jaxsim.high_level
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.physics
+import jaxsim.simulation.simulator_callbacks as scb
 import jaxsim.typing as jtp
 from jaxsim.high_level.common import VelRepr
 from jaxsim.high_level.model import Model, StepData
 from jaxsim.physics.algos.soft_contacts import SoftContactsParams
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.physics.model.physics_model import PhysicsModel
-from jaxsim.simulation import ode_integration, simulator_callbacks
+from jaxsim.simulation import ode_integration
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
-class SimulatorData:
+class SimulatorData(JaxsimDataclass):
 
     # Simulation time stored in ns in order to prevent floats approximation
-    time_ns: jtp.Int = jnp.array(0, dtype=int)
+    time_ns: jtp.Int = jnp.array(0, dtype=jnp.int64)
 
     # Terrain and contact parameters
     terrain: Terrain = jax_dataclasses.field(default_factory=lambda: FlatTerrain())
     contact_parameters: SoftContactsParams = jax_dataclasses.field(
         default_factory=lambda: SoftContactsParams()
     )
 
@@ -42,15 +43,15 @@
 
 
 @jax_dataclasses.pytree_dataclass
 class JaxSim(JaxsimDataclass):
 
     # Step size stored in ns in order to prevent floats approximation
     step_size_ns: jtp.Int = jax_dataclasses.field(
-        default_factory=lambda: jnp.array(1_000_000, dtype=int)
+        default_factory=lambda: jnp.array(1_000_000, dtype=jnp.int64)
     )
 
     # Number of substeps performed at each integration step
     steps_per_run: jtp.Int = jax_dataclasses.static_field(default=1)
 
     # Default velocity representation (could be overridden for individual models)
     velocity_representation: VelRepr = jax_dataclasses.field(default=VelRepr.Inertial)
@@ -69,15 +70,15 @@
         steps_per_run: jtp.Int = 1,
         velocity_representation: VelRepr = VelRepr.Inertial,
         integrator_type: ode_integration.IntegratorType = ode_integration.IntegratorType.EulerSemiImplicit,
         simulator_data: SimulatorData = None,
     ) -> "JaxSim":
 
         return JaxSim(
-            step_size_ns=jnp.array(step_size * 1e9, dtype=int),
+            step_size_ns=jnp.array(step_size * 1e9, dtype=jnp.int64),
             steps_per_run=int(steps_per_run),
             velocity_representation=velocity_representation,
             integrator_type=integrator_type,
             data=simulator_data if simulator_data is not None else SimulatorData(),
         )
 
     def reset(self, remove_models: bool = True) -> None:
@@ -87,15 +88,15 @@
         if remove_models:
             self.data.models = dict()
         else:
             _ = [m.zero() for m in self.models()]
 
     def set_step_size(self, step_size: float) -> None:
 
-        self.step_size_ns = jnp.array(step_size * 1e9, dtype=int)
+        self.step_size_ns = jnp.array(step_size * 1e9, dtype=jnp.int64)
 
     def dt(self) -> jtp.Float:
 
         return (self.step_size_ns * self.steps_per_run) / 1e9
 
     def time(self) -> jtp.Float:
 
@@ -138,28 +139,35 @@
     def insert_model_from_sdf(
         self,
         sdf: Union[pathlib.Path, str],
         model_name: str = None,
         considered_joints: List[str] = None,
     ) -> Model:
 
+        # Build the model from the input SDF resource
         model = jaxsim.high_level.model.Model.build_from_sdf(
             sdf=sdf,
             model_name=model_name,
             vel_repr=self.velocity_representation,
             considered_joints=considered_joints,
         )
 
-        if model_name in self.model_names():
-            msg = f"Model '{model_name}' is already part of the simulation"
+        # Make sure the model is not already part of the simulation
+        if model.name() in self.model_names():
+            msg = f"Model '{model.name()}' is already part of the simulation"
             raise ValueError(msg)
 
+        # Insert the model
         self.data.models[model.name()] = model
+
+        # Propagate the current mutability property to make sure that also the
+        # newly inserted model matches the mutability of the simulator
         self._set_mutability(self._mutability())
 
+        # Return the newly inserted model
         return self.data.models[model.name()]
 
     def insert_model(
         self, model_description: descriptions.ModelDescription, model_name: str = None
     ) -> Model:
 
         model_name = model_name if model_name is not None else model_description.name
@@ -190,16 +198,16 @@
             raise ValueError(msg)
 
         self.data.models.pop(model_name)
         self._set_mutability(self._mutability())
 
     def step(self, clear_inputs: bool = False) -> Dict[str, StepData]:
 
-        t0_ns = jnp.array(self.data.time_ns, dtype=int)
-        dt_ns = jnp.array(self.step_size_ns * self.steps_per_run, dtype=int)
+        t0_ns = jnp.array(self.data.time_ns, dtype=jnp.int64)
+        dt_ns = jnp.array(self.step_size_ns * self.steps_per_run, dtype=jnp.int64)
 
         tf_ns = t0_ns + dt_ns
 
         # We collect the StepData of all models
         step_data = dict()
 
         for model in self.models():
@@ -224,50 +232,48 @@
         return step_data
 
     @functools.partial(jax.jit, static_argnames=["horizon_steps"])
     def step_over_horizon(
         self,
         horizon_steps: jtp.Int,
         callback_handler: Union[
-            "simulator_callbacks.SimulatorCallback",
-            "simulator_callbacks.CallbackHandler",
+            "scb.SimulatorCallback",
+            "scb.CallbackHandler",
         ] = None,
         clear_inputs: jtp.Bool = False,
-    ) -> Union[
-        "JaxSim",
-        Tuple["JaxSim", Tuple["simulator_callbacks.SimulatorCallback", jtp.PyTree]],
-    ]:
+    ) -> Union["JaxSim", Tuple["JaxSim", Tuple["scb.SimulatorCallback", jtp.PyTree]]]:
+        """"""
 
         # Process a mutable copy of the simulator
         original_mutability = self._mutability()
         sim = self.copy().mutable(validate=True)
 
         # Helper to get callbacks from the handler
         get_cb = (
             lambda h, cb_name: getattr(h, cb_name)
             if h is not None and hasattr(h, cb_name)
             else None
         )
 
         # Get the callbacks
-        configure_cb: Optional[simulator_callbacks.ConfigureCallbackSignature] = get_cb(
+        configure_cb: Optional[scb.ConfigureCallbackSignature] = get_cb(
             h=callback_handler, cb_name="configure_cb"
         )
-        pre_step_cb: Optional[simulator_callbacks.PreStepCallbackSignature] = get_cb(
+        pre_step_cb: Optional[scb.PreStepCallbackSignature] = get_cb(
             h=callback_handler, cb_name="pre_step_cb"
         )
-        post_step_cb: Optional[simulator_callbacks.PostStepCallbackSignature] = get_cb(
+        post_step_cb: Optional[scb.PostStepCallbackSignature] = get_cb(
             h=callback_handler, cb_name="post_step_cb"
         )
 
         # Callback: configuration
         sim = configure_cb(sim) if configure_cb is not None else sim
 
         # Initialize the carry
-        Carry = Tuple[JaxSim, simulator_callbacks.CallbackHandler]
+        Carry = Tuple[JaxSim, scb.CallbackHandler]
         carry_init: Carry = (sim, callback_handler)
 
         def body_fun(carry: Carry, xs: None) -> Tuple[Carry, jtp.PyTree]:
 
             sim, callback_handler = carry
 
             # Make sure to pass a mutable version of the simulator to the callbacks
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev135/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 import abc
 from typing import Callable, Dict, Tuple
 
+import jaxsim
 import jaxsim.typing as jtp
 from jaxsim.high_level.model import StepData
-from jaxsim.simulation.simulator import JaxSim
 
-ConfigureCallbackSignature = Callable[[JaxSim], JaxSim]
-PreStepCallbackSignature = Callable[[JaxSim], JaxSim]
+ConfigureCallbackSignature = Callable[["jaxsim.JaxSim"], "jaxsim.JaxSim"]
+PreStepCallbackSignature = Callable[["jaxsim.JaxSim"], "jaxsim.JaxSim"]
 PostStepCallbackSignature = Callable[
-    [JaxSim, Dict[str, StepData]], Tuple[JaxSim, jtp.PyTree]
+    ["jaxsim.JaxSim", Dict[str, StepData]], Tuple["jaxsim.JaxSim", jtp.PyTree]
 ]
 
 
 class SimulatorCallback(abc.ABC):
     pass
 
 
 class ConfigureCallback(SimulatorCallback):
     @property
     def configure_cb(self) -> ConfigureCallbackSignature:
 
         return lambda sim: self.configure(sim=sim)
 
     @abc.abstractmethod
-    def configure(self, sim: JaxSim) -> JaxSim:
+    def configure(self, sim: "jaxsim.JaxSim") -> "jaxsim.JaxSim":
         pass
 
 
 class PreStepCallback(SimulatorCallback):
     @property
     def pre_step_cb(self) -> PreStepCallbackSignature:
 
         return lambda sim: self.pre_step(sim=sim)
 
     @abc.abstractmethod
-    def pre_step(self, sim: JaxSim) -> JaxSim:
+    def pre_step(self, sim: "jaxsim.JaxSim") -> "jaxsim.JaxSim":
         pass
 
 
 class PostStepCallback(SimulatorCallback):
     @property
     def post_step_cb(self) -> PostStepCallbackSignature:
 
         return lambda sim, step_data: self.post_step(sim=sim, step_data=step_data)
 
     @abc.abstractmethod
     def post_step(
-        self, sim: JaxSim, step_data: Dict[str, StepData]
-    ) -> Tuple[JaxSim, jtp.PyTree]:
+        self, sim: "jaxsim.JaxSim", step_data: Dict[str, StepData]
+    ) -> Tuple["jaxsim.JaxSim", jtp.PyTree]:
         pass
 
 
 class CallbackHandler(ConfigureCallback, PreStepCallback, PostStepCallback):
     pass
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/typing.py` & `jaxsim-0.1.dev135/src/jaxsim/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 ]
 
 # Mixed JAX / NumPy types
 Array = Union[npt.NDArray, ArrayJax]
 Tensor = Union[npt.NDArray, ArrayJax]
 Vector = Array
 Matrix = Array
-Bool = Union[bool, np.bool]
-Int = Union[int, np.int, IntJax]
-Float = Union[float, np.float, FloatJax]
+Bool = bool
+Int = Union[int, IntJax]
+Float = Union[float, FloatJax]
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim/utils.py` & `jaxsim-0.1.dev135/src/jaxsim/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,75 @@
 import abc
 import contextlib
 import copy
-from typing import ContextManager, TypeVar
+from typing import Any, ContextManager, TypeVar
 
 import jax.abstract_arrays
 import jax.flatten_util
 import jax.interpreters.partial_eval
 import jax_dataclasses
 from jax_dataclasses._copy_and_mutate import _Mutability as Mutability
 
 import jaxsim.typing as jtp
 
 T = TypeVar("T")
 
 
-def tracing(var) -> bool:
+def tracing(var: Any) -> bool:
+    """Returns True if the variable is being traced by JAX, False otherwise."""
 
-    return isinstance(
-        var,
-        (
-            jax.abstract_arrays.ShapedArray,
-            jax.interpreters.partial_eval.DynamicJaxprTracer,
-        ),
-    )
+    return jax.numpy.array(
+        [
+            isinstance(var, t)
+            for t in (
+                jax.abstract_arrays.ShapedArray,
+                jax.interpreters.partial_eval.DynamicJaxprTracer,
+            )
+        ]
+    ).any()
+
+
+def not_tracing(var: Any) -> bool:
+    """Returns True if the variable is not being traced by JAX, False otherwise."""
+
+    return True if tracing(var) is False else False
 
 
 class JaxsimDataclass(abc.ABC):
+    """"""
+
     @contextlib.contextmanager
     def editable(self: T, validate: bool = True) -> ContextManager[T]:
+        """"""
+
+        mutability = (
+            Mutability.MUTABLE if validate else Mutability.MUTABLE_NO_VALIDATION
+        )
+
+        with JaxsimDataclass.mutable_context(self.copy(), mutability=mutability) as obj:
+            yield obj
+
+        # with jax_dataclasses.copy_and_mutate(self, validate=validate) as self_rw:
+        #     yield self_rw
+        #
+        # self_rw._set_mutability(self._mutability())
+
+    @contextlib.contextmanager
+    def mutable_context(self: T, mutability: Mutability) -> ContextManager[T]:
+        """"""
+
+        original_mutability = self._mutability
 
-        with jax_dataclasses.copy_and_mutate(self, validate=validate) as self_rw:
-            yield self_rw
+        self._set_mutability(mutability)
+        yield self
 
-        self_rw._set_mutability(self._mutability())
+        self._set_mutability(original_mutability)
 
     def is_mutable(self: T, validate: bool = False) -> bool:
+        """"""
 
         return (
             self.__mutability__ is Mutability.MUTABLE
             if validate
             else self.__mutability__ is Mutability.MUTABLE_NO_VALIDATION
         )
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev135/src/jaxsim.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev118
+Version: 0.1.dev135
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
@@ -53,14 +53,16 @@
 - Support of SDF models (and, upon conversion, URDF models).
 - Collision detection between bodies and uneven ground surface.
 - Continuous soft contacts model with no friction cone approximations.
 - Full support of inertial properties of bodies.
 - Revolute, prismatic, and fixed joints support.
 - Integrators: forward Euler, semi-implicit Euler, Runge-Kutta 4.
 - High-level classes to compute multi-body dynamics quantities from simulation state.
+- High-level classes supporting both object-oriented and functional programming.
+- Optional validation of JAX pytrees to prevent JIT re-compilation. 
 
 Planned features:
 
 - Reinforcement Learning module developed in JAX.
 - Finalization of differentiable physics through the simulation.
 
 [jax]: https://github.com/google/jax/
@@ -107,14 +109,25 @@
 [PFS]: http://sdformat.org/tutorials?tut=pose_frame_semantics
 
 ## Contributing
 
 Pull requests are welcome. 
 For major changes, please open an issue first to discuss what you would like to change.
 
+## Citing
+
+```bibtex
+@software{ferigo_jaxsim_2022,
+  author = {Diego Ferigo and Silvio Traversaro and Daniele Pucci},
+  title = {{JAXsim}: A Physics Engine in Reduced Coordinates for Control and Robot Learning},
+  url = {http://github.com/ami-iit/jaxsin},
+  year = {2022},
+}
+```
+
 ## Maintainers
 
 | [<img src="https://github.com/diegoferigo.png" width="40">][df] | [@diegoferigo][df] |
 |:---------------------------------------------------------------:|:------------------:|
 
 [df]: https://github.com/diegoferigo
```

### Comparing `jaxsim-0.1.dev118/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev135/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

